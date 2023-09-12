---
audience: end-user
title: Inviare consegne di test
description: Scopri come definire e inviare consegne di test
exl-id: b2677579-c95d-443d-b207-466af364c208
badge: label="Beta"
source-git-commit: ed9d67c5d84826035785e9543f4ed7655aa094f1
workflow-type: tm+mt
source-wordcount: '1032'
ht-degree: 100%

---

# Inviare consegne di test {#send-test-deliveries}

>[!CONTEXTUALHELP]
>id="acw_email_preview_mode"
>title="Modalità anteprima"
>abstract="Visualizza l’anteprima e verifica il messaggio includendo la popolazione di test nel target principale."

**[!UICONTROL Adobe Campaign]** consente di testare un messaggio prima di inviarlo al pubblico principale.

L’invio di consegne di test (precedentemente note come “bozze”) è un passaggio importante nella convalida della campagna e utile per individuare potenziali problemi.

I destinatari di un test possono controllare vari elementi come collegamenti, collegamenti di rinuncia, immagini o pagine mirror, nonché rilevare eventuali errori nel rendering, nel contenuto, nelle impostazioni di personalizzazione e nella configurazione della consegna.

## Selezionare i destinatari del test {#test-recipients}

>[!CONTEXTUALHELP]
>id="acw_email_preview_option_test_target"
>title="Popolazione di test"
>abstract="Seleziona una modalità per la popolazione di test."

In base al canale utilizzato, i messaggi di test possono essere inviati a tre tipi di destinatari:

