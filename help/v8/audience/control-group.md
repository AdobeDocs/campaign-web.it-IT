---
audience: end-user
title: Imposta un gruppo di controllo
description: Scopri come impostare un gruppo di controllo per i messaggi nell’interfaccia utente Web di Campaign
exl-id: 02f3adec-681a-4cec-a895-41c80eb345db
source-git-commit: a59c133254632c49618fae6ad3d61a2f6e0a1eea
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 39%

---

# Imposta un gruppo di controllo {#control-group}

Puoi utilizzare i gruppi di controllo per evitare di inviare messaggi a una parte del pubblico, in modo da misurare l’impatto delle campagne.

A questo scopo, crea un gruppo di controllo quando definisci il pubblico della consegna. I profili vengono aggiunti al gruppo di controllo in modo casuale, filtrati o meno oppure in base a alcuni criteri. Puoi quindi confrontare il comportamento della popolazione di destinazione che ha ricevuto il messaggio con il comportamento dei contatti non mirati.

Il gruppo di controllo può essere estratto in modo casuale dal target principale e/o selezionato da una popolazione specifica. Ci sono quindi due vie principali per definire un gruppo di controllo:

* Estrarre un certo numero di profili dal target principale.
* Escludere alcuni profili in base ai criteri definiti in una query.

È possibile ricorrere a entrambi i metodi.

Tutti i profili che fanno parte del gruppo di controllo nella fase di preparazione della consegna verranno rimossi dal target principale, quindi non riceveranno il messaggio inviato.

Per creare un gruppo di controllo, fai clic sul pulsante **[!UICONTROL Imposta gruppo di controllo]** dal **Pubblico** della sezione dell’assistente per la creazione della consegna.

![](assets/control-group1.png)

## Estrai da target {#extract-target}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_target"
>title="Estrai da target"
>abstract="TBC"

Per definire un gruppo di controllo, puoi scegliere di estrarre dalla popolazione target una percentuale o un numero fisso di profili, in modo casuale o in base a un ordinamento.

Innanzitutto, definisci il modo in cui i profili verranno estratti dal target: in modo casuale o in base a un ordinamento.

Sotto la **Estrai dal target** sezione, scegli un **Tipo di esclusione**:

* **Casuale**: durante la preparazione della consegna, Adobe Campaign estrarrà in modo casuale un numero di profili corrispondente alla percentuale o al numero massimo che verrà impostato come limite di dimensioni.

   ![](assets/control-group.png)

* **Classificato per attributo/i**: questa opzione consente di escludere un set di profili basati su attributi specifici in uno o più ordini di ordinamento specifici.

   ![](assets/control-group2.png)

Quindi definisci il **Limite dimensione**: devi impostare il modo in cui limitare il numero di profili estratti dal target principale.

**Esempio**

Puoi visualizzare i registri per controllare e identificare i profili esclusi. Prendiamo l’esempio di un’esclusione casuale su cinque profili.

![](assets/control-group4.png)

Dopo la preparazione della consegna, puoi visualizzare le esclusioni nelle seguenti schermate:

* La **Per escludere** KPI nel dashboard di consegna, prima dell’invio.

   ![](assets/control-group5.png)

* La **Log di esclusione** visualizzare ciascun profilo e la relativa esclusione **Motivo**.

   ![](assets/control-group6.png)

* La **Cause di esclusione** visualizza il numero di profili esclusi per ogni regola di tipologia.

   ![](assets/control-group7.png)

Per ulteriori informazioni sui registri di consegna, consulta questo [sezione](../monitor/delivery-logs.md).

## Popolazione aggiuntiva {#extra-population}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_extra"
>title="Popolazione aggiuntiva"
>abstract="TBC"

Un altro modo per definire un gruppo di controllo consiste nell’escludere una popolazione specifica dal target utilizzando un pubblico esistente o definendo una query.

Da **Popolazione extra** della sezione **Gruppo di controllo** schermata di definizione, fai clic sul **[!UICONTROL Selezionare il pubblico]** pulsante .

![](assets/control-group3.png)

* Per utilizzare un pubblico esistente, fai clic su **Selezionare il pubblico**. Fai riferimento a questo [sezione](add-audience.md).

* Per definire una nuova query, seleziona **Crea il tuo** e definisci i criteri di esclusione utilizzando il generatore di regole. Fai riferimento a questo [sezione](segment-builder.md).

I profili inclusi nel pubblico o che corrispondono al risultato della query saranno esclusi dal target.