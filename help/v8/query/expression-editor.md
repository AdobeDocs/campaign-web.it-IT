---
audience: end-user
title: Creare la prima query utilizzando il modellatore di query
description: Scopri come creare la prima query in Adobe Campaign Web Query Modeler.
source-git-commit: e620df0ff9af0d32fc353a904e3dde37501495d0
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 79%

---

# Modificare le espressioni {#expression}

La modifica di un’espressione comporta l’immissione manuale di condizioni per formare una regola. Questa modalità ti consente di utilizzare funzioni avanzate. Queste funzioni ti consentono di manipolare i valori utilizzati per eseguire query specifiche, come la manipolazione di date, stringhe, campi numerici, ordinamento e così via.

Queste operazioni sono disponibili dal pulsante Modifica espressione di Query Modeler, disponibile per i campi Attributo e Valore durante la configurazione di una condizione personalizzata.

![](assets/edit-expression.png)

L’editor di espressioni fornisce:

* Un campo di input in cui è definita l’espressione.
* L’elenco dei campi disponibili che possono essere utilizzati nell’espressione e che corrispondono alla dimensione di targeting della query.
* L’elenco delle funzioni disponibili, ordinate per categoria.

Modifica l’espressione immettendo un’espressione direttamente nel campo di input o utilizzando gli elenchi dei campi e delle funzioni disponibili. A questo scopo, posizionare il cursore nell&#39;espressione inexpression nel punto in cui si desidera aggiungere l&#39;elemento e fare doppio clic sul campo o sull&#39;espressione desiderata.

È possibile utilizzare le variabili degli eventi dei flussi di lavoro per generare un’espressione. Per ulteriori informazioni, consulta xxxx.

## Sintassi delle espressioni {#expression-syntax}

### Sintassi standard {#standard-syntax}

Le espressioni standard sono composte da una o più condizioni che rispettano i seguenti elementi di sintassi:

* Ciascuna condizione assume la forma di **&lt;valore1> &lt;operatore di confronto> &lt;valore2>** in cui:

   * **&lt;valore1>** è un campo o una funzione. Ad esempio, **@created** per la data di creazione di un profilo oppure **Year(@created)** per l’anno di creazione di un profilo.
   * **&lt;comparison operator=&quot;&quot;>** è uno degli operatori elencati nella sezione Operatori di confronto. Questo operatore definisce il metodo di confronto tra **&lt;valore1>** e **&lt;valore2>**.
   * **&lt;valore2>** è un campo, una funzione o un valore immesso manualmente.

  >[!NOTE]
  >
  >I dati del tipo **&lt;valore1>** e **&lt;valore2>** devono essere identici. Ad esempio, se **&lt;valore1>** è una data, anche **&lt;valore2>** deve essere una data.

* Se desideri utilizzare diverse condizioni, puoi combinarle utilizzando operatori logici.

   * **[!UICONTROL E]**: due condizioni sono intersecate.
   * **[!UICONTROL OPPURE]**: due condizioni sono combinate.

Ad esempio:

```
Year(@created) = Year(GetDate()) AND Month(@created) = Month(GetDate())
```

In questo esempio, i profili la cui data di creazione è nel mese e nell’anno correnti sono oggetto di targeting.

### Sintassi JavaScript {#javascript-syntax}

Durante la definizione delle condizioni di visibilità di un blocco di testo dell’editor di contenuti HTML, devi utilizzare un’espressione con sintassi di tipo JavaScript.

Le espressioni JavaScript sono composte da una o più condizioni e utilizzano i seguenti elementi di sintassi:

* Ciascuna condizione assume la forma di **&lt;contesto> &lt;operatore di confronto> &lt;valore2>** in cui:

   * **&lt;contesto>** è un campo o una funzione che consente di specificare il contesto. Ad esempio **context.profile.@email** per l’indirizzo e-mail di un profilo o **context.profile.firstName.length()** per il numero di caratteri del nome di un profilo.
   * **&lt;comparison operator=&quot;&quot;>** è uno degli operatori elencati nella sezione Operatori di confronto. Questo operatore definisce il metodo di confronto tra **&lt;contesto>** e **&lt;valore2>**.
   * **&lt;valore2>** è un campo, una funzione o un valore immesso manualmente.

  >[!NOTE]
  >
  I dati del tipo **&lt;contesto>** e **&lt;valore2>** devono essere identici. Ad esempio, se **&lt;contesto>** è una data, anche **&lt;valore2>** deve essere una data.

* Se desideri utilizzare diverse condizioni, puoi combinarle utilizzando operatori logici.

   * **[!UICONTROL &amp;&amp;]**: due condizioni sono intersecate.
   * **[!UICONTROL ||]**: due condizioni sono combinate.

Ad esempio:

```
context.profile.age > 21 && context.profile.firstName.length() > 0
```

In questo esempio, i profili di età superiore a 21 anni il cui nome è stato fornito (rappresentato dal fatto che il campo **firstName** contiene almeno un carattere).

## Operatori di confronto {#comparison-operators}

Per alcune regole, l’editor delle query ti consente di scegliere un valore per definire la condizione.

Le condizioni devono essere collegate ai valori utilizzando uno dei seguenti operatori.

