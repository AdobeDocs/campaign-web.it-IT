---
title: Creare profili di test in Campaign
description: Scopri come creare e gestire i profili di test in Adobe Campaign
feature: Audiences, Profiles, Seed Address, Proofs
role: User
level: Beginner
badge: label="Disponibilità limitata"
source-git-commit: 78f9bba52f33fac0e444afb3476873d931a873d1
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 3%

---

# Creare e gestire i profili di test {#create-test-profiles}

>[!CONTEXTUALHELP]
>id="acw_recipients_testprofiles_menu"
>title="Creare profili di test"
>abstract="I profili di test vengono creati come indirizzi di seed. Si tratta di destinatari aggiuntivi nel database utilizzato per eseguire il targeting di profili fittizi che non corrispondono ai criteri di destinazione definiti."

I profili di test vengono creati come indirizzi di seed. Si tratta di destinatari aggiuntivi nel database utilizzato per eseguire il targeting di profili fittizi che non corrispondono ai criteri di destinazione definiti. Ti consentono di visualizzare in anteprima e testare la personalizzazione e il rendering prima di inviare la consegna, inviando loro delle bozze.

<!--Learn more on test profiles in the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html){target="_blank"}.-->

I passaggi per inviare messaggi di test agli indirizzi di seed sono descritti in [questa sezione](../preview-test/test-deliveries.md#test-profiles).

>[!NOTE]
>
>I profili di test vengono esclusi automaticamente dai rapporti sulle seguenti statistiche di consegna: **[!UICONTROL Clic]**, **[!UICONTROL Aperture]**, **[!UICONTROL Annullamenti iscrizione]**.

## Accedere e gestire i profili di test {#access-test-profiles}

Per accedere all’elenco dei profili di test, seleziona **[!UICONTROL Gestione clienti]** > **[!UICONTROL Profili]** dal menu a sinistra e fare clic su **[!UICONTROL Profili di test]** scheda.

![](assets/test-profile-list.png)

Puoi filtrare in base a una [cartella](../get-started/permissions.md#folders) utilizzando l’elenco a discesa o aggiungere regole utilizzando [query modeler](../query/query-modeler-overview.md).

![](assets/test-profile-list-filters.png)

Per modificare un profilo di test, fai clic sull’elemento desiderato dall’elenco.

Per eliminare un profilo di test, seleziona l’opzione corrispondente dal menu **[!UICONTROL Altre azioni]** menu.

![](assets/test-profile-list-delete.png)

## Creare un profilo di test {#create-test-profile}

>[!CONTEXTUALHELP]
>id="acw_recipients_testprofiles_additionaldata"
>title="Dati aggiuntivi dei profili di test"
>abstract="Immetti i dati di personalizzazione utilizzati per le consegne create nei flussi di lavoro di gestione dati e a cui desideri assegnare un valore specifico."

Per creare un profilo di test, segui i passaggi indicati di seguito.

1. Sfoglia per **[!UICONTROL Gestione clienti]** > **[!UICONTROL Profili]** e seleziona la **[!UICONTROL Profili di test]** scheda.

1. Fai clic su **[!UICONTROL Creare un profilo di test]** pulsante.

1. Inserisci i dettagli del profilo di test. <!--Most of the fields are the same as when creating profiles. [Learn more]-->

   ![](assets/test-profile-details.png)

   >[!NOTE]
   >
   >Il **[!UICONTROL Etichetta]** viene compilato automaticamente con il nome e il cognome definiti.

1. Per impostazione predefinita, i profili di test sono memorizzati nella **[!UICONTROL Indirizzi seed]** cartella. Puoi modificarlo navigando nella posizione desiderata. [Ulteriori informazioni](#seed-addresses-folders)

   ![](assets/test-profile-folder.png)

<!--
You do not need to enter all fields of each tab when creating a seed address. Missing personalization elements are entered randomly during delivery analysis. (Not valid?)
-->

1. In **[!UICONTROL Informazioni di contatto]** , immettere l&#39;indirizzo di posta elettronica e altri dati rilevanti. L’indirizzo e-mail viene visualizzato tra parentesi dopo l’etichetta del profilo di test.

   ![](assets/test-profile-address.png)

1. Se si seleziona la **[!UICONTROL Non contattare più (tramite alcun canale)]** , il profilo è in fase di inserisco nell&#39;elenco Bloccati. Tale destinatario non è più destinatario di alcun canale (e-mail, SMS, ecc.).

1. In **[!UICONTROL Dati aggiuntivi]** , immetti i dati di personalizzazione utilizzati per le consegne create nei flussi di lavoro di gestione dati e a cui desideri assegnare un valore specifico. [Ulteriori informazioni sui flussi di lavoro](../workflows/gs-workflows.md)

   ![](assets/test-profile-additional-data.png)

   Assicurati che siano stati definiti dati di destinazione aggiuntivi con un alias che inizia con &quot;@&quot; nel **[!UICONTROL Arricchimento]** attività del flusso di lavoro. In caso contrario, non puoi utilizzarlo correttamente con gli indirizzi seed nell’attività di consegna. [Ulteriori informazioni sull’attività Enrichment](../workflows/activities/enrichment.md)

1. Fai clic su **[!UICONTROL Salva]** pulsante.

Il profilo di test appena creato è ora pronto per essere utilizzato per inviare un test. [Ulteriori informazioni](../preview-test/test-deliveries.md#test-profiles)

<!--Use test profiles in Direct mail? cf v7/v8-->

## Gestire le cartelle degli indirizzi seed {#seed-addresses-folders}

Gli indirizzi di seed vengono memorizzati in un nodo dedicato della gerarchia di Adobe Campaign: **[!UICONTROL Esplora]** > **[!UICONTROL Risorse]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Indirizzi seed]**.

Per organizzare i profili di test, puoi creare sottocartelle dall’elenco a discesa Altre azioni. [Scopri come creare cartelle](../get-started/permissions.md#folders)

![](assets/test-profile-sub-folders.png)

Puoi anche creare un profilo di test da qualsiasi **[!UICONTROL Indirizzi seed]** cartella o sottocartella. Compila tutti i dettagli nello stesso modo in cui lo faresti dalla **[!UICONTROL Gestione clienti]** > **[!UICONTROL Profili]** menu. [Ulteriori informazioni](#create-test-profile)

Per modificare un profilo di test, fai clic sulla relativa etichetta nell’area **[!UICONTROL Profili di test]** dalla cartella in cui è memorizzato.


