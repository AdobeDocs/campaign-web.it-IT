---
title: Personalizzare i contenuti in Campaign
description: Scopri come personalizzare i contenuti nell’interfaccia web di Adobe Campaign
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
badge: label="Alpha" type="Positive"
source-git-commit: 573f0bbf396f795029c5e34b436521cb1c7b80a5
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 100%

---


# Blocchi di contenuto incorporati {#ootb-content-blocks}

I blocchi di contenuto incorporati sono:

* **[!UICONTROL Enabled by Adobe Campaign]** : inserisce il logo “Enabled by Adobe Campaign”.
* **[!UICONTROL Funzione di formattazione per nomi propri]**: genera la funzione JavaScript **[!UICONTROL toSmartCase]**, che applica il maiuscolo alla prima lettera di ogni parola.
* **[!UICONTROL Saluti]**: inserisce i saluti con il nome completo del destinatario, seguito da una virgola. Esempio: “Ciao John Doe,” 
* **[!UICONTROL Inserisci logo]**: inserisce un logo definito nelle impostazioni dell’istanza.
* **[!UICONTROL Collegamento a una pagina mirror]**: inserisce un collegamento alla [pagina mirror](../content/mirror-page.md). Il formato predefinito è: “Se non riesci a visualizzare correttamente questo messaggio, fai clic qui”.
* **[!UICONTROL URL pagina mirror]**: inserisce l’URL della pagina mirror, consentendo ai designer della consegna di controllare il collegamento.
* **[!UICONTROL URL per accettazione offerta in modalità unitaria]**: inserisce un URL che consente di impostare un’offerta su **[!UICONTROL Accettata]**. Questo blocco è disponibile se il modulo di interazione è abilitato
* **[!UICONTROL Conferma registrazione]**: inserisce un collegamento che consente di confermare la registrazione o l’iscrizione.
* **[!UICONTROL Collegamento di registrazione]**: inserisce un collegamento per la registrazione o l’iscrizione. Questo collegamento è definito nelle impostazioni dell’istanza. Il contenuto predefinito è: “Per registrarti, fai clic qui.”
* **[!UICONTROL Collegamento di registrazione (con destinatario che inoltra)]**: inserisce un collegamento di registrazione o iscrizione che consente di identificare il visitatore e la consegna. Questo collegamento è definito nelle impostazioni dell’istanza.
* **[!UICONTROL URL pagina di registrazione]**: inserisce un URL per registrarsi o iscriversi
* **[!UICONTROL Stile e-mail di contenuto]** e **[!UICONTROL Stile notifica]**: genera il codice necessario per formattare un’e-mail con stili HTML predefiniti.
* **[!UICONTROL Collegamento annullamento iscrizione]**: inserisce un collegamento che consente di annullare l’iscrizione a tutte le consegne (elenco Bloccati). Il contenuto associato predefinito è: “Hai ricevuto questo messaggio perché sei stato in contatto con ***nome organizzazione*** o una sua filiale. Per non ricevere più messaggi da ***nome organizzazione***, fai clic qui.”
