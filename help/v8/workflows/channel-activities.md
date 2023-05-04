---
audience: end-user
title: Utilizzare le attività del canale nei flussi di lavoro
description: Scopri come utilizzare le attività del canale nei flussi di lavoro di Adobe Campaign Web
badge: label="Alpha" type="Positive"
exl-id: 6f9be348-6138-470c-8c40-750dc0311424
source-git-commit: dd006d1e161dec49d9a1a6bcb8cb67503178479b
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 26%

---

# Attività del canale {#channel}

Adobe Campaign Web consente di automatizzare ed eseguire campagne di marketing su più canali, come e-mail, SMS o push. Con i flussi di lavoro Adobe Campaign, puoi combinare le attività dei canali nell’area di lavoro per creare flussi di lavoro cross-channel che possono attivare azioni in base al comportamento dei clienti.

Ad esempio, puoi creare una campagna e-mail di benvenuto che include una serie di messaggi tra diversi canali, come e-mail, SMS e push. Puoi anche inviare un’e-mail di follow-up dopo che un cliente ha completato un acquisto o inviare un messaggio di compleanno personalizzato a un cliente tramite SMS.

Utilizzando le attività dei canali, puoi creare campagne complete e personalizzate che coinvolgono i clienti su più punti di contatto e stimolano le conversioni.

Le attività Canale sono disponibili nella palette a sinistra dello schermo, nella sezione Canali .

## E-mail {#email}

descrizione, quale caso d’uso si può eseguire (altre attività comuni che si possono collegare prima o dopo l’attività)

come aggiungere e configurare l’attività

esempio di attività configurata all’interno di un flusso di lavoro


L’attività Email delivery ti consente di configurare l’invio di un’e-mail in un flusso di lavoro.

<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.-->

I destinatari delle e-mail sono definiti a monte dell’attività nello stesso flusso di lavoro, tramite un’attività di targeting del pubblico.

<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->