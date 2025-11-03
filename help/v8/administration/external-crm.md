---
title: Gestisci account esterno
description: Scopri come configurare gli account esterni CRM
source-git-commit: 934a37cfebfacd2df0b7610285252d883611f252
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 0%

---

# Account esterno CRM {#external-crm}

Utilizza un account di tipo CRM esterno per connettere Adobe Campaign a un database di terze parti.

Le impostazioni di configurazione per questo account esterno dipendono dal motore di database specifico a cui ti stai connettendo. Le istruzioni di configurazione dettagliate per ciascun database supportato sono fornite nelle sezioni seguenti.

## Microsoft Dynamics CRM

L’account esterno di Microsoft Dynamics CRM ti consente di collegare la tua istanza di Campaign al database esterno di Microsoft Dynamics CRM.

Nell&#39;interfaccia utente di Adobe Campaign Web configurare l&#39;account esterno di Microsoft Dynamics CRM.

1. [Crea il tuo account esterno](external-account.md) e seleziona **[!UICONTROL Database esterno]** come **[!UICONTROL Tipo]** del tuo account esterno e Microsoft Dynamics CRM come **[!UICONTROL Tipo provider]**.

1. Fai clic su **[!UICONTROL Crea]**.

1. Per configurare l&#39;account esterno **[!UICONTROL Microsoft Dynamics CRM]**, compilare i campi seguenti:

   ![Schermata che mostra i campi di configurazione dell&#39;account esterno di Microsoft Dynamics CRM.](assets/crm-microsoft-1.png)

   +++ Per CRM Tipo OAuth: credenziali password

   * **[!UICONTROL Server]**: immettere l&#39;URL del server Microsoft CRM.

     Per individuare l&#39;URL del server di Microsoft CRM, accedere all&#39;account di Microsoft Dynamics CRM, selezionare Dynamics 365, quindi aprire l&#39;app. L&#39;URL del server viene visualizzato nella barra degli indirizzi del browser, ad esempio:`https://myserver.crm.dynamics.com/`.

   * **[!UICONTROL Account]**: specificare l&#39;account utilizzato per accedere a Microsoft CRM.

   * **[!UICONTROL Password]**: immettere la password associata all&#39;account specificato.

   * **[!UICONTROL Identificatore client]**: immettere l&#39;ID client trovato nel portale di gestione di Microsoft Azure.

   * **[!UICONTROL Versione CRM]**: scegliere la versione CRM 365 di Dynamics CRM.

   +++

   </br>

   +++ Per il tipo di CRM O-Auth: Certificato

   * **[!UICONTROL Server]**: immettere l&#39;URL del server Microsoft CRM.

     Per individuare l&#39;URL del server di Microsoft CRM, accedere all&#39;account di Microsoft Dynamics CRM, selezionare Dynamics 365, quindi aprire l&#39;app. L&#39;URL del server viene visualizzato nella barra degli indirizzi del browser, ad esempio:`https://myserver.crm.dynamics.com/`.

   * **[!UICONTROL Chiave privata (codifica Base64)]**: fornire la chiave privata codificata nel formato Base64.

     A tale scopo, è possibile utilizzare l&#39;aiuto di un codificatore Base64 o la riga di comando `base64 -w0 private.key` per Linux.

   * **[!UICONTROL Identificatore chiave personalizzato]**: immetti l&#39;identificatore chiave personalizzato utilizzato per il certificato.

   * **[!UICONTROL ID chiave]**: immetti l&#39;ID chiave associato al certificato.

   * **[!UICONTROL Identificatore client]**: immettere l&#39;ID client trovato nella gestione di Microsoft Azure

   * **[!UICONTROL Versione CRM]**: scegliere la versione CRM 365 di Dynamics CRM.

   +++

1. Dopo aver configurato la connessione, accedere alla **[!UICONTROL Configurazione guidata di Microsoft CRM]** per generare l&#39;elenco delle tabelle di Microsoft CRM.

   Fai clic su **[!UICONTROL Avanti]** per selezionare le tabelle richieste.

   ![Schermata che mostra i campi di configurazione dell&#39;account esterno di Microsoft Dynamics CRM.](assets/crm-microsoft-2.png)

1. Selezionare le tabelle di Microsoft CRM da recuperare o aggiungere una tabella remota specificando **[!UICONTROL Etichetta tabella]** e **[!UICONTROL Nome interno tabella]**, quindi abilitare l&#39;interruttore **[!UICONTROL Selezionato]**.

   Fai clic su **[!UICONTROL Avanti]**.

1. Fare clic su **[!UICONTROL Inizio]** per iniziare a creare lo schema di Microsoft CRM in base alle tabelle selezionate.

1. Segui le istruzioni visualizzate per inserire pagine da Cronologia marketing e Gestione abbonamenti di Adobe Campaign direttamente in Microsoft Dynamics CRM.

1. Fai clic su **[!UICONTROL Visualizza URL cronologia marketing]** per visualizzare gli URL per l&#39;integrazione delle pagine di cronologia marketing oppure su **[!UICONTROL Visualizza URL per sottoscrizioni lead]** per visualizzare gli URL per l&#39;integrazione delle pagine di gestione sottoscrizioni.

   ![Schermata che mostra i campi di configurazione dell&#39;account esterno di Microsoft Dynamics CRM.](assets/crm-microsoft-3.png)

1. Fai clic su **[!UICONTROL Salva]** dopo aver configurato l&#39;account esterno di Microsoft CRM.

1. Dopo aver creato l&#39;account esterno, è ora possibile fare clic su **[!UICONTROL Sincronizzazione enumerazioni...]** per sincronizzare automaticamente le enumerazioni da Microsoft CRM all&#39;interfaccia utente Web di Adobe Campaign.

   ![Schermata che mostra i campi di configurazione dell&#39;account esterno di Microsoft CRM CRM.](assets/crm-microsoft-4.png)

1. Selezionare l&#39;enumerazione Adobe Campaign corrispondente all&#39;enumerazione Microsoft CRM.

   Per sostituire i valori di Adobe Campaign con i valori di Microsoft CRM, abilitare l&#39;opzione **[!UICONTROL Sostituisci]**.

## Salesforce {#salesforce}

Per configurare l’account esterno Salesforce per l’utilizzo con Adobe Campaign, è necessario fornire i seguenti dettagli:

1. [Crea il tuo account esterno](external-account.md) e seleziona **[!UICONTROL Database esterno]** come **[!UICONTROL Tipo]** del tuo account esterno e Salesforce.com come **[!UICONTROL Tipo provider]**.

   ![Schermata che mostra i campi di configurazione dell&#39;account esterno Salesforce.](assets/crm-salesforce-1.png)

1. Fai clic su **[!UICONTROL Crea]**.

1. Per configurare l&#39;account esterno **[!UICONTROL Salesforce]**, compilare i campi seguenti:

   * **[!UICONTROL Tipo CRM O-Auth]**: **[!UICONTROL Credenziali password]** o **[!UICONTROL Credenziali]**

   * **[!UICONTROL Account]**: account utilizzato per accedere a Salesforce CRM.

   * **[!UICONTROL Password]**: immettere la password associata all&#39;account specificato.

   * **[!UICONTROL Token di sicurezza]**: immetti il token di sicurezza Salesforce associato all&#39;account.

   * **[!UICONTROL Versione API]**: scegli la versione 49.

   ![Schermata che mostra i campi di configurazione dell&#39;account esterno Salesforce.](assets/crm-salesforce-2.png)

1. Apri la **[!UICONTROL Configurazione guidata di Salesforce CRM]** per generare l&#39;elenco delle tabelle di Salesforce CRM, quindi fai clic su **[!UICONTROL Avanti]**.

   ![Schermata che mostra i campi di configurazione dell&#39;account esterno di Salesforce CRM.](assets/crm-salesforce-3.png)

1. Selezionare le tabelle Salesforce da recuperare o aggiungere una tabella remota immettendo **[!UICONTROL Etichetta tabella]** e **[!UICONTROL Nome interno tabella]**, quindi attivare l&#39;interruttore **[!UICONTROL Selezionato]**.

   Fai clic su **[!UICONTROL Avanti]**.

1. Fare clic su **[!UICONTROL Inizio]** per iniziare a creare lo schema di Salesforce CRM in base alle tabelle selezionate.

1. Fare clic su **[!UICONTROL Creazione guidata collegamento Salesforce...]** per generare i collegamenti Web in Salesforce.

   Quindi, fai clic su **[!UICONTROL Avanti]** per recuperare i collegamenti Web per **Lead** e **Contatti** da Salesforce.

1. Selezionare i collegamenti da esportare nell&#39;elenco dei collegamenti Web di Salesforce.

1. Segui le istruzioni visualizzate per inserire **pagine Cronologia marketing** e **Gestione abbonamenti** dall&#39;interfaccia utente Web di Adobe Campaign in Salesforce CRM.

1. Fai clic su **[!UICONTROL Salva]** dopo aver configurato l&#39;account esterno di Salesforce CRM.

1. Dopo aver creato l&#39;account esterno, è ora possibile fare clic su **[!UICONTROL Sincronizzazione enumerazioni...]** per sincronizzare automaticamente le enumerazioni da Salesforce all&#39;interfaccia utente Web di Adobe Campaign.

   ![Schermata che mostra i campi di configurazione dell&#39;account esterno di Salesforce CRM.](assets/crm-salesforce-4.png)

1. Seleziona l’enumerazione Adobe Campaign che corrisponde all’enumerazione Salesforce.

   Per sostituire i valori Adobe Campaign con i valori Salesforce, abilitare l&#39;opzione **[!UICONTROL Sostituisci]**.

   ![Schermata che mostra i campi di configurazione dell&#39;account esterno di Salesforce CRM.](assets/crm-salesforce-5.png)

