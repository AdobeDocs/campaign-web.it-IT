---
audience: end-user
title: Progettare una consegna di notifiche push
description: Scopri come progettare una consegna di notifiche push con Adobe Campaign Web
badge: label="Alpha"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '1068'
ht-degree: 7%

---

# Progettare una consegna push {#content-push}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_android_content"
>title="Contenuto push per Android"
>abstract="Definisci il contenuto push per Android."

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_ios_content"
>title="Contenuto push per iOS"
>abstract="Definisci il contenuto push per iOS."

## Messaggio {#push-message}

>[!BEGINTABS]

>[!TAB Android]

Con Firebase Cloud Messaging puoi scegliere tra due tipi di messaggi:

* Il **[!UICONTROL Messaggio dati]e** è gestito dall’app client. Questi messaggi vengono inviati direttamente all’app mobile, che genera e visualizza una notifica Android sul dispositivo. I messaggi di dati contengono solo variabili dell’applicazione personalizzate.

  Per definire il contenuto, personalizzare i dati e aggiungere contenuto dinamico, fai clic sul pulsante **[!UICONTROL Messaggio]** e utilizza l’editor di espressioni. Puoi accedere a questo editor per personalizzare i messaggi In **[!UICONTROL Variabili dell’applicazione]** , le variabili dell&#39;applicazione vengono aggiunte automaticamente. Queste variabili ti consentono di definire il comportamento di notifica. Ad esempio, puoi configurare una schermata dell’applicazione specifica da visualizzare quando l’utente attiva la notifica.

  ![](assets/push_content_4.png)

* Il **[!UICONTROL Messaggio di notifica]**, gestito automaticamente dall’SDK FCM. FCM visualizza automaticamente il messaggio sui dispositivi degli utenti per conto dell’app client. I messaggi di notifica contengono un set predefinito di parametri e opzioni, ma possono ancora essere personalizzati con variabili di applicazione personalizzate.

  Per comporre il messaggio, fai clic su **[!UICONTROL Titolo]** e **[!UICONTROL Corpo]** campi. Utilizza l’editor espressioni per definire il contenuto, personalizzare i dati e aggiungere contenuto dinamico.

  Per personalizzare ulteriormente la notifica push, puoi scegliere un’immagine da aggiungere alla notifica push, l’icona della notifica da visualizzare sui dispositivi dei profili e il relativo colore.

  ![](assets/push_content_3.png)

>[!TAB iOS]

Per comporre il messaggio, fai clic su **[!UICONTROL Titolo]** e **[!UICONTROL Corpo]** campi. Utilizza l’editor espressioni per definire il contenuto, personalizzare i dati e aggiungere contenuto dinamico.

Puoi aggiungere una **[!UICONTROL Sottotitolo]**, valore del parametro dei sottotitoli del payload di notifica di iOS. Consulta questa sezione.

La modalità push silenzioso consente di inviare una notifica &quot;silenziosa&quot; a un’app mobile. L’utente non viene informato dell’arrivo della notifica. Viene trasferito direttamente all’applicazione.

![](assets/push_content_1.png)

>[!ENDTABS]

## Impostazioni avanzate {#push-advanced}

>[!BEGINTABS]

>[!TAB Android]

![](assets/push_content_5.png)

