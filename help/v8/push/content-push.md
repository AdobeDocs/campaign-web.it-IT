---
audience: end-user
title: Progettare una consegna di notifiche push
description: Scopri come progettare una consegna di notifiche push con Adobe Campaign Web
badge: label="Alpha" type="Positive"
source-git-commit: fbedfc5d1886b86932c156574037549270480f44
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 13%

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

* Il **Messaggio dati**, gestito dall&#39;app client. I messaggi vengono inviati direttamente all’app mobile che genererà e visualizzerà la notifica Android al dispositivo. I messaggi di dati contengono solo variabili dell’applicazione personalizzate.

   Fai clic su **[!UICONTROL Messaggio]** e utilizza l’editor espressioni per definire il contenuto, personalizzare i dati e aggiungere contenuto dinamico.

* Il messaggio di notifica, gestito automaticamente dall’SDK FCM. FCM visualizza automaticamente il messaggio sui dispositivi degli utenti per conto dell’app client. I messaggi di notifica contengono un set predefinito di parametri e opzioni, ma possono ancora essere personalizzati con variabili di applicazione personalizzate.

   Per comporre il messaggio, fai clic su **[!UICONTROL Titolo]** e **[!UICONTROL Corpo]** campi. Utilizza l’editor espressioni per definire il contenuto, personalizzare i dati e aggiungere contenuto dinamico.

   Per personalizzare ulteriormente la notifica push, puoi scegliere un’immagine da aggiungere alla notifica push, l’icona della notifica da visualizzare sui dispositivi dei profili e il relativo colore.

>[!TAB iOS]

![](assets/push_content_1.png)

Per comporre il messaggio, fai clic su **[!UICONTROL Titolo]** e **[!UICONTROL Corpo]** campi. Utilizza l’editor espressioni per definire il contenuto, personalizzare i dati e aggiungere contenuto dinamico.

Puoi aggiungere una **[!UICONTROL Sottotitolo]**, valore del parametro dei sottotitoli del payload di notifica di iOS. Consulta questa sezione.

La modalità push silenzioso consente di inviare una notifica &quot;silenziosa&quot; a un’app mobile. L’utente non viene informato dell’arrivo della notifica. Viene trasferito direttamente all’applicazione.

>[!ENDTABS]

## Impostazioni avanzate {#push-advanced}

>[!BEGINTABS]

>[!TAB Android]

| Parametro | Descrizione |
|---------|---------|
| **[!UICONTROL Suono]** | Impostare l&#39;audio da riprodurre quando il dispositivo riceve la notifica. |
| **[!UICONTROL Conteggio notifiche]** | Imposta il numero di nuove informazioni non lette da visualizzare direttamente sull’icona dell’applicazione. |
| **[!UICONTROL ID canale]** | Imposta l’ID canale della notifica. L’app deve creare un canale con questo ID canale prima di ricevere qualsiasi notifica con questo ID canale. |
| **[!UICONTROL Azione clic]** | Imposta l’azione associata a un utente che fa clic sulla notifica. |
| **[!UICONTROL Tag]** | Imposta l’identificatore utilizzato per sostituire le notifiche esistenti nel cassetto delle notifiche. |
| **[!UICONTROL Priorità]** | Imposta i livelli di priorità predefiniti, minimi, bassi o alti per la notifica. Per ulteriori informazioni, consulta la documentazione di FCM. |
| **[!UICONTROL Visibilità]** | Imposta i livelli di visibilità della notifica su public, private o secret. Per ulteriori informazioni, consulta la documentazione di FCM. |
| **[!UICONTROL Sticky]** | Se è disattivata, la notifica viene automaticamente ignorata quando l’utente fa clic su di essa. Se attivata, la notifica viene comunque visualizzata anche quando l’utente fa clic su di essa. |

>[!TAB iOS]

![](assets/push_content_2.png)

| Parametro | Descrizione |
|---------|---------|
| **[!UICONTROL Modalità avviso critico]** | Abilita questa opzione per aggiungere un suono alla notifica anche se il telefono dell’utente è impostato sulla modalità di attivazione o se l’iPhone è disattivato. |
| **[!UICONTROL Pulisci badge]** | Abilita queste opzioni per aggiornare il valore del badge. |
| **[!UICONTROL Conteggio notifiche]** | Impostare un numero che verrà utilizzato per visualizzare direttamente sull&#39;icona dell&#39;applicazione il numero di nuove informazioni non lette. |
| **[!UICONTROL Volume]** | Volume del suono da 0 a 100. |
| **[!UICONTROL Contenuto modificabile]** | Abilita questa opzione per consentire all’app mobile di scaricare contenuti multimediali. Per ulteriori informazioni, consulta la [documentazione per sviluppatori di Apple](https://developer.apple.com/library/content/documentation/NetworkingInternet/Conceptual/RemoteNotificationsPG/ModifyingNotifications.html). |
| **[!UICONTROL Punteggio rilevanza]** | Imposta un punteggio di rilevanza da 0 a 100. Il sistema utilizza questa funzione per ordinare le notifiche nel riepilogo delle notifiche. |
| **[!UICONTROL Livello di interruzione]** | <ul> <li>**[!UICONTROL Attivo]**: per impostazione predefinita, il sistema visualizza immediatamente la notifica, illumina lo schermo e può riprodurre un suono. Le notifiche non interrompono le modalità di attivazione.</li><li>**[!UICONTROL Passivo]**: il sistema aggiunge la notifica all’elenco delle notifiche senza accendere lo schermo o riprodurre un suono. Le notifiche non interrompono le modalità di attivazione.</li><li>**[!UICONTROL Sensibile al tempo]**: il sistema presenta immediatamente la notifica, accende lo schermo, può riprodurre un suono e interrompere le modalità di messa a fuoco. Questo livello non richiede un’autorizzazione speciale da Apple.</li> <li>**[!UICONTROL Critico]**: il sistema presenta immediatamente la notifica, accende lo schermo e ignora le modalità di disattivazione audio o di messa a fuoco. Tieni presente che questo livello richiede un’autorizzazione speciale da parte di Apple.</ul> |
| **[!UICONTROL Thread-id]** | Identificatore utilizzato per raggruppare le notifiche correlate. |
| **[!UICONTROL Categoria]** | Nome dell&#39;ID categoria che visualizzerà i pulsanti di azione. Queste notifiche forniscono all’utente un modo più rapido per eseguire diverse attività in risposta a una notifica senza aprire o esplorare l’applicazione. |
| **[!UICONTROL ID contenuto di destinazione]** | Identificatore utilizzato per individuare la finestra dell’applicazione da portare avanti quando viene aperta la notifica. |
| **[!UICONTROL Immagine di avvio]** | Nome del file dell&#39;immagine di avvio da visualizzare. Se l’utente sceglie di avviare l’applicazione, viene visualizzata l’immagine selezionata invece della schermata di avvio dell’applicazione. |

>[!ENDTABS]

<!--Sounds must be included in the application and defined when the service is created. Refer to this section.-->



