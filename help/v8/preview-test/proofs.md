---
audience: end-user
title: Invia e-mail di test
description: Scopri come definire e inviare e-mail di test
exl-id: b2677579-c95d-443d-b207-466af364c208
source-git-commit: 8398c0cacb2e6e2198e295787bb5e4e25af74e6e
workflow-type: tm+mt
source-wordcount: '524'
ht-degree: 1%

---

# Invia e-mail di test {#send-proofs}

![](../assets/do-not-localize/badge.png)

L’invio di e-mail di test è un passaggio importante nella convalida della campagna e-mail e nell’identificazione dei potenziali problemi. Inviando e-mail di test, puoi controllare vari elementi come collegamenti, collegamenti di rinuncia, immagini e pagine mirror, nonché rilevare eventuali errori.

Le e-mail di test possono essere inviate a due tipi di destinatari:

* **Profili di test**: inviare e-mail di prova agli indirizzi di seed, che sono destinatari aggiuntivi e fittizi nel database,

* **Sostituzione dal target principale**: invia e-mail di test a un indirizzo e-mail specifico durante la rappresentazione di un profilo esistente. Questo ti consente di utilizzare l’e-mail come i destinatari, fornendo una rappresentazione accurata del messaggio che il profilo riceverà.

## Selezionare i destinatari del test {#recipients}

1. Accedi alla schermata di simulazione del contenuto dell’e-mail, quindi fai clic sul **[!UICONTROL Test]** pulsante .

   ![](assets/test-button.png)

1. Utilizza la **[!UICONTROL Modalità]** elenco a discesa per scegliere il tipo di destinatari che riceveranno il messaggio e-mail di test:

   * **Profili di test**: inviare l’e-mail di prova agli indirizzi di seed, che sono destinatari aggiuntivi e fittizi nel database,

   * **Sostituzione dal target principale**: invia l’e-mail di test a un indirizzo e-mail specifico durante la rappresentazione di un profilo esistente. Questo ti consente di utilizzare l’e-mail come i destinatari, fornendo una rappresentazione accurata del messaggio che il profilo riceverà.

   ![](assets/test-mode.png)

   >[!NOTE]
   >
   >Per impostazione predefinita, la **[!UICONTROL Profili di test]** modalità selezionata. Se hai già selezionato dei profili per visualizzare l’anteprima dell’e-mail nella schermata di simulazione del contenuto, questi profili vengono preselezionati come destinatari del test. Puoi deselezionare la selezione e/o aggiungere altri destinatari.

1. Per inviare e-mail di test ai profili di sostituzione, scegli la **[!UICONTROL Sostituzione dal target]** quindi segui questi passaggi:

   1. Fai clic sul pulsante **[!UICONTROL Aggiungi indirizzo]** e specifica l’indirizzo e-mail che riceverà l’e-mail di test.

      Puoi inserire qualsiasi indirizzo e-mail. Questo consente di inviare e-mail di test a qualsiasi utente, anche se non è utente di Adobe Campaign V8.

   1. Seleziona il profilo dalla destinazione da utilizzare per inviare l’e-mail di test. Puoi anche consentire ad Adobe Campaign di selezionare un profilo casuale dal target.

   1. Conferma il destinatario e ripeti l’operazione per aggiungere tutti gli indirizzi necessari.

      ![](assets/substitution.png)

1. Una volta selezionati i destinatari del test, puoi inviare l’e-mail di test. [Scopri come inviare e-mail di test](#send)

   >[!NOTE]
   >
   >Se desideri inviare il messaggio e-mail finale ai destinatari dell’e-mail di test, abilita **[!UICONTROL Includere la popolazione di test nel target principale]** su .

## Invia l’e-mail di test {#send}

Per inviare l’e-mail di test ai destinatari selezionati, fai clic su **[!UICONTROL Invia e-mail di test]** quindi conferma l’invio.

![](assets/send-proof.png)

Invia tutte le e-mail di test necessarie fino a quando non avrai finalizzato il contenuto della consegna. Al termine, puoi inviare l’e-mail al target principale. [Scopri come preparare e inviare il tuo messaggio e-mail](../monitor/prepare-send.md)

## Accedere alle e-mail di test inviate {#access-proofs}

Una volta inviate le e-mail di test, puoi accedere ai registri dedicati dal **[!UICONTROL Visualizza registro e-mail di prova]** pulsante .

Questi registri ti consentono di accedere a tutte le e-mail di test inviate per la consegna selezionata e di visualizzare statistiche specifiche correlate al loro invio. [Scopri come monitorare i registri di consegna](../monitor/delivery-logs.md)

![](assets/proof-log.png)

Puoi anche accedere alle e-mail di test inviate dall’elenco delle consegne, come qualsiasi consegna.

![](assets/delivery-list.png)
