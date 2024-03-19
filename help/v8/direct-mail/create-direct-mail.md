---
audience: end-user
title: Creare una consegna direct mailing
description: Scopri come creare una consegna di direct mailing con Adobe Campaign Web
source-git-commit: 717f6f2fb5e07213fb6a16f7ed701f450d1e257e
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 35%

---


# Creare una consegna direct mailing {#create-direct-mail}

Puoi creare una consegna di direct mailing autonoma o una consegna di direct mailing nel contesto di un flusso di lavoro della campagna. I passaggi seguenti descrivono la procedura per una consegna direct mailing indipendente (una tantum). Se lavori nel contesto di un flusso di lavoro della campagna, i passaggi di creazione sono descritti in [questa sezione](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow).

Per creare una nuova consegna di direct mailing autonoma, effettua le seguenti operazioni:

1. Passa al menu **[!UICONTROL Consegne]** nella barra di navigazione a sinistra, quindi fai clic sul pulsante **[!UICONTROL Crea consegna]**.

1. Sotto **[!UICONTROL Canale]** , scegliere **[!UICONTROL Direct mail]** come canale e seleziona un modello. [Ulteriori informazioni sui modelli](../msg/delivery-template.md)

1. Fai clic sul pulsante **[!UICONTROL Crea una consegna]** per confermare.

   ![](assets/dm-create.png){zoomable=&quot;yes&quot;}

1. Immetti un’**[!UICONTROL etichetta]** per la consegna e accedi al menu a discesa **[!UICONTROL Opzioni aggiuntive]**. Se la consegna è basata su uno schema esteso, sono disponibili campi specifici di **Opzioni personalizzate**.

   ![](assets/dm-properties.png){zoomable=&quot;yes&quot;}

   +++Configura le seguenti impostazioni in base alle tue esigenze.
   * **[!UICONTROL Nome interno]**: assegna un identificatore univoco alla consegna.
   * **[!UICONTROL Cartella]**: memorizza la consegna in una cartella specifica.
   * **[!UICONTROL Codice di consegna]**: organizza le consegne in base alla convenzione di denominazione.
   * **[!UICONTROL Descrizione]**: specifica una descrizione della consegna.
   * **[!UICONTROL Natura]**: specifica la natura della consegna a scopo di classificazione.
+++

1. Fai clic su **[!UICONTROL Seleziona pubblico]** per rivolgerti a un pubblico esistente o crearne uno tuo.

   * [Scopri come selezionare un pubblico esistente](../audience/add-audience.md)
   * [Scopri come creare un nuovo pubblico](../audience/one-time-audience.md)

   ![](assets/dm-audience.png){zoomable=&quot;yes&quot;}

   >[!NOTE]
   >
   >I destinatari della direct mailing devono contenere almeno i propri nomi e indirizzi postali. Un indirizzo è considerato completo se il nome, il campo CAP e i campi città non sono vuoti. Tutti i destinatari con indirizzi incompleti saranno esclusi dalle consegne di direct mailing.

1. Attiva l’opzione **[!UICONTROL Abilita gruppo di controllo]** per impostare un gruppo di controllo per misurare l’impatto della consegna. I messaggi non vengono inviati a tale gruppo di controllo, in modo da poter confrontare il comportamento della popolazione che ha ricevuto il messaggio con quello dei contatti che non lo hanno fatto. [Scopri come utilizzare i gruppi di controllo](../audience/control-group.md)

1. Clic **[!UICONTROL Modifica contenuto]** per definire le informazioni (colonne) da esportare nel file di estrazione. [Ulteriori informazioni](content-direct-mail.md)

   ![](assets/dm-content.png){zoomable=&quot;yes&quot;}

1. Per pianificare la consegna a una data e un’ora specifiche, attiva l’opzione **[!UICONTROL Abilita pianificazione]**. Dopo aver avviato la consegna, il file di estrazione viene generato automaticamente alla data e all’ora esatte definite. [Scopri come pianificare le consegne](../msg/gs-messages.md#gs-schedule).

   >[!NOTE]
   >
   >Quando una consegna viene inviata nel contesto di un flusso di lavoro, devi utilizzare **Scheduler** attività. Per ulteriori informazioni, consulta [questa pagina](../workflows/activities/scheduler.md).

1. Clic **[!UICONTROL Impostazioni]** per accedere alle opzioni avanzate relative al modello di consegna. [Ulteriori informazioni](../advanced-settings/delivery-settings.md)

   ![](assets/dm-settings.png){zoomable=&quot;yes&quot;}

1. Quando la consegna direct mailing è pronta, fai clic sul pulsante **[!UICONTROL Rivedi e invia]** per convalidare e inviare la consegna e generare il file di estrazione. [Scopri come visualizzare in anteprima e inviare una consegna direct mailing](send-direct-mail.md)

