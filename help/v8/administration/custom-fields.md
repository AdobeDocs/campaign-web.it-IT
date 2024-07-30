---
title: Campi personalizzati
description: Scopri come configurare i campi personalizzati
exl-id: 34e7e0b7-3981-43b1-95a5-6c672adafdc9
source-git-commit: 728bc032614067bc420b80a4cac634a08f594ff8
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 8%

---

# Configurare campi personalizzati {#custom-fields}

I Campi personalizzati sono ulteriori attributi aggiunti agli schemi predefiniti tramite la console Adobe Campaign. Ulteriori informazioni sono disponibili nella [documentazione di Adobe Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/shemas-forms/extend-schema.html){target="_blank"}

Questi campi personalizzati vengono visualizzati in varie schermate, ad esempio nei dettagli di un profilo o di un profilo di test.

Nell’interfaccia utente web, non è possibile creare campi personalizzati, ma è possibile modificarne la modalità di visualizzazione. Le modifiche vengono applicate a tutti gli utenti di Campaign.

>[!NOTE]
>
>Per modificare i campi personalizzati è necessario disporre dei diritti di amministratore.

I campi personalizzati sono disponibili nei seguenti schemi:

* Destinatari (nms)
* Campagne (nms)
* Consegne (nms)
* Indirizzi seed (nms)

Per configurare i campi personalizzati, effettua le seguenti operazioni:

1. In **Amministrazione**, fare clic su **Schemi**.

   ![](assets/custom-fields.png){zoomable="yes"}

1. Individua lo schema desiderato, ad esempio lo schema **Destinatari (nms)**.

   ![](assets/custom-fields2.png){zoomable="yes"}

1. Fai clic sul pulsante **Altre azioni** e seleziona **Modifica dettagli personalizzati**.

   ![](assets/custom-fields3.png){zoomable="yes"}

   Nella schermata **Modifica dettagli personalizzati** vengono visualizzati tutti i campi personalizzati e il relativo tipo.

   ![](assets/custom-fields4.png){zoomable="yes"}

   Questa schermata consente di eseguire le azioni seguenti:

   * modificare l&#39;ordine dei diversi campi utilizzando le frecce su e giù.
   * rendi il campo obbligatorio: seleziona la casella **Obbligatorio**.
   * rendere visibile o nascondere il campo: fare clic sul pulsante **Visibile**.
   * aggiungi una condizione di visibilità: fai clic sul pulsante **Visible if** e scrivi l&#39;espressione xtk utilizzando le funzioni xtk disponibili.

1. Passa alla schermata che visualizza il campo personalizzato. Nel nostro esempio, si tratta della schermata dei dettagli del profilo.

   ![](assets/custom-fields5.png){zoomable="yes"}
