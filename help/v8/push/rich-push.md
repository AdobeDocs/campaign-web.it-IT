---
audience: end-user
title: Progettare una consegna di notifiche push potenziata
description: Scopri come progettare una consegna di notifiche push potenziata da Android con Adobe Campaign Web
exl-id: a87cb933-b564-4fa4-b173-6a94d7e27da5
source-git-commit: bb61fdb34fecb4131d4069965cda8a3a5099b6bc
workflow-type: tm+mt
source-wordcount: '1420'
ht-degree: 34%

---

# Progettare una consegna push potenziata per Android {#rich-push}


>[!CONTEXTUALHELP]
>id="acw_deliveries_push_remind_later"
>title="Pulsante Ricorda più tardi"
>abstract="Il pulsante **Ricorda più tardi** conente di pianificare un promemoria. Il campo Timestamp richiede un valore che rappresenti il passaggio del tempo in secondi."

>[!AVAILABILITY]
>
>Questa funzionalità si trova in **Disponibilità limitata** (LA).

Con Firebase Cloud Messaging puoi scegliere tra due tipi di messaggi:

* Il **[!UICONTROL Messaggio dati]** è gestito dall’app client. Questi messaggi vengono inviati direttamente all’app mobile, che genera e visualizza una notifica Android sul dispositivo. I messaggi di dati contengono solo variabili dell’applicazione personalizzate.

* Il **[!UICONTROL Messaggio di notifica]**, gestito automaticamente dall’SDK FCM. FCM mostra automaticamente il messaggio sui dispositivi degli utenti per conto dell’app client. I messaggi di notifica contengono un set preimpostato di parametri e opzioni, ma possono ancora essere personalizzati con variabili personalizzate dell’applicazione.

![](assets/rich_push.png){zoomable="yes"}

## Definisci il contenuto della notifica {#push-message}

Una volta creata la consegna push, puoi definirne il contenuto. Sono disponibili tre modelli:

* **Modello predefinito** ti consente di inviare notifiche con una semplice icona e un&#39;immagine associata.

* **Modello base** può includere testo, immagini e pulsanti nelle notifiche.

* **Modello carosello** consente di inviare notifiche con testo e più immagini scorrevoli.

Per ulteriori informazioni su come personalizzare questi modelli, accedi alle schede seguenti.

>[!BEGINTABS]

>[!TAB Modello predefinito]

1. Dal menu a discesa **[!UICONTROL Modello]**, seleziona **[!UICONTROL Predefinito]**.

   ![](assets/rich_push_default.png)

1. Per comporre il messaggio, immetti il testo nei campi **[!UICONTROL Titolo]** e **[!UICONTROL Messaggio]**.

   ![](assets/rich_push_default_2.png)

1. Utilizza l’editor espressioni per definire il contenuto, personalizzare i dati e aggiungere contenuto dinamico. [Ulteriori informazioni](../personalization/personalize.md)

1. Definisci l&#39;**[!UICONTROL azione clic]** associata a un utente che fa clic sulla notifica. Questo determina il comportamento quando l’utente interagisce con la notifica, ad esempio aprendo una schermata specifica o eseguendo un’azione specifica nell’app.

1. Per personalizzare ulteriormente la notifica push, puoi scegliere un URL **[!UICONTROL Immagine]** da aggiungere alla notifica push e l&#39;**[!UICONTROL icona]** della notifica da visualizzare sui dispositivi dei profili.

   ![](assets/rich_push_default_3.png)

