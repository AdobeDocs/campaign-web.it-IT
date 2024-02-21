---
title: Creare una pagina di destinazione
description: Scopri come configurare e pubblicare una pagina di destinazione in Campaign Web
feature: Landing Pages
source-git-commit: 26c41105a4c04b72e0aedf05a4b3268b0e475d40
workflow-type: tm+mt
source-wordcount: '1340'
ht-degree: 24%

---

# Creare e pubblicare pagine di destinazione {#create-lp}

>[!CONTEXTUALHELP]
>id="acw_landingpages_menu"
>title="Creare e gestire pagine di destinazione"
>abstract="Adobe Campaign consente di creare, progettare e condividere pagine di destinazione per indirizzare gli utenti a pagine web online in cui gestire l’acquisizione, l’iscrizione/annullamento dell’iscrizione e inserire nell’elenco Bloccati casi d’uso, in base ai modelli incorporati."

L’interfaccia utente di Campaign Web consente di creare, progettare e pubblicare pagine di destinazione. Dopo la pubblicazione, puoi inserire un collegamento al modulo in una consegna. Dopo che i destinatari hanno fatto clic su tale collegamento, vengono indirizzati alla pagina di destinazione corrispondente.

[!DNL Adobe Campaign] viene fornito con quattro modelli per gestire i seguenti casi d’uso: **acquisizione**, **abbonamento**, **annullamento iscrizione**, e **inserisco nell&#39;elenco Bloccati**.

## Accedere alle pagine di destinazione {#access-landing-pages}

Per accedere all’elenco delle pagine di destinazione, seleziona **[!UICONTROL Gestione delle campagne]** > **[!UICONTROL Pagine di destinazione]** dal menu a sinistra.

![](assets/lp-inventory.png){zoomable=&quot;yes&quot;}

