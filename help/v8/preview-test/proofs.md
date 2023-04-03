---
audience: end-user
title: Inviare e-mail di test
description: Scopri come definire e inviare e-mail di test
exl-id: b2677579-c95d-443d-b207-466af364c208
badge: label="Alpha" type="Positive"
source-git-commit: b5af5099d62e0e424fffdd8eb74d67f12777b0f2
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 99%

---

# Inviare e-mail di test {#send-proofs}

L’invio di e-mail di test è un passaggio importante nella convalida della campagna e-mail, utile per individuare potenziali problemi. Inviando e-mail di test, puoi verificare il funzionamento di vari elementi come collegamenti, collegamenti di rinuncia, immagini e pagine mirror, nonché rilevare eventuali errori.

Le e-mail di test possono essere inviate a due tipi di destinatari:

* **Profili di test**: invia e-mail di test agli indirizzi seed, ossia destinatari aggiuntivi e fittizi presenti nel database. Possono essere creati nella console Adobe Campaign nella cartella **[!UICONTROL Risorse]**/**[!UICONTROL Gestione delle campagne]**/**[!UICONTROL Indirizzi seed]**.

* **Sostituisci dal target principale**: invia le e-mail di test a un indirizzo e-mail specifico impersonando un profilo esistente. Questo consente di verificare l’esperienza dell’e-mail così come verrà ricevuta dai destinatari, con una rappresentazione accurata del messaggio per quello specifico profilo.

## Selezionare i destinatari del test {#recipients}

1. Accedi alla schermata di simulazione del contenuto e-mail, quindi fai clic sul pulsante **[!UICONTROL Test]**.

   ![](assets/test-button.png)

1. Utilizza l’elenco a discesa **[!UICONTROL Modalità]** per scegliere il tipo di destinatari che ricevono il messaggio e-mail di test:

   * **Profili di test**: invia e-mail di test agli indirizzi seed, ossia destinatari aggiuntivi e fittizi presenti nel database.

   * **Sostituisci dal target principale**: invia le e-mail di test a un indirizzo e-mail specifico impersonando un profilo esistente. Questo consente di verificare l’esperienza dell’e-mail così come verrà ricevuta dai destinatari, con una rappresentazione accurata del messaggio per quello specifico profilo.

   ![](assets/test-mode.png)

   >[!NOTE]
   >
   >Per impostazione predefinita, viene selezionata la modalità **[!UICONTROL Profili di test]**. Se hai già selezionato dei profili per visualizzare l’anteprima dell’e-mail nella schermata di simulazione del contenuto, questi vengono preselezionati come destinatari del test. Puoi deselezionare la selezione e/o aggiungere altri destinatari.

1. Per inviare e-mail di test ai profili di sostituzione, scegli la modalità **[!UICONTROL Sostituisci dal target]** quindi segui questi passaggi:

   1. Fai clic sul pulsante **[!UICONTROL Aggiungi indirizzo]** e specifica l’indirizzo e-mail che riceverà l’e-mail di test.

      Puoi inserire qualsiasi indirizzo e-mail. Questo consente di inviare e-mail di test a qualsiasi utente, anche se non è utente di Adobe Campaign V8.

   1. Seleziona il profilo dal target da utilizzare per inviare l’e-mail di test. Puoi anche consentire ad Adobe Campaign di selezionare un profilo casuale dal target.

   1. Conferma il destinatario e ripeti l’operazione per aggiungere tutti gli indirizzi necessari.

      ![](assets/substitution.png)

1. Una volta selezionati i destinatari del test, puoi inviare l’e-mail di test. [Scopri come inviare e-mail di test](#send)

   >[!NOTE]
   >
   >Se desideri inviare il messaggio e-mail finale ai destinatari dell’e-mail di test, abilita **[!UICONTROL Includi la popolazione di test nel target principale]**.

## Inviare e-mail di test {#send}

Per inviare l’e-mail di test ai destinatari selezionati, fai clic su **[!UICONTROL Invia e-mail di test]** quindi conferma l’invio.

![](assets/send-proof.png)

Invia tutte le e-mail di test necessarie fino a quando non avrai finalizzato il contenuto della consegna. Al termine, puoi inviare l’e-mail al target principale. [Scopri come preparare e inviare un messaggio e-mail](../monitor/prepare-send.md)

## Accedere alle e-mail di test inviate {#access-proofs}

Una volta inviate le e-mail di test, puoi accedere ai registri dedicati dal pulsante **[!UICONTROL Visualizza registro e-mail di test]**.

Questi registri consentono di accedere a tutte le e-mail di test inviate per la consegna selezionata e di visualizzare specifiche statistiche relative all’invio. [Scopri come monitorare i registri di consegna](../monitor/delivery-logs.md)

![](assets/proof-log.png)

Puoi anche accedere alle e-mail di test inviate dall’elenco delle consegne, come qualsiasi altra consegna.

![](assets/delivery-list.png)