1. Configura le **[!UICONTROL Impostazioni avanzate]** della notifica push. [Ulteriori informazioni](#push-advanced)

Dopo aver definito il contenuto del messaggio, puoi utilizzare gli abbonati di prova per visualizzare in anteprima e verificare il messaggio.

>[!TAB Modello base]

1. Dal menu a discesa **[!UICONTROL Modello]**, selezionare **[!UICONTROL Base]**.

   ![](assets/rich_push_basic.png)

1. Per comporre il messaggio, immetti il testo nei campi **[!UICONTROL Titolo]**, **[!UICONTROL Messaggio]** e **[!UICONTROL Messaggio espanso]**.

   Il testo del **[!UICONTROL Messaggio]** viene visualizzato nella visualizzazione compressa mentre il **[!UICONTROL Messaggio espanso]** viene visualizzato quando la notifica viene espansa.

   ![](assets/rich_push_basic_2.png)

1. Utilizza l’editor espressioni per definire il contenuto, personalizzare i dati e aggiungere contenuto dinamico. [Ulteriori informazioni](../personalization/personalize.md)

1. Aggiungi l&#39;URL che definisce l&#39;**[!UICONTROL azione clic]** associata a un utente che fa clic sulla notifica. Questo determina il comportamento quando l’utente interagisce con la notifica, ad esempio aprendo una schermata specifica o eseguendo un’azione specifica nell’app.

1. Seleziona il **[!UICONTROL tipo di collegamento]** dell&#39;URL aggiunto al campo **[!UICONTROL Azione clic]**:

   * **[!UICONTROL URL Web]**: gli URL Web indirizzano gli utenti al contenuto online. Facendo clic su, viene richiesto al browser Web predefinito del dispositivo di aprire e passare all&#39;URL designato.

   * **[!UICONTROL Deeplink]**: i collegamenti profondi sono URL che indirizzano gli utenti a sezioni specifiche all&#39;interno di un&#39;app, anche se l&#39;app è chiusa. Facendo clic su di esso, può essere visualizzata una finestra di dialogo che consente agli utenti di scegliere tra varie app in grado di gestire il collegamento.

   * **[!UICONTROL Apri app]**: gli URL aperti dell&#39;app consentono di connettersi direttamente al contenuto di un&#39;applicazione. Consente all’applicazione di impostarsi come gestore predefinito per un tipo specifico di collegamento, ignorando la finestra di dialogo per la disambiguazione.

   Per ulteriori informazioni su come gestire i collegamenti alle app Android, consulta la [documentazione per sviluppatori di Android](https://developer.android.com/training/app-links).

   ![](assets/rich_push_basic_3.png)

1. Per personalizzare ulteriormente la notifica push, puoi scegliere un URL **[!UICONTROL Immagine]** da aggiungere alla notifica push e l&#39;**[!UICONTROL icona]** della notifica da visualizzare sui dispositivi dei profili.

1. Fai clic su **[!UICONTROL Aggiungi pulsante]** e compila i campi seguenti:

   * **[!UICONTROL Etichetta]**: testo visualizzato sul pulsante.
   * **[!UICONTROL URI collegamento]**: specificare l&#39;URI da eseguire facendo clic sul pulsante.
   * **[!UICONTROL Tipo di collegamento]**: tipo di collegamento **[!UICONTROL URL Web]**, **[!UICONTROL Deeplink]** o **[!UICONTROL Apri app]**.

   È possibile includere fino a tre pulsanti nella notifica push. Se si sceglie il pulsante **[!UICONTROL Ricordare più tardi]**, è possibile includere solo un massimo di due pulsanti.

   ![](assets/rich_push_basic_4.png)

1. Fai clic sul pulsante **[!UICONTROL Aggiungi promemoria più tardi]** per aggiungere un&#39;opzione Ricordami più tardi alla notifica push. Immetti un **[!UICONTROL Etichetta]** e un **[!UICONTROL Timestamp]**.

   Il campo Timestamp prevede un valore che rappresenti l’epoca in secondi.

   ![](assets/rich_push_basic_5.png)

1. Configura le **[!UICONTROL Impostazioni avanzate]** della notifica push. [Ulteriori informazioni](#push-advanced)

Dopo aver definito il contenuto del messaggio, puoi utilizzare gli abbonati di prova per visualizzare in anteprima e verificare il messaggio.

>[!TAB Modello carosello]

1. Dal menu a discesa **[!UICONTROL Modello]**, seleziona **[!UICONTROL Carosello]**.

   ![](assets/rich_push_carousel.png)

1. Per comporre il messaggio, immetti il testo nei campi **[!UICONTROL Titolo]**, **[!UICONTROL Messaggio]** e **[!UICONTROL Messaggio espanso]**.

   Il testo del **[!UICONTROL Messaggio]** viene visualizzato nella visualizzazione compressa mentre il **[!UICONTROL Messaggio espanso]** viene visualizzato quando la notifica viene espansa.

   ![](assets/rich_push_carousel_1.png)

1. Utilizza l’editor espressioni per definire il contenuto, personalizzare i dati e aggiungere contenuto dinamico. [Ulteriori informazioni](../personalization/personalize.md)

1. Aggiungi l&#39;URL che definisce l&#39;**[!UICONTROL azione clic]** associata a un utente che fa clic sulla notifica. Questo determina il comportamento quando l’utente interagisce con la notifica, ad esempio aprendo una schermata specifica o eseguendo un’azione specifica nell’app.

1. Seleziona il **[!UICONTROL tipo di collegamento]** dell&#39;URL aggiunto al campo **[!UICONTROL Azione clic]**:

   * **[!UICONTROL URL Web]**L: gli URL Web indirizzano gli utenti al contenuto online. Facendo clic su, viene richiesto al browser Web predefinito del dispositivo di aprire e passare all&#39;URL designato.

   * **[!UICONTROL Deeplink]**: i collegamenti profondi sono URL che indirizzano gli utenti a sezioni specifiche all&#39;interno di un&#39;app, anche se l&#39;app è chiusa. Facendo clic su di esso, può essere visualizzata una finestra di dialogo che consente agli utenti di scegliere tra varie app in grado di gestire il collegamento.

   * **[!UICONTROL Apri app]**: gli URL aperti dell&#39;app consentono di connettersi direttamente al contenuto di un&#39;applicazione. Consente all’applicazione di impostarsi come gestore predefinito per un tipo specifico di collegamento, ignorando la finestra di dialogo per la disambiguazione.

   Per ulteriori informazioni su come gestire i collegamenti alle app Android, consulta la [documentazione per sviluppatori di Android](https://developer.android.com/training/app-links).

   ![](assets/rich_push_carousel_2.png)

1. Per personalizzare ulteriormente la notifica push, puoi scegliere l&#39;**[!UICONTROL icona]** della notifica da visualizzare sui dispositivi dei profili.

1. Scegli come funziona il **[!UICONTROL carosello]**:

   * **[!UICONTROL Automatico]**: scorre automaticamente le immagini come diapositive, passando a intervalli predefiniti.
   * **[!UICONTROL Manuale]**: consente agli utenti di scorrere manualmente tra le diapositive per spostarsi tra le immagini.

     Abilita l&#39;opzione **[!UICONTROL Filmstrip]** per includere anteprime delle immagini precedenti e successive accanto alla diapositiva principale.

1. Fai clic su **[!UICONTROL Aggiungi immagine]** e immetti l&#39;URL e il testo dell&#39;immagine.

   Assicurati di includere un minimo di tre immagini e un massimo di cinque.

   ![](assets/rich_push_carousel_3.png)

1. Gestire l&#39;ordine delle immagini con le frecce Giù e Su.

1. Configura le **[!UICONTROL Impostazioni avanzate]** della notifica push. [Ulteriori informazioni](#push-advanced)

Dopo aver definito il contenuto del messaggio, puoi utilizzare gli abbonati di prova per visualizzare in anteprima e verificare il messaggio.

>[!ENDTABS]

## Impostazioni avanzate della notifica push {#push-advanced}

![](assets/push_content_5.png){zoomable="yes"}

| Parametro | Descrizione |
|---------|---------|
| **[!UICONTROL Colore icona]** | Impostare il colore dell&#39;icona con i codici colore esadecimali. |
| **[!UICONTROL Colore titolo]** | Imposta il colore del Titolo con i codici colore Esadecimali. |
| **[!UICONTROL Colore testo messaggio]** | Impostare il colore del testo del messaggio con i codici colore esadecimali. |
| **[!UICONTROL Colore di sfondo notifica]** | Imposta il colore dello sfondo della notifica con i codici di colore esadecimali. |
| **[!UICONTROL Suono]** | Imposta l’audio da riprodurre quando il dispositivo riceve la notifica. |
| **[!UICONTROL Conteggio notifiche]** | Imposta il numero di nuove informazioni non lette da visualizzare direttamente sull’icona dell’applicazione. Questo consente all’utente di visualizzare rapidamente il numero di notifiche in sospeso. |
| **[!UICONTROL ID canale]** | Imposta l’ID canale della notifica. L’app deve creare un canale con questo ID canale prima di ricevere qualsiasi notifica con questo ID canale. |
| **[!UICONTROL Tag]** | Imposta un identificatore utilizzato per sostituire le notifiche esistenti nella barra delle notifiche. In questo modo si evita l’accumulo di notifiche multiple e si garantisce che venga visualizzata solo la notifica pertinente più recente. |
| **[!UICONTROL Priorità]** | Imposta il livello di priorità della notifica, che può essere predefinito, minimo, basso o alto. Il livello di priorità determina l’importanza e l’urgenza della notifica, influenzandone la modalità di visualizzazione e la possibilità di ignorare determinate impostazioni di sistema. Per ulteriori informazioni, consulta la [documentazione FCM ](https://firebase.google.com/docs/reference/fcm/rest/v1/projects.messages#notificationpriority). |
| **[!UICONTROL Visibilità]** | Imposta il livello di visibilità della notifica, che può essere pubblica, privata o segreta. Il livello di visibilità determina la quantità di contenuto della notifica viene visualizzata nella schermata di blocco e in altre aree sensibili. Per ulteriori informazioni, consulta la [documentazione FCM](https://firebase.google.com/docs/reference/fcm/rest/v1/projects.messages#visibility). |
| **[!UICONTROL Notifica fissa]** | Quando è attivata, la notifica rimane visibile anche dopo che l’utente fa clic su di essa. <br>Se è disattivata, la notifica viene automaticamente ignorata quando l’utente interagisce con essa. Il comportamento permanente consente alle notifiche importanti di rimanere sullo schermo per periodi più lunghi. |
| **[!UICONTROL Variabili dell’applicazione]** | Consente di definire il comportamento di notifica. Queste variabili sono completamente personalizzabili e sono incluse nel payload del messaggio inviato al dispositivo mobile. |
