---
title: Branding
description: Scopri come configurare il brand
audience: administration
context-tags: branding,overview;branding,main
role: Admin
level: Experienced
exl-id: 7afc802d-e90c-48c8-aa04-3ea543dfdfbc
source-git-commit: 8b93ddd9c655c9ca461f28392c70872e4005b44f
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 29%

---

# Configurare i brand {#branding-configure}

>[!IMPORTANT]
>
>I brand non possono essere creati o modificati dagli utenti finali: queste operazioni devono essere eseguite dall’amministratore tecnico di Adobe Campaign. Per qualsiasi richiesta, contatta l’Assistenza cliente di Adobe.

In Adobe Campaign V8, i Marchi si trovano nel menu **[!UICONTROL Amministrazione > Piattaforma > Marchio]**.

Un **[!UICONTROL Brand]** è definito dalle seguenti caratteristiche:

* Una **[!UICONTROL Identity]**, che definisce e personalizza il brand. Questa sezione contiene i seguenti campi:

   * **[!UICONTROL Label]**, visibile nell’interfaccia
   * **[!UICONTROL ID]**
   * **[!UICONTROL Brand name]**
   * **[!UICONTROL Website URL]** e **[!UICONTROL Website label]** del brand
   * **[!UICONTROL Logo del brand]**

  ![](assets/branding_1.png)

* **[!UICONTROL Parametri di intestazione delle e-mail inviate]** che personalizzano i contenuti visualizzati dai destinatari delle campagne. Questa sezione contiene i seguenti campi:

   * **[!UICONTROL Sender (email address)]**, che contiene l’indirizzo e-mail del brand.
   * **[!UICONTROL Sender (name)]**, che contiene il nome del brand.
   * **[!UICONTROL Reply to (email address)]**, che contiene l’indirizzo e-mail a cui il cliente può rispondere.
   * **[!UICONTROL Reply to (name)]**, che contiene il nome del brand.
   * **[!UICONTROL Error (email address)]**, che contiene l’indirizzo e-mail da utilizzare in caso di errore.

  >[!IMPORTANT]
  >
  >Dopo aver aggiornato i parametri di intestazione delle e-mail, se il nome e l’indirizzo e-mail del mittente non sono cambiati nell’e-mail creata dal modello, controlla le impostazioni avanzate del modello.

  ![](assets/branding_2.png)

* **[!UICONTROL Brand configs]** definisce i server utilizzati per il tracciamento anche per l&#39;accesso alle pagine di destinazione. Questa sezione contiene i seguenti campi:

   * **[!UICONTROL Il sottodominio del marchio]** fa riferimento all&#39;URL del sottodominio designato specifico per questo marchio, richiesto per la delega da Adobe.

  Si noti che la configurazione per i server di monitoraggio, mirroring e applicazioni viene memorizzata in account esterni separati associati al routing. Queste impostazioni vengono applicate durante il provisioning e non devono essere modificate. Per visualizzare gli URL, accedi alla scheda **[!UICONTROL Prefissi di branding]** dal tuo account esterno.

  ![](assets/branding_3.png)

* Il menu **[!UICONTROL Configurazioni URL di tracciamento]** consente di migliorare il tracciamento degli URL definendo parametri aggiuntivi per l&#39;integrazione con strumenti di analisi web come Adobe Analytics e Google Analytics.

  Utilizza il menu **[!UICONTROL Parametri URL aggiuntivi]** per creare parametri aggiuntivi come coppie chiave-valore insieme alle relative condizioni di applicabilità. Ogni nome di parametro deve essere univoco e non vuoto e ogni valore di parametro non deve essere vuoto. La condizione di applicabilità può essere vuota, ma nessuno di questi valori può includere tag JST.

  Questi parametri verranno applicati agli URL tracciati che corrispondono a qualsiasi nome di dominio specificato nell&#39;**[!UICONTROL Elenco di nomi di dominio]**, che può includere espressioni regolari.

  **Esempio:** Un URL tracciato come `https://www.example.com` diventerà `https://www.example.com/?age=21&deliveryName=DM101` quando i parametri aggiuntivi `age=21` e `deliveryName=DM101` saranno configurati per tale dominio.

## Configurare il branding per la messaggistica transazionale {#branding-transactional-config}

>[!IMPORTANT]
>
>Questa sezione si applica solo alla messaggistica transazionale (Centro messaggi).
>
>Anche se le funzionalità transazionali sono disponibili nell’interfaccia utente di Campaign Web, i passaggi seguenti devono essere eseguiti nella console client di Campaign v8 (istanza di controllo).

Se utilizzi la messaggistica transazionale (Centro messaggi) con il branding, è necessaria una configurazione aggiuntiva.

### Tracciamento delle formule per le istanze in tempo reale

Quando si attiva il branding su un’istanza di controllo in tempo reale (RT), vengono utilizzate opzioni di tracciamento specifiche per gestire le formule di tracciamento. Queste formule vengono configurate centralmente nell&#39;istanza di controllo RT anziché singolarmente in ogni istanza di esecuzione RT.

Le seguenti opzioni definiscono le formule di tracciamento utilizzate dalle consegne RT:

* **`NmsTracking_RT_ClickFormula`**: specifica la formula utilizzata per il tracciamento dei clic sulle istanze RT

* **`NmsTracking_RT_OpenFormula`**: specifica la formula utilizzata per il tracciamento delle aperture nelle istanze RT

Se la tua implementazione richiede formule di tracciamento personalizzate per la messaggistica transazionale, utilizza l’opzione seguente:

* **`Branding_RT_ListXtkOptions_toPublish`**: elencare i nomi delle opzioni XTK per le formule personalizzate qui (separati da virgole). In questo modo, le consegne RT possono applicare le formule di tracciamento personalizzate.