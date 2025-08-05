---
title: Creare una pagina di destinazione
description: Scopri come configurare e pubblicare una pagina di destinazione in Campaign Web
feature: Landing Pages
exl-id: d4a49048-5ab1-4b69-9e12-1ffa235c51f4
source-git-commit: e82c19df7faecbb75521bca54e32b1ba84ea1f81
workflow-type: tm+mt
source-wordcount: '1643'
ht-degree: 24%

---


# Creare e pubblicare pagine di destinazione {#create-lp}

>[!CONTEXTUALHELP]
>id="acw_landingpages_menu"
>title="Creare e gestire pagine di destinazione"
>abstract="Adobe Campaign consente di creare, progettare e condividere le pagine di destinazione per indirizzare gli utenti a pagine web online in cui puoi gestire casi d’uso di acquisizione, iscrizione o annullamento dell’inscrizione e inserimento nell’elenco Bloccati, in base ai modelli incorporati."

L’interfaccia utente di Campaign Web consente di creare, progettare e pubblicare pagine di destinazione. Dopo la pubblicazione, è possibile inserire un collegamento al modulo in una consegna. Quando i destinatari fanno clic su tale collegamento, vengono indirizzati alla pagina di destinazione corrispondente.

[!DNL Adobe Campaign] viene fornito con quattro modelli per gestire i seguenti casi d&#39;uso: **acquisizione**, **sottoscrizione**, **annullamento sottoscrizione** e **elenco Bloccati**. [Ulteriori informazioni](lp-use-cases.md)

## Accedere alle pagine di destinazione {#access-landing-pages}

Per accedere all&#39;elenco delle pagine di destinazione, seleziona **[!UICONTROL Gestione contenuto]** > **[!UICONTROL Pagine di destinazione]** dal menu a sinistra.

