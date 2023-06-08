---
audience: end-user
title: Progettare una consegna di notifiche push
description: Scopri come progettare una consegna di notifiche push con Adobe Campaign Web
badge: label="Alpha" type="Positive"
source-git-commit: 7fa6a5adb22b4fc4569b93383a8e269703944582
workflow-type: tm+mt
source-wordcount: '785'
ht-degree: 9%

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

Per comporre il messaggio, fai clic su **[!UICONTROL Titolo]** e **[!UICONTROL Corpo]** campi. Utilizza l’editor espressioni per definire il contenuto, personalizzare i dati e aggiungere contenuto dinamico.

Puoi aggiungere una **[!UICONTROL Sottotitolo]**, valore del parametro dei sottotitoli del payload di notifica di iOS. Consulta questa sezione.

La modalità push silenzioso consente di inviare una notifica &quot;silenziosa&quot; a un’app mobile. L’utente non viene informato dell’arrivo della notifica. Viene trasferito direttamente all’applicazione.

>[!ENDTABS]

## Impostazioni avanzate {#push-advanced}

>[!BEGINTABS]

>[!TAB Android]

* **[!UICONTROL Suono]**: consente di impostare l&#39;audio da riprodurre quando il dispositivo riceve la notifica.

* **[!UICONTROL Conteggio notifiche]**: imposta il numero di nuove informazioni non lette da visualizzare direttamente sull’icona dell’applicazione.

* **[!UICONTROL ID canale]**: imposta l’ID canale della notifica. L’app deve creare un canale con questo ID canale prima di ricevere qualsiasi notifica con questo ID canale.

* **[!UICONTROL Azione clic]**: imposta l’azione associata a un utente che fa clic sulla notifica.

* **[!UICONTROL Tag]**: imposta l’identificatore utilizzato per sostituire le notifiche esistenti nel cassetto delle notifiche.

* **[!UICONTROL Priorità]**: imposta i livelli di priorità della notifica su predefinito, minimo, basso o alto. Per ulteriori informazioni, consulta la documentazione di FCM.

* **[!UICONTROL Visibilità]**: imposta i livelli di visibilità della notifica su pubblico, privato o segreto. Per ulteriori informazioni, consulta la documentazione di FCM.

* **[!UICONTROL Sticky]**: se è disattivata, la notifica viene automaticamente ignorata quando l’utente fa clic su di essa. Se attivata, la notifica viene comunque visualizzata anche quando l’utente fa clic su di essa.

>[!TAB iOS]

* **[!UICONTROL Modalità avviso critico]**: abilita questa opzione per aggiungere un suono alla notifica anche se il telefono dell’utente è impostato sulla modalità di attivazione o se l’iPhone è disattivato.

* **[!UICONTROL Pulisci badge]**: abilita queste opzioni per aggiornare il valore del badge.

* **[!UICONTROL Conteggio notifiche]**: imposta un numero che verrà utilizzato per visualizzare direttamente sull’icona dell’applicazione il numero di nuove informazioni non lette.

* **[!UICONTROL Volume]**: volume del suono da 0 a 100.

* **[!UICONTROL Contenuto variabile]** Solo per iOS: invia il flag di contenuto mutabile nel payload push e consentirà la modifica del contenuto della notifica push da parte di un’estensione dell’applicazione del servizio di notifica fornita nell’SDK di iOS. Per ulteriori informazioni, consulta la [documentazione per sviluppatori di Apple](https://developer.apple.com/library/content/documentation/NetworkingInternet/Conceptual/RemoteNotificationsPG/ModifyingNotifications.html). abilita questa opzione per consentire all’app mobile di scaricare contenuti multimediali.

* **[!UICONTROL Punteggio di rilevanza]**: imposta un punteggio di rilevanza da 0 a 100. Il sistema utilizza questa funzione per ordinare le notifiche nel riepilogo delle notifiche.

* **[!UICONTROL Livello di interruzione]**:

   * **[!UICONTROL Attivo]**: per impostazione predefinita, il sistema visualizza immediatamente la notifica, illumina lo schermo e può riprodurre un suono. Le notifiche non interrompono le modalità di attivazione.

   * **[!UICONTROL Passivo]**: il sistema aggiunge la notifica all’elenco delle notifiche senza accendere lo schermo o riprodurre un suono. Le notifiche non interrompono le modalità di attivazione.

   * **[!UICONTROL Sensibile al tempo]**: il sistema presenta immediatamente la notifica, accende lo schermo, può riprodurre un suono e interrompere le modalità di messa a fuoco. Questo livello non richiede un’autorizzazione speciale da Apple.

   * **[!UICONTROL Critico]**: il sistema presenta immediatamente la notifica, accende lo schermo e ignora le modalità di disattivazione audio o di messa a fuoco. Tieni presente che questo livello richiede un’autorizzazione speciale da parte di Apple.

* **[!UICONTROL Thread-id]**: identificatore utilizzato per raggruppare le notifiche correlate.

* **[!UICONTROL Categoria]**: nome dell’ID categoria che visualizzerà i pulsanti di azione. Queste notifiche forniscono all’utente un modo più rapido per eseguire diverse attività in risposta a una notifica senza aprire o esplorare l’applicazione.

* **[!UICONTROL ID contenuto di destinazione]**: identificatore utilizzato per individuare la finestra dell’applicazione da inoltrare quando viene aperta la notifica.

* **[!UICONTROL Avvia immagine]**: nome del file dell&#39;immagine di avvio da visualizzare. Se l’utente sceglie di avviare l’applicazione, viene visualizzata l’immagine selezionata invece della schermata di avvio dell’applicazione.

>[!ENDTABS]

<!--Sounds must be included in the application and defined when the service is created. Refer to this section.-->



