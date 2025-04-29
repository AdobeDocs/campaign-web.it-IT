---
audience: end-user
product: campaign
title: Utilizzare i modelli di contenuto
description: Scopri come creare modelli per riutilizzare il contenuto nelle e-mail di Adobe Campaign
feature: Templates
topic: Content Management
role: User
level: Beginner
exl-id: 23818080-d7c6-4829-8117-d6b359bd76dd
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '1085'
ht-degree: 15%

---

# Utilizzare i modelli di contenuto {#content-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_menu"
>title="Modelli di contenuto"
>abstract="Per un processo di progettazione più rapido e migliore, puoi creare modelli e-mail indipendenti che consentono di riutilizzare facilmente contenuti personalizzati in più campagne. Questi modelli di contenuto possono essere progettati da zero, sulla base di modelli incorporati o personalizzati, creati da un contenuto esistente o importati nell’editor di modelli di contenuto."

Per accelerare e migliorare il processo di progettazione, è possibile creare modelli autonomi per riutilizzare facilmente i contenuti personalizzati in [!DNL Adobe Campaign]. Questi modelli di contenuto possono essere progettati da zero, basati su modelli incorporati o personalizzati, creati da contenuti esistenti o importati nell’editor di modelli di contenuto.

Questa funzionalità consente agli utenti orientati ai contenuti di lavorare su modelli autonomi, in modo che gli utenti di marketing possano riutilizzarli e adattarli all’interno delle proprie campagne e-mail.

>[!NOTE]
>
>Attualmente sono supportati solo i modelli di contenuto **e-mail**.

## Accedere ai modelli di contenuto {#access-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_edition"
>title="Modificare il contenuto del modello"
>abstract="Fai clic sul pulsante **Modifica contenuto** per aggiornare il contenuto con E-mail Designer."

Per accedere all&#39;elenco dei modelli di contenuto, passa al menu **[!UICONTROL Gestione contenuto]** > **[!UICONTROL Modelli di contenuto]** dalla barra a sinistra.

![Dashboard elenco modelli di contenuto con i modelli disponibili](assets/content-template-list.png){zoomable="yes"}

