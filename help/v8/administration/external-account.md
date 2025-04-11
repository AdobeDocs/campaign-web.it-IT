---
title: Gestisci account esterno
description: Scopri come configurare gli account esterni
exl-id: e37d6cb0-f8fa-4f1c-9cdd-46f9666c2d18
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 2%

---

# Configurare account esterni {#external-accounts}

>[!AVAILABILITY]
>
>* Gli account esterni sono attualmente disponibili solo per le e-mail non recapitate (POP3), il routing e l’istanza di esecuzione. Ulteriori tipi di account verranno aggiunti in seguito.
>
>* Gli account esterni non supportati creati nella console di Adobe Campaign sono visibili nell’interfaccia utente web ma non possono essere modificati né utilizzati.

Adobe Campaign include account esterni preconfigurati per una facile integrazione con vari sistemi. Per connettersi a piattaforme aggiuntive o personalizzare le connessioni in base al flusso di lavoro, creare nuovi account esterni utilizzando l&#39;interfaccia utente Web. Questo garantisce trasferimenti di dati senza soluzione di continuità.

## Creare un account esterno {#create-ext-account}

Per creare un nuovo account esterno, segui i passaggi indicati di seguito. Le impostazioni dettagliate dipendono dal tipo di account esterno. [Ulteriori informazioni](#campaign-specific)

1. Dal menu del riquadro di sinistra, selezionare **[!UICONTROL Account esterni]** in **[!UICONTROL Amministrazione]**.

1. Fai clic su **[!UICONTROL Crea account esterno]**.

   ![Schermata che mostra l&#39;opzione per creare un account esterno nell&#39;interfaccia utente Web.](assets/external_account_create_1.png)

1. Immetti la **[!UICONTROL etichetta]** e seleziona l&#39;account esterno **[!UICONTROL Tipo]**.

   >[!NOTE]
   >
   >Le impostazioni per i tipi specifici di Campaign sono descritte in [questa sezione](#campaign-specific).

   ![Schermata che mostra i campi per l&#39;immissione dell&#39;etichetta e la selezione del tipo di account esterno.](assets/external_account_create_2.png)

1. Fai clic su **[!UICONTROL Crea]**.

1. Dall&#39;elenco a discesa **[!UICONTROL Opzioni aggiuntive]**, se necessario, modifica il percorso **[!UICONTROL Internal name]** o **[!UICONTROL Folder]**.

   ![Schermata con opzioni aggiuntive per la configurazione del nome interno e del percorso della cartella.](assets/external_account_create_3.png)

1. Abilita l&#39;opzione **[!UICONTROL Esportato automaticamente nei pacchetti]** per esportare automaticamente i dati gestiti da questo account esterno. <!--Exported where??-->

   ![Schermata che mostra l&#39;opzione per abilitare l&#39;esportazione automatica nei pacchetti.](assets/external_account_create_exported.png)

1. Nella sezione **[!UICONTROL Dettagli]** configura l&#39;accesso all&#39;account specificando le credenziali in base al tipo di account esterno scelto. [Ulteriori informazioni](#bounce)

1. Fai clic su **[!UICONTROL Verifica connessione]** per verificare che la configurazione sia corretta.

1. Dal menu **[!UICONTROL Altro...]**, duplica o elimina il tuo account esterno.

   ![Schermata che mostra il menu Altro con opzioni per duplicare o eliminare l&#39;account esterno.](assets/external_account_create_4.png)

1. Al termine della configurazione, fare clic su **[!UICONTROL Salva]**.

## Account esterni specifici per la campagna {#campaign-specific}

A seconda del tipo di account esterno selezionato, segui i passaggi seguenti per configurare le impostazioni dell’account.

### Messaggi non recapitati (POP3) {#bounce}

>[!AVAILABILITY]
>
> OAuth 2.0 non è attualmente supportato.

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

### Indirizzamento {#routing}

Per configurare un account esterno specifico per le consegne esterne, segui i passaggi seguenti.

1. Crea un account esterno. [Ulteriori informazioni](../administration/external-account.md#create-ext-account)

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

### Istanza di esecuzione {#instance-exec}

Se si dispone di un&#39;architettura segmentata, identificare le istanze di esecuzione associate all&#39;istanza di controllo e stabilire connessioni tra di esse. I modelli di messaggi transazionali vengono distribuiti nell’istanza di esecuzione.

![Schermata che mostra i campi di configurazione dell&#39;account esterno dell&#39;istanza di esecuzione.](assets/external_account_exec.png)

Per configurare l&#39;account esterno **[!UICONTROL Istanza di esecuzione]**:

* **[!UICONTROL URL]** - URL del server in cui è installata l&#39;istanza di esecuzione.

* **[!UICONTROL Account]** - Nome dell&#39;account corrispondente all&#39;agente del Centro messaggi definito nella cartella dell&#39;operatore.

* **[!UICONTROL Password]** - Password dell&#39;account definita nella cartella dell&#39;operatore.

* **[!UICONTROL Metodo]** - Scegliere tra servizio Web o Federated Data Access (FDA).

  Per FDA, seleziona il tuo account FDA. La connessione di Campaign a sistemi esterni è limitata agli utenti avanzati e disponibile solo dalla console client. [Ulteriori informazioni](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/fda#_blank)

* **[!UICONTROL Crea flusso di lavoro di archiviazione]** - Per ogni istanza di esecuzione registrata nel Centro messaggi, indipendentemente dal fatto che siano presenti una o più istanze, crea un flusso di lavoro di archiviazione separato per ogni account esterno associato all&#39;istanza di esecuzione.