<table> 
 <thead> 
  <tr> 
   <th> Operatore<br /> </th> 
   <th> Sintassi standard<br /> </th> 
   <th> Sintassi JavaScript<br /> </th> 
   <th> Descrizione<br /> </th> 
   <th> Esempio<br /> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <span class="uicontrol">Uguale a</span> <br /> </td> 
   <td> =<br /> </td> 
   <td> ==<br /> </td> 
   <td> Il primo valore deve essere del tutto identico al secondo valore.<br /> </td> 
   <td> <strong>@lastName = Martin</strong> recupera i profili il cui cognome è “Martin”, contenenti solo questi stessi caratteri.<br /> </td> 
  </tr> 
  <tr> 
   <td> <span class="uicontrol">Maggiore di</span> <br /> </td> 
   <td> &gt;<br /> </td> 
   <td> &gt;<br /> </td> 
   <td> Il primo valore deve essere categoricamente maggiore del secondo valore.<br /> </td> 
   <td> <strong>@age &gt; 50</strong> recupera i profili con età maggiore di “50”, quindi “51”, “52”, ecc.<br /> </td> 
  </tr> 
  <tr> 
   <td> <span class="uicontrol">Minore di</span> <br /> </td> 
   <td> &lt;<br /> </td> 
   <td> &lt;<br /> </td> 
   <td> Il primo valore deve essere categoricamente minore del secondo valore.<br /> </td> 
   <td> <strong>@created &lt; DaysAgo(100)</strong> recupera tutti i profili creati nel database meno di 100 giorni fa.<br /> </td> 
  </tr> 
  <tr> 
   <td> <span class="uicontrol">Maggiore o uguale a</span> <br /> </td> 
   <td> &gt;=<br /> </td> 
   <td> &gt;=<br /> </td> 
   <td> Il primo valore deve essere maggiore o uguale al secondo valore.<br /> </td> 
   <td> <strong>@age &gt;= 30</strong> recupera i profili di età maggiore o uguale a 30 anni.<br /> </td> 
  </tr> 
  <tr> 
   <td> <span class="uicontrol">Minore o uguale a</span> <br /> </td> 
   <td> &lt;=<br /> </td> 
   <td> &lt;=<br /> </td> 
   <td> Il primo valore deve essere minore o uguale al secondo valore.<br /> </td> 
   <td> <strong>@age &lt;= 60</strong> recupera i profili di età minore o uguale a 60 anni.<br /> </td> 
  </tr> 
  <tr> 
   <td> <span class="uicontrol">Diverso </span> <br /> </td> 
   <td> !=<br /> </td> 
   <td> !=<br /> </td> 
   <td> Il primo valore deve essere diverso dal secondo valore.<br /> </td> 
   <td> <strong>@language != English</strong> recupera i profili che non sono stati definiti come anglofoni.<br /> </td> 
  </tr> 
  <tr> 
   <td> <span class="uicontrol">Contiene</span> <br /> </td> 
   <td> IN<br /> </td> 
   <td> N/D<br /> </td> 
   <td> Il primo valore deve contenere il secondo valore.<br /> </td> 
   <td> <strong>@domain IN mail</strong>. In questo caso, tutti i nomi di dominio con il valore “mail” vengono restituiti nel risultato. Di conseguenza, il nome di dominio “gmail.com” farà parte dei risultati restituiti.<br /> </td> 
  </tr> 
  <tr> 
   <td> <span class="uicontrol">Simile</span> <br /> </td> 
   <td> LIKE<br /> </td> 
   <td> N/D<br /> </td> 
   <td> <span class="uicontrol">Simile</span> è molto simile all’operatore <span class="uicontrol">Contains</span>. Ti consente di inserire un carattere jolly <span class="uicontrol">%</span> nel valore ricercato.<br /> </td> 
   <td> <strong>@lastName LIKE Mart%n</strong>. In questo caso, il carattere di sostituzione <strong>%</strong> serve come un "jolly" per trovare il nome "Martin" nel caso ipotetico che l’ortografia non sia corretta.<br /> </td> 
  </tr> 
  <tr> 
   <td> <span class="uicontrol">Diverso</span> <br /> </td> 
   <td> NOT<br /> </td> 
   <td> N/D<br /> </td> 
   <td> È simile a <span class="uicontrol">Simile</span>. Ti consente di non recuperare il valore immesso. Anche in questo caso, il valore immesso deve contenere il carattere jolly <span class="uicontrol">%</span>.<br /> </td> 
   <td> <strong>@lastName NOT Smi%h</strong>. In questo caso, i destinatari corrispondono al nome “Smi%h” (quindi Smith, ecc.) non vengono restituiti come risultato.<br /> </td> 
  </tr> 
  <tr> 
   <td> <span class="uicontrol">È vuoto</span> <br /> </td> 
   <td> IS NULL<br /> </td> 
   <td> N/D<br /> </td> 
   <td> Il primo valore deve corrispondere a un valore vuoto.<br /> </td> 
   <td> <strong>@mobilePhone IS NULL</strong> recupera tutti i profili il cui numero di telefono cellulare non è stato fornito.<br /> </td> 
  </tr> 
 </tbody> 
</table>