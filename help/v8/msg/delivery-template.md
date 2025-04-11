---
product: campaign
title: Utilizzare i modelli di consegna
description: Scopri come creare e utilizzare i modelli di consegna in Campaign Web
feature: Email, Push, SMS, Direct Mail, Cross Channel Orchestration
role: User
level: Beginner
exl-id: cd3d4c2d-7bb2-4574-aeb8-6aac0683ec59
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '1102'
ht-degree: 59%

---

# Utilizzare i modelli di consegna {#work-with-delivery-templates}

>[!CONTEXTUALHELP]
>id="acw_delivery_template_for_campaign"
>title="Modelli di consegna"
>abstract="Per accelerare e migliorare il processo di progettazione, crea modelli di consegna per riutilizzare contenuti e impostazioni personalizzati in tutte le campagne. Questa funzionalità standardizza l’aspetto creativo e velocizza l’esecuzione e il lancio delle campagne."

Per accelerare e migliorare il processo di progettazione, crea modelli di consegna per riutilizzare contenuti e impostazioni personalizzati in tutte le campagne. Questa funzionalità standardizza l’aspetto creativo e velocizza l’esecuzione e il lancio delle campagne.

Un modello include:

* La **cartella** e la **cartella di esecuzione** del modello. La cartella è la posizione in cui viene salvato il modello di consegna. La cartella di esecuzione è la cartella in cui vengono salvate le consegne create in base a questo modello.
* [Tipologie](../advanced-settings/delivery-settings.md#typology)
* L’indirizzo del mittente
* Un [pubblico](../audience/about-recipients.md), compresi [gruppi di controllo](../audience/control-group.md)
* [Contenuto](../email/edit-content.md) personalizzato
* [Campi personalizzati](../personalization/personalize.md) e [contenuto condizionale](../personalization/conditions.md)
* Collegamenti a [pagine mirror](../email/mirror-page.md) e [collegamenti](../email/message-tracking.md) per annullare l’iscrizione
* Altre proprietà di consegna, ad esempio validità delle risorse, parametri per nuovi tentativi o impostazioni di quarantena

>[!NOTE]
>
>I modelli di consegna sono diversi dai [modelli di contenuto](../email/create-email-templates.md), che consentono di riutilizzare solo il contenuto delle e-mail e iniziare a creare contenuti con uno dei modelli di e-mail di esempio forniti come predefiniti.

## Accedere ai modelli di consegna e gestirli {#access-manage-templates}

>[!CONTEXTUALHELP]
>id="acw_delivery_templates"
>title="Utilizzare i modelli di consegna"
>abstract="Utilizza i modelli di consegna per creare e salvare le impostazioni di consegna da utilizzare in futuro nelle campagne. Crea modelli di consegna da zero, duplica un modello esistente o converti una consegna in un modello."

Per accedere all’elenco dei modelli di contenuto, dal menu a sinistra seleziona **[!UICONTROL Gestione delle campagne]** > **[!UICONTROL Consegne]** e passa alla scheda **Modelli**.

![Scheda Modelli nel menu Consegne](assets/templates-tab.png){zoomable="yes"}

Vengono visualizzati tutti i modelli creati nell’ambiente corrente.

Puoi filtrare i modelli di contenuto per canali e cartelle. È inoltre possibile impostare filtri avanzati creando una regola con attributi di consegna. [Ulteriori informazioni su Query Modeler](../audience/../query/query-modeler-overview.md)

![Opzioni di filtro per i modelli](assets/templates-filters.png){zoomable="yes"}

Per modificare un modello, fai clic sull’elemento desiderato nell’elenco. Quindi puoi eseguire le seguenti operazioni:

* Modifica il contenuto, le proprietà, il pubblico ed eventuali offerte associate.
* Verifica il modello. [Ulteriori informazioni](#test-template)

![Modifica di un modello](assets/templates-edition.png){zoomable="yes"}

Per eliminare o [duplicare](#copy-an-existing-template) un modello, seleziona l’azione corrispondente dal menu **[!UICONTROL Altre azioni]**, nell’elenco **[!UICONTROL Modelli]** o in una schermata per la modifica dei modelli.

![Menu altre azioni per i modelli](assets/templates-more-actions.png){zoomable="yes"}

>[!NOTE]
>
>La modifica o l’eliminazione di un modello non ha alcun effetto sulle consegne che sono già state create con tale modello.

## Creare un modello di consegna {#create-a-delivery-template}

Per creare un modello di consegna, puoi utilizzare diversi metodi:

* Duplicare un modello esistente - [Ulteriori informazioni](#copy-an-existing-template)
* Convertire una consegna esistente in un modello - [Ulteriori informazioni](#convert-an-existing-delivery)
* Creare un modello di consegna da zero - [Ulteriori informazioni](#create-a-new-template)

### Duplicare un modello di consegna esistente {#copy-an-existing-template}

Campaign include modelli incorporati per ogni canale: e-mail, push e SMS. Il modo più semplice per creare un modello di consegna consiste nel duplicare e personalizzare un modello incorporato.

>[!NOTE]
>
>Puoi duplicare anche un modello personalizzato.

Per duplicare un modello di consegna, effettua le seguenti operazioni:

1. Passa alla scheda **Modelli** dal menu a sinistra **Consegne**. [Ulteriori informazioni](#access-manage-templates)
1. Fai clic sul pulsante **[!UICONTROL Altre azioni]** a destra del nome del modello desiderato e seleziona **[!UICONTROL Duplica]**.

   Puoi anche selezionare un modello dall’elenco e scegliere questa opzione dalla schermata dell’edizione del modello.

1. Conferma la duplicazione.

   ![Finestra di dialogo di conferma per duplicare un modello](assets/templates-duplicate-confirm.png){zoomable="yes"}

1. La nuova dashboard del modello si apre nella schermata centrale. Modifica le impostazioni del modello in base alle esigenze.

   ![Dashboard modello duplicato](assets/templates-duplicated-item.png){zoomable="yes"}

1. Fai clic sul pulsante **[!UICONTROL Rivedi]** per salvare e rivedere il modello. È comunque possibile modificarne tutte le impostazioni, eliminarle e duplicarle.

   ![Schermata di revisione per un modello](assets/templates-review-screen.png){zoomable="yes"}

1. Se necessario, puoi testare come viene riprodotto il modello. [Ulteriori informazioni](#test-template)

Il nuovo modello viene aggiunto all’elenco [**Modelli**](#access-manage-templates). Ora puoi selezionarlo durante la creazione di una nuova consegna.

### Convertire una consegna in un modello {#convert-an-existing-delivery}

Qualsiasi consegna può essere convertita in un modello da riutilizzare in futuro per nuove consegne simili.

Per salvare una consegna come modello, effettua le seguenti operazioni:

1. Sfoglia nel menu **[!UICONTROL Gestione delle campagne]** > **[!UICONTROL Consegne]**.
1. Nella scheda **[!UICONTROL Sfoglia]**, fai clic sul pulsante **[!UICONTROL Altre azioni]** a destra del nome della consegna desiderata e seleziona **[!UICONTROL Copia come modello]**.

   ![Opzione per copiare una consegna come modello](assets/templates-convert-delivery.png){zoomable="yes"}

   Puoi anche selezionare un modello dall’elenco e scegliere questa opzione dalla schermata dell’edizione del modello.

1. Conferma la duplicazione.

1. La nuova dashboard del modello si apre nella schermata centrale. Modifica le impostazioni del modello in base alle esigenze.

1. Fai clic sul pulsante **[!UICONTROL Rivedi]** per salvare e rivedere il modello. È comunque possibile modificarne tutte le impostazioni, eliminarle e duplicarle.

1. Se necessario, puoi testare come viene riprodotto il modello. [Ulteriori informazioni](#test-template)

Il nuovo modello viene aggiunto all’elenco [**Modelli**](#access-manage-templates). Ora puoi selezionarlo durante la creazione di una nuova consegna.

### Creare un nuovo modello di consegna {#create-a-new-template}

>[!NOTE]
>
>Per evitare errori di configurazione, Adobe consiglia di [duplicare un modello incorporato](#copy-an-existing-template) e personalizzarne le proprietà anziché creare un nuovo modello.

Per configurare un modello di consegna da zero, effettua le seguenti operazioni:

1. Passa alla scheda **Modelli** dal menu a sinistra **Consegne**. [Ulteriori informazioni](#access-manage-templates)
1. Fai clic sul pulsante **[!UICONTROL Crea modello]**.

   ![Pulsante Crea modello](assets/templates-create-button.png){zoomable="yes"}

1. Seleziona il canale da utilizzare per il modello.
1. Per impostazione predefinita, viene utilizzato il modello di consegna incorporato per tale canale per facilitare la creazione di un modello personalizzato. Se necessario, utilizza il pulsante dedicato a destra del canale selezionato per selezionare un altro modello.

   ![Selezione canale per un nuovo modello](assets/templates-channel-browse.png){zoomable="yes"}


1. Fai di nuovo clic sul pulsante **[!UICONTROL Crea modello]**.

1. Definisci le proprietà del modello, [pubblico](../audience/add-audience.md) e il contenuto a seconda del canale selezionato.

   >[!NOTE]
   >
   >Ulteriori informazioni sui canali di consegna e su come progettare i rispettivi contenuti sono disponibili nelle sezioni seguenti:
   >
   > * [Canale e-mail](../email/create-email.md)
   > * [Canale di notifica push](../push/gs-push.md)
   > * [Canale SMS](../sms/create-sms.md)

1. Inoltre, per i modelli e-mail, è possibile accedere a impostazioni avanzate, come regole di tipologia e mappature di destinazione, tramite il pulsante **[!UICONTROL Impostazioni]** in alto a destra. [Ulteriori informazioni](../advanced-settings/delivery-settings.md)

1. Fai clic sul pulsante **[!UICONTROL Rivedi]** per salvare e rivedere il modello. È comunque possibile modificarne tutte le impostazioni, eliminarle e duplicarle.

1. Se necessario, puoi testare come viene riprodotto il modello. [Ulteriori informazioni](#test-template)

Il nuovo modello viene aggiunto all’elenco [**Modelli**](#access-manage-templates). Ora puoi selezionarlo durante la creazione di una nuova consegna.

## Testare un modello di consegna {#test-template}

Puoi testare come verrà riprodotto qualsiasi modello di consegna, che sia stato creato da zero o da contenuti esistenti. Per farlo, segui questi passaggi:

1. Sfoglia la scheda **Modelli** a cui puoi accedere dal menu **[!UICONTROL Gestione delle campagne]** > **[!UICONTROL Consegne]** e seleziona un modello. [Ulteriori informazioni](#access-manage-templates)

1. Fai clic sul pulsante **[!UICONTROL Simula contenuto]** in alto a destra dello schermo.

   ![Pulsante Simula contenuto](assets/templates-simulate-button.png){zoomable="yes"}

1. Seleziona uno o più profili di test per controllare come vengono riprodotte le e-mail. Puoi anche selezionare profili reali dal database. [Ulteriori informazioni sui profili di test](../audience/test-profiles.md)

1. Passa da un profilo all’altro per ottenere una rappresentazione personalizzata del messaggio in base al profilo selezionato. Puoi anche regolare il livello di zoom e scegliere la visualizzazione su desktop o dispositivo mobile.

[Ulteriori informazioni sull’anteprima dei contenuti](../preview-test/preview-content.md)

   ![Anteprima contenuto simulato](assets/templates-stimulate.png){zoomable="yes"}

1. Chiudere la finestra per tornare alla schermata dell&#39;edizione del modello.

>[!NOTE]
>
>Da un modello di consegna non è possibile utilizzare il rendering delle e-mail né inviare delle bozze.