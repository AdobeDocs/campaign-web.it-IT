---
title: Personalizzare i contenuti in Campaign
description: Scopri come personalizzare i contenuti in Adobe Campaign Web
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
badge: label="Beta"
exl-id: 45cdd310-7c0c-4b57-bb7f-0576d8eca19d
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 96%

---

# Aggiungere blocchi di contenuto incorporati {#ootb-content-blocks}

Adobe Campaign offre un elenco di blocchi di contenuto preconfigurati. Questi blocchi di contenuto sono dinamici, personalizzati e hanno un rendering specifico che puoi inserire nelle consegne. Ad esempio, puoi aggiungere un logo, un messaggio di auguri o un collegamento alla pagina mirror.

Per aggiungere un blocco di contenuto a una consegna, segui questi passaggi:

1. Apri una consegna e modificane il contenuto.

1. Individua il campo in cui desideri aggiungere un blocco di contenuto e fai clic sull’icona **[!UICONTROL Apri finestra di personalizzazione]** per aprire l’editor di espressioni.

   ![](assets/content-block-access.png){zoomable=&quot;yes&quot;}{width="800" align="center"}

1. Nell’editor di espressioni, passa al menu a sinistra **[!UICONTROL Blocchi di contenuto]**.

1. Per aggiungere un blocco di contenuto, posiziona il cursore nella posizione desiderata all’interno del contenuto e fai clic sul pulsante “+” per inserirlo.

   ![](assets/content-blocks.png){zoomable=&quot;yes&quot;}{width="800" align="center"}

I blocchi di contenuto incorporati sono:

* **[!UICONTROL Banner di rinuncia predefinito]**
* **[!UICONTROL Enabled by Adobe Campaign]** : inserisce il logo “Enabled by Adobe Campaign”.
* **[!UICONTROL Funzione di formattazione per nomi propri]**: genera la funzione JavaScript **[!UICONTROL toSmartCase]**, che applica il maiuscolo alla prima lettera di ogni parola.
* **[!UICONTROL Saluti]**: inserisce i saluti con il nome completo del destinatario, seguito da una virgola. Esempio: “Ciao John Doe,” 
* **[!UICONTROL Inserisci logo]**: inserisce un logo definito nelle impostazioni dell’istanza.
* **[!UICONTROL Collegamento a una pagina mirror]**: inserisce un collegamento alla [pagina mirror](../email/mirror-page.md). Il formato predefinito è: “Se non riesci a visualizzare correttamente questo messaggio, fai clic qui”.
* **[!UICONTROL URL pagina mirror]**: inserisce l’URL della pagina mirror, consentendo ai designer della consegna di controllare il collegamento.
* **[!UICONTROL Stile notifica]**
* **[!UICONTROL URL per accettazione offerta in modalità unitaria]**: inserisce un URL che consente di impostare un’offerta su **[!UICONTROL Accettata]**. Questo blocco è disponibile se il modulo di interazione è abilitato
* **[!UICONTROL Conferma registrazione]**: inserisce un collegamento che consente di confermare la registrazione o l’iscrizione.
* **[!UICONTROL Collegamento di registrazione]**: inserisce un collegamento per la registrazione o l’iscrizione. Questo collegamento è definito nelle impostazioni dell’istanza. Il contenuto predefinito è: “Per registrarti, fai clic qui.”
* **[!UICONTROL Collegamento di registrazione (con destinatario che inoltra)]**: inserisce un collegamento di registrazione o iscrizione che consente di identificare il visitatore e la consegna. Questo collegamento è definito nelle impostazioni dell’istanza.
* **[!UICONTROL URL pagina di registrazione]**: inserisce un URL per registrarsi o iscriversi
* Collegamenti per condivisione sui social network
* **[!UICONTROL Stile e-mail di contenuto]** e **[!UICONTROL Stile notifica]**: genera il codice necessario per formattare un’e-mail con stili HTML predefiniti.
* **[!UICONTROL Collegamento annullamento iscrizione]**: inserisce un collegamento che consente di annullare l’iscrizione a tutte le consegne (elenco Bloccati). Il contenuto associato predefinito è: “Hai ricevuto questo messaggio perché sei stato in contatto con ***nome organizzazione*** o una sua filiale. Per non ricevere più messaggi da ***nome organizzazione***, fai clic qui.”

>[!NOTE]
>
>Puoi definire nuovi blocchi dalla console di Adobe Campaign v8, che ti consentono di ottimizzare la personalizzazione delle consegne. Per ulteriori informazioni, consulta la [documentazione di Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/personalize/personalization-blocks.html?lang=it#create-custom-personalization-blocks){target="_blank"}.
