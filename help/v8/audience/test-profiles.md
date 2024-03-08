---
title: Creare profili di test in Campaign
description: Scopri come creare e gestire i profili di test in Adobe Campaign
feature: Audiences, Profiles, Seed Address, Proofs
role: User
level: Beginner
exl-id: d372713d-3024-46a1-b62e-f271b8ac829f
source-git-commit: 3879f217f3a6a1cae0d6c924733d2ef1fd4ab9e7
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 9%

---

# Creare e gestire profili di test {#create-test-profiles}

>[!CONTEXTUALHELP]
>id="acw_recipients_testprofiles_menu"
>title="Creare profili di test"
>abstract="I profili di test sono destinatari aggiuntivi che ti consentono di visualizzare in anteprima e testare la personalizzazione e il rendering prima di inviare i messaggi. Puoi selezionare un profilo di test quando visualizzi l’anteprima del contenuto di un messaggio e inviare bozze ai profili di test per controllare e convalidare il contenuto e le impostazioni del messaggio."

I profili di test vengono utilizzati per inviare bozze e convalidare il contenuto e le impostazioni del messaggio. Questi profili sono destinatari aggiuntivi che ti consentono di visualizzare in anteprima e testare la personalizzazione e il rendering prima di inviare i messaggi. Puoi selezionare un profilo di test quando visualizzi l’anteprima del contenuto di un messaggio e inviare bozze ai profili di test per controllare e convalidare il contenuto e le impostazioni del messaggio.

<!--Learn more on test profiles in the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html){target="_blank"}.-->

I passaggi per inviare bozze ai profili di test sono descritti in [questa sezione](../preview-test/test-deliveries.md#test-profiles).

>[!NOTE]
>
>* I profili di test vengono creati come indirizzi di seed nella console Client.
>
>* I profili di test vengono esclusi automaticamente dai rapporti sulle seguenti statistiche di consegna: **[!UICONTROL Clic]**, **[!UICONTROL Aperture]**, **[!UICONTROL Annullamenti iscrizione]**.

## Accedere e gestire i profili di test {#access-test-profiles}

Per accedere all’elenco dei profili di test, seleziona **[!UICONTROL Gestione clienti]** > **[!UICONTROL Profili]** dal menu a sinistra e fare clic su **[!UICONTROL Profili di test]** scheda.

![](assets/test-profile-list.png){zoomable=&quot;yes&quot;}

* Puoi filtrare in base a una [cartella](../get-started/permissions.md#folders) utilizzando l’elenco a discesa o aggiungere regole utilizzando [query modeler](../query/query-modeler-overview.md).

  ![](assets/test-profile-list-filters.png){zoomable=&quot;yes&quot;}

* Puoi duplicare qualsiasi profilo di test e aggiornarlo in base alle esigenze. I passaggi per modificare un profilo di test sono gli stessi di quando [creazione di un profilo di test](#create-test-profile).

* Per eliminare un profilo di test, seleziona l’opzione corrispondente dal menu **[!UICONTROL Altre azioni]** menu.

  ![](assets/test-profile-list-delete.png){zoomable=&quot;yes&quot;}

* Per modificare un profilo di test, fai clic sull’elemento desiderato dall’elenco. I passaggi per modificare un profilo di test sono gli stessi di quando [creazione di un profilo di test](#create-test-profile).

Puoi anche accedere ai profili di test tramite **[!UICONTROL Esplora]** vista, da **[!UICONTROL Risorse]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Indirizzi seed]** nodo.

Da qui è possibile sfogliare, creare e gestire cartelle o sottocartelle, nonché verificare le autorizzazioni associate. [Scopri come creare cartelle](../get-started/permissions.md#folders)

![](assets/test-profiles-folders.png){zoomable=&quot;yes&quot;}

Dalla sezione **[!UICONTROL Esplora]** visualizzazione puoi anche filtrare, eliminare, modificare e [creare](#create-test-profile) profili di test.

## Creare un profilo di test {#create-test-profile}

>[!CONTEXTUALHELP]
>id="acw_recipients_testprofiles_additionaldata"
>title="Dati aggiuntivi dei profili di test"
>abstract="Immetti i dati di personalizzazione utilizzati per le consegne create nei flussi di lavoro di gestione dati a cui desideri assegnare un valore specifico."

Per creare un profilo di test, effettua le seguenti operazioni:

1. Sfoglia per **[!UICONTROL Gestione clienti]** > **[!UICONTROL Profili]** e seleziona la **[!UICONTROL Profili di test]** scheda.

1. Fai clic su **[!UICONTROL Creare un profilo di test]** pulsante.

   ![](assets/test-profile-create.png){zoomable=&quot;yes&quot;}

1. Compila i dettagli del profilo di test, se necessario. <!--Most of the fields are the same as when creating profiles. [Learn more]-->

   ![](assets/test-profile-details.png){zoomable=&quot;yes&quot;}

   >[!NOTE]
   >
   >Il **[!UICONTROL Etichetta]** viene compilato automaticamente con il nome e il cognome definiti.

1. Per impostazione predefinita, i profili di test sono memorizzati nella **[!UICONTROL Indirizzi seed]** cartella. Puoi modificarlo navigando nella posizione desiderata. [Scopri come utilizzare le cartelle](../get-started/permissions.md#folders)

   <!--![](assets/test-profile-folder.png){zoomable="yes"}-->

<!--
You do not need to enter all fields of each tab when creating a seed address. Missing personalization elements are entered randomly during delivery analysis. (Not valid?)
-->

1. In **[!UICONTROL Informazioni di contatto]** , immettere l&#39;indirizzo di posta elettronica e altri dati rilevanti. L’indirizzo e-mail viene visualizzato tra parentesi dopo l’etichetta del profilo di test.

   ![](assets/test-profile-address.png){zoomable=&quot;yes&quot;}

1. Se si seleziona la **[!UICONTROL Non contattare più (tramite alcun canale)]** , il profilo di test è in fase di inserisco nell&#39;elenco Bloccati. Tale destinatario non è più destinatario di alcun canale (e-mail, SMS, ecc.).

1. In **[!UICONTROL Dati aggiuntivi]** , immetti i dati di personalizzazione utilizzati per le consegne create nei flussi di lavoro di gestione dati e a cui desideri assegnare un valore specifico. [Ulteriori informazioni sui flussi di lavoro](../workflows/gs-workflows.md)

   ![](assets/test-profile-additional-data.png){zoomable=&quot;yes&quot;}

   Assicurati che siano stati definiti dati di destinazione aggiuntivi con un alias che inizia con &quot;@&quot; nel **[!UICONTROL Arricchimento]** attività del flusso di lavoro. In caso contrario, non puoi utilizzarlo correttamente con gli indirizzi seed nell’attività di consegna. [Ulteriori informazioni sull’attività Enrichment](../workflows/activities/enrichment.md)

1. Fai clic su **[!UICONTROL Salva]** pulsante.

Il profilo di test appena creato è ora pronto per essere utilizzato per inviare una bozza. [Ulteriori informazioni](../preview-test/test-deliveries.md#test-profiles)

<!--Use test profiles in Direct mail? cf v7/v8-->
