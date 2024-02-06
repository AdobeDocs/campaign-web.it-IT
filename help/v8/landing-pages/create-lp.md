---
title: Creare una pagina di destinazione
description: Scopri come configurare e pubblicare una pagina di destinazione in Campaign Web
badge: label="Disponibilità limitata"
source-git-commit: 7635ab284900c8a4cd5ceca5675e57dbedb39f3a
workflow-type: tm+mt
source-wordcount: '1006'
ht-degree: 7%

---

# Creare e pubblicare pagine di destinazione {#create-lp}

>[!CONTEXTUALHELP]
>id="acw_landingpages_menu"
>title="Creare e gestire le pagine di destinazione"
>abstract="Adobe Campaign consente di creare, progettare e condividere pagine di destinazione per indirizzare gli utenti a pagine web online in cui gestire acquisizioni, abbonamenti/annullamenti di abbonamenti e casi di utilizzo di elenchi Bloccati, in base a modelli incorporati."

Adobe Campaign consente di creare, progettare e condividere pagine di destinazione per indirizzare gli utenti a pagine web online in cui gestire acquisizioni, abbonamenti/annullamenti di abbonamenti e casi di utilizzo di elenchi Bloccati, in base a modelli incorporati.

## Accedere alle pagine di destinazione {#access-landing-pages}

Per accedere all’elenco delle pagine di destinazione, seleziona **[!UICONTROL Gestione delle campagne]** > **[!UICONTROL Pagine di destinazione]** dal menu a sinistra.

![](assets/lp-inventory.png)

