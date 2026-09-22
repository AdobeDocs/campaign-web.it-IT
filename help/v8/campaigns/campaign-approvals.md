---
audience: end-user
title: Impostare e gestire il processo di approvazione
description: Scopri come gestire le approvazioni di campagne di marketing in Campaign Web
feature: Approvals, Campaigns
exl-id: 8140f904-ec0a-44e1-981f-0e050d3c9cdb
TQID: https://experienceleague.adobe.com/Gpk7fY-VSFdgvgJo2STGjJ8-mHBkVZnp8cD-bFZrWpU
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
    internal-label: Campaigns
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
    internal-label: Personalization
source-git-commit: 1c4cdd5164d0cf572e9b88881bbe240b06308866
workflow-type: tm+mt
source-wordcount: '932'
ht-degree: 8%
---
# Gestire il processo di approvazione {#campaign-approvals}

>[!IMPORTANT]
>
>Le approvazioni sono disponibili solo per le campagne e le consegne create all’interno di una campagna.

Il processo di approvazione aiuta a coordinare più stakeholder e garantisce il controllo di qualità prima dell’invio delle consegne. Utilizza le approvazioni quando l’organizzazione richiede la convalida da parte di team diversi, ad esempio responsabili di marketing che rivedono il contenuto o analisti di dati che convalidano i tipi di pubblico target.

Quando le approvazioni sono abilitate, devi inviare il contenuto o la destinazione per l’approvazione. I revisori designati ricevono notifiche e-mail con richiesta di convalida e possono approvare o rifiutare direttamente dall’interfaccia utente web. Le consegne non possono essere inviate finché non vengono concesse tutte le approvazioni richieste. Puoi abilitare:

* **Approvazione del contenuto**: convalida contenuto, progettazione e personalizzazione del messaggio. È possibile aggiungere un passaggio di modifica prima dell’approvazione del contenuto, gestito da un operatore designato, e un passaggio di approvazione per un revisore esterno una volta che il contenuto è stato approvato internamente.
* **Approvazione target**: convalida il pubblico e i criteri di targeting
* **Approvazione del budget**: convalida il budget di consegna
* **Inizio consegna**: limita chi può iniziare a inviare la consegna a un revisore specifico
* **Conferma consegna**: richiede una conferma finale prima dell&#39;invio

## Configurare le impostazioni di approvazione {#configure-approvals}

Le impostazioni di approvazione vengono ereditate dal modello della campagna e possono essere modificate per le singole campagne. La stessa sezione **[!UICONTROL Approvazioni]** è disponibile anche nelle impostazioni di una consegna creata all&#39;interno di una campagna, consentendo di ignorare la configurazione a livello di campagna solo per tale consegna.

Per configurare le impostazioni di approvazione a livello di campagna, segui la procedura riportata di seguito:

1. Apri la campagna o il modello di campagna o creane uno nuovo dal menu **[!UICONTROL Campagne]**.

1. Fai clic sul pulsante **[!UICONTROL Impostazioni]** in alto a destra nel dashboard della campagna.

1. Nella sezione **[!UICONTROL Approvazioni]**, configura le opzioni seguenti:

   ![Schermata che mostra le impostazioni di approvazione della campagna](assets/approvals1.png){zoomable="yes"}

   >[!NOTE]
   >
   > Se decidi di abilitare un&#39;opzione di approvazione, fai clic sull&#39;icona della cartella nel campo **[!UICONTROL Revisore]** per selezionare un operatore o un gruppo di operatori.

1. Configura **[!UICONTROL Approvazione contenuto]**: se abilitata, il contenuto della consegna deve essere approvato prima dell&#39;invio. Quando questa opzione è abilitata, vengono visualizzati due campi:

   * **[!UICONTROL Assegna modifica contenuto]**: aggiunge un passaggio di modifica prima dell&#39;approvazione del contenuto. A un operatore designato, ad esempio un webmaster, viene notificato di modificare il contenuto e quindi di renderlo disponibile per l’approvazione.
   * **[!UICONTROL Approvazione del contenuto esterno]**: aggiunge un passaggio di approvazione per un revisore esterno, ad esempio un partner o un fornitore, che convalida il rendering della consegna (ad esempio la coerenza del marchio) dopo l&#39;approvazione interna del contenuto.

1. Definisci l&#39;**[!UICONTROL approvazione target]**: se abilitata, il pubblico di destinazione della consegna deve essere approvato.

