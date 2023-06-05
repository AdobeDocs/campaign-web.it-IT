---
product: campaign
title: Utilizzare i modelli di consegna
description: Scopri come creare e utilizzare i modelli di consegna in Campaign
feature: Email, Push, SMS, Direct Mail, Cross Channel Orchestration
role: User
level: Beginner
exl-id: 4a8513bb-8290-432a-8e40-822cd1337cb3
source-git-commit: 84ef79098494236d3ea2d3b46b72280603ad5c94
workflow-type: tm+mt
source-wordcount: '921'
ht-degree: 4%

---

# Utilizzare i modelli di consegna {#work-with-delivery-templates}

Per un processo di progettazione accelerato e migliorato, puoi creare modelli di consegna per riutilizzare facilmente i contenuti personalizzati nelle campagne. Questa funzionalità consente di standardizzare l’aspetto creativo per velocizzare l’esecuzione e il lancio delle campagne.

Un modello può includere:

<!--[Typologies](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/campaign-typologies.html)?
Sender and reply-to addresses?-->
* Un [pubblico](../audience/about-audiences.md), tra cui [gruppi di controllo](../audience/control-group.md)
* Personalizzato [contenuto](../content/edit-content.md)<!--company logo, or signature-->
* [Campi personalizzati](../personalization/personalize.md) e [contenuto condizionale](../personalization/conditions.md) <!--basic [personalization blocks](../personalization/personalize.md#ootb-content-blocks)-->
* Collegamenti a [pagina mirror](../content/mirror-page.md) e annullamento dell’abbonamento [collegamenti](../content/message-tracking.md)

<!--Other delivery properties, such as resource validity, retry parameters, or quarantine settings.-->

## Accedere e gestire i modelli {#access-manage-templates}

>[!CONTEXTUALHELP]
>id="acw_delivery_templates"
>title="Utilizzare i modelli di consegna"
>abstract="Utilizza i modelli di consegna per creare e salvare facilmente le consegne esistenti per utilizzi futuri."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/delivery-template.html#copy-an-existing-template" text="Duplica un modello esistente"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/delivery-template.html#convert-an-existing-delivery" text="Convertire una consegna in un modello"

Per accedere all&#39;elenco dei modelli di contenuto, selezionare **[!UICONTROL Campaign Management]** > **[!UICONTROL Consegne]** dal menu a sinistra e passare alla **Modelli** scheda.

![](assets/templates-tab.png)

Tutti i modelli che erano [creato](#create-a-delivery-template) nell&#39;ambiente corrente.

Puoi filtrare i modelli di contenuto per canali e cartelle. Puoi anche impostare filtri avanzati creando una regola utilizzando gli attributi di consegna. [Ulteriori informazioni sul generatore di regole](../audience/segment-builder.md)

![](assets/templates-filters.png)

Per modificare un modello, fai clic sull’elemento desiderato dall’elenco. Da lì:

* Puoi modificarne il contenuto, le proprietà, il pubblico e tutte le offerte associate.
* Puoi anche verificare il modello. [Ulteriori informazioni](#test-template)

![](assets/templates-edition.png)

Per eliminare o [duplicare](#copy-an-existing-template) in un modello, seleziona l’azione corrispondente da **[!UICONTROL Altre azioni]** dal menu **[!UICONTROL Modelli]** o da una schermata di modifica dei modelli.

![](assets/templates-more-actions.png)

>[!NOTE]
>
>Quando un modello viene modificato o eliminato, le consegne create utilizzando questo modello non sono interessate.

## Creare un modello {#create-a-delivery-template}

Per creare un modello di consegna, puoi:
* Duplica un modello esistente - [Ulteriori informazioni](#copy-an-existing-template)
* Convertire una consegna esistente in un modello - [Ulteriori informazioni](#convert-an-existing-delivery)
* Creare un modello di consegna da zero - [Ulteriori informazioni](#create-a-new-template)

### Duplica un modello esistente {#copy-an-existing-template}

Campaign è dotato di un set di modelli incorporati per ogni canale: e-mail, push, SMS. Il modo più semplice per creare un modello di consegna è duplicare e personalizzare un modello incorporato.

>[!NOTE]
>
>Puoi anche duplicare qualsiasi modello personalizzato.

Per duplicare un modello di consegna, effettua le seguenti operazioni:

1. Accedi a **Modelli** , dalla scheda **Consegne** menu a sinistra. [Ulteriori informazioni](#access-manage-templates)
1. Fai clic su **[!UICONTROL Altre azioni]** a destra del nome del modello desiderato e seleziona  **[!UICONTROL Duplica]**.

   Puoi anche selezionare un modello dall’elenco e selezionare questa opzione dalla schermata dell’edizione del modello.

1. Conferma la duplicazione.

   ![](assets/templates-duplicate-confirm.png)

1. Il nuovo dashboard modelli si apre nella schermata centrale. Modifica le impostazioni del modello in base alle esigenze.

   ![](assets/templates-duplicated-item.png)

1. Fai clic su **[!UICONTROL Revisione]** per salvare e rivedere il modello. Puoi comunque modificarne tutte le impostazioni, eliminarle e duplicarle.

   ![](assets/templates-review-screen.png)

1. Se necessario, verifica il rendering del modello. [Ulteriori informazioni](#test-template)

Il nuovo modello viene aggiunto al [**Modelli** list](#access-manage-templates). Ora puoi selezionarlo durante la creazione di una nuova consegna.

### Convertire una consegna in un modello {#convert-an-existing-delivery}

Qualsiasi consegna può essere convertita in un modello per future azioni di consegna ripetute.

Per salvare una consegna come modello, effettua le seguenti operazioni:

1. Vai a **[!UICONTROL Gestione delle campagne]** > **[!UICONTROL Consegne]** menu.
1. Dalla sezione **[!UICONTROL Sfoglia]** , fare clic sulla scheda **[!UICONTROL Altre azioni]** a destra del nome della consegna desiderata e seleziona **[!UICONTROL Copia come modello]**.

   ![](assets/templates-convert-delivery.png)

1. Conferma la duplicazione.

1. Il nuovo dashboard modelli si apre nella schermata centrale. Modifica le impostazioni del modello in base alle esigenze.

1. Fai clic su **[!UICONTROL Revisione]** per salvare e rivedere il modello. Puoi comunque modificarne tutte le impostazioni, eliminarle e duplicarle.

1. Se necessario, verifica il rendering del modello. [Ulteriori informazioni](#test-template)

Il nuovo modello viene aggiunto al [**Modelli** list](#access-manage-templates). Ora puoi selezionarlo durante la creazione di una nuova consegna.

### Crea un nuovo modello {#create-a-new-template}

>[!NOTE]
>
>Per evitare errori di configurazione, l’Adobe consiglia di: [duplicare un modello incorporato](#copy-an-existing-template) e personalizzarne le proprietà anziché creare un nuovo modello.

Per configurare un modello di consegna da zero, segui i passaggi seguenti:

1. Accedi a **Modelli** , dalla scheda **Consegne** menu a sinistra. [Ulteriori informazioni](#access-manage-templates)
1. Fai clic su **[!UICONTROL Crea modello]** pulsante.

   ![](assets/templates-create-button.png)

1. Seleziona il canale da utilizzare per il modello.
1. Per impostazione predefinita, viene utilizzato il modello di consegna integrato per tale canale per facilitare la creazione di un modello personalizzato. Se necessario, utilizza il pulsante dedicato a destra del canale selezionato per selezionare un altro modello.

   ![](assets/templates-channel-browse.png)

1. Fai clic su **[!UICONTROL Crea modello]** pulsante di nuovo.

1. Definire le proprietà del modello, [pubblico](../audience/add-audience.md) e il contenuto a seconda del canale selezionato.

   >[!NOTE]
   >
   >Ulteriori informazioni sui canali di consegna e su come progettare i rispettivi contenuti sono disponibili nelle sezioni seguenti:
   >
   > * [Canale e-mail](../email/create-email.md)
   > * [Canale di notifica push](../push/gs-push.md)
   > * [Canale SMS](../sms/create-sms.md)


1. Fai clic su **[!UICONTROL Revisione]** per salvare e rivedere il modello. Puoi comunque modificarne tutte le impostazioni, eliminarle e duplicarle.

1. Se necessario, verifica il rendering del modello. [Ulteriori informazioni](#test-template)

Il nuovo modello viene aggiunto al [**Modelli** list](#access-manage-templates). Ora puoi selezionarlo durante la creazione di una nuova consegna.

## Testare un modello di consegna {#test-template}

Puoi verificare il rendering di qualsiasi modello di consegna, creato da zero o da un contenuto esistente. A questo scopo, segui i passaggi riportati qui sotto.

1. Accedi a **Modelli** tramite il **[!UICONTROL Gestione delle campagne]** > **[!UICONTROL Consegne]** e selezionare un modello. [Ulteriori informazioni](#access-manage-templates)

1. Fai clic su **[!UICONTROL Simula contenuto]** in alto a destra.

   ![](assets/templates-simulate-button.png)

1. Seleziona uno o più profili di test per controllare il rendering delle e-mail. Puoi anche selezionare profili reali dal database.

1. Passa da un profilo all’altro per ottenere una rappresentazione personalizzata del messaggio in base al profilo selezionato.

   <!--[Learn moreon test profiles](../preview-test/proofs.md#recipients)-->

   È inoltre possibile regolare il livello di zoom e scegliere la visualizzazione desktop o mobile.

   ![](assets/templates-stimulate.png)

1. Chiudere la finestra per tornare alla schermata dell&#39;edizione del modello.

>[!NOTE]
>
>Non puoi utilizzare il rendering di e-mail o inviare bozze in un modello di consegna.

* [Ulteriori informazioni sull’anteprima del contenuto delle e-mail](../preview-test/preview-content.md)

* [Ulteriori informazioni sull’anteprima del contenuto SMS](../sms/content-sms.md)

* [Ulteriori informazioni sull’anteprima dei contenuti push](../push/gs-push.md)