Il **[!UICONTROL Pagine di destinazione]** inventory visualizza tutti gli articoli creati. Puoi filtrarli utilizzando **Mostra filtri** pulsante. È possibile limitare i risultati a uno specifico [cartella](../get-started/permissions.md#folders) utilizzando l’elenco a discesa, oppure aggiungi regole utilizzando [query modeler](../query/query-modeler-overview.md).

![](assets/lp-inventory-filter.png)

<!--From this list, you can access the [landing page Live report](../reports/lp-report-live.md) or [landing page Global report](../reports/lp-report-global.md) for published items.-->

>[!CAUTION]
>
>Non è possibile visualizzare o modificare le pagine di destinazione create dalla console client in Campaign Web. Per ulteriori informazioni, consulta [Documentazione della console di Campaign](https://experienceleague.adobe.com/docs/campaign/campaign-v8/content/webapps.html){target="_blank"}.

<!--If you unpublish a landing page which is referenced in a message, the link to the landing page will be broken and an error page will be displayed. You cannot delete a published landing page. To delete it, you must first unpublish it.-->

Puoi duplicare o eliminare una pagina di destinazione. Fai clic sui tre punti accanto a una pagina di destinazione per selezionare l’azione desiderata.

## Creare una pagina di destinazione {#create-landing-page}

>[!CONTEXTUALHELP]
>id="acw_landingpages_properties"
>title="Definire le proprietà della pagina di destinazione"
>abstract="Compila i campi delle proprietà, ad esempio l’etichetta, e modifica lo schema, se necessario. Inoltre, puoi modificare il nome interno, cambiare la cartella in cui è memorizzata la pagina di destinazione e fornire una descrizione."

>[!CONTEXTUALHELP]
>id="acw_landingpages_pages_list"
>title="Definire il contenuto delle pagine"
>abstract="Modifica il contenuto di ogni pagina che fa parte di questa pagina di destinazione."

>[!CONTEXTUALHELP]
>id="acw_landingpages_schedule"
>title="Pianificare la pagina di destinazione"
>abstract="Puoi definire una data di inizio e una data di fine per la pagina di destinazione. Quando la pagina è scaduta, il **Scade** viene visualizzata."


>[!CONTEXTUALHELP]
>id="acw_landingpages_primarypage"
>title="Definire le impostazioni della pagina principale"
>abstract="La pagina principale viene visualizzata immediatamente dagli utenti dopo aver fatto clic sul collegamento alla pagina di destinazione, ad esempio da un’e-mail o da un sito web."

>[!CONTEXTUALHELP]
>id="acw_landingpages_subscription"
>title="Impostare la pagina di destinazione dell’abbonamento"
>abstract="Una pagina di abbonamento consente ai clienti di abbonarsi a un servizio."

<!--The main steps to create landing pages are as follows:

![](assets/lp-creation-process.png)-->

1. Dalla sezione **[!UICONTROL Pagine di destinazione]** inventory, fai clic su **[!UICONTROL Crea pagina di destinazione]**.

   ![](assets/lp-create-button.png)

1. Seleziona un modello:
   * **[!UICONTROL Acquisizione]**: questo è il modello predefinito per le pagine di destinazione, che ti consente di acquisire e aggiornare i dati del profilo.
   * **[!UICONTROL Abbonamento]**: utilizza questo modello per offrire abbonamenti a un servizio.
   * **[!UICONTROL Annullamento iscrizione]**: è possibile collegare questo modello da un’e-mail inviata agli abbonati a un servizio, per consentire loro di annullare l’abbonamento a tale servizio.
   * **[!UICONTROL Inserisco nell&#39;elenco Bloccati]**: questo modello deve essere utilizzato quando un profilo non desidera più essere contattato da Campaign. Ulteriori informazioni sulla gestione dei inserisce nell&#39;elenco Bloccati di

   ![](assets/lp-templates.png)

1. Fai clic su **[!UICONTROL Crea]**.

1. Compila i campi delle proprietà, ad esempio l’etichetta. Per impostazione predefinita, le pagine di destinazione sono memorizzate in **[!UICONTROL Applicazioni web]** cartella. È possibile modificarlo individuando la posizione desiderata nella **[!UICONTROL Opzioni aggiuntive]**. [Scopri come utilizzare le cartelle](../get-started/permissions.md#folders)

   ![](assets/lp-properties.png)

1. In **[!UICONTROL Precaricamento dati]** , le due opzioni seguenti sono selezionate per impostazione predefinita:

   * Il **[!UICONTROL Precompilare con i dati a cui si fa riferimento nel modulo]** consente di precaricare automaticamente i dati che corrispondono ai campi di input e di unione nel modulo.

   * Il **[!UICONTROL Salta il precaricamento se non è presente alcun ID]** deve essere selezionata se non desideri aggiornare i profili. In questo caso, ogni profilo inserito verrà aggiunto al database dopo l’approvazione del modulo. Questa opzione viene utilizzata, ad esempio, quando il modulo viene pubblicato su un sito Web.

1. In **[!UICONTROL Pagine]** , fare clic sul pulsante **[!UICONTROL Modifica contenuto]** per ogni pagina che desideri progettare per questa pagina di destinazione. Il contenuto di ogni pagina è già precompilato. Modificali in base alle esigenze. [Ulteriori informazioni](lp-content.md)

   ![](assets/lp-pages.png)

1. Il **[!UICONTROL Aggiornare il record precaricato]** è selezionata per impostazione predefinita. Se desideri aggiornare i profili memorizzati nel database tramite la pagina di destinazione, puoi utilizzare una casella di precaricamento. La casella di precaricamento consente di indicare come trovare il record da aggiornare nel database. Puoi anche scegliere tra i campi nel contesto corrente della pagina di destinazione, quelli che verranno utilizzati per trovare il profilo corrispondente nel database.

   ![](assets/lp-storage-schedule.png)

1. Puoi definire una data di inizio e una data di fine per la pagina di destinazione. Seleziona **[!UICONTROL Abilita pianificazione]** e impostare le date. Quando la pagina è scaduta, il **[!UICONTROL Scade]** viene visualizzata.

1. Clic **[!UICONTROL Revisione e pubblicazione]**.

Dopo aver configurato e progettato tutte le pagine, puoi [test](#test-landing-page) e [pubblicare](#publish-landing-page) la pagina di destinazione.

## Verifica della pagina di destinazione {#test-landing-page}

>[!CONTEXTUALHELP]
>id="acw_landingpages_simulate"
>title="Simulare la pagina di destinazione"
>abstract="Puoi visualizzare un’anteprima della pagina di destinazione nell’interfaccia utente di Campaign Web oppure aprirla in una nuova scheda del browser web."

>[!CONTEXTUALHELP]
>id="ac_preview_lp_profiles"
>title="Visualizzare l’anteprima e testare la pagina di destinazione"
>abstract="Una volta definite le impostazioni e il contenuto della pagina di destinazione, puoi utilizzare i profili di test per visualizzarli in anteprima."

Una volta definiti le impostazioni e il contenuto della pagina di destinazione, puoi utilizzare i profili di test per visualizzarne l’anteprima. Se è stato inserito [contenuti personalizzati](../personalization/gs-personalization.md), potrai controllare come vengono visualizzati questi contenuti nella pagina di destinazione utilizzando i dati del profilo di test.

>[!CAUTION]
>
>Per poter visualizzare in anteprima i messaggi e inviare le bozze, è necessario disporre di profili di test. Scopri come [creare profili di test](../audience/test-profiles.md).

1. Nell’interfaccia della pagina di destinazione, fai clic su **[!UICONTROL Simula contenuto]** per accedere alla selezione del profilo di test.

   ![](assets/lp-simulate-content.png)

1. Dalla sezione **[!UICONTROL Simula]** , seleziona uno o più profili di test.

   I passaggi per selezionare i profili di test sono gli stessi utilizzati per testare un messaggio. Sono descritte in dettaglio nella [Anteprima e test](../preview-test/preview-test.md) sezione.

1. Seleziona **[!UICONTROL Apri anteprima]** per verificare la pagina di destinazione.

   ![](assets/lp-open-preview.png)

1. L’anteprima della pagina di destinazione viene visualizzata in una nuova scheda. Gli elementi personalizzati vengono sostituiti dai dati del profilo di test selezionati.

   ![](assets/lp-preview.png)

1. Seleziona altri profili di test per visualizzare in anteprima il rendering per ogni variante della pagina di destinazione.

<!--Can you preview Confirmation/Error/Expiration pages?-->

## Pubblicare la pagina di destinazione {#publish-landing-page}

Una volta che la pagina di destinazione è pronta, puoi pubblicarla per renderla disponibile per l’utilizzo in un messaggio.

Una volta pubblicata, la pagina di destinazione viene aggiunta all’elenco delle pagine di destinazione con **[!UICONTROL Pubblicato]** stato. Ora è attivo e pronto per essere utilizzato.

![](assets/lp-published.png)

Dopo la pubblicazione, puoi copiare e incollare i **[!UICONTROL URL della pagina di destinazione]** che viene visualizzata nella parte superiore della pagina in un browser web.

Puoi monitorare l’impatto della pagina di destinazione tramite registri e rapporti specifici.
