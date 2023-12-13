---
audience: end-user
title: Creare la prima query utilizzando il modellatore di query
description: Scopri come creare la prima query in Adobe Campaign Web Query Modeler.
source-git-commit: cc909bdf7507e66e000297440e31f9b5260f1257
workflow-type: tm+mt
source-wordcount: '1319'
ht-degree: 3%

---

# Creare la prima query {#build-query}

Per iniziare a creare una query, accedi al modellatore di query dalla posizione desiderata, a seconda dell’azione da eseguire. Verrà aperto Query Modeler con un&#39;area di lavoro vuota. Fai clic su **+** per configurare il primo nodo della query.

Puoi aggiungere due tipi di elementi:

* **Filtraggio dei componenti** (Condizione personalizzata, Seleziona pubblico, Filtro predefinito) ti consente di creare regole personalizzate, selezionare un pubblico o un filtro predefinito per perfezionare la query. [Scopri come utilizzare i componenti di filtro](#filtering)

  Esempio:

  *Destinatari che si sono iscritti alla newsletter &quot;Sport&quot;*. *Destinatari che vivono a New York*, *Destinatari residenti a San Francisco*

* **Operatori di gruppo** (AND, OR, EXCEPT) consente di raggruppare i componenti di filtro nel diagramma in base alle proprie esigenze. [Scopri come lavorare con gli operatori](#filtering)

  Esempio:

  *Destinatari che si sono iscritti alla newsletter &quot;Sport&quot;**E**che vivono a New York **OPPURE**San Francisco*.

![](assets/query-add-component.png)

## Aggiungere componenti di filtro {#filtering}

I componenti di filtro consentono di perfezionare la query utilizzando:

* **Condizioni personalizzate**: filtra la query creando la tua condizione con gli attributi del database e le espressioni avanzate.
* **Tipi di pubblico**: filtra la query utilizzando un pubblico esistente.
* **Filtro predefinito**: filtra la query utilizzando filtri predefiniti esistenti.

### Configurare una condizione personalizzata

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_customcondition"
>title="Condizione personalizzata"
>abstract="Condizione personalizzata"

Per filtrare la query utilizzando una condizione personalizzata, effettua le seguenti operazioni:

1. Fai clic su **+** sul nodo desiderato e seleziona **[!UICONTROL Condizione personalizzata]**. Il riquadro delle proprietà della condizione personalizzata viene visualizzato sul lato destro.

1. In **Attributo** selezionare l&#39;attributo dal database che si desidera utilizzare per creare la condizione. L’elenco degli attributi include tutti gli attributi del database Campaign, inclusi gli attributi collegati alla tabella.

   ![](assets/query-custom-condition-fields.png)

   >[!NOTE]
   >
   >Il pulsante Modifica espressione consente di sfruttare l’editor di espressioni web di Campaign per definire manualmente un’espressione utilizzando i campi delle funzioni di supporto e del database.

1. Seleziona l’operatore da applicare dall’elenco a discesa. Sono disponibili vari operatori.Si noti che gli operatori disponibili nell&#39;elenco a discesa dipendono dal tipo di dati dell&#39;attributo selezionato.

   +++Elenco degli operatori disponibili

   | Operatore | Finalità | Esempio |
   |  ---  |  ---  |  ---  |
   | Uguale | Restituisce un risultato identico ai dati immessi nella seconda colonna Valore. | Cognome (@lastName) uguale a &quot;Jones&quot;, restituirà solo i destinatari il cui cognome è Jones. |
   | Diverso da | Restituisce tutti i valori non identici al valore inserito. | Lingua (@language) uguale a &#39;Inglese&#39; |
   | Maggiore di | Restituisce un valore maggiore del valore immesso. | Età (@age) superiore a 50 anni</strong>, restituirà tutti i valori maggiori di &quot;50&quot;, ovvero &quot;51&quot;, &quot;52&quot;, ecc. |
   | Minore di | Restituisce un valore minore del valore inserito. | Data di creazione (@created) prima di &#39;DaysAgo(100)&#39;</strong>, restituirà tutti i destinatari creati meno di 100 giorni fa. |
   | Maggiore o uguale a | Restituisce tutti i valori uguali o maggiori del valore inserito. | Età (@age) maggiore o uguale a &#39;30&#39;</strong>, restituirà tutti i destinatari di almeno 30 anni di età. |
   | Minore o uguale a | Restituisce tutti i valori uguali o inferiori al valore inserito. | Età (@age) minore o uguale a &#39;60&#39;</strong>, restituirà tutti i destinatari di età non superiore a 60 anni. |
   | Incluso in | Restituisce i risultati inclusi nei valori indicati. Questi valori devono essere separati da una virgola. | La data di nascita (@birthDate) è inclusa in &#39;12/10/1979,12/10/1984&#39; e restituisce i destinatari nati tra queste date. |
   | Non in entrata | Funziona come l’operatore È incluso in. In questo caso, vogliamo escludere i destinatari in base ai valori immessi. | La data di nascita (@birthDate) non è inclusa in &quot;12/10/1979,12/10/1984&quot;. A differenza dell’esempio precedente, i destinatari nati in queste date non verranno restituiti. |
   | È vuoto | In questo caso, il risultato che stiamo cercando corrisponde a un valore vuoto nella seconda colonna Valore. | Mobile (@mobilePhone) è vuoto restituisce tutti i destinatari che non hanno un numero di cellulare. |
   | Non è vuoto | Funziona in modo inverso rispetto all&#39;operatore Is empty. Non è necessario immettere dati nella seconda colonna Valore. | Il campo E-mail (@email) non è vuoto. |
   | Inizia con | Restituisce i risultati a partire dal valore inserito. | Il numero account (@account) inizia con &quot;32010&quot;. |
   | Non inizia con | Restituisce i risultati che non iniziano con il valore inserito | Il numero account (@account) non inizia con &quot;20&quot; |
   | Contiene | Restituisce i risultati contenenti almeno il valore inserito. | Il dominio e-mail (@domain) contiene &quot;mail&quot;</strong>, restituirà tutti i nomi di dominio che contengono &quot;mail&quot;. Quindi verrà restituito anche il dominio &quot;gmail.com&quot;. |
   | Non contiene | Restituisce risultati che non contengono il valore inserito. | Il dominio e-mail (@domain) non contiene &#39;vo&#39;</strong>. In questo caso, i nomi di dominio che contengono &#39;vo&#39; non verranno restituiti. Il nome di dominio &quot;voilà.fr&quot; non verrà visualizzato nei risultati. |
   | Mi piace | Simile è molto simile all’operatore Contains. Ti consente di inserire un carattere jolly % nel valore. | Cognome (@lastName) come &#39;Jon%s&#39;. Qui, il carattere jolly viene usato come un &quot;jolly&quot; per trovare il nome &quot;Jones&quot;, se l&#39;operatore avesse dimenticato la lettera mancante tra la &quot;n&quot; e la &quot;s&quot;. |
   | Non simile a | Simile è molto simile all’operatore Contains. Ti consente di inserire un carattere jolly % nel valore. | Cognome (@lastName) diverso da &quot;Smi%h&quot;. In questo caso, i destinatari il cui cognome è &#39;Smi%h&#39; non verranno restituiti. |

+++

1. In **Valore** , definisci il valore previsto. Puoi anche sfruttare l’editor di espressioni web di Campaign per definire manualmente un’espressione utilizzando i campi del database e le funzioni di supporto. A questo scopo, fai clic su **Modifica espressione** pulsante.

   *Esempio di query che restituisce tutti i profili di età pari o superiore a 21 anni:*

   ![](assets/query-custom-condition.png)

### Selezionare un pubblico

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_selectaudience"
>title="Seleziona il tipo di pubblico"
>abstract="Seleziona il tipo di pubblico"

Per filtrare la query utilizzando un pubblico esistente, effettua le seguenti operazioni:

1. Fai clic su **+** sul nodo desiderato e scegliere **[!UICONTROL Seleziona pubblico]**.

1. Il **Seleziona pubblico** il riquadro proprietà si apre sul lato destro. Scegli il pubblico da utilizzare per filtrare la query.

   *Esempio di query che restituisce tutti i profili appartenenti al pubblico &quot;Partecipanti al festival&quot;:*

   ![](assets/query-audience.png)

### Utilizza un filtro preimpostato

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_predefinedfilter"
>title="Filtro preimpostato"
>abstract="Filtro preimpostato"

Per filtrare la query utilizzando un filtro predefinito, effettua le seguenti operazioni:

1. Fai clic su **+** sul nodo desiderato e seleziona **[!UICONTROL Filtro predefinito]**.

1. Il **Filtro predefinito** il riquadro proprietà si apre sul lato destro. Seleziona un filtro predefinito dall’elenco dei filtri personalizzati o dai preferiti.

   *Esempio di query che restituisce tutti i profili corrispondenti al filtro predefinito &quot;Clienti inattivi&quot;:*

   ![](assets/query-predefined-filter.png)

## Combinare componenti di filtro con operatori {#operators}

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_group"
>title="Gruppo"
>abstract="Gruppo"

Ogni volta che aggiungi un nuovo componente di filtro alla query, questo viene collegato automaticamente all’altro componente da un operatore AND. Ciò significa che i risultati di entrambi i componenti di filtro vengono combinati nei risultati della query.

In questo esempio, è stato aggiunto un nuovo componente di filtro per il tipo di pubblico alla seconda transizione. Il componente è collegato alla condizione del tipo di filtro predefinito con un operatore AND, il che significa che i risultati della query includono i destinatari interessati dal filtro predefinito &quot;Madridians&quot; E appartenenti al pubblico &quot;Discount hunters&quot;.

![](assets/query-operator.png)

Per modificare l’operatore utilizzato per collegare insieme le condizioni di filtro, fai clic su di esso e seleziona l’operatore desiderato nel riquadro Gruppo che si apre sul lato destro.

Gli operatori disponibili sono:

* **AND (intersezione)**: combina i risultati di tutti i componenti di filtro nelle transizioni in uscita.
* **O (Unione)**: include i risultati di almeno uno dei componenti di filtro nelle transizioni in uscita.
* **ECCETTO (esclusione)**: esclude i risultati da tutti i componenti di filtro nella transizione in uscita.

![](assets/query-operator-change.png)

## Verifica e convalida la query

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_ruleproperties"
>title="Proprietà della regola"
>abstract="Proprietà della regola"

Dopo aver creato la query nell’area di lavoro, puoi controllarla utilizzando **Proprietà delle regole** sul lato destro. Le operazioni disponibili sono:

* **Visualizza risultati:** Visualizza i dati risultanti dalla query.
* **Vista Codice**: visualizza una versione basata su codice della query in SQL.
* **Calcola**: aggiorna e visualizza il numero di record interessati dalla query.
* **Seleziona o salva il filtro**: scegli un filtro predefinito esistente da utilizzare nell’area di lavoro oppure salva la query come filtro predefinito da riutilizzare in futuro. [Scopri come utilizzare i filtri preimpostati](../get-started/predefined-filters.md)

  >[!IMPORTANT]
  >
  >Selezionare un filtro predefinito dal riquadro Proprietà regola sostituisce la query creata nell&#39;area di lavoro con il filtro selezionato.