Il **[!UICONTROL Pagine di destinazione]** inventory visualizza tutti gli articoli creati. Puoi filtrarli utilizzando **Mostra filtri** pulsante. È possibile limitare i risultati a uno specifico [cartella](../get-started/permissions.md#folders) utilizzando l’elenco a discesa, oppure aggiungi regole utilizzando [query modeler](../query/query-modeler-overview.md).

![](assets/lp-inventory-filter.png){zoomable=&quot;yes&quot;}

<!--From this list, you can access the [landing page Live report](../reports/lp-report-live.md) or [landing page Global report](../reports/lp-report-global.md) for published items.-->

>[!CAUTION]
>
>Non è possibile visualizzare o modificare le pagine di destinazione create dalla console client (moduli web) nell’interfaccia utente di Campaign Web. Per ulteriori informazioni, consulta [Documentazione della console di Campaign](https://experienceleague.adobe.com/docs/campaign/campaign-v8/content/webapps.html){target="_blank"}.

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
>abstract="Adatta il contenuto di ogni pagina appartenente a questa pagina di destinazione, ad esempio il modulo stesso, la pagina di conferma visualizzata al momento dell’invio del modulo oppure la pagina a cui gli utenti vengono indirizzati nel caso in cui si verifichi un errore."

>[!CONTEXTUALHELP]
>id="acw_landingpages_schedule"
>title="Pianificare la pagina di destinazione"
>abstract="Puoi definire una data di inizio e una data di fine per la pagina di destinazione. Al termine del periodo di validità della pagina, il modulo non è più disponibile. Viene invece visualizzata la pagina la pagina **Scadenza**."

>[!CONTEXTUALHELP]
>id="acw_landingpages_primarypage"
>title="Definire le impostazioni della pagina principale"
>abstract="La pagina principale viene visualizzata immediatamente dagli utenti dopo aver fatto clic sul collegamento alla pagina di destinazione, ad esempio da un’e-mail o da un sito web."

>[!CONTEXTUALHELP]
>id="acw_landingpages_subscription"
>title="Impostare la pagina di destinazione dell&#39;iscrizione"
>abstract="Una pagina di iscrizione consente ai clienti di iscriversi a un servizio."

<!--The main steps to create landing pages are as follows:

![](assets/lp-creation-process.png){zoomable="yes"}-->

Per creare una pagina di destinazione, effettua le seguenti operazioni:

1. Dalla sezione **[!UICONTROL Pagine di destinazione]** inventory, fai clic su **[!UICONTROL Crea pagina di destinazione]**.

   ![](assets/lp-create-button.png){zoomable=&quot;yes&quot;}

1. Seleziona un modello:
   * **[!UICONTROL Acquisizione]**: questo è il modello predefinito per le pagine di destinazione, che ti consente di acquisire e aggiornare i dati del profilo.
   * **[!UICONTROL Abbonamento]**: utilizza questo modello per consentire agli utenti di abbonarsi a uno specifico [servizio](../audience/manage-services.md).
   * **[!UICONTROL Annullamento iscrizione]**: questo modello può essere utilizzato in una consegna inviata agli abbonati di un servizio, per consentire loro di annullare l’abbonamento [servizio](../audience/manage-services.md).
   * **[!UICONTROL Inserisco nell&#39;elenco Bloccati]**: questo modello deve essere utilizzato quando un profilo fa clic su un collegamento di rinuncia in una consegna e non desidera più essere contattato.

   ![](assets/lp-templates.png){zoomable=&quot;yes&quot;}

   >[!NOTE]
   >
   >Scopri come implementare i diversi casi d’uso corrispondenti a ciascun modello in [questa pagina](lp-use-cases.md).

1. Fai clic su **[!UICONTROL Crea]**.

1. Compila il **[!UICONTROL Proprietà]** campi come l’etichetta.

   Per impostazione predefinita, le pagine di destinazione sono memorizzate in **[!UICONTROL Applicazioni web]** cartella. È possibile modificarlo individuando la posizione desiderata nella **[!UICONTROL Opzioni aggiuntive]**. [Scopri come utilizzare le cartelle](../get-started/permissions.md#folders)

   ![](assets/lp-properties.png){zoomable=&quot;yes&quot;}

1. In **[!UICONTROL Precaricamento dati]** , le due opzioni seguenti sono selezionate per impostazione predefinita:

   * Quando **[!UICONTROL Precompilare con i dati a cui si fa riferimento nel modulo]** se l’opzione è selezionata, se il visitatore della pagina di destinazione corrisponde a un profilo del database, le informazioni del profilo vengono precaricate automaticamente nel modulo. L’utente deve solo compilare i campi mancanti e, se necessario, aggiornare i valori esistenti. Questo consente di unire i dati per i profili esistenti invece di creare duplicati.

   * Il **[!UICONTROL Salta il precaricamento se non è presente alcun ID]** deve essere selezionata se non desideri aggiornare i profili. In questo caso, ogni profilo inserito verrà aggiunto al database dopo l’approvazione del modulo. Questa opzione viene utilizzata, ad esempio, quando il modulo viene pubblicato su un sito Web.

1. Una pagina di destinazione può avere pagine successive. Per aggiungere delle pagine, sfoglia **[!UICONTROL Pagine]** e fare clic sul pulsante **[!UICONTROL Modifica contenuto]** per ogni pagina che desideri progettare per questa pagina di destinazione. Il contenuto di ogni pagina è già precompilato. Modificali in base alle esigenze. [Ulteriori informazioni](lp-content.md)

   ![](assets/lp-pages.png){zoomable=&quot;yes&quot;}

1. Il **[!UICONTROL Aggiornare il record precaricato]** è selezionata per impostazione predefinita. Consente di aggiornare i profili memorizzati nel database tramite la pagina di destinazione. La casella di precaricamento consente di indicare come trovare il record da aggiornare nel database.

   Puoi anche scegliere tra i campi nel contesto corrente della pagina di destinazione, quelli che verranno utilizzati per trovare il profilo corrispondente nel database. Per farlo, deseleziona la **[!UICONTROL Aggiornare il record precaricato]** e seleziona i campi desiderati in **[!UICONTROL Opzioni di riconciliazione]**.

   ![](assets/lp-storage.png){zoomable=&quot;yes&quot;}

1. Puoi definire una data di inizio e una data di fine per la pagina di destinazione. Seleziona **[!UICONTROL Abilita pianificazione]** e impostare le date.

   ![](assets/lp-schedule.png){zoomable=&quot;yes&quot;}

   * La pagina di destinazione viene pubblicata automaticamente nella data/ora di inizio specificata.

     >[!NOTE]
     >
     >Se non è definita alcuna data di inizio, la pagina di destinazione diventa attiva non appena viene pubblicata.

   * Quando la pagina raggiunge la data di fine, <!--the landing page is automatically unpublished and -->modulo non più disponibile. Viene invece visualizzata la pagina la pagina **[!UICONTROL Scadenza]**.

     >[!NOTE]
     >
     >Per motivi di sicurezza e prestazioni della piattaforma, l’Adobe consiglia di impostare una data di fine.

1. Clic **[!UICONTROL Revisione e pubblicazione]**.

Una volta definite tutte le impostazioni e [progettato](lp-content.md) tutte le pagine, puoi [test](#test-landing-page) e [pubblicare](#publish-landing-page) la pagina di destinazione come descritto di seguito.

## Verificare la pagina di destinazione {#test-landing-page}

>[!CONTEXTUALHELP]
>id="acw_landingpages_simulate"
>title="Simulare una pagina di destinazione"
>abstract="Puoi visualizzare un’anteprima della pagina di destinazione nell’interfaccia utente di Campaign Web oppure aprirla in una nuova scheda del browser web."

>[!CONTEXTUALHELP]
>id="ac_preview_lp_profiles"
>title="Visualizzare l’anteprima e testare la pagina di destinazione"
>abstract="Una volta definite le impostazioni e il contenuto della pagina di destinazione, puoi utilizzare i profili di test per visualizzarli in anteprima."

Una volta definiti le impostazioni e il contenuto della pagina di destinazione, puoi utilizzare i profili di test per visualizzarne l’anteprima. Se è stato inserito [contenuti personalizzati](../personalization/gs-personalization.md), potrai controllare come vengono visualizzati questi contenuti nella pagina di destinazione utilizzando i dati del profilo di test.

>[!CAUTION]
>
>Per poter visualizzare in anteprima i messaggi e inviare le bozze, è necessario disporre di profili di test. [Ulteriori informazioni sui profili di test](../audience/test-profiles.md)

Per verificare la pagina di destinazione, effettua le seguenti operazioni:

1. Dopo aver fatto clic su **[!UICONTROL Revisione e pubblicazione]**, seleziona la **[!UICONTROL Simula contenuto]** dal dashboard della pagina di destinazione per accedere alla selezione del profilo di test.

   ![](assets/lp-simulate-content.png){zoomable=&quot;yes&quot;}

1. Dalla sezione **[!UICONTROL Simula]** , seleziona uno o più profili di test.

   I passaggi per selezionare i profili di test sono gli stessi utilizzati per testare un messaggio. Sono descritte in dettaglio nella [Anteprima e test](../preview-test/preview-test.md) sezione.

1. Seleziona **[!UICONTROL Apri anteprima]** per verificare la pagina di destinazione.

   ![](assets/lp-open-preview.png){zoomable=&quot;yes&quot;}

1. L’anteprima della pagina di destinazione viene visualizzata in una nuova scheda. Gli elementi personalizzati vengono sostituiti dai dati del profilo di test selezionati.

   Se hai selezionato **[!UICONTROL Precompilare con i dati a cui si fa riferimento nel modulo]** nelle impostazioni della pagina di destinazione, i campi del modulo vengono precompilati automaticamente con i dati del profilo di test corrispondenti.<!--TBC-->

   ![](assets/lp-preview.png){zoomable=&quot;yes&quot;}

1. Seleziona altri profili di test per visualizzare in anteprima il rendering per ogni variante della pagina di destinazione.

<!--Can you preview Confirmation/Error/Expiration pages?-->

## Pubblicare la pagina di destinazione {#publish-landing-page}

Una volta che la pagina di destinazione è pronta e convalidata, pubblicala per renderla disponibile per l’utilizzo in una consegna utilizzando il pulsante corrispondente.

Dopo la pubblicazione:

* La pagina di destinazione viene aggiunta all’elenco delle pagine di destinazione con **[!UICONTROL Pubblicato]** stato. Ora è attivo e pronto per essere utilizzato come riferimento nei contenuti.

* È possibile copiare e incollare **[!UICONTROL URL della pagina di destinazione]** che viene visualizzata nella parte superiore della pagina in un browser web per visualizzare l’anteprima della pagina di destinazione.

>[!CAUTION]
>
>Per testare o sfruttare appieno la pagina di destinazione, non puoi copiare e incollare questo collegamento direttamente in un browser web o nelle consegne. Invece, utilizza [Simula contenuto](#test-landing-page) per testarlo e seguire i passaggi descritti in [questa sezione](lp-use-cases.md) per utilizzare correttamente la pagina di destinazione.

![](assets/lp-published.png){zoomable=&quot;yes&quot;}

Puoi monitorare l’impatto della pagina di destinazione tramite i registri<!--and specific reports-->. Fai clic su **[!UICONTROL Registri]** pulsante.
