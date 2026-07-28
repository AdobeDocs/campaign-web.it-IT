---
title: Azioni di controllo sui dati
description: Scopri come limitare la creazione, la modifica e l’eliminazione di azioni sui record di schema personalizzati.
source-git-commit: 75aeccc9878bb0aab7bdaf62113303dbd14f985b
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 0%

---

# Azioni di controllo sui dati {#action-data}

>[!CONTEXTUALHELP]
>id="acw_schema_action_data"
>title="Dati delle azioni"
>abstract="Configura le azioni disponibili per le schermate di dettaglio e di elenco dello schema. Abilita **[!UICONTROL Sola lettura]** per impostare la schermata di dettaglio come di sola lettura e rimuovere le azioni dall&#39;elenco. Abilita **[!UICONTROL Non consentire eliminazione]** per rimuovere l&#39;azione di eliminazione dalle schermate dei dettagli e dell&#39;elenco."

La sezione **[!UICONTROL Dati azione]** ti consente di limitare le azioni disponibili nei record di uno schema personalizzato, indipendentemente dalle [regole di sicurezza](../get-started/work-with-folders.md) configurate nelle singole cartelle. Questa restrizione si applica a livello di schema, in ogni cartella, per ogni utente, inclusi gli amministratori.

>[!NOTE]
>
>Questa sezione è disponibile solo per gli schemi personalizzati.

Per ulteriori informazioni sulla schermata di definizione dello schermo e su come accedervi, fare riferimento alla sezione [Accedere alla definizione dello schermo](schemas-browse-access.md#screen-def).

Per configurare i dati delle azioni, segui i passaggi seguenti:

1. Accedi al menu **[!UICONTROL Schemi]** e individua gli schemi modificabili utilizzando i filtri.

1. Selezionare il nome dello schema nell&#39;elenco per aprirlo e fare clic sul pulsante **[!UICONTROL Screen edition]** nella visualizzazione dei dettagli dello schema per accedere alla definizione dello schermo.

1. Scorri verso il basso fino alla sezione **[!UICONTROL Dati azione]**, nella parte inferiore della definizione dello schermo.

   ![Sezione dati azione nella definizione dello schermo](assets/schemas-action-data1.png)

1. Selezionare una o entrambe le opzioni disponibili:

   * **[!UICONTROL Sola lettura]**: la schermata di dettaglio diventa di sola lettura per tutti gli utenti. Non è disponibile alcuna azione di creazione, duplicazione, aggiornamento o eliminazione dall&#39;elenco e le azioni di eliminazione e duplicazione sono nascoste dalla schermata di dettaglio. La selezione di questa opzione è simile alla configurazione di una visualizzazione: gli utenti possono ancora aprire i record e riutilizzarli, ad esempio quando eseguono il targeting di una consegna, ma non possono modificarli.

   * **[!UICONTROL Non consentire eliminazione]**: l&#39;azione di eliminazione viene rimossa dalla schermata di dettaglio e dall&#39;elenco in ogni cartella. Altre azioni, come la creazione, la duplicazione e l’aggiornamento, rimangono disponibili.

     >[!NOTE]
     >
     >L&#39;abilitazione di **[!UICONTROL Sola lettura]** copre automaticamente anche l&#39;eliminazione, pertanto l&#39;opzione **[!UICONTROL Non consentire eliminazione]** è disabilitata mentre è selezionata l&#39;opzione **[!UICONTROL Sola lettura]**.

1. Fai clic su **[!UICONTROL Salva]**.

1. Selezionare l&#39;elenco dei record per questo schema per verificare il risultato.

   In questo esempio, **[!UICONTROL Sola lettura]** è abilitato: nell&#39;elenco non vengono più visualizzate le azioni di duplicazione ed eliminazione.

   ![Rendering di sola lettura nella schermata elenco](assets/schemas-action-data2.png)

1. Aprire un record per controllare la schermata dei dettagli. I campi vengono visualizzati senza consentire alcuna modifica.

   ![Rendering di sola lettura nella schermata dei dettagli](assets/schemas-action-data3.png)
