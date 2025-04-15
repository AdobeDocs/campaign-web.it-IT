---
audience: end-user
title: Creare la prima query utilizzando il query modeler
description: Scopri come creare la prima query nel query modeler di Adobe Campaign Web.
exl-id: efd762b5-a7ae-49b4-ab74-5b43da1e574d
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '2310'
ht-degree: 37%

---


# Creare la prima query {#build-query}

Per iniziare a creare una query, accedi al query modeler dalla posizione desiderata, a seconda dell’azione da eseguire. Il modello di query si apre con un&#39;area di lavoro vuota. Fai clic sul pulsante **+** per configurare il primo nodo della query.

Puoi aggiungere due tipi di elementi:

* **I componenti** di filtro (condizione personalizzata, Seleziona pubblico, Filtro predefinito) consentono di versione le proprie regole, selezionare un pubblico o utilizzare un filtro predefinito per perfezionare la query. Vengono aggiunti all&#39;inizio della query e nelle transizioni punteggiate. [Scopri come utilizzare i componenti per il filtro](#filtering)

  Esempio: *Destinatari che si sono iscritti alla newsletter* &quot;Sport&quot;, *Destinatari residenti a Nuovo York*, *Destinatari residenti a San Francisco*

  ![Esempio di aggiunta di componenti filtro a una query.](assets/query-add-component.png){zoomable="yes"}

