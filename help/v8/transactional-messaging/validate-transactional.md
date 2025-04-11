---
audience: end-user
title: Convalidare messaggi transazionali
description: Scopri come convalidare un messaggio transazionale nell’interfaccia utente di Campaign Web
exl-id: 4a24792f-b9f4-4224-b3a8-75f6969b64da
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 1%

---

# Convalidare messaggi transazionali

Durante o dopo la creazione del messaggio transazionale, puoi convalidare il contenuto utilizzando un esempio di dati.

## Simula contenuto {#simulate-content}

Per simulare il contenuto del messaggio, segui la procedura riportata di seguito:

* Assicurati che il percorso di personalizzazione nel contenuto del messaggio corrisponda all’esempio di contesto. Nell&#39;esempio seguente, per visualizzare il nome del profilo di test, utilizzare il percorso *rtEvent.ctx.basicDetails.firstName*.

  Puoi modificare il contenuto del messaggio o l’esempio di contesto per allinearli.

  ![Schermata che mostra la verifica dei percorsi di personalizzazione nel contenuto del messaggio](assets/validate-verification.png){zoomable="yes"}

* Fai clic sul pulsante **[!UICONTROL Simula contenuto]** per visualizzare in anteprima il messaggio transazionale con i dati immessi nell&#39;esempio di contesto.

  ![Schermata che mostra il pulsante Simula contenuto e la funzionalità di anteprima](assets/validate-simulate.png){zoomable="yes"}

  Dopo aver esaminato il contenuto, fai clic sul pulsante **[!UICONTROL Chiudi]**.

* Se hai apportato modifiche al contenuto, fai clic sul pulsante **[!UICONTROL Ripubblica]**.

## Invia bozza

Per testare e provare il messaggio transazionale così come verrebbe consegnato attraverso il canale scelto, ad esempio e-mail, SMS o notifiche push, utilizza la funzione bozza.

Nella finestra del contenuto della [simulazione](#simulate-content), fare clic sul pulsante **[!UICONTROL Invia bozza]**.

![Schermata che mostra il pulsante Invia bozza nella finestra del contenuto della simulazione](assets/transactional-proof.png){zoomable="yes"}

Nella nuova finestra visualizzata, inserisci l’indirizzo e-mail o il numero di telefono, a seconda del canale, dove desideri ricevere la bozza. Dopo aver immesso l&#39;indirizzo desiderato, fare clic sui pulsanti **[!UICONTROL Invia bozza]** e **[!UICONTROL Conferma]**. Questa azione invia un esempio del messaggio transazionale, garantendo che tutte le personalizzazioni, il contenuto dinamico e la formattazione vengano visualizzati correttamente come farebbero per gli utenti finali.

![Schermata che mostra la funzionalità Send proof e il processo di conferma](assets/transactional-sendproof.png){zoomable="yes"}

Questo passaggio è essenziale per identificare eventuali problemi prima di pubblicare il messaggio sulle transazioni.