| Parametro | Descrizione |
|---------|---------|
| **[!UICONTROL Suono]** | Impostare l&#39;audio da riprodurre quando il dispositivo riceve la notifica. |
| **[!UICONTROL Conteggio notifiche]** | Imposta il numero di nuove informazioni non lette da visualizzare direttamente sull’icona dell’applicazione. Questo consente all’utente di visualizzare rapidamente il numero di notifiche in sospeso. |
| **[!UICONTROL ID canale]** | Imposta l’ID canale della notifica. L’app deve creare un canale con questo ID canale prima di ricevere qualsiasi notifica con questo ID canale. |
| **[!UICONTROL Azione clic]** | Definisci l’azione associata a un utente che fa clic sulla notifica. Questo determina il comportamento quando l’utente interagisce con la notifica, ad esempio aprendo una schermata specifica o eseguendo un’azione specifica nell’app. |
| **[!UICONTROL Tag]** | Imposta un identificatore utilizzato per sostituire le notifiche esistenti nel cassetto delle notifiche. In questo modo si evita l’accumulo di notifiche multiple e si garantisce che venga visualizzata solo la notifica pertinente più recente. |
| **[!UICONTROL Priorità]** | Imposta il livello di priorità della notifica, che può essere predefinito, minimo, basso o alto. Il livello di priorità determina l’importanza e l’urgenza della notifica, influenzandone la modalità di visualizzazione e la capacità di ignorare determinate impostazioni di sistema. Per ulteriori informazioni, consulta [Documentazione FCM](https://firebase.google.com/docs/reference/fcm/rest/v1/projects.messages#notificationpriority). |
| **[!UICONTROL Visibilità]** | Imposta il livello di visibilità della notifica, che può essere pubblica, privata o segreta. Il livello di visibilità determina la quantità di contenuto della notifica visualizzata nella schermata di blocco e in altre aree sensibili. Per ulteriori informazioni, consulta [Documentazione FCM](https://firebase.google.com/docs/reference/fcm/rest/v1/projects.messages#visibility). |
| **[!UICONTROL Sticky]** | Quando è attivata, la notifica rimane visibile anche dopo che l’utente fa clic su di essa. <br>Se è disattivata, la notifica viene automaticamente ignorata quando l’utente interagisce con essa. Il comportamento fisso consente alle notifiche importanti di rimanere sullo schermo per periodi più lunghi. |
| **[!UICONTROL Variabili dell’applicazione]** | Consente di definire il comportamento di notifica. Queste variabili sono completamente personalizzabili e sono incluse nel payload del messaggio inviato al dispositivo mobile. |

>[!TAB iOS]

![](assets/push_content_2.png)

| Parametro | Descrizione |
|---------|---------|
| **[!UICONTROL Modalità avviso critico]** | Abilita questa opzione per aggiungere un suono alla notifica, anche quando il telefono dell’utente è impostato sulla modalità di attivazione o se l’iPhone è disattivato. In questo modo l’utente noterà gli avvisi importanti. |
| **[!UICONTROL Pulisci badge]** | Abilita questa opzione per aggiornare il valore del badge visualizzato sull’icona dell’applicazione. In questo modo il badge riflette accuratamente il numero di nuove informazioni non lette. |
| **[!UICONTROL Conteggio notifiche]** | Impostare un numero che verrà visualizzato direttamente sull&#39;icona dell&#39;applicazione, indicando il numero di nuove informazioni non lette. Questo fornisce un riferimento visivo rapido per l’utente. |
| **[!UICONTROL Volume]** | Volume del suono da 0 a 100. |
| **[!UICONTROL Contenuto modificabile]** | Abilita questa opzione per consentire all’app mobile di scaricare il contenuto multimediale associato alla notifica. Per ulteriori informazioni, consulta la [documentazione per sviluppatori di Apple](https://developer.apple.com/library/content/documentation/NetworkingInternet/Conceptual/RemoteNotificationsPG/ModifyingNotifications.html). |
| **[!UICONTROL Punteggio rilevanza]** | Imposta un punteggio di rilevanza da 0 a 100 per assegnare la priorità all’ordine delle notifiche nel riepilogo delle notifiche. Punteggi più alti indicano notifiche più importanti. |
| **[!UICONTROL Livello di interruzione]** | <ul> <li>**[!UICONTROL Attivo]**: per impostazione predefinita, il sistema visualizza immediatamente la notifica, illumina lo schermo e può riprodurre un suono. Le notifiche non interrompono le modalità di attivazione.</li><li>**[!UICONTROL Passivo]**: il sistema aggiunge la notifica all’elenco delle notifiche senza accendere lo schermo o riprodurre un suono. Le notifiche non interrompono le modalità di attivazione.</li><li>**[!UICONTROL Sensibile al tempo]**: il sistema presenta immediatamente la notifica, accende lo schermo, può riprodurre un suono e interrompere le modalità di messa a fuoco. Questo livello non richiede un’autorizzazione speciale da Apple.</li> <li>**[!UICONTROL Critico]**: il sistema presenta immediatamente la notifica, accende lo schermo e ignora le modalità di disattivazione audio o di messa a fuoco. Tieni presente che questo livello richiede un’autorizzazione speciale da parte di Apple.</ul> |
| **[!UICONTROL Thread-id]** | Identificatore utilizzato per raggruppare le notifiche correlate. Le notifiche con lo stesso ID thread sono organizzate come una singola conversazione o thread nell’elenco delle notifiche. |
| **[!UICONTROL Categoria]** | Specifica il nome dell’ID categoria associato alla notifica. Questo consente la visualizzazione dei pulsanti di azione, consentendo all’utente di eseguire varie attività direttamente dalla notifica senza aprire l’applicazione. |
| **[!UICONTROL ID contenuto di destinazione]** | Identificatore utilizzato per individuare la finestra dell’applicazione da portare avanti quando viene aperta la notifica. |
| **[!UICONTROL Immagine di avvio]** | Specifica il nome del file dell&#39;immagine di avvio da visualizzare quando l&#39;utente sceglie di avviare l&#39;applicazione dalla notifica. Viene visualizzata l&#39;immagine selezionata al posto della normale schermata di avvio dell&#39;applicazione. |
| **[!UICONTROL Variabili dell’applicazione]** | Consente di definire il comportamento di notifica. Queste variabili sono completamente personalizzabili e sono incluse nel payload del messaggio inviato al dispositivo mobile. |

>[!ENDTABS]

<!--Sounds must be included in the application and defined when the service is created. Refer to this section.-->



