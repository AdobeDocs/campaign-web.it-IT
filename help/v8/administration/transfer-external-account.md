---
title: Gestisci account esterno
description: Scopri come configurare gli account esterni
exl-id: 6daa35c2-21cf-4121-ba57-3749e1ed9c2d
source-git-commit: 155a7f3fb55a579dbf9a2ad81a1dc7e4ea3847df
workflow-type: tm+mt
source-wordcount: '664'
ht-degree: 6%

---

# Trasferisci dati account esterni {#transfer-external-account}

## Servizio Amazon Simple Storage (S3) {#amazon-simple-storage-service--s3--external-account}

Il connettore Amazon Simple Storage Service (S3) può essere utilizzato per importare o esportare dati in Adobe Campaign. Può essere impostato in un’attività del flusso di lavoro. Per ulteriori informazioni, consulta [questa pagina](https://experienceleague.adobe.com/en/docs/campaign-web/v8/wf/design-workflows/transfer-file){target=_blank}.

![Schermata che mostra i campi di configurazione dell&#39;account esterno Amazon Simple Storage Service S3.](assets/external-AWS.png)

Quando imposti questo nuovo account esterno, dovrai fornire i seguenti dettagli:

* **[!UICONTROL Server account AWS S3]**

  URL del server, deve essere compilato come segue:

  `  <S3bucket name>.s3.amazonaws.com/<s3object path>`

* **[!UICONTROL ID chiave di accesso AWS]**

  Per sapere dove trovare l&#39;ID della chiave di accesso AWS, consulta questa [pagina](https://docs.aws.amazon.com/general/latest/gr/aws-sec-cred-types.html#access-keys-and-secret-access-keys).

* **[!UICONTROL Chiave di accesso segreta ad AWS]**

  Per sapere dove trovare la chiave di accesso segreta ad AWS, consulta questa [pagina](https://aws.amazon.com/fr/blogs/security/wheres-my-secret-access-key/).

* **[!UICONTROL Area geografica AWS]**

  Per ulteriori informazioni sull&#39;area geografica di AWS, consulta questa [pagina](https://aws.amazon.com/about-aws/global-infrastructure/regions_az/).

* La casella di controllo **[!UICONTROL Usa crittografia lato server]** consente di archiviare il file in modalità crittografata S3.

Per informazioni su dove trovare l&#39;ID della chiave di accesso e la chiave di accesso segreta, consulta la [documentazione](https://docs.aws.amazon.com/general/latest/gr/aws-sec-cred-types.html#access-keys-and-secret-access-keys) dei servizi Web Amazon.

## Archiviazione BLOB di Azure {#azure-blob-external-account}

L&#39;account esterno **[!UICONTROL Archiviazione BLOB di Azure]** può essere utilizzato per importare o esportare dati in Adobe Campaign utilizzando un&#39;attività del flusso di lavoro **[!UICONTROL Trasferisci file]**. Per ulteriori informazioni al riguardo, consulta [questa sezione](https://experienceleague.adobe.com/en/docs/campaign-web/v8/wf/design-workflows/transfer-file){target=_blank}.

![Schermata che mostra i campi di configurazione dell&#39;account esterno Archiviazione BLOB di Azure.](assets/external-azure.png)

Per configurare l&#39;**[!UICONTROL account esterno Azure]** per l&#39;utilizzo con Adobe Campaign, è necessario fornire i dettagli seguenti:

* **[!UICONTROL Server]**

  URL del server di archiviazione BLOB di Azure.

* **[!UICONTROL Crittografia]**

  Tipo di crittografia scelta tra **[!UICONTROL Nessuno]** o **[!UICONTROL SSL]**.

* **[!UICONTROL Chiave di accesso]**

  Per sapere dove trovare la tua **[!UICONTROL chiave di accesso]**, fai riferimento a questa [pagina](https://docs.microsoft.com/en-us/azure/storage/common/storage-account-keys-manage?tabs=azure-portal).

## SFTP

L’account esterno SFTP consente di configurare e testare l’accesso a un server esterno a Adobe Campaign.

![Schermata che mostra i campi di configurazione dell&#39;account esterno SFTP.](assets/ext-account-sftp.png)

Per configurare l&#39;account esterno **[!UICONTROL SFTP]**, compila i campi seguenti:

* **[!UICONTROL Server]**

  Immetti il nome o l’indirizzo del server SFTP.

* **[!UICONTROL Porta]**

  Specifica il numero della porta di connessione SFTP. La porta predefinita è 22.

* **[!UICONTROL Account]**

  Immetti il nome utente utilizzato per connettersi al server SFTP.

* **[!UICONTROL Password]**

  Immetti la password per l’account SFTP.

* **[!UICONTROL Tipo di autenticazione SFTP]**

  Scegli il metodo di autenticazione con il server SFTP. Le opzioni includono:

   * **[!UICONTROL Password]**: esegui l&#39;autenticazione utilizzando la password dell&#39;account.

   * **[!UICONTROL Chiave pubblica]**: eseguire l&#39;autenticazione utilizzando una coppia di chiavi SSH (chiave privata e chiave pubblica).

Se è selezionata l&#39;autenticazione **[!UICONTROL Chiave pubblica]**, è necessario compilare i campi seguenti:

* **[!UICONTROL File di chiave privata]**

  Specifica il file della chiave SSH privata utilizzato per l’autenticazione.

* **[!UICONTROL File di chiave pubblica]**

  Specifica la chiave SSH pubblica corrispondente registrata sul server SFTP.

* **[!UICONTROL Passphrase chiave SSH]**

  Immetti la passphrase per decrittografare la chiave privata se è protetta.

## HTTP

L’account esterno HTTP consente di configurare e testare l’accesso a un server esterno a Adobe Campaign.

![Schermata che mostra i campi di configurazione dell&#39;account esterno HTTP.](assets/ext-account-http.png)

Per configurare l&#39;account esterno **[!UICONTROL HTTP]**, compilare i campi seguenti:

* **[!UICONTROL Server]**

  Immettere il nome o l&#39;indirizzo del server HTTP.

* **[!UICONTROL Porta]**

  Specificare il numero della porta di connessione HTTP. La porta predefinita è 80.

* **[!UICONTROL Account]**

  Immettere il nome utente per l&#39;autenticazione.

* **[!UICONTROL Password]**

  Immettere la password associata all&#39;account utente.

* **[!UICONTROL Tipo di autenticazione SFTP]**

  Selezionare il tipo di autenticazione per la connessione. Le opzioni includono:

   * Password
   * Chiave pubblica

Se si utilizza l&#39;autenticazione **[!UICONTROL Chiave pubblica]**, dal menu **[!UICONTROL Autenticazione chiave pubblica]** immettere i valori richiesti per:

* **[!UICONTROL Password]**: passphrase di protezione della chiave privata, se applicabile.

* **[!UICONTROL Chiave privata]**: la chiave privata utilizzata per autenticare l&#39;account Snowflake.



## FTP

L’account esterno FTP consente di configurare e testare l’accesso a un server esterno a Adobe Campaign.

![Schermata che mostra i campi di configurazione dell&#39;account esterno FTP.](assets/ext-account-ftp.png)

Per configurare l&#39;account esterno **[!UICONTROL FTP]**, compilare i campi seguenti:

* **[!UICONTROL Server]**

  Immettere il nome o l&#39;indirizzo del server FTP.

* **[!UICONTROL Porta]**

  Specificare il numero della porta di connessione FTP. La porta predefinita è 21.

* **[!UICONTROL Account]**

  Immettere il nome utente per l&#39;autenticazione.

* **[!UICONTROL Password]**

  Immettere la password associata all&#39;account utente.

* **[!UICONTROL Crittografia]**

  Selezionare il tipo di crittografia per la connessione. Le opzioni includono:

   * Per impostazione predefinita
   * POP3 + STARTTLS
   * POP3 non protetto
   * POP3 protetto