Questo dashboard mostra tutti i modelli di contenuto disponibili come un elenco. Puoi filtrare in base a una [cartella](../get-started/permissions.md#folders) specifica utilizzando l&#39;elenco a discesa oppure aggiungere regole utilizzando [modellatore query](../query/query-modeler-overview.md).

![Filtri per elenchi di modelli di contenuto per cartelle e regole](assets/content-template-list-filters.png){zoomable="yes"}

Dall’elenco, puoi modificare, duplicare o eliminare i modelli di contenuto esistenti. Utilizza il pulsante nella sezione superiore per creare un modello di contenuto.

### Modello di contenuto in modalità di sola lettura {#template-readonly}

I diritti di accesso possono essere applicati ai modelli di contenuto.

Se non si dispone delle autorizzazioni di modifica per un modello di contenuto specifico, il modello di contenuto verrà visualizzato in **modalità di sola lettura**. In questo caso, il pulsante **[!UICONTROL Modifica contenuto]** viene sostituito dal pulsante **[!UICONTROL Visualizza contenuto]**, che consente di visualizzare il modello senza apportare modifiche.

![Modalità di sola lettura per i modelli di contenuto](assets/template-readonly.png){zoomable="yes"}

Come mostrato di seguito, tutte le icone delle funzioni sono disattivate, limitando l’interazione alla sola visualizzazione.

![Visualizzazione di sola lettura dei modelli di contenuto](assets/template-readonly-view.png){zoomable="yes"}

## Creare modelli di contenuto {#create-content-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_design"
>title="Progettazione del modello di contenuto"
>abstract="Progetta il modello di contenuto delle e-mail."

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_selection"
>title="Selezione del modello di contenuto"
>abstract="Seleziona il modello di contenuto delle e-mail."

I modelli di contenuto possono essere creati [salvando un messaggio e-mail esistente come modello](#save-as-template) o dall&#39;elenco dei modelli e-mail, tramite il pulsante **Crea modello di contenuto**, [come descritto di seguito](#create-template-from-scratch).

Una volta salvato, puoi utilizzare questo modello per creare qualsiasi [e-mail](../email/create-email.md) in [!DNL Adobe Campaign]. [Scopri come](use-email-templates.md)

>[!NOTE]
>
>* Le modifiche apportate ai modelli di contenuto non vengono propagate alle e-mail.
>
>* Allo stesso modo, quando i modelli vengono utilizzati in un messaggio e-mail, eventuali modifiche apportate al contenuto dell’e-mail non influiscono sul modello di contenuto utilizzato in precedenza.

### Creare un nuovo modello di contenuto {#create-template-from-scratch}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_properties"
>title="Definire le proprietà del modello"
>abstract="Definisci facilmente le proprietà del modello di contenuto e-mail da recuperare quando necessario."

Per creare un nuovo modello di contenuto dal dashboard modelli di contenuto, effettua le seguenti operazioni:

1. Dalla barra a sinistra **[!UICONTROL Gestione contenuto]** > **[!UICONTROL Modelli di contenuto]**, accedi all&#39;elenco dei modelli di contenuto.

1. Seleziona **[!UICONTROL Crea modello]**.

   ![Pulsante Crea modello di contenuto nel dashboard](assets/content-template-create.png){zoomable="yes"}

1. Immetti l’etichetta del modello e le proprietà. È possibile selezionare la cartella in cui memorizzare il modello. Per impostazione predefinita, i modelli di contenuto sono archiviati in una cartella dedicata della gerarchia Adobe Campaign: **[!UICONTROL Explorer]** > **[!UICONTROL Risorse]** > **[!UICONTROL Modelli]** > **[!UICONTROL Modelli di contenuto]**. Ulteriori informazioni sulle cartelle in [questa pagina](../get-started/permissions.md#folders)

   ![Schermata Dettagli modello per etichetta e proprietà](assets/content-template-details.png){zoomable="yes"}

1. Fai clic su **[!UICONTROL Crea]** e scegli la modalità di progettazione del modello tra le diverse opzioni:

   * [Progetta il contenuto da zero](create-email-content.md) tramite l&#39;interfaccia di E-mail Designer.
   * [Codice o copia-incolla HTML non elaborato](code-content.md) direttamente nel Designer e-mail.
   * [Importa contenuto HTML esistente](existing-content.md) da un file o da una cartella .zip.
   * Utilizza il contenuto esistente da un elenco di modelli incorporati o personalizzati. I passaggi per utilizzare un modello di contenuto in un messaggio e-mail sono descritti in [questa sezione](use-email-templates.md).

   ![Opzioni Designer e-mail per la creazione di modelli](assets/email_designer-templates.png){zoomable="yes"}

1. Viene visualizzato E-mail Designer. Modifica il contenuto in base alle esigenze, come faresti per qualsiasi e-mail, in base all’opzione selezionata. Scopri come utilizzare il Designer e-mail in [questa sezione](get-started-email-designer.md).

   <!--You can test your content if needed. [Learn how](#test-template)-->

1. Quando il modello è pronto, fai clic su **[!UICONTROL Salva]**.

   Se necessario, fai clic sulla freccia accanto al nome del modello per tornare alla schermata **[!UICONTROL Dettagli]** e modificare il modello.

   ![Salva e torna alla schermata dei dettagli](assets/content-template-save-back.png){zoomable="yes"}

Il modello è disponibile nell&#39;elenco **[!UICONTROL Modelli di contenuto]**. [Ulteriori informazioni](#access-templates)

Ora puoi utilizzare questo modello per creare nuovi contenuti. È disponibile nella scheda **[!UICONTROL Modelli salvati]** di E-mail Designer. [Scopri come](use-email-templates.md)

### Salvare il contenuto di un’e-mail come modello {#save-as-template}

Dopo aver [progettato un&#39;e-mail](create-email-content.md), puoi salvarne il contenuto come modello da riutilizzare in futuro. I modelli salvati sono disponibili per tutti gli utenti dell’ambiente Adobe Campaign.

Per salvare un contenuto e-mail come modello, segui la procedura seguente:

1. In E-mail Designer, fai clic sul pulsante **[!UICONTROL Altro]** in alto a destra dello schermo.

1. Seleziona **[!UICONTROL Salva come modello di contenuto]** dal menu a discesa.

   ![Opzione Salva come modello di contenuto in e-mail designer](assets/email_designer-save-template.png){zoomable="yes"}

1. Immetti un nome per il modello e salvalo.

   ![Immettere il nome per il modello salvato](assets/email_designer-template-name.png){zoomable="yes"}

Il modello viene salvato e visualizzato nell&#39;elenco **[!UICONTROL Modelli di contenuto]**. Diventa un modello di contenuto autonomo accessibile, modificato ed eliminato come qualsiasi altro elemento dell&#39;elenco. [Ulteriori informazioni](#access-manage-templates)

Ora puoi utilizzare questo modello per creare nuovi contenuti. È disponibile nella scheda **[!UICONTROL Modelli salvati]** di E-mail Designer. [Scopri come](use-email-templates.md)

![Modello salvato in E-mail Designer](assets/email_designer-saved-template.png){zoomable="yes"}

>[!NOTE]
>
>Eventuali modifiche a tale nuovo modello non vengono propagate all’e-mail da cui provengono. Allo stesso modo, quando il contenuto originale viene modificato all’interno dell’e-mail, il nuovo modello non viene modificato.

<!--

Test your content template {#test-template}

You can test the rendering of any email content template, whether created from scratch or from an email. To do so, follow the steps below.

1. Access the content template list.

1. Click **[!UICONTROL Edit content]** from the **[!UICONTROL Template properties]**.

1. Click **[!UICONTROL Simulate Content]** and select a test profile to check your email rendering. You can choose the desktop or mobile view.

1. You can send a proof to test your content and have it approved by some internal users before using it. To do so, click the **[!UICONTROL Send proof]** button and follow the steps described in .

-->

## Modificare un modello di contenuto {#modify-delete}

Per aggiornare un modello di contenuto esistente, effettua le seguenti operazioni:

1. Dall’elenco dei modelli di contenuto, fai clic sull’etichetta del modello per modificarlo.

1. Fai clic sul pulsante **[!UICONTROL Modifica contenuto]** per aggiornare il contenuto con [Invia e-mail a Designer](get-started-email-designer.md).

![Opzione Modifica modello di contenuto](assets/content-template-edition.png){zoomable="yes"}

>[!NOTE]
>
>Le modifiche apportate ai modelli di contenuto non vengono propagate alle e-mail che utilizzano questo modello di contenuto.

## Eliminare un modello di contenuto {#content-delete}

Sono disponibili due modi per eliminare un modello di contenuto:

* Nell&#39;elenco dei modelli di contenuto, fare clic sul pulsante con i puntini di sospensione, quindi selezionare **Elimina**.

  ![Eliminare un modello di contenuto dal dashboard](assets/content-template-list-delete.png){zoomable="yes"}

* Dal modello di contenuto stesso, fare clic sul pulsante **Altro**, quindi selezionare **Elimina**.

>[!NOTE]
>
>L’eliminazione di un modello di contenuto non influisce sulle consegne create utilizzando questo modello.

## Duplicare un modello di contenuto {#content-duplicate}

Sono disponibili due modi per duplicare un modello di contenuto:

* Nell&#39;elenco dei modelli di contenuto, fare clic sul pulsante con i puntini di sospensione, quindi selezionare **Duplica**.

* Dal modello di contenuto stesso, fare clic sul pulsante **Altro**, quindi selezionare **Duplica**.

In entrambi i casi, conferma la duplicazione per creare il nuovo modello di contenuto. L&#39;etichetta del nuovo modello di contenuto è **Copia di`<label of the initial campaign>`**. Selezionare le impostazioni del modello per aggiornare l&#39;etichetta.