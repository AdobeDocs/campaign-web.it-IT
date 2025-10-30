---
audience: end-user
title: Creare una consegna direct mail
description: Scopri come creare una consegna di direct mailing con Adobe Campaign Web
exl-id: 9b5172b2-1880-4768-a33b-8a20ec5a30ab
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 23%

---

# Creare una consegna direct mail {#create-direct-mail}

Puoi creare una consegna di direct mailing autonoma o una consegna di direct mailing nel contesto di un flusso di lavoro della campagna. I passaggi seguenti descrivono la procedura per una consegna direct mailing indipendente (una tantum). Se lavori nel contesto di un flusso di lavoro della campagna, i passaggi di creazione sono descritti in [questa sezione](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow).

Per creare una nuova consegna di direct mailing autonoma, effettua le seguenti operazioni:

1. Passa al menu **[!UICONTROL Consegne]** nella barra a sinistra e fai clic sul pulsante **[!UICONTROL Crea consegna]**.

1. Nella sezione **[!UICONTROL Canale]**, scegli **[!UICONTROL Direct mail]** come canale e seleziona un modello. [Ulteriori informazioni sui modelli](../msg/delivery-template.md)

1. Fai clic sul pulsante **[!UICONTROL Crea una consegna]** per confermare.

   ![Schermata che mostra la creazione di una consegna direct mailing](assets/dm-create.png){zoomable="yes"}

1. Immetti un **[!UICONTROL Label]** per la consegna e accedi al menu a discesa **[!UICONTROL Opzioni aggiuntive]**. Se la consegna è basata su uno schema esteso, sono disponibili campi specifici di **Opzioni personalizzate**.

   ![Schermata che mostra la configurazione delle proprietà per una consegna direct mailing](assets/dm-properties.png){zoomable="yes"}

   +++Configura le seguenti impostazioni in base alle tue esigenze.
   * **[!UICONTROL Nome interno]**: assegna un identificatore univoco alla consegna.
   * **[!UICONTROL Cartella]**: memorizza la consegna in una cartella specifica.
   * **[!UICONTROL Codice di consegna]**: organizza le consegne in base alla convenzione di denominazione.
   * **[!UICONTROL Descrizione]**: specifica una descrizione della consegna.
   * **[!UICONTROL Natura]**: specifica la natura della consegna a scopo di classificazione.
   +++

1. Fai clic sul pulsante **[!UICONTROL Seleziona pubblico]** per eseguire il targeting di un pubblico esistente o crearne uno tuo.

   * [Scopri come selezionare un pubblico esistente](../audience/add-audience.md)
   * [Scopri come creare un nuovo pubblico](../audience/one-time-audience.md)

   ![Schermata che mostra la selezione del pubblico per una consegna direct mailing](assets/dm-audience.png){zoomable="yes"}

   >[!NOTE]
   >
   >I destinatari della direct mailing devono contenere almeno i propri nomi e indirizzi postali. Un indirizzo è considerato completo se il nome, il campo CAP e i campi città non sono vuoti. Tutti i destinatari con indirizzi incompleti saranno esclusi dalle consegne di direct mailing.

1. Attiva l’opzione **[!UICONTROL Abilita gruppo di controllo]** per impostare un gruppo di controllo per misurare l’impatto della consegna. I messaggi non vengono inviati a tale gruppo di controllo, pertanto puoi confrontare il comportamento della popolazione che ha ricevuto il messaggio con quello dei contatti che non lo hanno fatto. [Scopri come utilizzare i gruppi di controllo](../audience/control-group.md)

1. Fare clic su **[!UICONTROL Modifica contenuto]** per definire le informazioni (colonne) da esportare nel file di estrazione. [Ulteriori informazioni](content-direct-mail.md)

   ![Schermata che mostra la modifica del contenuto per una consegna direct mailing](assets/dm-content.png){zoomable="yes"}

1. Per pianificare la consegna a una data e un’ora specifiche, attiva l’opzione **[!UICONTROL Abilita pianificazione]**. Dopo aver avviato la consegna, il file di estrazione viene generato automaticamente alla data e all’ora esatte definite. [Scopri come pianificare le consegne](../msg/gs-deliveries.md#gs-schedule).

   >[!NOTE]
   >
   >Quando una consegna viene inviata nel contesto di un flusso di lavoro, è necessario utilizzare l&#39;attività **Scheduler**. Ulteriori informazioni su [questa pagina](../workflows/activities/scheduler.md).

1. Fai clic su **[!UICONTROL Impostazioni]** per accedere alle opzioni avanzate relative al modello di consegna. [Ulteriori informazioni](../advanced-settings/delivery-settings.md)

   ![Schermata che mostra le impostazioni avanzate per una consegna direct mailing](assets/dm-settings.png){zoomable="yes"}

1. Quando la consegna direct mailing è pronta, fai clic sul pulsante **[!UICONTROL Rivedi e invia]** per convalidare e inviare la consegna e generare il file di estrazione. [Scopri come visualizzare in anteprima e inviare una consegna direct mailing](send-direct-mail.md)