![Schermata che mostra l&#39;inventario delle pagine di destinazione nell&#39;interfaccia Web di Campaign.](assets/lp-inventory.png){zoomable="yes"}

Nell&#39;inventario **[!UICONTROL Pagine di destinazione]** vengono visualizzati tutti gli elementi creati. Puoi filtrarli utilizzando il pulsante **[!UICONTROL Mostra filtri]**.

* Puoi filtrare gli elementi creati o modificati.
* È possibile limitare i risultati a una [cartella](../get-started/permissions.md#folders) specifica utilizzando l&#39;elenco a discesa oppure aggiungere regole utilizzando [modeler query](../query/query-modeler-overview.md).

![Schermata che mostra le opzioni filtro nell&#39;inventario delle pagine di destinazione.](assets/lp-inventory-filter.png){zoomable="yes"}

<!--From this list, you can access the [landing page Live report](../reports/lp-report-live.md) or [landing page Global report](../reports/lp-report-global.md) for published items.-->

>[!CAUTION]
>
>Non è possibile visualizzare o modificare le pagine di destinazione create dalla console client (moduli web) nell’interfaccia utente di Campaign Web. Ulteriori informazioni sono disponibili nella [documentazione della console Campaign](https://experienceleague.adobe.com/docs/campaign/campaign-v8/content/webapps.html?lang=it){target="_blank"}.

<!--If you unpublish a landing page which is referenced in a message, the link to the landing page will be broken and an error page will be displayed. You cannot delete a published landing page. To delete it, you must first unpublish it.-->

Puoi duplicare o eliminare una pagina di destinazione. Fai clic sui puntini di sospensione accanto a una pagina di destinazione per selezionare l’azione desiderata.

## Creare una pagina di destinazione {#create-landing-page}

>[!CONTEXTUALHELP]
>id="acw_landingpages_properties"
>title="Definire le proprietà della pagina di destinazione"
>abstract="Compila i campi delle proprietà, ad esempio l’etichetta, e, se necessario, modifica lo schema. Inoltre, puoi modificare il nome interno, cambiare la cartella in cui è memorizzata la pagina di destinazione e fornire una descrizione."

>[!CONTEXTUALHELP]
>id="acw_landingpages_pages_list"
>title="Definire il contenuto di ciascuna pagina"
>abstract="Adatta il contenuto di ogni pagina che fa parte di questa pagina di destinazione, ad esempio il modulo stesso, la pagina di conferma visualizzata al momento dell’invio del modulo oppure la pagina a cui gli utenti vengono indirizzati nel caso in cui si verifichi un errore."

>[!CONTEXTUALHELP]
>id="acw_landingpages_schedule"
>title="Pianificare la pagina di destinazione"
>abstract="Definisci una data di inizio e una data di fine per la pagina di destinazione. Al termine del periodo di validità della pagina, il modulo non è più disponibile. Viene invece visualizzata la pagina la pagina **Scadenza**."

>[!CONTEXTUALHELP]
>id="acw_landingpages_preload"
>title="Definire le opzioni di precaricamento"
>abstract="Quando l’opzione **Precompila con i dati a cui si fa riferimento nel modulo** è selezionata, se il visitatore della pagina di destinazione corrisponde a un profilo del database, le informazioni del profilo vengono precaricate automaticamente nel modulo. Con l’opzione **Autorizza l’assenza di ID** selezionata, tutti i visitatori, inclusi gli utenti anonimi, possono accedere alla pagina di destinazione."

<!--With the **Skip preloading if no ID** option selected, each profile entered will be added to the database after approval of the form."-->

>[!CONTEXTUALHELP]
>id="acw_landingpages_storage"
>title="Definire le opzioni di archiviazione"
>abstract="La sezione di precaricamento consente di indicare come trovare il record da aggiornare nel database."

<!--The main steps to create landing pages are as follows:

![](assets/lp-creation-process.png){zoomable="yes"}-->

Per creare una pagina di destinazione, effettua le seguenti operazioni:

1. Nell&#39;inventario **[!UICONTROL Pagine di destinazione]**, fare clic su **[!UICONTROL Crea pagina di destinazione]**.

   ![Schermata che mostra il pulsante Crea pagina di destinazione.](assets/lp-create-button.png){zoomable="yes"}

1. Seleziona un modello:
   * **[!UICONTROL Acquisizione]**: questo è il modello predefinito per le pagine di destinazione, che ti consente di acquisire e aggiornare i dati del profilo.
   * **[!UICONTROL Sottoscrizione]**: utilizzare questo modello per consentire agli utenti di sottoscrivere un [servizio](../audience/manage-services.md) specifico.
   * **[!UICONTROL Annullamento abbonamento]**: questo modello può essere utilizzato in una consegna inviata agli abbonati di un servizio per consentire loro di annullare l&#39;abbonamento a questo [servizio](../audience/manage-services.md).
   * **[!UICONTROL Inserisco nell&#39;elenco Bloccati di]**: utilizzare questo modello quando un profilo fa clic su un collegamento di rinuncia in una consegna e non desidera più essere contattato.

   ![Schermata che mostra i modelli della pagina di destinazione.](assets/lp-templates.png){zoomable="yes"}

   >[!NOTE]
   >
   >Scopri come implementare i diversi casi d&#39;uso corrispondenti a ciascun modello in [questa pagina](lp-use-cases.md).

1. Fai clic su **[!UICONTROL Crea]**.

1. Compila i campi **[!UICONTROL Proprietà]** come l&#39;etichetta.

   Per impostazione predefinita, le pagine di destinazione sono memorizzate nella cartella **[!UICONTROL Applicazioni Web]**. Puoi modificarlo sfogliando la posizione desiderata nelle **[!UICONTROL Opzioni aggiuntive]**. [Scopri come utilizzare le cartelle](../get-started/permissions.md#folders).

   Puoi anche impostare il captcha per proteggere la pagina di destinazione. [Ulteriori informazioni](#captcha).

   ![Schermata che mostra la sezione delle proprietà della pagina di destinazione.](assets/lp-properties.png){zoomable="yes"}

1. Nella sezione **[!UICONTROL Precaricamento dati]** sono disponibili le seguenti opzioni:

   * Quando l’opzione **[!UICONTROL Precompila con i dati a cui si fa riferimento nel modulo]** è selezionata, se il visitatore della pagina di destinazione corrisponde a un profilo del database, le informazioni del profilo vengono precaricate automaticamente nel modulo. L’utente deve solo compilare i campi mancanti e aggiornare i valori esistenti, se necessario. Questo consente di unire i dati per i profili esistenti invece di creare duplicati.

     >[!NOTE]
     >
     >Questa opzione è selezionata per impostazione predefinita per tutti i modelli di pagina di destinazione.

   * L&#39;opzione **[!UICONTROL Autorizza assenza ID]** consente a qualsiasi visitatore di accedere alla pagina di destinazione. Deselezionando questa opzione si impedisce ai visitatori anonimi di utilizzarla, il che significa che solo gli utenti identificati possono accedere al modulo e inviarlo.

     Per i modelli **[!UICONTROL Acquisizione]** e **[!UICONTROL Sottoscrizione]**, questa opzione è selezionata per impostazione predefinita. Per i modelli **[!UICONTROL Annullamento sottoscrizione]** e **[!UICONTROL Inserisco nell&#39;elenco Bloccati]**, questa opzione è deselezionata per impostazione predefinita e non può essere modificata.

1. Una pagina di destinazione può avere pagine successive. Per aggiungere pagine, sfoglia la sezione **[!UICONTROL Pagine]** e fai clic sul pulsante **[!UICONTROL Modifica contenuto]** per ogni pagina che desideri progettare per questa pagina di destinazione. Il contenuto di ogni pagina è già precompilato. Modificali in base alle esigenze. [Ulteriori informazioni](lp-content.md).

   ![Schermata che mostra la sezione pagine dell&#39;editor pagine di destinazione.](assets/lp-pages.png){zoomable="yes"}

1. Nella sezione **[!UICONTROL Archiviazione]**, l&#39;opzione **[!UICONTROL Aggiorna il record precaricato]** è selezionata per impostazione predefinita. Consente di aggiornare i profili memorizzati nel database tramite la pagina di destinazione. La casella di precaricamento consente di indicare come trovare il record da aggiornare nel database.

   Puoi anche scegliere tra i campi nel contesto corrente della pagina di destinazione, quelli che verranno utilizzati per trovare il profilo corrispondente nel database. A tale scopo, deselezionare l&#39;opzione **[!UICONTROL Aggiorna il record precaricato]** e selezionare i campi desiderati in **[!UICONTROL Opzioni di riconciliazione]**.

   ![Schermata che mostra le opzioni di archiviazione per la pagina di destinazione.](assets/lp-storage.png){zoomable="yes"}

1. Crea **[!UICONTROL Dati aggiuntivi]** per memorizzare i dati interni durante l&#39;invio della pagina di destinazione. Questi dati non sono visibili agli utenti che visitano la pagina. Vengono presi in considerazione solo i valori costanti.

   ![Schermata che mostra la sezione dei dati aggiuntivi.](assets/lp-additional-data.png){zoomable="yes"}

1. Puoi definire una data di inizio e una data di fine per la pagina di destinazione. Selezionare **[!UICONTROL Abilita pianificazione]** e impostare le date.

   ![Schermata che mostra le opzioni di pianificazione per la pagina di destinazione.](assets/lp-schedule.png){zoomable="yes"}

   * La pagina di destinazione viene pubblicata automaticamente nella data/ora di inizio specificata.

     >[!NOTE]
     >
     >Se non è definita alcuna data di inizio, la pagina di destinazione diventa attiva non appena viene pubblicata.

   * Quando la pagina raggiunge la data di fine, il modulo non è più disponibile. Viene invece visualizzata la pagina la pagina **[!UICONTROL Scadenza]**.

     >[!NOTE]
     >
     >Per motivi di sicurezza e prestazioni della piattaforma, Adobe consiglia di impostare una data di fine.

1. Fai clic su **[!UICONTROL Rivedi e pubblica]**.

Una volta definite tutte le impostazioni e [progettate](lp-content.md) tutte le pagine, puoi [testare](#test-landing-page) e [pubblicare](#publish-landing-page) la tua pagina di destinazione come descritto di seguito.

## Proteggi la pagina di destinazione con un captcha {#captcha}

La configurazione di un captcha ti aiuta a proteggere la pagina di destinazione da spam e abusi.

Per utilizzarlo, vai alle **[!UICONTROL Proprietà]** della pagina di destinazione.
Anche nelle **[!UICONTROL Opzioni aggiuntive]**. Attiva l&#39;interruttore **[!UICONTROL Soluzione Captcha aggiuntiva]**.

![Schermata che mostra l&#39;interruttore della soluzione Captcha di abilitazione aggiuntiva](assets/lp-properties-captcha.png){zoomable="yes"}

Per verificare le impostazioni captcha, fare clic sul pulsante **[!UICONTROL Rivedi e pubblica]** e su **[!UICONTROL Simula contenuto]**. Durante l’invio del modulo, viene visualizzato il widget captcha che funziona durante la convalida come indicato di seguito.

![Schermata del widget captcha](assets/lp-captcha.png){zoomable="yes"}

>[!NOTE]
>
>Il widget captcha in Adobe Campaign v8 è ALTCHA e funziona in modalità mobile. Viene visualizzato durante la convalida e scompare al termine del processo.


## Verificare la pagina di destinazione {#test-landing-page}

>[!CONTEXTUALHELP]
>id="acw_landingpages_simulate"
>title="Simulare una pagina di destinazione"
>abstract="Puoi visualizzare un’anteprima della pagina di destinazione nell’interfaccia utente di Campaign Web oppure aprirla in una nuova scheda del browser web."

>[!CONTEXTUALHELP]
>id="ac_preview_lp_profiles"
>title="Visualizzare l’anteprima e testare la pagina di destinazione"
>abstract="Una volta definite le impostazioni e il contenuto della pagina di destinazione, puoi utilizzare i profili di test per visualizzarli in anteprima."

Una volta definiti le impostazioni e il contenuto della pagina di destinazione, puoi utilizzare i profili di test per visualizzarne l’anteprima. Se hai inserito [contenuti personalizzati](../personalization/gs-personalization.md), potrai controllare come questi contenuti vengono visualizzati nella pagina di destinazione utilizzando i dati del profilo di test.

>[!CAUTION]
>
>Per poter visualizzare in anteprima i messaggi e inviare le bozze, è necessario disporre di profili di test. [Ulteriori informazioni sui profili di test](../audience/test-profiles.md)

Per verificare la pagina di destinazione, effettua le seguenti operazioni:

1. Dopo aver fatto clic su **[!UICONTROL Rivedi e pubblica]**, seleziona il pulsante **[!UICONTROL Simula contenuto]** dal dashboard della pagina di destinazione per accedere alla selezione del profilo di test.

   ![Schermata del pulsante Simula contenuto](assets/lp-simulate-content.png){zoomable="yes"}

1. Dalla schermata **[!UICONTROL Simula]**, selezionare uno o più profili di test.

   I passaggi per selezionare i profili di test sono gli stessi utilizzati per testare un messaggio. Sono descritte in dettaglio nella sezione [Anteprima e test](../preview-test/preview-test.md).

1. Durante il test di una pagina di destinazione dinamica (con l&#39;opzione **[!UICONTROL Servizio dall&#39;URL]** selezionata - [ulteriori informazioni](../landing-pages/create-lp.md#define-actions-on-form-submission)

1. Seleziona **[!UICONTROL Apri anteprima]** per verificare la pagina di destinazione.

   ![Schermata del pulsante Apri anteprima](assets/lp-open-preview.png){zoomable="yes"}

1. L’anteprima della pagina di destinazione viene visualizzata in una nuova scheda. Gli elementi personalizzati vengono sostituiti dai dati del profilo di test selezionati.

   Se hai selezionato l&#39;opzione **[!UICONTROL Precompila con i dati a cui si fa riferimento nel modulo]** nelle impostazioni della pagina di destinazione, i campi del modulo vengono precompilati automaticamente con i dati del profilo di test corrispondenti.<!--TBC-->

   ![Esempio di consegna](assets/lp-preview.png){zoomable="yes"}

1. Seleziona altri profili di test per visualizzare in anteprima il rendering per ogni variante della pagina di destinazione.

<!--Can you preview Confirmation/Error/Expiration pages?-->

## Pubblicare la pagina di destinazione {#publish-landing-page}

Una volta che la pagina di destinazione è pronta e convalidata, pubblicala per renderla disponibile per l’utilizzo in una consegna utilizzando il pulsante corrispondente.

Dopo la pubblicazione:

* La pagina di destinazione viene aggiunta all&#39;elenco delle pagine di destinazione con lo stato **[!UICONTROL Pubblicato]**. Ora è attivo e pronto per essere utilizzato come riferimento nei contenuti.

* È possibile copiare e incollare l&#39;**[!UICONTROL URL della pagina di destinazione]** visualizzato nella parte superiore della pagina in un browser Web per visualizzare l&#39;anteprima della pagina di destinazione.

>[!CAUTION]
>
>Per testare o sfruttare appieno la pagina di destinazione, non puoi copiare e incollare questo collegamento direttamente in un browser web o nelle consegne. Utilizza invece la funzione [Simula contenuto](#test-landing-page) per verificarlo e segui i passaggi descritti in [questa sezione](lp-use-cases.md) per utilizzare correttamente la pagina di destinazione.

![Schermata che mostra l&#39;URL della pagina di destinazione](assets/lp-published.png){zoomable="yes"}

Puoi monitorare l&#39;impatto della pagina di destinazione tramite i registri<!--and specific reports-->. Fai clic sul pulsante **[!UICONTROL Registri]**.