---
audience: end-user
title: Utilizzare le attività di dei flussi di lavoro
description: Scopri come eseguire le attività del flusso di lavoro
badge: label="Alpha" type="Positive"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: ec569f7d5acc06a027416794c056328d5fce1567
workflow-type: tm+mt
source-wordcount: '853'
ht-degree: 80%

---


# Attività dei flussi di lavoro {#workflow-activities}

## Attività di targeting {#targeting}

Queste attività consentono di creare uno o più target definendo dei set e suddividendo o combinando tali set mediante le operazioni di intersezione, unione o esclusione.

### Creazione del pubblico {#build-audience}

Questa attività ti consente di definire un pubblico. Puoi selezionare un pubblico esistente di Campaign oppure utilizzare il generatore di regole per definire una query personalizzata.

Il **Creare un pubblico** L’attività può essere inserita all’inizio del flusso di lavoro o dopo qualsiasi altra attività. Qualsiasi attività può essere inserita dopo il **Creare un pubblico**.

Per creare una query personalizzata:

1. Seleziona **Crea il tuo (query)**.
1. Scegli la **Dimensione targeting**. La dimensione targeting consente di definire la popolazione target dell’operazione: destinatari, beneficiari del contratto, operatore, abbonati, ecc. Per impostazione predefinita, il target viene selezionato dai destinatari. Consulta la sezione [Documentazione di v8](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/wf-type/targeting-workflows.html#targeting-and-filtering-dimensions){target="_blank"}.
1. Clic **Continua**.
1. Utilizza il generatore di regole per definire la query, nello stesso modo in cui crei un pubblico durante la progettazione di una nuova e-mail. Fai riferimento a questa [sezione](../audience/segment-builder.md).

Per selezionare un pubblico esistente:

1. Seleziona **Read audience**.
1. Clic **Continua**.
1. Seleziona il pubblico nello stesso modo in cui utilizzi un pubblico durante la progettazione di una nuova e-mail. Fai riferimento a questa [sezione](../audience/add-audience.md).

### Combina {#combine}

Il **Combina** L’attività può essere inserita dopo qualsiasi altra attività, ma non all’inizio del flusso di lavoro. Qualsiasi attività può essere inserita dopo il **Combina**.

### Arricchimento {#enrichment}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_data"
>title="Attività di arricchimento"
>abstract="L’attività di arricchimento consente di migliorare i dati di destinazione con informazioni aggiuntive provenienti dal database. Viene comunemente utilizzata in un flusso di lavoro dopo le attività di targeting.<br/>Una volta aggiunti al flusso di lavoro, i dati di arricchimento possono essere utilizzati nelle attività aggiunte dopo l’attività di arricchimento per segmentare i clienti in gruppi distinti in base ai loro comportamenti, preferenze e esigenze, o per creare messaggi e campagne di marketing personalizzati che hanno maggiori probabilità di risonanza nel pubblico di destinazione."

L’attività di arricchimento consente di migliorare i dati di destinazione con informazioni aggiuntive provenienti dal database. Viene comunemente utilizzata in un flusso di lavoro dopo le attività di targeting.

I dati di arricchimento possono provenire:

* **Dalla stessa tabella di lavoro** come quella che è stata inserita nel flusso di lavoro:

   *Eseguire il targeting di un gruppo di clienti e aggiungere il campo “Data di nascita” alla tabella di lavoro corrente*

* **Da un’altra tabella di lavoro**:

   *Eseguire il targeting di un gruppo di clienti e aggiungere i campi “Importo” e “Tipo di prodotto” provenienti dalla tabella “Acquisto”*.

Una volta aggiunti al flusso di lavoro, i dati di arricchimento possono essere utilizzati nelle attività aggiunte dopo l’attività di arricchimento per segmentare i clienti in gruppi distinti in base ai loro comportamenti, preferenze e esigenze, o per creare messaggi e campagne di marketing personalizzati che hanno maggiori probabilità di risonanza nel pubblico di destinazione.

Ad esempio, è possibile aggiungere alla tabella di lavoro del flusso di lavoro le informazioni relative agli acquisti dei clienti e utilizzare questi dati per personalizzare le e-mail con il loro acquisto più recente o con l’importo speso per tali acquisti.

Per aggiungere un’attività di arricchimento nel flusso di lavoro, segui i passaggi seguenti:

1. aggiungi attività
1. seleziona l’attributo da utilizzare come dato di arricchimento

   visualizza opzione campi avanzati
pulsante

   nota: attributi dalla dimensione di destinazione

1. Seleziona la modalità di raccolta dei dati
1. numero di record da recuperare se si desidera recuperare una raccolta di più record
1. Applica filtri e crea regole

   seleziona un filtro esistente
salva filtro per riutilizzo
visualizza risultati del filtro visivamente o in vista codice

1. ordina i record utilizzando un attributo

riutilizza i dati di arricchimento nella campagna

dove si possono utilizzare i dati di arricchimento: personalizzazione e-mail, altri casi d’uso?


## Attività del canale {#channel}

Adobe Campaign Web consente di automatizzare ed eseguire campagne di marketing su più canali, come e-mail, SMS o push. Con i flussi di lavoro Adobe Campaign, puoi combinare le attività dei canali nell’area di lavoro per creare flussi di lavoro cross-channel che possono attivare azioni in base al comportamento dei clienti.

Ad esempio, puoi creare una campagna e-mail di benvenuto che include una serie di messaggi su diversi canali, come e-mail, SMS e push. Puoi anche inviare un’e-mail di follow-up dopo che un cliente ha completato un acquisto o inviare un messaggio di auguri di compleanno personalizzato a un cliente tramite SMS.

Utilizzando le attività dei canali, puoi creare campagne complete e personalizzate che coinvolgono i clienti su più punti di contatto e danno impulso alle conversioni.

Le attività dei canali sono disponibili nella palette a sinistra dello schermo, nella sezione Canali.

### E-mail {#email}

descrizione, quale caso d’uso si può eseguire (altre attività comuni che si possono collegare prima o dopo l’attività)

come aggiungere e configurare l’attività

esempio di attività configurata all’interno di un flusso di lavoro


L’attività Consegna e-mail ti consente di configurare l’invio di un’e-mail in un flusso di lavoro.

<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.-->

I destinatari delle e-mail sono definiti a monte dell’attività nello stesso flusso di lavoro, tramite un’attività di targeting del pubblico.

<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->


### SMS {#sms}

### Notifica push (Android) {#push-android}

### Notifica push (iOS) {#push-ios}

## Attività di controllo del flusso {#flow-control}

contenuto da definire

<!--à reformuler-->Queste attività consentono di creare uno o più target definendo dei set e suddividendo o combinando tali set mediante le operazioni di intersezione, unione o esclusione.

Le attività di controllo del flusso vengono utilizzate per coordinare le attività del flusso di lavoro.

### Attività Fork {#fork}

### Attività AND-join {#join}


### Attività Wait {#wait}

### Fine {#end}

## Attività di gestione dati {#data-management}

panoramica: a cosa servono
quali casi d’uso si possono utilizzare con essi

elenco delle attività disponibili + descrizione breve + riferimento alla sezione

