---
title: Gestisci account esterno
description: Scopri come configurare gli account esterni
source-git-commit: 16fe04858870c58b2f0244f33f691f1606050e61
workflow-type: tm+mt
source-wordcount: '648'
ht-degree: 2%

---

# Account esterni specifici per la campagna {#external-account}

Segui i passaggi seguenti per configurare le impostazioni dell’account in base al tipo di account esterno selezionato.

## Messaggi non recapitati (POP3) {#bounce}

L’account esterno Messaggi non recapitati specifica l’account POP3 esterno utilizzato per connettersi al servizio e-mail. Tutti i server configurati per l&#39;accesso POP3 possono ricevere la posta di ritorno.

![Schermata che mostra i campi di configurazione dell&#39;account esterno Messaggi non recapitati (POP3).](assets/external_account_bounce.png)

Per configurare l&#39;account esterno **[!UICONTROL Messaggi non recapitati (POP3)]**, compila i campi seguenti:

* **[!UICONTROL Server]** - URL del server POP3.

* **[!UICONTROL Porta]** - Numero porta di connessione POP3 (la porta predefinita è 110).

* **[!UICONTROL Account]** - Nome utente.

* **[!UICONTROL Password]** - Password dell&#39;account utente.

* **[!UICONTROL Crittografia]** - Tipo di crittografia scelta, inclusi:
   * Per impostazione predefinita (POP3 se porta 110, POP3S se porta 995).
   * POP3 che passa a SSL dopo l’invio di un STARTTLS.
   * POP3 non protetto (porta 110 per impostazione predefinita).
   * POP3 protetto sopra SSL (porta 995 per impostazione predefinita).

* **[!UICONTROL Funzione]** - Selezionare **[!UICONTROL Posta in arrivo]** per configurare l&#39;account per la ricezione delle e-mail in arrivo o **[!UICONTROL router SOAP]** per gestire le richieste SOAP.

>[!IMPORTANT]
>
>Prima di configurare l’account esterno POP3 utilizzando Microsoft OAuth 2.0, è necessario registrare l’applicazione nel portale di Azure. Per ulteriori informazioni, consulta [questa pagina](https://learn.microsoft.com/en-us/entra/identity-platform/quickstart-register-app){target=_blank}.

Per configurare un POP3 esterno tramite Microsoft OAuth 2.0, seleziona l’opzione Microsoft OAuth 2.0 e compila i seguenti campi:

* **[!UICONTROL Tenant Azure]**

  Azure ID (o ID directory (tenant)) si trova nell’elenco a discesa Essentials della panoramica dell’applicazione nel portale di Azure.

* **[!UICONTROL ID client Azure]**

  L’ID client (o ID applicazione (client)) si trova nell’elenco a discesa Essentials della panoramica dell’applicazione nel portale di Azure.

* **[!UICONTROL Segreto client Azure]**

  L’ID del segreto client si trova nella colonna Segreti client dal menu Certificati e segreti dell’applicazione nel portale di Azure.

* **[!UICONTROL URL reindirizzamento Azure]**

  L’URL di reindirizzamento si trova nel menu Autenticazione dell’applicazione nel portale di Azure. Deve terminare con la seguente sintassi nl/jsp/oauth.jsp, ad esempio `https://redirect.adobe.net/nl/jsp/oauth.jsp`.

L’accesso a Internet è necessario per la configurazione e per utilizzare il pulsante Prova connessione nella console client. Dopo la configurazione, il processo inMail può comunicare con i server Microsoft senza Internet.

Dopo aver immesso le diverse credenziali, puoi fare clic su Imposta la connessione per completare la configurazione dell’account esterno.

## Indirizzamento {#routing}

Per configurare un account esterno specifico per le consegne esterne, segui i passaggi seguenti.

1. Crea un account esterno. [Ulteriori informazioni](create-external-account.md)

1. Selezionare il tipo **[!UICONTROL Indirizzamento]**.

   ![Schermata che mostra la selezione del tipo di account esterno di indirizzamento.](assets/external-account-routing.png){zoomable="yes"}

1. Selezionare il canale desiderato e fare clic su **[!UICONTROL Crea]**.

1. Nella sezione **[!UICONTROL Dettagli]** dell&#39;account esterno, **[!UICONTROL Esterno]** è selezionato per impostazione predefinita come **[!UICONTROL Modalità di consegna]**.

   ![Schermata che mostra la configurazione della modalità di consegna per l&#39;instradamento di account esterni.](assets/external-account-delivery-mode.png){zoomable="yes"}

   >[!NOTE]
   >
   >Attualmente, **[!UICONTROL External]** è l&#39;unica modalità disponibile.

1. Per gestire il processo dopo l’esecuzione della consegna, esternalizzalo in un flusso di lavoro di post-elaborazione. Crea un flusso di lavoro con un&#39;attività [External signal](../workflows/activities/external-signal.md) e selezionala dal campo **[!UICONTROL Post-elaborazione]**.

   ![Schermata che mostra la configurazione del campo di post-elaborazione per il routing di account esterni.](assets/external-account-post-processing.png){zoomable="yes"}

1. Nel campo **[!UICONTROL Attività]**, modifica il nome dell&#39;attività del flusso di lavoro di post-elaborazione visualizzata nei registri. <!--you can edit the name of the activity that will be created if you add an external or bulk delivery to a workflow-->

## Istanza di esecuzione {#instance-exec}

Se si dispone di un&#39;architettura segmentata, identificare le istanze di esecuzione associate all&#39;istanza di controllo e stabilire connessioni tra di esse. I modelli di messaggi transazionali vengono distribuiti nell’istanza di esecuzione.

![Schermata che mostra i campi di configurazione dell&#39;account esterno dell&#39;istanza di esecuzione.](assets/external_account_exec.png)

Per configurare l&#39;account esterno **[!UICONTROL Istanza di esecuzione]**:

* **[!UICONTROL URL]** - URL del server in cui è installata l&#39;istanza di esecuzione.

* **[!UICONTROL Account]** - Nome dell&#39;account corrispondente all&#39;agente del Centro messaggi definito nella cartella dell&#39;operatore.

* **[!UICONTROL Password]** - Password dell&#39;account definita nella cartella dell&#39;operatore.

* **[!UICONTROL Metodo]** - Scegliere tra servizio Web o Federated Data Access (FDA).

  Per FDA, seleziona il tuo account FDA. La connessione di Campaign a sistemi esterni è limitata agli utenti avanzati e disponibile solo dalla console client. [Ulteriori informazioni](https://experienceleague.adobe.com/it/docs/campaign/campaign-v8/connect/fda#_blank)

* **[!UICONTROL Crea flusso di lavoro di archiviazione]** - Per ogni istanza di esecuzione registrata nel Centro messaggi, indipendentemente dal fatto che siano presenti una o più istanze, crea un flusso di lavoro di archiviazione separato per ogni account esterno associato all&#39;istanza di esecuzione.
