---
audience: end-user
title: Preparare e inviare un messaggio e-mail
description: Documentazione Web di Campaign v8
source-git-commit: fe06419e429f48dbcc71802c372130be22e68d52
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 2%

---

# Prepara e invia il tuo messaggio e-mail {#prepare-send}

>[!CONTEXTUALHELP]
>id="acw_homepage_card5"
>title="Prepara e invia il tuo messaggio e-mail"
>abstract="Scopri come preparare il tuo messaggio e-mail e ulteriori informazioni sull’invio di KPI."

>[!NOTE]
>
>Questa documentazione è in fase di costruzione e viene aggiornata frequentemente. La versione finale di questo contenuto sarà pronta a gennaio 2023.

<!--

	show how to prepare and send the email + the live kpis in the dashboard

like acc when preparation, target calculated then send
real time KPIs, not in AJO. similar to ACS.
exclusion logs, causes
-->

<!--
send also KPIs
-->

## Preparare l’invio

Durante la preparazione, la popolazione target viene calcolata e il contenuto del messaggio generato per ciascun profilo incluso nel target. Al termine della preparazione, i messaggi sono pronti per essere inviati, immediatamente o alla data e all’ora pianificate. Le regole di convalida utilizzate durante l&#39;analisi sono descritte in questo [sezione](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/key-steps-when-creating-a-delivery/steps-validating-the-delivery.html?lang=en#validation-process-with-typologies).

1. Fai clic sul pulsante **Preparare** nell&#39;angolo in alto a destra.

1. Viene visualizzato l’avanzamento della preparazione. A seconda della dimensione della popolazione target, questa operazione potrebbe richiedere del tempo.

   >[!NOTE]
   >
   >Puoi interrompere la preparazione in qualsiasi momento utilizzando la **Arresta preparazione** pulsante . Durante la fase di preparazione, non vengono inviati messaggi. È quindi possibile iniziare o interrompere questo processo senza rischi di influire su nulla.

1. Al termine della preparazione, controlla il **Target**, **Per fornire** e **Per escludere** KPI. Se il numero di messaggi da inviare non corrisponde alle tue aspettative, modifica il pubblico e riavvia la preparazione.

1. Fai clic sul pulsante **Registri** e controlla che non vi siano errori. Vengono elencati tutti i passaggi, gli avvisi e gli errori di convalida. Le icone colorate mostrano il tipo di messaggio:

   * L’icona grigia indica un messaggio informativo.
   * L’icona gialla indica un errore di elaborazione non critico.
   * L’icona rossa indica un errore critico che impedisce l’invio della consegna.

1. Dopo aver apportato le modifiche, riavvia la preparazione.

Una volta completata la preparazione, il messaggio è pronto per essere inviato. Per ulteriori informazioni, consulta Conferma dell’invio.


## Invia il messaggio

Al termine della preparazione, segui i passaggi seguenti per inviare il messaggio.

1. Fai clic sul pulsante **Pulsante Invia** nell’angolo in alto a destra e conferma.

1. L’avanzamento dell’invio viene visualizzato insieme a tre KPI: Consegnato, Aperture, Clic.

1. Per completare l’invio, fai clic sul pulsante OK .

REGISTRI

>[!NOTE]
>
>Se il messaggio è pianificato, viene inviato al raggiungimento dell’orario di invio. Per ulteriori informazioni sulla pianificazione dei messaggi, consulta questa sezione.