* [Profili di test](#test-profiles): invia **e-mail e SMS di test** agli indirizzi seed, ossia destinatari aggiuntivi presenti nel database. Possono essere creati nella console [!DNL Campaign] nella cartella **[!UICONTROL Risorse]** > **[!UICONTROL Gestione delle campagne]** > **[!UICONTROL Indirizzi seed]**. Ulteriori informazioni sono disponibili nella [documentazione di Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html?lang=it){target="_blank"}

* [Sostituisci dal target principale](#substitution-profiles): invia **e-mail e SMS di test** a un indirizzo e-mail o numero di telefono specifico impersonando un profilo esistente. Questo consente di vivere l’esperienza del messaggio così come verrà ricevuta dai destinatari, con una rappresentazione accurata del contenuto per quello specifico profilo.

* [Abbonati](#subscribers): invia le **notifiche push di test** agli abbonati fittizi aggiunti al database. I profili di test possono essere creati nella console [!DNL Campaign] nella cartella **[!UICONTROL Risorse]** > **[!UICONTROL Gestione delle campagne]** > **[!UICONTROL Indirizzi seed]**. Ulteriori informazioni sono disponibili nella [documentazione di Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html?lang=it){target="_blank"}

Per selezionare i destinatari di una consegna di test, segui i passaggi seguenti in base al tipo di profili che desideri utilizzare.

### Profili di test {#test-profiles}

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_test_mode"
>title="Destinazione della bozza"
>abstract="Puoi caricare un secondo file come “destinazione della bozza”, se desideri testare la consegna prima di inviarla al target principale."

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_test_upload"
>title="Carica profili"
>abstract="Puoi caricare un secondo file con profili aggiuntivi se desideri testare la consegna con un set diverso da quello utilizzato per il target principale."

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_test_sample"
>title="File modello"
>abstract="La formattazione del file deve essere uguale a quella del file originale.<br/>Formati di file supportati: txt, csv. Dimensione massima del file: 15 MB. Utilizza la prima riga come intestazione di colonna."

1. Passa alla schermata di modifica del contenuto della consegna e-mail o SMS, quindi fai clic sul pulsante **[!UICONTROL Simula contenuto]**.

1. Fai clic sul pulsante **[!UICONTROL Test]**

   >[!NOTE]
   >
   >Se hai già selezionato i profili per [visualizzare l’anteprima della consegna](preview-content.md), sono elencati nel riquadro a sinistra.

   ![](assets/simulate-test-button-email.png)

1. Dall’elenco a discesa **[!UICONTROL Modalità]**, scegli **[!UICONTROL Profili di test]** per eseguire il targeting di destinatari fittizi che riceveranno la consegna e-mail o SMS di test.

   ![](assets/simulate-profile-mode.png)

1. Se hai già selezionato dei profili per [visualizzare l’anteprima del messaggio](preview-content.md) nella schermata di simulazione del contenuto, questi vengono preselezionati come destinatari del test. Puoi cancellare la selezione e/o aggiungere altri destinatari utilizzando il pulsante **[!UICONTROL Aggiungi profili di test]**.

   >[!NOTE]
   >
   >Per impostazione predefinita, viene selezionata la modalità **[!UICONTROL Utilizza profili di test]**.

1. Per inviare il messaggio finale anche ai destinatari della consegna di test, seleziona l’opzione **[!UICONTROL Includi la popolazione di test nel target principale]**.

1. Una volta selezionati i profili di test, puoi [inviare la consegna di test](#send-test).

### Profili di sostituzione {#substitution-profiles}

Per inviare un’e-mail o un SMS di test a un indirizzo e-mail o a un numero di telefono specifico durante la visualizzazione dei dati da un profilo esistente del database [!DNL Campaign], utilizza profili di sostituzione.

1. Prima di inviare un test, assicurati di definire un pubblico target per la consegna. [Ulteriori informazioni](../audience/about-audiences.md)

1. Passa alla schermata di modifica del contenuto della consegna e-mail o SMS, quindi fai clic sul pulsante **[!UICONTROL Simula contenuto]**.

1. Fai clic sul pulsante **[!UICONTROL Test]**

   ![](assets/simulate-test-button-email.png)

1. Dall’elenco a discesa **[!UICONTROL Modalità]**, scegli **[!UICONTROL Sostituisci dal target principale]** per inviare un test a un indirizzo e-mail o a un numero di telefono specifico durante la visualizzazione dei dati da un profilo esistente.

   >[!CAUTION]
   >
   >Se non hai selezionato un [pubblico](../audience/about-audiences.md) per la consegna, l’opzione **[!UICONTROL Sostituisci dal target principale]** sarà disattivata e non sarà possibile selezionare profili di sostituzione.

1. Fai clic sul pulsante **[!UICONTROL Aggiungi indirizzo]** e specifica l’indirizzo e-mail o il numero di telefono che riceverà la consegna di test.

   ![](assets/simulate-add-substitution-address.png)

   >[!NOTE]
   >
   >Puoi inserire qualsiasi indirizzo e-mail o numero di telefono. Questo consente di inviare consegne di test a qualsiasi destinatario, anche se non è utente di [!DNL Adobe Campaign].

1. Seleziona il profilo dal target definito per la consegna da utilizzare come sostituto. Puoi anche consentire ad [!DNL Adobe Campaign] di selezionare un profilo casuale dal target. I dati del profilo dal profilo selezionato verranno visualizzati nella consegna di test.

1. Conferma il destinatario e ripeti l’operazione per aggiungere tutti gli indirizzi e-mail o i numeri di telefono necessari.

   ![](assets/simulate-profile-substitute.png)

1. Per inviare il messaggio finale anche ai destinatari della consegna di test, seleziona l’opzione **[!UICONTROL Includi la popolazione di test nel target principale]**.

1. Una volta selezionati i profili di sostituzione, puoi [inviare la consegna di test](#send-test).

### Abbonati {#subscribers}

Quando si utilizzano le notifiche push, le consegne di test possono essere inviate solo agli abbonati. Per selezionarli, segui i passaggi seguenti.

1. Passa alla schermata di modifica del contenuto della consegna, quindi fai clic sul pulsante **[!UICONTROL Simula contenuto]**.

1. Fai clic sul pulsante **[!UICONTROL Test]**

   ![](assets/simulate-test-button-push.png)

1. Se hai già selezionato degli abbonati per [visualizzare l’anteprima della consegna](preview-content.md) nella schermata di simulazione del contenuto, questi profili vengono preselezionati come abbonati a scopo di test.

   Puoi cancellare la selezione e/o aggiungere altri abbonati utilizzando il pulsante dedicato.

   ![](assets/simulate-test-subscribers.png)

1. Per inviare la notifica push finale anche agli abbondati a scopo di test, seleziona l’opzione **[!UICONTROL Includi la popolazione di test nel target principale]**.

1. Una volta selezionati gli iscritti, puoi [inviare la consegna di test](#send-test).

## Inviare la consegna di test {#send-test}

Per inviare la consegna di test ai destinatari selezionati, segui i passaggi indicati di seguito.

1. Fai clic sul pulsante **[!UICONTROL Invia test]**

1. Conferma l’invio.

   ![](assets/simulate-send-test.png)

1. Invia tutti i test necessari fino a quando non avrai finalizzato il contenuto della consegna.

Al termine, puoi preparare la consegna e inviarla al target principale. Scopri come nelle sezioni dedicate di seguito:

* [Inviare l’e-mail](../monitor/prepare-send.md)
* [Inviare la notifica push](../push/send-push.md#send-push)
* [Inviare la consegna SMS](../sms/send-sms.md#send-sms)

## Accedere alle consegne di test inviate {#access-proofs}

Una volta inviate le consegne di test, puoi accedere ai registri dedicati mediante il pulsante **[!UICONTROL Visualizza registro di test]**.

Questi registri consentono di accedere a tutti i test inviati per la consegna selezionata e di visualizzare specifiche statistiche relative all’invio. [Scopri come monitorare i registri di consegna](../monitor/delivery-logs.md)

![](assets/simulate-test-log.png)

Puoi anche accedere ai test inviati dall’[elenco delle consegne](../msg/gs-messages.md), come qualsiasi altra consegna.

![](assets/simulate-deliveries-list.png)