1. Imposta l&#39;**[!UICONTROL approvazione budget]**: se abilitata, il budget di consegna deve essere approvato. Questa opzione richiede l’assegnazione di un budget alla campagna, operazione che al momento viene eseguita dalla console client.

1. Imposta **[!UICONTROL Inizio consegna]**: limita l&#39;inizio della consegna a un operatore o gruppo di operatori specifico. Se un operatore non autorizzato tenta di inviare la consegna, viene visualizzato un errore che indica che non è autorizzato a eseguire questa azione.

1. Imposta **[!UICONTROL Conferma la consegna prima dell&#39;invio]**: richiede una conferma manuale finale prima dell&#39;invio, anche dopo il completamento di tutte le altre approvazioni.

>[!NOTE]
>
>* Se non viene specificato alcun revisore, il proprietario della campagna viene assegnato come revisore.
>* I revisori devono disporre delle autorizzazioni appropriate per approvare le consegne. Solo gli utenti identificati nell’elenco dei revisori possono approvare.

## Invio per approvazione {#submit-approval}

Dopo aver creato la consegna, segui la procedura riportata di seguito per inviare il contenuto e il target per l’approvazione.

>[!NOTE]
>
>Le approvazioni si applicano indipendentemente dal fatto che la consegna sia stata creata direttamente nella campagna o tramite un flusso di lavoro della campagna.

1. Dal dashboard di consegna, fare clic sul pulsante **[!UICONTROL Invia contenuto]**. I revisori designati possono approvare o rifiutare. Consulta questa [sezione](#approve-reject).

   ![Schermata che mostra il pulsante Invia contenuto](assets/approvals2.png){zoomable="yes"}

   Lo stato di approvazione cambia in sospeso nella sezione **[!UICONTROL Proprietà]** del dashboard di consegna. Consulta questa [sezione](#track-approvals).

1. Una volta approvato il contenuto, fai clic sul pulsante **[!UICONTROL Prepara]** per preparare la destinazione della consegna. Il sistema prepara il pubblico e i criteri di targeting.

1. Fare clic sul pulsante **[!UICONTROL Invia destinazione]**. I revisori designati possono quindi approvare o rifiutare. Consulta questa [sezione](#approve-reject).

   ![Schermata che mostra il pulsante Invia destinazione](assets/approvals5.png){zoomable="yes"}

   Lo stato di approvazione cambia in In sospeso. Consulta questa [sezione](#track-approvals).

1. Se è abilitata l&#39;approvazione del budget, sottomettere il budget per l&#39;approvazione seguendo lo stesso principio. I revisori designati possono approvare o rifiutare. Consulta questa [sezione](#approve-reject).

1. Una volta approvato il target e, se applicabile, il budget, la preparazione riprende e la consegna può essere inviata.

>[!NOTE]
>Se un’approvazione viene rifiutata, il proprietario della consegna deve apportare tutte le modifiche necessarie al contenuto o al target in base al feedback del revisore e inviarle nuovamente per l’approvazione.

## Approva o rifiuta {#approve-reject}

I revisori designati possono approvare o rifiutare l&#39;invio di contenuti, target e budget. Consulta questa [sezione](#submit-approval).

>[!NOTE]
>Affinché la notifica e-mail venga inviata, l’indirizzo del revisore deve essere configurato nell’istanza.

1. Quando ricevi l’e-mail di notifica, apri la consegna che richiede l’approvazione direttamente dall’interfaccia utente web.

1. Rivedi il contenuto o le informazioni di destinazione.

1. Fai clic sul pulsante **[!UICONTROL Approva contenuto]**, **[!UICONTROL Approva destinazione]** o **[!UICONTROL Approva budget]**.

   ![Schermata che mostra il pulsante Approva contenuto nel dashboard di consegna](assets/approvals3.png){zoomable="yes"}

1. Fai clic su **[!UICONTROL Approva]** o **[!UICONTROL Rifiuta]**.

1. Se necessario, aggiungi un **[!UICONTROL commento]** per spiegare la tua decisione.

   ![Schermata che mostra la finestra di dialogo di approvazione con i pulsanti Approva, Rifiuta e il campo Commento](assets/approvals4.png){zoomable="yes"}

1. Conferma la tua decisione. Lo stato di approvazione viene aggiornato immediatamente nel dashboard di consegna. Consulta questa [sezione](#track-approvals).

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
