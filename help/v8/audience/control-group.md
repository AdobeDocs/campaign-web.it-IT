---
audience: end-user
title: Impostare un gruppo di controllo
description: Scopri come impostare un gruppo di controllo per i messaggi nell’interfaccia utente di Campaign Web
exl-id: 02f3adec-681a-4cec-a895-41c80eb345db
badge: label="Beta"
source-git-commit: 97e2d37d0a91e50b516f2fa0b6d5559f89b6c096
workflow-type: tm+mt
source-wordcount: '785'
ht-degree: 97%

---

# Impostare un gruppo di controllo {#control-group}

Un gruppo di controllo è una sottopopolazione esclusa dalla consegna. Puoi definire un gruppo di controllo per evitare di inviare messaggi a una parte del pubblico e confrontare il comportamento successivo alla consegna rispetto al target principale. Questa opzione consente di misurare l’impatto della campagna.

## Abilita gruppo di controllo{#add-a-control-group}

Per aggiungere un gruppo di controllo, abilita questa opzione durante la definizione del pubblico della consegna. Il gruppo di controllo può essere estratto in modo casuale dal target principale e/o selezionato da una popolazione specifica. Ci sono quindi due vie principali per definire un gruppo di controllo:

* Estrarre un certo numero di profili dal target principale.
* Escludere alcuni profili da un elenco o in base ai criteri definiti in una query.

Quando si definisce un gruppo di controllo, è possibile usare entrambi questi metodi.

Tutti i profili che fanno parte del gruppo di controllo nella fase di preparazione della consegna verranno rimossi dal target principale e non riceveranno il messaggio.

>[!CAUTION]
>
>Non è possibile utilizzare i gruppi di controllo quando si carica la popolazione target [da un file esterno](file-audience.md).

Per aggiungere un gruppo di controllo a una consegna, attiva l’opzione **[!UICONTROL Abilita gruppo di controllo]**, nella sezione **Pubblico** della schermata di creazione della consegna.

![Opzione Abilita gruppo di controllo](assets/control-group1.png)


## Estrarre dal target {#extract-target}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_target"
>title="Modalità estrazione"
>abstract="Un gruppo di controllo è un set di profili esclusi dalla consegna. Per definire un gruppo di controllo, puoi scegliere di estrarre dalla popolazione target una percentuale o un numero fisso di profili, in modo casuale o in base a un ordinamento."


### Creare un gruppo di controllo {#build-extract-target}

Per definire un gruppo di controllo, puoi scegliere di estrarre dalla popolazione target una percentuale o un numero fisso di profili, in modo casuale o in base a un ordinamento. Se preferisci aggiungere un’altra popolazione, scegli **Nessuna estrazione** e seleziona la popolazione aggiuntiva [come descritto qui](#extra-population).

Innanzitutto, definisci il modo in cui i profili verranno estratti dal target: in modo casuale o in base a un ordinamento.

Nella sezione **Gruppo di controllo**, scegli una **Modalità estrazione**:

* **Casuale**: durante la preparazione della consegna, Adobe Campaign estrarrà in modo casuale un numero di profili corrispondente alla percentuale o al numero massimo che verrà impostato come limite di dimensione.

* **Classificato per attributo/i**: questa opzione consente di escludere un set di profili in base ad attributi specifici in uno o più ordini specifici.


Quindi, nella sezione **Dimensione limite** imposta il numero di profili da estrarre dal target principale. Può essere un numero non elaborato (ad esempio 50 profili da escludere) o una percentuale del pubblico iniziale (ad esempio il 5% del target principale).


### Esempio di gruppo di controllo{#control-group-sample}

Ad esempio, per creare un gruppo di controllo con i 100 nuovi destinatari più giovani, segui questi passaggi:

1. Seleziona il campo **Età** come criterio di ordinamento. Lascia l’opzione di ordinamento **Crescente**.
1. Aggiungi il campo **Data di creazione**. Seleziona l’opzione di ordinamento **Decrescente**.
1. Definisci 100 come soglia nella sezione **Dimensione limite**.

   ![](assets/control-group2.png)

Questi 100 nuovi destinatari più giovani verranno esclusi dal target principale.

### Verificare il gruppo di controllo {#check-control-group}

Puoi visualizzare i registri per controllare e identificare i profili esclusi. Prendiamo l’esempio di un’esclusione casuale su cinque profili.

![](assets/control-group4.png)

Dopo la preparazione della consegna, puoi rivedere come sono state applicate le esclusioni:

* Nella dashboard della consegna, prima dell’invio, controlla il KPI **Da escludere**.

  ![](assets/control-group5.png)

* Nei registri di consegna, la scheda Registri mostra il passaggio di esclusione.

  ![](assets/control-group-sample-logs.png)
<!--

 * The **Exclusion logs** tab displays each profile and the related exclusion **Reason**.

    ![](assets/control-group6.png)
-->

* La scheda **Cause di esclusione** mostrano il numero di profili esclusi per ogni regola di tipologia.

  ![](assets/control-group7.png)

Per ulteriori informazioni sui registri di consegna, consulta questa [sezione](../monitor/delivery-logs.md).

## Aggiungere una popolazione aggiuntiva {#extra-population}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_extra"
>title="Popolazione aggiuntiva"
>abstract="Un gruppo di controllo è un set di profili esclusi dalla consegna. Per escludere una popolazione specifica dal pubblico della consegna, puoi selezionare un pubblico esistente o definire una query."

Un altro modo per definire un gruppo di controllo consiste nel selezionare una popolazione specifica dal pubblico esistente o definendo una query.

Nella sezione **Popolazione aggiuntiva** della schermata di definizione del **Gruppo di controllo**, fai clic sul pulsante **[!UICONTROL Seleziona pubblico]**.

![](assets/control-group3.png)

* Per utilizzare un pubblico esistente, fai clic su **Seleziona pubblico**. Per ulteriori informazioni, consulta [questa sezione](add-audience.md).

* Per definire una nuova query, seleziona **Crea il tuo** e definiscono i criteri di esclusione utilizzando Query Modeler. Per ulteriori informazioni, consulta [questa sezione](../query/query-modeler-overview.md).

I profili inclusi nel pubblico o che corrispondono al risultato della query sono **esclusi** dal target della consegna e non ricevono alcun messaggio.

## Confrontare i risultati{#control-group-results}

Una volta inviata la consegna, puoi estrarre i registri di invio per confrontare il comportamento tra i profili che non hanno ricevuto la comunicazione e il target effettivo. Puoi anche utilizzare i registri di consegna per creare un nuovo targeting.

Per vedere quali profili sono stati rimossi dal target, controlla i **Registri di consegna**. Per ulteriori informazioni, consulta [questa sezione](#check-control-group).


