---
audience: end-user
title: Impostare un gruppo di controllo
description: Scopri come impostare un gruppo di controllo per i messaggi nell’interfaccia utente web di Campaign
exl-id: 02f3adec-681a-4cec-a895-41c80eb345db
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '799'
ht-degree: 36%

---

# Impostare un gruppo di controllo {#control-group}

Un gruppo di controllo è una sottopopolazione esclusa dalla consegna. Puoi definire un gruppo di controllo per evitare di inviare messaggi a una parte del pubblico e confrontare il comportamento successivo alla consegna con il target principale. Questa opzione consente di misurare l’impatto della campagna.

➡️ [Scopri questa funzione nel video](create-audience.md#video)

## Abilita gruppo di controllo {#add-a-control-group}

Per aggiungere un gruppo di controllo, abilita questa opzione durante la definizione del pubblico della consegna. Il gruppo di controllo può essere estratto in modo casuale dal target principale o selezionato da una popolazione specifica. Di conseguenza, esistono due modi principali per definire un gruppo di controllo:

* Estrarre un certo numero di profili dal target principale.
* Escludi alcuni profili da un elenco o in base ai criteri definiti in una query.

Quando si definisce un gruppo di controllo, è possibile usare entrambi questi metodi.

Tutti i profili inclusi nel gruppo di controllo nella fase di preparazione della consegna vengono rimossi dal target principale. e non riceveranno il messaggio.

>[!CAUTION]
>
>Non è possibile utilizzare i gruppi di controllo quando si carica la popolazione target [da un file esterno](file-audience.md).

Per aggiungere un gruppo di controllo a una consegna, attiva l&#39;interruttore **[!UICONTROL Abilita gruppo di controllo]** dalla sezione **Pubblico** della schermata di creazione della consegna.

![Attiva opzione gruppo di controllo nella schermata di creazione della consegna](assets/control-group1.png)

## Estrarre dal target {#extract-target}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_target"
>title="Modalità estrazione"
>abstract="Un gruppo di controllo è un set di profili esclusi dalla consegna. Per definire un gruppo di controllo, puoi scegliere di estrarre dalla popolazione target una percentuale o un numero fisso di profili, in modo casuale o in base a un ordinamento."

### Creare un gruppo di controllo {#build-extract-target}

Per definire un gruppo di controllo, scegli di estrarre dalla popolazione target una percentuale o un numero fisso di profili, in modo casuale o in base a un ordinamento. Se aggiungi una popolazione aggiuntiva, scegli l&#39;opzione **Nessuna estrazione** e seleziona la popolazione aggiuntiva [come descritto qui](#extra-population).

Innanzitutto, definisci il modo in cui i profili vengono estratti dal target: in modo casuale o in base a un ordinamento.

Nella sezione **Gruppo di controllo**, scegli una **Modalità estrazione**:

* **Casuale**: durante la preparazione della consegna, Adobe Campaign estrae in modo casuale un numero di profili corrispondente alla percentuale o al numero massimo impostato come limite di dimensioni.
* **Classificati per attributi**: questa opzione esclude un set di profili basati su attributi specifici in un ordinamento specifico.

Quindi, utilizza la sezione **Limite dimensioni** per impostare il numero di profili da estrarre dalla destinazione principale. Può essere un numero non elaborato (ad esempio, 50 profili da escludere) o una percentuale del pubblico iniziale (ad esempio, 5% del target principale).

### Esempio di gruppo di controllo {#control-group-sample}

Ad esempio, per creare un gruppo di controllo con i 100 profili più giovani, segui questi passaggi:

1. Seleziona il campo **Età** come criterio di ordinamento. Lascia l’opzione di ordinamento **Crescente**.
1. Aggiungi il campo **Data di creazione**. Seleziona l’opzione di ordinamento **Decrescente**.
1. Definisci 100 come soglia nella sezione **Dimensione limite**.

   ![Configurazione gruppo di controllo per profili più giovani](assets/control-group2.png){zoomable="yes"}

Questi 100 profili più giovani sono quindi esclusi dal target principale.

### Verificare il gruppo di controllo {#check-control-group}

Visualizza i registri per verificare e identificare i profili esclusi. Ad esempio, considera un’esclusione casuale di cinque profili.

![Esempio di profili esclusi nei registri](assets/control-group4.png){zoomable="yes"}

Dopo la preparazione della consegna, controlla come sono state applicate le esclusioni:

* Nel dashboard di consegna, prima dell&#39;invio, controlla l&#39;indicatore KPI **Da escludere**.

  ![Dashboard di consegna che mostra l&#39;indicatore KPI &quot;Da escludere&quot;](assets/control-group5.png){zoomable="yes"}

* Nei registri di consegna, la scheda Registri mostra il passaggio di esclusione.

  ![Registri di consegna che mostrano il passaggio di esclusione](assets/control-group-sample-logs.png){zoomable="yes"}

<!--

 * The **Exclusion logs** tab displays each profile and the related exclusion **Reason**.

    ![](assets/control-group6.png){zoomable="yes"}

-->

* Nella scheda **Exclusion causes** viene visualizzato il numero di profili esclusi per ogni regola di tipologia.

  ![La scheda Cause di esclusione mostra le esclusioni delle regole di tipologia](assets/control-group7.png){zoomable="yes"}

Per ulteriori informazioni sui registri di consegna, consulta questa [sezione](../monitor/delivery-logs.md).

## Aggiungere una popolazione aggiuntiva {#extra-population}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_extra"
>title="Popolazione aggiuntiva"
>abstract="Un gruppo di controllo è un set di profili esclusi dalla consegna. Per escludere una popolazione specifica dal pubblico della consegna, puoi selezionare un pubblico esistente o definire una query."

Un altro modo per definire un gruppo di controllo consiste nel selezionare una popolazione specifica in un pubblico esistente o nel definire una query.

Nella sezione **Popolazione aggiuntiva** della schermata di definizione del **Gruppo di controllo**, fai clic sul pulsante **[!UICONTROL Seleziona pubblico]**.

![Schermata di selezione popolazione aggiuntiva](assets/control-group3.png){zoomable="yes"}

* Per utilizzare un pubblico esistente, fai clic su **Seleziona pubblico**. Per ulteriori informazioni, consulta [questa sezione](add-audience.md).
* Per definire una nuova query, seleziona **Crea la tua** e definisci i criteri di esclusione utilizzando il modellatore di query. Per ulteriori informazioni, consulta [questa sezione](../query/query-modeler-overview.md).

I profili inclusi nel pubblico o corrispondenti al risultato della query sono **esclusi** dal target di consegna. Non ricevono alcun messaggio.

## Confrontare i risultati {#control-group-results}

Una volta inviata la consegna, estrai i registri di invio per confrontare il comportamento tra i profili che non hanno ricevuto la comunicazione e il target effettivo. Utilizza i registri di consegna per creare un nuovo targeting.

Per vedere quali profili sono stati rimossi dal target, controlla i **Registri di consegna**. Per ulteriori informazioni, consulta [questa sezione](#check-control-group).