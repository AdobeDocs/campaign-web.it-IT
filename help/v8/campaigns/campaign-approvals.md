---
audience: end-user
title: Impostare e gestire il processo di approvazione
description: Scopri come gestire le approvazioni di campagne di marketing in Campaign Web
feature: Approvals, Campaigns
source-git-commit: f238fde4a79d3303f2b5c9a2d26b11ffad8ac54e
workflow-type: tm+mt
source-wordcount: '694'
ht-degree: 4%

---

# Gestire il processo di approvazione {#campaign-approvals}

>[!IMPORTANT]
>
>Le approvazioni sono disponibili solo per le consegne create all’interno di una campagna. Questo non si applica alle consegne autonome o alle consegne create nei flussi di lavoro al di fuori di un contesto di campagna.

Il processo di approvazione aiuta a coordinare più parti interessate e garantisce il controllo di qualità prima dell’invio delle consegne. Utilizza le approvazioni quando l’organizzazione richiede la convalida da parte di team diversi, ad esempio responsabili marketing che rivedono il contenuto o analisti di dati che convalidano i tipi di pubblico target.

Quando le approvazioni sono abilitate, devi inviare il contenuto o la destinazione per l’approvazione. I revisori designati ricevono notifiche e-mail con richiesta di convalida e possono approvare o rifiutare direttamente dall’interfaccia utente web. Le consegne non possono essere inviate finché non vengono concesse tutte le approvazioni richieste. Puoi abilitare:

* **Approvazione del contenuto**: convalida contenuto, progettazione e personalizzazione del messaggio
* **Approvazione target**: convalida il pubblico e i criteri di targeting
* **Conferma consegna**: richiede una conferma finale prima dell&#39;invio

## Configurare le impostazioni di approvazione {#configure-approvals}

Le impostazioni di approvazione vengono ereditate dal modello della campagna e possono essere modificate per le singole campagne. Per configurare le impostazioni di approvazione, effettua le seguenti operazioni:

1. Apri la campagna o il modello di campagna o creane uno nuovo dal menu **[!UICONTROL Campagne]**.

1. Fai clic sul pulsante **[!UICONTROL Impostazioni]** in alto a destra nel dashboard della campagna.

1. Nella sezione **[!UICONTROL Approvazioni]**, configura le opzioni seguenti:

   ![Schermata che mostra le impostazioni di approvazione della campagna](assets/approvals1.png){zoomable="yes"}

   * **[!UICONTROL Abilita approvazione contenuto]**: se abilitata, il contenuto della consegna deve essere approvato prima dell&#39;invio. Fare clic sull&#39;icona della cartella nel campo **[!UICONTROL Revisore]** per selezionare un operatore o un gruppo di operatori.

   * **[!UICONTROL Abilita approvazione destinazione]**: se abilitata, il pubblico di destinazione della consegna deve essere approvato. Fare clic sull&#39;icona della cartella nel campo **[!UICONTROL Revisore]** per selezionare un operatore o un gruppo di operatori.

   * **[!UICONTROL Conferma la consegna prima dell&#39;invio]**: richiede una conferma manuale finale prima dell&#39;invio, anche dopo il completamento di tutte le altre approvazioni.

>[!NOTE]
>
>* Se non viene specificato alcun revisore, il proprietario della campagna viene assegnato come revisore.
>* I revisori devono disporre delle autorizzazioni appropriate per approvare le consegne. Solo gli utenti identificati nell’elenco dei revisori possono approvare.

## Invio per approvazione {#submit-approval}

Dopo aver creato la consegna, segui la procedura riportata di seguito per inviare il contenuto e il target per l’approvazione.

>[!NOTE]
>Le approvazioni sono disponibili sia nelle consegne del flusso di lavoro della campagna che nelle consegne autonome della campagna.

1. Dal dashboard di consegna, fare clic sul pulsante **[!UICONTROL Invia contenuto]**. I revisori designati possono approvare o rifiutare. Consulta questa [sezione](#approve-reject).

   ![Schermata che mostra il pulsante Invia contenuto](assets/approvals2.png){zoomable="yes"}

   Lo stato di approvazione cambia in sospeso nella sezione **[!UICONTROL Proprietà]** del dashboard di consegna. Consulta questa [sezione](#rack-approvals).

1. Una volta approvato il contenuto, fai clic sul pulsante **[!UICONTROL Prepara]** per preparare la destinazione della consegna. Il sistema prepara il pubblico e i criteri di targeting.

1. Fare clic sul pulsante **[!UICONTROL Invia destinazione]**. I revisori designati possono quindi approvare o rifiutare. Consulta questa [sezione](#approve-reject).

   ![Schermata che mostra il pulsante Invia destinazione](assets/approvals5.png){zoomable="yes"}

   Lo stato di approvazione cambia in In sospeso. Consulta questa [sezione](#rack-approvals).

1. Una volta approvato il target, la preparazione riprende e la consegna può essere inviata.

>[!NOTE]
>Se un’approvazione viene rifiutata, il proprietario della consegna deve apportare tutte le modifiche necessarie al contenuto o al target in base al feedback del revisore e inviarle nuovamente per l’approvazione.

## Approva o rifiuta {#approve-reject}

I revisori designati possono approvare o rifiutare i contenuti e gli invii di destinazione. Consulta questa [sezione](#submit-approval).

>[!NOTE]
>Affinché la notifica e-mail venga inviata, l’indirizzo del revisore deve essere configurato nell’istanza.

1. Quando ricevi l’e-mail di notifica, apri la consegna che richiede l’approvazione direttamente dall’interfaccia utente web.

1. Rivedi il contenuto o le informazioni di destinazione.

1. Fare clic sul pulsante **[!UICONTROL Approva contenuto]** o **[!UICONTROL Approva destinazione]**.

   ![Schermata che mostra il pulsante Approva contenuto nel dashboard di consegna](assets/approvals3.png){zoomable="yes"}

1. Fai clic su **[!UICONTROL Approva]** o **[!UICONTROL Rifiuta]**.

1. Se necessario, aggiungi un **[!UICONTROL commento]** per spiegare la tua decisione.

   ![Schermata che mostra la finestra di dialogo di approvazione con i pulsanti Approva, Rifiuta e il campo Commento](assets/approvals4.png){zoomable="yes"}

1. Conferma la tua decisione. Lo stato di approvazione viene aggiornato immediatamente nel dashboard di consegna. Consulta questa [sezione](#rack-approvals).

## Tracciare lo stato di approvazione {#track-approvals}

Lo stato di approvazione è visibile nella sezione **[!UICONTROL Proprietà]** del dashboard di consegna. Lo stato mostra quali approvazioni sono in attesa e il loro stato corrente:

![Schermata che mostra lo stato di approvazione](assets/approvals5.png){zoomable="yes"}

* **[!UICONTROL In fase di modifica]**: il contenuto o la destinazione non è ancora stato inviato per l&#39;approvazione
* **[!UICONTROL In attesa di approvazione]**: il contenuto o la destinazione è in attesa di revisione
* **[!UICONTROL Approvato]**: il contenuto o la destinazione è stata approvata dal revisore
* **[!UICONTROL Rifiutato]**: il contenuto o la destinazione è stata rifiutata dal revisore

La sezione approvazione mostra in tempo reale tutte le approvazioni e gli aggiornamenti abilitati quando i revisori convalidano o rifiutano ogni passaggio.

## Argomenti correlati {#related}

* [Creare campagne](create-campaigns.md)
* [Gestire le campagne](manage-campaigns.md)
