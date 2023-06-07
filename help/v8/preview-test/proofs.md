---
audience: end-user
title: Inviare e-mail di test
description: Scopri come definire e inviare e-mail di test
exl-id: b2677579-c95d-443d-b207-466af364c208
badge: label="Alpha" type="Positive"
source-git-commit: c6ebdf23c22cb197a816684108c782aa2180dc1e
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 44%

---

# Inviare e-mail di test {#send-test-emails}

**[!UICONTROL Adobe Campaign]** consente di testare un messaggio prima di inviarlo al pubblico principale.

L’invio di e-mail di test è un passaggio importante nella convalida della campagna e-mail, utile per individuare potenziali problemi.

I destinatari di un test possono controllare vari elementi come collegamenti, collegamenti di rinuncia, immagini e pagine mirror, nonché rilevare eventuali errori nel rendering, nel contenuto, nelle impostazioni di personalizzazione e nella configurazione dell’e-mail.

## Selezionare i destinatari del test {#test-recipients}

Le e-mail di test possono essere inviate a due tipi di destinatari:

* **Profili di test** : invia e-mail di test agli indirizzi seed, che sono destinatari aggiuntivi e fittizi nel database. Possono essere create in [!DNL Campaign] console in **[!UICONTROL Risorse]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Indirizzi seed]** cartella. [Ulteriori informazioni](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/using-seed-addresses/creating-seed-addresses.html){target="_blank"}

* **Sostituisci dal target principale** : invia e-mail di test a un indirizzo e-mail specifico mentre impersona un profilo esistente. Questo consente di verificare l’esperienza dell’e-mail così come verrà ricevuta dai destinatari, con una rappresentazione accurata del messaggio per quello specifico profilo.

Per selezionare i destinatari del test e-mail, segui la procedura indicata di seguito.

1. Accedere all’e-mail [Modifica contenuto](../content/edit-content.md) schermata o al [E-mail Designer](../content/get-started-email-designer.md), quindi fare clic su **[!UICONTROL Simula contenuto]** pulsante.

1. Fai clic su **[!UICONTROL Test]** pulsante.

   ![](assets/simulate-test-button.png)

1. Utilizza l’elenco a discesa **[!UICONTROL Modalità]** per scegliere il tipo di destinatari che ricevono il messaggio e-mail di test:

   * **Profili di test** per eseguire il targeting di destinatari fittizi

   * **Sostituisci dal target principale** per inviare un test a un indirizzo e-mail specifico durante la visualizzazione dei dati da un profilo esistente.

   ![](assets/simulate-profile-mode.png)

   >[!NOTE]
   >
   >Per impostazione predefinita, il **[!UICONTROL Utilizzare i profili di test]** è selezionata. Se hai già selezionato dei profili per visualizzare l’anteprima dell’e-mail nella schermata di simulazione del contenuto, questi vengono preselezionati come destinatari del test. Puoi deselezionare la selezione e/o aggiungere altri destinatari.

1. Per inviare e-mail di test ai profili di sostituzione, scegli la **[!UICONTROL Sostituisci da destinazione]** , quindi eseguire la procedura seguente:

   1. Fai clic sul pulsante **[!UICONTROL Aggiungi indirizzo]** e specifica l’indirizzo e-mail che riceverà l’e-mail di test.

      Puoi inserire qualsiasi indirizzo e-mail. Questo consente di inviare e-mail di test a qualsiasi utente, anche se non è utente di [!DNL Adobe Campaign].

   1. Selezionare il profilo dalla destinazione da utilizzare come sostituto. Puoi anche consentire [!DNL Adobe Campaign] selezionare un profilo casuale dalla destinazione. I dati del profilo dal profilo selezionato verranno visualizzati nell’e-mail del test.

   1. Conferma il destinatario e ripeti l’operazione per aggiungere tutti gli indirizzi necessari.

      ![](assets/simulate-profile-substitute.png)

1. Dopo aver selezionato i destinatari del test, puoi [invia l’e-mail del test](#send-test).

   >[!NOTE]
   >
   >Per inviare anche il messaggio e-mail finale ai destinatari del messaggio e-mail di test, seleziona la **[!UICONTROL Includi la popolazione di test nel target principale]** opzione.

## Inviare e-mail di test {#send-test}

Per inviare l’e-mail di test ai destinatari selezionati, segui la procedura indicata di seguito.

1. Clic **[!UICONTROL Invia e-mail di test]**.

1. Conferma l’invio.

   ![](assets/simulate-send-test.png)

1. Invia tutte le e-mail di test necessarie fino a quando non avrai finalizzato il contenuto della consegna.

Una volta fatto, puoi [preparare e inviare l’e-mail](../monitor/prepare-send.md) al target principale.

## Accedere alle e-mail di test inviate {#access-proofs}

Una volta inviate le e-mail di test, puoi accedere ai registri dedicati dal pulsante **[!UICONTROL Visualizza registro e-mail di test]**.

Questi registri consentono di accedere a tutte le e-mail di test inviate per la consegna selezionata e di visualizzare specifiche statistiche relative all’invio. [Scopri come monitorare i registri di consegna](../monitor/delivery-logs.md)

![](assets/simulate-test-log.png)

Puoi anche accedere alle e-mail di test inviate dalla [elenco consegne](../msg/gs-messages.md), come qualsiasi consegna.

![](assets/simulate-deliveries-list.png)
