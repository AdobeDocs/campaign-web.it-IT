---
audience: end-user
title: Creare la prima query utilizzando il query modeler
description: Scopri come creare la prima query nel query modeler di Adobe Campaign Web.
badge: label="Disponibilità limitata"
source-git-commit: 95be832f5f5f330bb72f9abbf780965b452e2e5e
workflow-type: tm+mt
source-wordcount: '1634'
ht-degree: 89%

---

# Creare la prima query {#build-query}

Per iniziare a creare una query, accedi al query modeler dalla posizione desiderata, a seconda dell’azione da eseguire. Verrà visualizzato il query modeler con un’area di lavoro vuota. Fai clic sul pulsante **+** per configurare il primo nodo della query.

Puoi aggiungere due tipi di elementi:

* **Componenti per il filtro** (Condizione personalizzata, Seleziona pubblico, Filtro predefinito) ti consente di creare regole personalizzate, selezionare un pubblico o un filtro predefinito per perfezionare la query. [Scopri come utilizzare i componenti per il filtro](#filtering)

  Esempio:

  *Destinatari che si sono iscritti alla newsletter “Sport”*. *Destinatari che vivono a New York*, *Destinatari che vivono a San Francisco*

* Gli **operatori del gruppo** (AND, OR, EXCEPT) consentono di raggruppare i componenti per il filtro nel diagramma in base alle esigenze. [Scopri come utilizzare gli operatori](#filtering)

  Esempio:

  *Destinatari che si sono iscritti alla newsletter “Sport”**AND**vivono a New York **OR**a San Francisco*.

![](assets/query-add-component.png)

## Aggiungere i componenti per il filtro {#filtering}

I componenti per il filtro consentono di perfezionare la query utilizzando:

* **Condizioni personalizzate**: per filtrare la query creando la tua condizione personalizzata con gli attributi dal database e le espressioni avanzate.
* **Tipi di pubblico**: per filtrare la query utilizzando un pubblico esistente.
* **Filtro predefinito**: per filtrare la query utilizzando filtri preimpostati esistenti.

### Configurare una condizione personalizzata

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_customcondition"
>title="Condizione personalizzata"
>abstract="Condizione personalizzata"

Per filtrare la query utilizzando una condizione personalizzata, effettua le seguenti operazioni:

1. Fai clic sul pulsante **+** sul nodo desiderato e seleziona **[!UICONTROL Condizione personalizzata]**. Il pannello delle proprietà della condizione personalizzata viene visualizzato sul lato destro.

1. Nel campo **Attributo**, seleziona l’attributo dal database che desideri sfruttare per creare la condizione. L’elenco degli attributi include tutti gli attributi del database di Campaign, inclusi gli attributi collegati alla tabella.

   ![](assets/query-custom-condition-fields.png)

   >[!NOTE]
   >
   >Il pulsante Modifica espressione consente di sfruttare l’editor di espressioni di Campaign Web per definire manualmente un’espressione utilizzando i campi dal database e le funzioni Helper.

1. Seleziona l’operatore da applicare dall’elenco a discesa. Sono disponibili diversi operatori da utilizzare. Gli operatori disponibili nell’elenco a discesa dipendono dal tipo di dati dell’attributo.

   +++Elenco degli operatori disponibili

   | Operatore | Scopo | Esempio |
   |  ---  |  ---  |  ---  |
   | Uguale a | Restituisce un risultato identico ai dati immessi nella seconda colonna Valore. | Cognome (@lastName) uguale a “Jones”, restituirà solo i destinatari il cui cognome è Jones. |
   | Non uguale a | Restituisce tutti i valori non identici al valore inserito. | Lingua (@language) uguale a “Inglese” |
   | Maggiore di | Restituisce un valore maggiore del valore immesso. | Età (@age) maggiore di 50 anni</strong>, restituirà tutti i valori maggiori di “50”, ovvero “51”, “52”, ecc. |
   | Minore di | Restituisce un valore minore del valore immesso. | Data di creazione (@created) prima di “DaysAgo(100)”</strong>, restituirà tutti i destinatari creati meno di 100 giorni fa. |
   | Maggiore o uguale a | Restituisce tutti i valori uguali o maggiori del valore immesso. | Età (@age) maggiore o uguale a “30”</strong>, restituirà tutti i destinatari con un’età pari o superiore ai 30 anni. |
   | Minore o uguale a | Restituisce tutti i valori uguali o inferiori al valore immesso. | Età (@age) minore o uguale a “60”</strong>, restituirà tutti i destinatari di età uguale o inferiore ai 60 anni. |
   | Incluso in | Restituisce i risultati inclusi nei valori indicati. Questi valori devono essere separati da una virgola. | La data di nascita (@birthDate) inclusa in “10/12/1979,10/12/1984” restituirà i destinatari nati nell’intervallo tra queste date. |
   | Non in | Funziona come l’operatore Incluso in. In questo caso, desideriamo escludere i destinatari in base ai valori immessi. | La data di nascita (@birthDate) non è inclusa in “10/12/1979,10/12/1984”. A differenza dell’esempio precedente, i destinatari nati in questo intervallo di date non verranno restituiti. |
   | È vuoto | In questo caso, il risultato che stiamo cercando corrisponde a un valore vuoto nella seconda colonna Valore. | Cellulare (@mobilePhone) è vuoto restituisce tutti i destinatari che non hanno un numero di cellulare. |
   | Non è vuoto | Funziona in modo inverso rispetto all’operatore È vuoto. Non è necessario immettere dati nella seconda colonna Valore. | Il campo E-mail (@email) non è vuoto. |
   | Inizia con | Restituisce i risultati a partire dal valore immesso. | Account # (@account) inizia con “32010”. |
   | Non inizia con | Restituisce i risultati che non iniziano con il valore immesso | Account # (@account) non inizia con “20” |
   | Contiene | Restituisce i risultati che contengono almeno il valore immesso. | Il dominio e-mail (@domain) contiene “mail”</strong>, restituirà tutti i nomi di dominio che contengono “mail”. Quindi verrà restituito anche il dominio “gmail.com”. |
   | Non contiene | Restituisce risultati che non contengono il valore immesso. | Il dominio e-mail (@domain) non contiene “vo”</strong>. In questo caso, i nomi di dominio che contengono “vo” non verranno restituiti. Il nome di dominio “voilà.fr” non verrà visualizzato nei risultati. |
   | Simile a | Simile a è identico all’operatore Contiene. Ti consente di inserire un carattere jolly % nel valore. | Cognome (@lastName) simile a “Jon%s”. Qui, il carattere jolly viene usato come un “jolly” per trovare il nome “Jones”, nel caso in cui l’operatore avesse dimenticato la lettera mancante tra la “n” e la “s”. |
   | Diverso da | Simile a è identico all’operatore Contiene. Ti consente di inserire un carattere jolly % nel valore. | Cognome (@lastName) diverso da “Smi%h”. In questo caso, i destinatari con il cognome è “Smi%h” non verranno restituiti. |

+++

1. Nel campo **Valore**, definisci il valore previsto. Puoi anche sfruttare l’editor di espressioni di Campaign Web per definire manualmente un’espressione utilizzando i campi dal database e le funzioni Helper. A questo scopo, fai clic sul pulsante **Modifica espressione**.

   *Esempio di query che restituisce tutti i profili di età pari o superiore a 21 anni:*

   ![](assets/query-custom-condition.png)

**Condizioni personalizzate per tabelle distanti (collegamenti 1-1 e 1-N)**

Le condizioni personalizzate consentono di eseguire query su tabelle distanti collegate alla tabella Destinatari.

Per un **collegamento 1-1** con un’altra risorsa del database, seleziona un valore direttamente dalla tabella di destinazione.

+++Esempio di query

In questo caso, la query esegue il targeting dei destinatari il cui paese o area geografica è incluso nei valori forniti (Regno Unito e Stati Uniti)

![](assets/custom-condition-1-1.png)

+++

Per un **collegamento 1-N** con un’altra risorsa del database, puoi definire condizioni secondarie sui campi di questa seconda risorsa.

Ad esempio, puoi selezionare l’operatore Esiste sugli acquisti del profilo per eseguire il targeting di tutti i profili per i quali esistono acquisti. Al termine, aggiungi una condizione personalizzata nella transizione in uscita e crea un filtro che soddisfi le tue esigenze.

+++Esempio di query

In questo caso, la query è rivolta a destinatari che hanno effettuato acquisti relativi al prodotto BrewMaster, per un importo totale di almeno 100$.

![](assets/custom-condition-1-N.png)

+++

### Selezionare un pubblico

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_selectaudience"
>title="Selezionare il tipo di pubblico"
>abstract="Selezionare il tipo di pubblico"

Per filtrare la query utilizzando un pubblico esistente, effettua le seguenti operazioni:

1. Fai clic sul pulsante **+** sul nodo desiderato e scegli **[!UICONTROL Seleziona pubblico]**.

1. Il pannello delle proprietà **Seleziona pubblico** si apre sul lato destro. Scegli il pubblico che desideri utilizzare per filtrare la query.

   *Esempio di query che restituisce tutti i profili appartenenti al pubblico “Partecipanti al festival”:*

   ![](assets/query-audience.png)

### Utilizzare un filtro preimpostato

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_predefinedfilter"
>title="Filtro preimpostato"
>abstract="Filtro preimpostato"

Per filtrare la query utilizzando un filtro preimpostato, effettua le seguenti operazioni:

1. Fai clic sul pulsante **+** sul nodo desiderato e seleziona **[!UICONTROL Filtro preimpostato]**.

1. Il pannello delle proprietà **Filtro preimpostato** si apre sul lato destro. Seleziona un filtro preimpostato dall’elenco dei filtri personalizzati o dai preferiti.

   *Esempio di query che restituisce tutti i profili corrispondenti al filtro preimpostato “Clienti inattivi”:*

   ![](assets/query-predefined-filter.png)

## Combinare componenti di filtraggio con operatori {#operators}

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_group"
>title="Gruppo"
>abstract="Gruppo"

Ogni volta che aggiungi un nuovo componente di filtraggio alla query, questo viene collegato automaticamente all’altro componente da un operatore AND. Ciò significa che i risultati di entrambi i componenti di filtraggio vengono combinati nei risultati della query.

In questo esempio, è stato aggiunto un nuovo componente di filtraggio per il tipo di pubblico alla seconda transizione. Il componente è collegato alla condizione del tipo di filtro preimpostato con un operatore AND, il che significa che i risultati della query includono i destinatari interessati dal filtro preimpostato “Madridians” e appartenenti al pubblico “Discount hunters”.

![](assets/query-operator.png)

Per modificare l’operatore utilizzato per collegare insieme le condizioni di filtraggio, fai clic su di esso e seleziona l’operatore desiderato nel riquadro Gruppo che si apre sul lato destro.

Gli operatori disponibili sono:

* **AND (intersezione)**: combina i risultati che corrispondono a tutti i componenti di filtraggio nelle transizioni in uscita.
* **OR (Unione)**: include i risultati che corrispondono ad almeno uno dei componenti di filtraggio nelle transizioni in uscita.
* **ECCETTO (esclusione)**: esclude i risultati che corrispondono a tutti i componenti di filtraggio nella transizione in uscita.

![](assets/query-operator-change.png)

### Copiare e incollare componenti di filtro {#copy}

Query Modeler consente di copiare uno o più componenti di filtro e incollarli al termine di una transizione. Questa operazione può essere eseguita nell’area di lavoro query corrente o in qualsiasi area di lavoro all’interno dell’istanza.

>[!NOTE]
>
>La selezione copiata viene mantenuta per tutto il tempo in cui si lavora nell’istanza. Se si disconnette e si effettua nuovamente l&#39;accesso, la selezione non sarà più disponibile per l&#39;incollamento.

Per copiare e incollare i componenti di filtro, effettua le seguenti operazioni:

1. Seleziona il componente filtro da copiare facendo clic su di esso nell’area di lavoro della query. Per selezionare più componenti, utilizza lo strumento per la selezione multipla disponibile nella barra degli strumenti situata nell’angolo superiore destro dell’area di lavoro.

1. Fai clic su **[!UICONTROL Copia]** nel riquadro delle proprietà del componente oppure, se hai selezionato più componenti, sulla barra multifunzione blu nella parte inferiore dello schermo.

   | Copiare un singolo componente | Copiare più componenti |
   |  ---  |  ---  |
   | ![](assets/copy-single-component.png){width="200" align="center" zoomable="yes"} | ![](assets/copy-multiple-components.png){width="200" align="center" zoomable="yes"} |

1. Per incollare i componenti, fai clic sul pulsante + alla fine della transizione desiderata e seleziona **Incolla n elementi**.

![](assets/copy-paste.png)

## Controllare e convalidare la query

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_ruleproperties"
>title="Proprietà delle regole"
>abstract="Proprietà delle regole"

Dopo aver creato la query nell’area di lavoro, puoi controllarla utilizzando il pannello **Proprietà delle regole** sul lato destro. Le operazioni disponibili sono:

* **Visualizza risultati:** visualizza i dati risultanti dalla query.
* **Vista codice**: visualizza una versione della query basata su codice in SQL.
* **Calcola**: aggiorna e visualizza il numero di record interessati dalla query.
* **Selezionare o salvare il filtro**: scegli un filtro preimpostato esistente da utilizzare nell’area di lavoro oppure salva la query come filtro preimpostato per riutilizzarla in futuro. [Scopri come utilizzare i filtri preimpostati](../get-started/predefined-filters.md)

  >[!IMPORTANT]
  >
  >La selezione di un filtro preimpostato dal pannello Proprietà regole sostituisce la query creata nell’area di lavoro con il filtro selezionato.