* **Gli operatori di gruppo** (AND, OR, EXCEPT) consentono di raggruppare i componenti di filtro nel diagramma. Vengono aggiunte alle transizioni esistenti prima di un componente di filtro. [Scopri come utilizzare gli operatori](#filtering)

  Esempio: *Destinatari abbonati alla newsletter &quot;Sport&quot;**AND**che vivono a New York **OR**San Francisco*.

  ![Descrizione: esempio di aggiunta di operatori di gruppo a una query.](assets/query-add-operator.png){zoomable="yes"}

## Distribuzione dei valori in una query {#distribution-values-query}

La distribuzione dei valori mostra la percentuale di ciascun valore di un campo all’interno di una tabella, in base ai parametri di query correnti. Conoscere la distribuzione dei valori all&#39;interno di una query è utile per perfezionare Segmentazione.

Per accesso questa opzione, nella query fai clic sul pulsante di selezione degli attributi come mostrato di seguito. Quindi, fai clic sull&#39;icona **[!UICONTROL Informazioni]** accanto all&#39;attributo selezionato. È possibile accesso la **[!UICONTROL Distribuzione dei valori]** pulsante.

![Descrizione: Accesso all&#39;opzione di distribuzione dei valori in una query.](assets/values_query.png){zoomable="yes"}

>[!NOTE]
>
>* Per i campi con molti valori, vengono visualizzati solo i primi venti valori. In questi casi, viene visualizzato un avviso notifica **[!UICONTROL Carico]** parziale.
>* L&#39;opzione **[!UICONTROL Distribuzione dei valori]** è accessibile in ogni selettore di attributi. [Scopri come selezionare gli attributi](../get-started/attributes.md)
>* Puoi aggiungere condizioni ai risultati utilizzando **[!Afiltri avanzati]**. [Ulteriori informazioni](../get-started/work-with-folders.md#filter-the-values).

## Aggiungere i componenti per il filtro {#filtering}

I componenti per il filtro consentono di perfezionare la query utilizzando:

* **[Condizioni personalizzate](#custom-condition)**: per filtrare la query creando la tua condizione personalizzata con gli attributi dal database e le espressioni avanzate.
* **[Tipi di pubblico](#audiences)**: per filtrare la query utilizzando un pubblico esistente.
* **[Filtro predefinito](#predefined-filters)**: per filtrare la query utilizzando filtri preimpostati esistenti.

### Configurare una condizione personalizzata {#custom-condition}

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_customcondition"
>title="Condizione personalizzata"
>abstract="Le condizioni personalizzate sono componenti di filtraggio che consentono di filtrare la query creando la propria condizione con attributi provenienti dal database ed espressioni avanzate."

Per filtrare la query utilizzando una condizione personalizzata, effettua le seguenti operazioni:

1. Fai clic sul pulsante **+** sul nodo desiderato e seleziona **[!UICONTROL Condizione personalizzata]**. Il riquadro delle proprietà delle condizioni personalizzate si apre sul lato destro.

1. **Nel campo Attributo** selezionare dal database l&#39;attributo che si desidera utilizzare per creare la condizione. Nell&#39;elenco degli attributi sono inclusi tutti gli attributi del database delle campagne, inclusi gli attributi delle tabelle collegate. [Scopri come selezionare gli attributi e aggiungerli ai preferiti](../get-started/attributes.md)

   ![Selezione degli attributi di una condizione personalizzata in una query.](assets/query-custom-condition-fields.png){zoomable="yes"}

   >[!NOTE]
   >
   >Il **pulsante di espressioni** Modifica consente di utilizzare il editor di espressioni Web Campaign per definire manualmente un&#39;espressione utilizzando i campi del database e delle funzioni di supporto. [Scopri come modificare le espressioni](expression-editor.md)

1. Seleziona l’operatore da applicare dall’elenco a discesa. Sono disponibili diversi operatori da utilizzare. Gli operatori disponibili nell’elenco a discesa dipendono dal tipo di dati dell’attributo.

   +++Elenco degli operatori disponibili

   | Operatore | Scopo | Esempio |
   |---|---|---|
   | Uguale a | Restituisce un risultato identico ai dati immessi nella seconda colonna Valore. | Il cognome (@lastName) uguale a &quot;Jones&quot; restituirà solo i destinatari il cui cognome è Jones. |
   | Non uguale a | Restituisce tutti i valori non identici al valore inserito. | Lingua (@language) non uguale a &#39;Inglese&#39;. |
   | Maggiore di | Restituisce un valore maggiore del valore immesso. | L&#39;età (@age) maggiore di 50 restituirà tutti i valori maggiori di &#39;50&#39;, ad esempio &#39;51&#39;, &#39;52&#39;. |
   | Minore di | Restituisce un valore minore del valore immesso. | La data di creazione (@created) prima di &quot;DaysAgo(100)&quot; restituirà tutti i destinatari creati meno di 100 giorni fa. |
   | Maggiore o uguale a | Restituisce tutti i valori uguali o maggiori del valore immesso. | L&#39;età (@age) maggiore o uguale a &quot;30&quot; restituirà tutti i destinatari di età pari o superiore a 30 anni. |
   | Minore o uguale a | Restituisce tutti i valori uguali o inferiori al valore immesso. | L&#39;età (@age) inferiore o uguale a &quot;60&quot; restituirà tutti i destinatari di età pari o inferiore a 60 anni. |
   | Incluso in | Restituisce i risultati inclusi nei valori indicati. Questi valori devono essere separati da una virgola. | La data di nascita (@birthDate) è inclusa in &#39;12/10/1979,12/10/1984&#39; restituirà i destinatari nati tra queste date. |
   | Non in | Funziona come l’operatore Incluso in. Qui, i destinatari vengono esclusi in base ai valori immessi. | La data di nascita (@birthDate) non è inclusa in “10/12/1979,10/12/1984”. I destinatari nati entro queste date non saranno restituiti. |
   | È vuoto | Restituisce risultati che corrispondono a un valore vuoto nella seconda colonna Valore. | Cellulare (@mobilePhone) è vuoto restituisce tutti i destinatari che non hanno un numero di cellulare. |
   | Non è vuoto | Funziona in modo inverso rispetto all’operatore È vuoto. Non è necessario immettere dati nella seconda colonna Valore. | Il campo E-mail (@email) non è vuoto. |
   | Inizia con | Restituisce i risultati che iniziano con il valore immesso. | Account # (@account) inizia con “32010”. |
   | Non inizia con | Restituisce risultati che non iniziano con il valore immesso. | Il numero account (@account) non inizia con &quot;20&quot;. |
   | Contiene | Restituisce risultati contenenti almeno il valore immesso. | Email domain (@domain) contains &#39;mail&#39; restituirà tutti i nomi di dominio che contengono &#39;mail&#39;, ad esempio &#39;gmail.com&#39;. |
   | Non contiene | Restituisce risultati che non contengono il valore immesso. | Il dominio e-mail (@domain) non contiene &#39;vo&#39;. I nomi di dominio contenenti &#39;vo&#39;, ad esempio &#39;voilà.fr&#39;, non verranno visualizzati nei risultati. |
   | Simile a | Simile all&#39;operatore Contains, consente di inserire un carattere jolly % nel valore. | Cognome (@lastName) simile a “Jon%s”. Il carattere jolly funge da &quot;jolly&quot; per trovare nomi come &quot;Jones&quot;. |
   | Diverso da | Analogamente all&#39;operatore Contains, consente di inserire un carattere jolly % nel valore. | Cognome (@lastName) diverso da “Smi%h”. I destinatari il cui cognome è &quot;Smith&quot; non saranno restituiti. |

+++

1. Nel campo **Valore**, definisci il valore previsto. È inoltre possibile utilizzare il editor delle espressioni Web Campaign per definire manualmente un&#39;espressione utilizzando i campi del database e delle funzioni di supporto. A tale scopo, fare clic sull&#39;espressione **** Modifica pulsante. [Scopri come modificare le espressioni](expression-editor.md)

   *Esempio di query che restituisce tutti i profili di età pari o superiore a 21 anni:*

   ![Esempio di query per il targeting di profili di età pari o superiore a 21 anni.](assets/query-custom-condition.png){zoomable="yes"}

   Per gli attributi di tipo data, i valori predefiniti sono disponibili utilizzando l&#39;opzione **[!UICONTROL Predefiniti]**.

   ![Esempio di utilizzo di predefiniti di data in una query.](assets/date-presets.png){zoomable="yes"}

#### Condizioni personalizzate per le tabelle collegate (collegamenti 1-1 e 1-N){#links}

Le condizioni personalizzate consentono di eseguire query sulle tabelle collegate alla tabella attualmente utilizzata dalla regola. Questo include tabelle con un collegamento di cardinalità 1-1 o tabelle di raccolta (collegamento 1-N).

Per un collegamento **1-1**, passare alla tabella collegata, selezionare l&#39;attributo desiderato e definire il valore previsto.

Puoi anche selezionare direttamente un collegamento alla tabella nel selettore **Valore** e confermare. In tal caso, i valori disponibili per la tabella selezionata devono essere selezionati utilizzando un selettore dedicato, come illustrato nell’esempio seguente.

+++Esempio di query

Qui, la query è targeting marchi la cui etichetta è &quot;in esecuzione&quot;.

1. Navigare all&#39;interno della **tabella Brand** e selezionare l&#39;attributo **Etichetta** .

   ![Schermata della tabella Brand (Marchio)](assets/1-1-attribute.png){zoomable="yes"}{width="85%" align="center"}

1. Definire il valore previsto per l&#39;attributo.

   ![Esempio di valore atteso definito](assets/1-1-table.png){zoomable="yes"}{width="85%" align="center"}

Ecco un esempio di query in cui è stato selezionato direttamente un collegare di tabella. I valori disponibili per questa tabella devono essere selezionati da un selettore dedicato.

![Esempio di query di esempio](assets/1-1-table-direct.png){zoomable="yes"}{width="85%" align="center"}

+++

Per un **collegare** 1-N, è possibile definire sottocondizioni per perfezionare la query, come illustrato nell&#39;esempio seguente.

+++Esempio di query

In questo caso, la query è rivolta a destinatari che hanno effettuato acquisti relativi al prodotto BrewMaster, per un importo totale di almeno 100$.

1. Seleziona la **tabella Acquisti** e conferma.

   ![Schermata della tabella Acquisti](assets/1-N-collection.png){zoomable="yes"}{width="50%" align="center"}

1. Viene aggiunto un transizione in uscita che consente di creare sottocondizioni.

   ![Esempio di transizione in uscita](assets/1-n-subcondition.png){zoomable="yes"}{width="85%" align="center"}

1. Seleziona l&#39;attributo **Prezzo** e destinazione acquisti a partire da 1000

   ![Schermata dell&#39;attributo Price](assets/1-n-price.png){zoomable="yes"}{width="85%" align="center"}

1. Aggiungi condizioni secondarie in base alle tue esigenze. Qui abbiamo aggiunto una condizione ai profili di destinazione che hanno acquistato un prodotto BrewMaster.

   ![Esempio di sottocondizioni](assets/custom-condition-1-N.png){zoomable="yes"}{width="85%" align="center"}

+++

#### Utilizzare i dati aggregato {#aggregate}

Condizioni personalizzate consentono di eseguire operazioni aggregato. Per fare ciò, è necessario selezionare direttamente un attributo da una tabella raccolta:

1. Spostarsi all&#39;interno della tabella dei raccolta desiderata e selezionare l&#39;attributo per il quale si desidera eseguire un&#39;operazione aggregato.

   ![Schermata dell&#39;elenco di attributi](assets/aggregate-attribute.png){zoomable="yes"}{width="85%" align="center"}

1. Nel riquadro delle proprietà, attivare l&#39;opzione **Aggregate data** e selezionare la funzione di aggregazione desiderata.

   ![Schermata dell&#39;opzione Aggregate data](assets/aggregate.png){zoomable="yes"}{width="85%" align="center"}

### Selezionare un pubblico {#audiences}

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_selectaudience"
>title="Selezionare il tipo di pubblico"
>abstract="Utilizzando l’opzione **Seleziona pubblico**, puoi scegliere il pubblico da utilizzare per filtrare la query."

Per filtrare la query utilizzando un pubblico esistente, effettua le seguenti operazioni:

1. Fai clic sul pulsante **+** sul nodo desiderato e scegli **[!UICONTROL Seleziona pubblico]**.

1. Il pannello delle proprietà **Seleziona pubblico** si apre sul lato destro. Scegli il pubblico che desideri utilizzare per filtrare la query.

   *Esempio di query che restituisce tutti i profili appartenenti al pubblico “Partecipanti al festival”:*

   ![Schermata di un esempio di query](assets/query-audience.png){zoomable="yes"}

### Utilizzare un filtro preimpostato {#predefined-filters}

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_predefinedfilter"
>title="Filtro preimpostato"
>abstract="Con l’opzione **Filtro preimpostato** puoi selezionare un filtro preimpostato dall’elenco dei filtri personalizzati o dai preferiti."

Per filtrare la query utilizzando un filtro preimpostato, effettua le seguenti operazioni:

1. Fai clic sul pulsante **+** sul nodo desiderato e seleziona **[!UICONTROL Filtro preimpostato]**.

1. Il pannello delle proprietà **Filtro preimpostato** si apre sul lato destro. Seleziona un filtro preimpostato dall’elenco dei filtri personalizzati o dai preferiti.

   *Esempio di query che restituisce tutti i profili corrispondenti al filtro preimpostato “Clienti inattivi”:*

   ![Schermata di un esempio di query](assets/query-predefined-filter.png){zoomable="yes"}

### Copiare e incollare componenti {#copy}

Query Modeler consente di copiare uno o più componenti di filtro e incollarli al termine di una transizione. Questa operazione può essere eseguita nell’area di lavoro query corrente o in qualsiasi area di lavoro all’interno dell’istanza.

>[!NOTE]
>
>La selezione copiata viene mantenuta per tutto il tempo in cui si lavora in istanza. Se ti disconnetti ed esegui nuovamente l&#39;accesso, la selezione non sarà più disponibile per essere incollata.

Per copiare e incollare i componenti filtranti, seguire seguenti operazioni:

1. Seleziona il componente di filtro che desideri copiare facendo clic su di esso nell&#39;area di lavoro della query. Per selezionare più componenti, usa il strumento di selezione multipla disponibile nella barra degli strumenti situata nell&#39;angolo superiore destro del quadro.

1. Fare clic sul **[!UICONTROL pulsante Copia]** nel riquadro delle proprietà del componente o sulla barra blu nella parte inferiore dello schermo se sono stati selezionati più componenti.

   | Copiare un singolo componente | Copiare più componenti |
   |  ---  |  ---  |
   | ![](assets/copy-single-component.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} | ![](assets/copy-multiple-components.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} |

1. Per incollare i componenti, fai clic sul pulsante + alla fine della transizione desiderata e seleziona **Incolla n elementi**.

   ![Esempio di incollamento dei componenti](assets/copy-paste.png){zoomable="yes"}

## Combinare componenti di filtraggio con operatori {#operators}

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_group"
>title="Gruppo"
>abstract="In questo riquadro, puoi modificare l’operatore utilizzato per collegare insieme più condizioni di filtro."

Ogni volta che si aggiunge un nuovo componente di filtro alla query, questo viene automaticamente collegato all&#39;altro componente da un operatore **AND**. Ciò significa che i risultati dei due componenti di filtraggio sono combinati.

In questo esempio, è stato aggiunto un nuovo componente di filtraggio per il tipo di pubblico alla seconda transizione. Il componente è collegato alla condizione di filtro predefinita con un operatore **AND**, il che significa che i risultati della query includono destinatari del filtro predefinito &quot;Madridians&quot; E appartenenti al pubblico &quot;Discount hunters&quot;.

![Esempio di query](assets/query-operator.png){zoomable="yes"}

Per modificare l&#39;operatore utilizzato per collegare insieme le condizioni di filtraggio, fare clic su di esso e selezionare l&#39;operatore desiderato nel **riquadro Gruppo** che si apre sul lato destro.

Gli operatori disponibili sono:

* **AND (intersezione)**: combina i risultati che corrispondono a tutti i componenti di filtraggio nelle transizioni in uscita.
* **OR (Unione)**: include i risultati che corrispondono ad almeno uno dei componenti di filtraggio nelle transizioni in uscita.
* **ECCETTO (esclusione)**: esclude i risultati che corrispondono a tutti i componenti di filtraggio nella transizione in uscita.

![Esempio di query](assets/query-operator-change.png){zoomable="yes"}

Inoltre, è possibile creare gruppi intermedi di componenti facendo clic sul **simbolo +** pulsante in un transizione. In questo modo è possibile aggiungere un operatore in questa posizione specifica per raggruppare più componenti e perfezionare la query.

Nell&#39;esempio riportato di seguito, abbiamo creato un gruppo intermedio per includere i risultati del pubblico &quot;VIP premiare&quot; o &quot;Super VIP&quot;.

![Esempio di query](assets/query-intermediate-group.png){zoomable="yes"}

## Controllare e convalidare la query

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_ruleproperties"
>title="Proprietà delle regole"
>abstract="Dopo aver creato la query nell’area di lavoro, puoi verificarla utilizzando il riquadro **Proprietà delle regole** sul lato destro.<br/>Questo riquadro consente di visualizzare i dati risultanti, recuperare una versione del codice SQL della query e verificare il numero di record target.<br/>Utilizza il pulsante **Seleziona o salva il filtro** per salvare la query come filtro preimpostato o sostituisci il contenuto dell’area di lavoro con un filtro esistente."

Una volta creata la query nell&#39;area di lavoro, puoi verificarla usando il riquadro delle proprietà&#x200B;**della** regola situato sul lato destro Questo riquadro viene visualizzato quando crei una query per creare un&#39;audience. Le operazioni disponibili sono:

* **Visualizza risultati:** visualizza i dati risultanti dalla query.
* **Vista codice**: visualizza una versione della query basata su codice in SQL.
* **Calcola**: aggiorna e visualizza il numero di record interessati dalla query.
* **Selezionare o salvare il filtro**: scegli un filtro preimpostato esistente da utilizzare nell’area di lavoro oppure salva la query come filtro preimpostato per riutilizzarla in futuro. [Scopri come utilizzare i filtri preimpostati](../get-started/predefined-filters.md)

  >[!IMPORTANT]
  >
  >La selezione di un filtro preimpostato dal pannello Proprietà regole sostituisce la query creata nell’area di lavoro con il filtro selezionato.

Quando la query è pronta, fai clic sull&#39;pulsante **[!UICONTROL Conferma]** nell&#39;angolo in alto a destra per salvarla.

Puoi modificare la query in qualsiasi momento aprendola. Tenere presente che all&#39;apertura di una query esistente, questa viene visualizzata in una visualizzazione semplificata senza la visibilità di **+** pulsanti. Per aggiungere nuovi elementi alla query, selezionare un componente o un operatore nell&#39;area di lavoro per visualizzare i pulsanti **+**.

![Esempio di query](assets/edit-audience.png){zoomable="yes"}

