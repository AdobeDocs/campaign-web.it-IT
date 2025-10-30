---
audience: end-user
title: Configurare una consegna multilingue
description: Scopri come configurare una consegna multilingue
source-git-commit: d8d78f97cdf99e67c59827a91c54851b1cbbeb16
workflow-type: tm+mt
source-wordcount: '586'
ht-degree: 8%

---

# Configurare una consegna multilingue {#multilingual-delivery}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_multilingual"
>title="Aggiungere lingue"
>abstract="In questa scheda troverai un elenco delle lingue in cui deve essere inviata la consegna. Puoi aggiungere altre lingue facendo clic sul pulsante Aggiungi lingua o duplicando un’altra lingua tramite questa scheda."

Nell’interfaccia utente web di Campaign, puoi impostare le consegne come multilingue, che consente di inviare messaggi in base alla lingua preferita di un profilo. Se non è definita alcuna preferenza, il messaggio viene inviato nella lingua predefinita.

In una distribuzione multilingue, la gestione della lingua si basa su varianti. Ogni variante rappresenta una lingua. Durante la creazione della consegna, puoi aggiungere più varianti di lingua in modo che corrispondano al numero di lingue richieste nel messaggio. Puoi anche modificare la lingua predefinita in qualsiasi momento dopo l’aggiunta di queste varianti.

La funzionalità multilingue è attualmente disponibile per e-mail, notifiche push, messaggi transazionali e SMS.

>[!AVAILABILITY]
>
>Le notifiche push multilingue, i messaggi transazionali e gli SMS sono disponibili solo per un set di organizzazioni (disponibilità limitata) e verranno implementati a livello globale in una versione futura. Il server deve essere aggiornato alla versione 8.8.2 o successiva.

Per impostare le consegne multilingue, segui questi passaggi principali:

1. Aggiungi una variante di lingua, [ulteriori informazioni](#add-variant)
1. Definisci il contenuto per ogni variante, [ulteriori informazioni](#define-content)
1. Gestisci varianti di lingua, [leggi tutto](#manage-variant)

## Aggiungi una variante di lingua{#add-variant}

Per creare varianti di lingua, effettua le seguenti operazioni:

1. Dal dashboard di consegna, fai clic sull&#39;icona della matita per accedere alla schermata di modifica del contenuto della consegna, quindi fai clic su **[!UICONTROL Aggiungi lingua]**.

   >[!IMPORTANT]
   >
   >Il pulsante **[!UICONTROL Aggiungi lingua]** è disponibile solo se la dimensione di destinazione contiene lo schema **Lingua**. Per ulteriori informazioni sugli schemi e sulle dimensioni di destinazione, consulta la [documentazione dettagliata](../audience/targeting-dimensions.md).

   ![](assets/edit-content_2.png){zoomable="yes"}

1. Dal menu a discesa **Aggiungi lingua**, seleziona la lingua da aggiungere, quindi conferma.

   La prima lingua aggiunta viene impostata automaticamente come predefinita e il contenuto esistente diventa la versione predefinita. Quando vengono aggiunte altre lingue, il loro contenuto viene inizialmente copiato dalla lingua predefinita.

   ![](assets/edit-content_3.png){zoomable="yes"}

   >[!NOTE]
   >
   >Le lingue disponibili in questo elenco dipendono dai valori definiti dall&#39;attributo **Lingua** (valori quali: system, user, dbenum e così via). Ulteriori informazioni sulla gestione dell&#39;enumerazione in questa [sezione](../administration/enumerations.md).

1. Ripetere l&#39;operazione per aggiungere altre lingue. Il pannello **[!UICONTROL Lingue]** a sinistra mostra l&#39;elenco delle lingue scelte, il numero di lingue e la lingua predefinita.

   Ad esempio, se hai scelto l’inglese, il francese e lo svedese, puoi visualizzare queste 3 lingue come illustrato di seguito:

   ![](assets/edit-content_9.png){zoomable="yes"}

   Per informazioni su come gestire le varianti di lingua, consulta questa [sezione](#manage-variant).

## Definisci il contenuto per ogni variante{#define-content}

Una volta impostate le lingue, definisci il contenuto della consegna per ogni lingua.

1. Dalla schermata dell&#39;edizione del contenuto della consegna, seleziona una lingua dal pannello **[!UICONTROL Lingue]**, a sinistra.

   ![](assets/edit-content_11.png){zoomable="yes"}

1. Definisci il contenuto del messaggio per questa lingua. Ulteriori informazioni in questa [sezione](../msg/create-deliveries.md).

1. Ripetere questa operazione per ogni lingua.

<!--
>[!BEGINTABS]

>[!TAB Email delivery]

1. From the delivery content edition screen, choose a language and click the **[!UICONTROL Edit email body]** button. You can also hover over the email preview and select **[!UICONTROL Open email designer]**.

    ![](assets/edit-content_11.png){zoomable="yes"}

1. Define the content of your email for this language. [Read more](../email/get-started-email-designer.md#start-authoring)

1. Repeat this operation for each language.

>[!TAB SMS delivery]

1. From the delivery content edition screen, choose a language.

1. Edit the content of the SMS message for this language. [Read more](../sms/create-sms.md)

    ![](assets/edit-content_11-sms.png){zoomable="yes"}

1. Repeat this operation for each language.

>[!ENDTABS]

-->

Per visualizzare in anteprima la consegna, fai clic sul pulsante **[!UICONTROL Simula contenuto]** e scegli i profili. Assicurati che per ogni profilo venga visualizzato il contenuto corretto.

![](assets/edit-content_5.png){zoomable="yes"}

## Gestione varianti di lingua{#manage-variant}

Nel pannello a sinistra vengono visualizzate tutte le informazioni sulle varianti di lingua. Per eliminare tutte le lingue, fare clic sul pulsante di espansione e quindi su **[!UICONTROL Elimina tutte le varianti]**.

![](assets/edit-content_13.png){zoomable="yes"}

Nell’elenco delle varianti di lingua, puoi eseguire le azioni seguenti:

* **Modifica**: modifica la lingua mantenendo il contenuto associato.
* **Imposta come predefinito**: imposta la lingua come predefinita. Quando un profilo non ha una lingua definita, il messaggio viene inviato nella lingua predefinita.
* **Duplicato**: duplica il contenuto definito per questa lingua e scegli un&#39;altra variante.
* **Elimina**: elimina la variante e il contenuto associato.

![](assets/edit-content_13-sms.png){zoomable="yes"}

