---
title: Campi personalizzati
description: Scopri come configurare i campi personalizzati
source-git-commit: 97769e885145d771685752f6367c5ea00831701d
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 5%

---

# Configurare campi personalizzati {#custom-fields}

I campi personalizzati sono attributi aggiuntivi aggiunti agli schemi predefiniti tramite la console Adobe Campaign. Per ulteriori informazioni, consulta [Documentazione di Adobe Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/shemas-forms/extend-schema.html){target="_blank"}

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

1. Sotto **Amministrazione**, fai clic su **Schemi**.

   ![](assets/custom-fields.png){zoomable=&quot;yes&quot;}

1. Individua lo schema desiderato, ad esempio **Destinatari (nms)** schema.

   ![](assets/custom-fields2.png){zoomable=&quot;yes&quot;}

1. Fai clic su **Altre azioni** e seleziona **Modifica dettagli personalizzati**.

   ![](assets/custom-fields3.png){zoomable=&quot;yes&quot;}

   Il **Modifica dettagli personalizzati** nella schermata vengono visualizzati tutti i campi personalizzati e il relativo tipo.

   ![](assets/custom-fields4.png){zoomable=&quot;yes&quot;}

   Questa schermata consente di eseguire le azioni seguenti:

   * modificare l&#39;ordine dei diversi campi utilizzando le frecce su e giù.
   * rendere il campo obbligatorio: seleziona la **Obbligatorio** casella.
   * rendere visibile o nascondere il campo: fare clic sul pulsante **Visibile** pulsante.
   * aggiungi una condizione di visibilità: fai clic su **Visibile se** e scrivere l’espressione xtk utilizzando le funzioni xtk disponibili.

1. Passa alla schermata che visualizza il campo personalizzato. Nel nostro esempio, si tratta della schermata dei dettagli del profilo.

   ![](assets/custom-fields5.png){zoomable=&quot;yes&quot;}
