---
audience: end-user
title: Invia bozze
description: Documentazione Web di Campaign v8
exl-id: b2677579-c95d-443d-b207-466af364c208
source-git-commit: 28cada1d6b645bd6f0c365528c9302bf4b03ad65
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 2%

---

# Invia bozze {#send-proofs}

>[!NOTE]
>
>Questa documentazione è in fase di costruzione e viene aggiornata frequentemente. La versione finale di questo contenuto sarà pronta a gennaio 2023.

L’invio di bozze consente di convalidare l’e-mail e controllare vari elementi come collegamenti, collegamenti di rinuncia e pagine mirror, immagini e rilevare eventuali errori.

Le bozze possono essere inviate a due tipi di destinatari:

* **Profili di test/pubblico**: inviare bozze agli indirizzi di seed, che sono destinatari aggiuntivi nel database che non fanno parte della destinazione dell’e-mail,

* **Profili sostitutivi**: invia bozze a un indirizzo e-mail specifico utilizzando un profilo esistente. Questo ti consente di collocarti nella posizione dei profili e di ottenere una rappresentazione esatta del messaggio che il profilo riceverà.

## Selezionare i destinatari delle bozze {#recipients}

1. Accedi alla schermata di creazione del contenuto dell’e-mail, quindi fai clic su **[!UICONTROL Simulazione del contenuto]**.

1. Fai clic sul pulsante **[!UICONTROL Test]** quindi utilizzare il pulsante **[!UICONTROL Modalità]** elenco a discesa per scegliere il tipo di destinatari che riceveranno le bozze:

<!-- to check: by default, profiles selected in previous screen are pre-selected for proofs. Can add addtitional profiles + remove preselected?-->

### Inviare bozze ai profili di test

1. Scegli la **[!UICONTROL Utilizzare i profili di test]** modalità.

1. Aggiungi i profili di test che riceveranno le e-mail di test.

   Puoi anche creare un pubblico per selezionare i profili di test in base ai tuoi criteri, utilizzando **[!UICONTROL Aggiungi pubblico di test]** pulsante .

   ![](assets/test-profiles-audience.png)

### Inviare bozze ai profili di sostituzione

1. Scegli la **[!UICONTROL Sostituzione dal target]** modalità.

1. Aggiungi gli indirizzi e-mail che riceveranno le bozze.

   >[!NOTE]
   >
   >Puoi specificare qualsiasi indirizzo e-mail. Questo consente di inviare bozze a qualsiasi utente, anche se non è utente di Adobe Campaign V8.

1. Per ogni indirizzo e-mail, seleziona il profilo dalla destinazione da utilizzare. Puoi anche consentire ad Adobe Campaign di selezionare un profilo casuale dal target.

   ![](assets/substitution.png)

Una volta selezionati i destinatari della bozza, puoi inviare l’e-mail di test. [Scopri come inviare bozze](#send)

>[!NOTE]
>
>Se desideri inviare il messaggio e-mail finale ai destinatari delle bozze, abilita la **[!UICONTROL Includere la popolazione di test nel target principale]** su .

## Invia le bozze {#send}

Per inviare le bozze ai destinatari selezionati, fai clic su **[!UICONTROL Invia e-mail di test]** quindi conferma l’invio.

![](assets/send-proof.png)

Una volta inviate le bozze, puoi accedere ai registri dedicati dal **[!UICONTROL Visualizza registro e-mail di prova]** pulsante . Questi registri ti consentono di accedere alle bozze inviate e alle statistiche specifiche relative all’invio della bozza.

![](assets/proof-log.png)

Invia tutte le bozze necessarie fino a quando non avrai finalizzato il contenuto della consegna. Al termine, puoi inviare l’e-mail al target principale. [Scopri come preparare e inviare il tuo messaggio e-mail](../monitor/prepare-send.md)
