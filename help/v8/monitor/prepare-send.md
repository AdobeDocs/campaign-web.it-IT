---
audience: end-user
title: Preparare e inviare un messaggio e-mail
description: Scopri come preparare e inviare un’e-mail con l’interfaccia utente web di Campaign
exl-id: 80c16d2d-2a31-48f1-a161-ee574ec24172
source-git-commit: a59c133254632c49618fae6ad3d61a2f6e0a1eea
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 4%

---

# Prepara e invia il tuo messaggio e-mail {#prepare-send}

![](../assets/do-not-localize/badge.png)

>[!CONTEXTUALHELP]
>id="acw_homepage_card5"
>title="Prepara e invia il tuo messaggio e-mail"
>abstract="Scopri come preparare il tuo messaggio e-mail e ulteriori informazioni sull’invio di KPI."

<!--

	show how to prepare and send the email + the live kpis in the dashboard

like acc when preparation, target calculated then send
real time KPIs, not in AJO. similar to ACS.
exclusion logs, causes
-->

<!--
send also KPIs
-->

## Preparare l’invio{#prepare}

Una volta definiti il contenuto, il pubblico e la pianificazione, puoi preparare il messaggio. Durante la preparazione, la popolazione target viene calcolata e il contenuto del messaggio generato per ciascun profilo incluso nel target. Al termine della preparazione, i messaggi sono pronti per essere inviati, immediatamente o alla data e all’ora pianificate. Le regole di convalida utilizzate durante l&#39;analisi sono descritte nella sezione [Documentazione di Campaign Classic v7](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/key-steps-when-creating-a-delivery/steps-validating-the-delivery.html#validation-process-with-typologies){target="_blank"}.

Segui i passaggi seguenti:

1. Dal dashboard di consegna, fai clic su **Preparare** nell’angolo in alto a destra e conferma.

   ![](assets/prepare.png)

   Viene visualizzato l’avanzamento della preparazione. A seconda della dimensione della popolazione target, questa operazione potrebbe richiedere del tempo.

   >[!NOTE]
   >
   >Puoi interrompere la preparazione in qualsiasi momento utilizzando la **Arresta preparazione** pulsante . Durante la fase di preparazione, non vengono inviati messaggi. È quindi possibile iniziare o interrompere questo processo senza rischi di influire su nulla.

1. Al termine della preparazione, controlla i KPI. Se il numero di messaggi da inviare non corrisponde alle tue aspettative, modifica il pubblico e riavvia la preparazione.

   ![](assets/prepare2.png)

   Di seguito sono riportati i diversi KPI visualizzati:

   * **Target**: il numero di destinatari
   * **Per fornire**: il numero di messaggi che verranno inviati
   * **Per escludere**: il numero di messaggi esclusi da una regola di tipologia

1. Fai clic sul pulsante **Registri** e controlla che non vi siano errori. Nell’ultimo messaggio di log vengono visualizzati tutti i messaggi di errore e il numero di errori. Per ulteriori informazioni, consulta questa [sezione](delivery-logs.md).

   ![](assets/prepare-logs.png)

Se la preparazione rileva un errore critico che impedisce l’invio della consegna, lo stato di preparazione viene visualizzato come non riuscito nel dashboard di consegna.

![](assets/prepare-error.png)

Per apportare eventuali modifiche alla consegna dopo la preparazione, è necessario riavviare la preparazione per tenere conto di tali modifiche.

Una volta completata la preparazione senza errori, il messaggio è pronto per essere inviato. Per ulteriori informazioni, consulta questa [sezione](#send).

## Invia il messaggio{#send}

Una volta completata la preparazione, puoi inviare il messaggio. Questo passaggio è necessario solo per i messaggi inviati immediatamente. Se il messaggio è pianificato, viene inviato alla data definita.

Segui questi passaggi:

1. Dal dashboard di consegna, fai clic su **Invia** nell’angolo in alto a destra e conferma.

   ![](assets/send.png)

1. Viene visualizzato l’avanzamento dell’invio. Controlla i KPI visualizzati. Puoi anche controllare i registri. Per ulteriori informazioni, consulta questa [sezione](delivery-logs.md).

   ![](assets/send2.png)

   Di seguito sono riportati i diversi KPI visualizzati:

   * **Consegnato**: numero di messaggi recapitati correttamente. La percentuale visualizzata si basa sul numero totale di messaggi inviati.
   * **Aperture**: il numero di messaggi aperti. La percentuale visualizzata è il rapporto tra il numero di aperture distinte e il numero di messaggi consegnati.
   * **Clic**: il numero di destinatari che hanno fatto clic almeno una volta nell’e-mail. La percentuale visualizzata è il rapporto tra il numero di clic distinti e il numero di messaggi consegnati.

   >[!NOTE]
   >
   >La **Aperture** e **Clic** Gli indicatori saranno aggiornati dopo 5 minuti.

   Puoi sospendere l’invio in qualsiasi momento e quindi riprendere. Se interrompi la consegna durante l’invio, non potrai riprendere.
