---
title: Account esterno
description: Scopri come configurare gli account esterni
source-git-commit: 6ba9706ce0a2b5431fb619093789ad54af65813f
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 9%

---

# Configurare account esterni {#external-accounts}

>[!AVAILABILITY]
>
> Gli account esterni sono attualmente disponibili solo per le e-mail non recapitate (POP3) e per l’istanza Execution, con tipi di account aggiuntivi da aggiungere in futuro.
> Gli account esterni non supportati creati nella console di Adobe Campaign sono visibili nell’interfaccia utente web ma non possono essere modificati né utilizzati.

Adobe Campaign viene fornito con un set di account esterni preconfigurati per una facile integrazione con vari sistemi. Se devi connetterti a piattaforme aggiuntive o personalizzare le connessioni in base al tuo flusso di lavoro, ora puoi facilmente creare nuovi account esterni utilizzando l’Interfaccia utente web per soddisfare le tue esigenze specifiche e garantire trasferimenti di dati fluidi.

## Creare un account esterno {#create-ext-account}

Per creare un nuovo account esterno, segui i passaggi indicati di seguito. Le impostazioni dettagliate dipendono dal tipo di account esterno.

1. Dal menu del riquadro di sinistra, selezionare **[!UICONTROL Account esterni]** in **[!UICONTROL Amministrazione]**.

1. Fai clic su **[!UICONTROL Crea account esterno]**.

   ![](assets/external_account_create_1.png)

1. Immetti la **[!UICONTROL etichetta]** e seleziona il tuo account esterno **[!UICONTROL Tipo]**.

   ![](assets/external_account_create_2.png)

1. Fai clic su **[!UICONTROL Crea]**.

1. Dall&#39;elenco a discesa **[!UICONTROL Opzioni avanzate]**, è possibile modificare il percorso **[!UICONTROL Internal name]** o **[!UICONTROL Folder]** se necessario.

   ![](assets/external_account_create_3.png)

1. Abilita **[!UICONTROL Esportato automaticamente]** se desideri che i dati gestiti da questo account esterno vengano esportati automaticamente.

1. Configura l’accesso all’account specificando le credenziali in base al tipo di account esterno scelto.

1. Fai clic su **[!UICONTROL Verifica la connessione]** per verificare che la configurazione sia corretta

1. Dal menu **[!UICONTROL Altro...]**, duplica o elimina il tuo account esterno.

   ![](assets/external_account_create_4.png)

1. Al termine della configurazione, fai clic su **[!UICONTROL Salva]**.

## Account esterni specifici per la campagna {#campaign-specific}

### Messaggi non recapitati (POP3) {#bounce}

>[!AVAILABILITY]
>
> OAuth 2.0 non è attualmente supportato.

L&#39;account esterno Posta non recapitata specifica l&#39;account POP3 esterno utilizzato per connettersi al servizio e-mail. Tutti i server configurati per l&#39;accesso POP3 possono ricevere la posta di ritorno.

![](assets/external_account_bounce.png)

Per configurare l&#39;account esterno **[!UICONTROL Messaggi non recapitati (POP3)]**:

* **[!UICONTROL Server]**

  URL del server POP3

* **[!UICONTROL Porta]**

  Numero porta di connessione POP3 (la porta predefinita è 110)

* **[!UICONTROL Account]**

  Nome dell’utente

* **[!UICONTROL Password]**

  Password account utente

* **[!UICONTROL Crittografia]**

  Tipo di crittografia scelta tra:

   * Per impostazione predefinita (POP3 se porta 110, POP3S se porta 995)
   * POP3 che cambia in SSL dopo l’invio di uno STARTTLS
   * POP3 non sicuro (porta 110 per impostazione predefinita)
   * Protezione POP3 su SSL (porta 995 per impostazione predefinita)

* **[!UICONTROL Funzione]**

  E-mail in entrata, quando l’account esterno è configurato per ricevere e-mail in entrata, o router SOAP, per gestire le richieste SOAP.

### Istanza di esecuzione{#instance-exec}

Se si dispone di un&#39;architettura segmentata, è necessario identificare le istanze di esecuzione associate all&#39;istanza di controllo e stabilire connessioni tra di esse. I modelli di messaggi transazionali vengono distribuiti nell’istanza di esecuzione.

![](assets/external_account_exec.png)

Per configurare l&#39;account esterno **[!UICONTROL Istanza di esecuzione]**:

* **[!UICONTROL URL]**

  URL del server in cui è installata l’istanza di esecuzione.

* **[!UICONTROL Account]**

  Il nome dell&#39;account deve corrispondere all&#39;agente del Centro messaggi definito nella cartella dell&#39;operatore.

* **[!UICONTROL Password]**

  Password dell’account definita nella cartella dell’operatore.

* **[!UICONTROL Metodo]**

  Scegli tra servizio Web o Federated Data Access (FDA).
In caso di metodo FDA, seleziona il tuo account FDA. La connessione di Campaign a sistemi esterni è limitata agli utenti avanzati e disponibile solo dalla console client. [Ulteriori informazioni](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/fda#_blank)

* **[!UICONTROL Crea flusso di lavoro di archiviazione]**

  Per ogni istanza di esecuzione registrata nel Centro messaggi, indipendentemente dal fatto che si disponga di una o più istanze, è necessario creare un flusso di lavoro di archiviazione separato per ogni account esterno associato all’istanza di esecuzione.
