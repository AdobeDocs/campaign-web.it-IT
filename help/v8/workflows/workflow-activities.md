---
audience: end-user
title: Utilizzare le attività di dei flussi di lavoro
description: Scopri come eseguire le attività del flusso di lavoro
badge: label="Alpha" type="Positive"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: 38db8be3319c348d3afc6af02a65dce582e3cc97
workflow-type: tm+mt
source-wordcount: '1122'
ht-degree: 67%

---


# Attività dei flussi di lavoro {#workflow-activities}

## Attività di targeting {#targeting}

Queste attività consentono di creare uno o più target definendo dei set e suddividendo o combinando tali set mediante le operazioni di intersezione, unione o esclusione.

### Creazione del pubblico {#build-audience}

Questa attività ti consente di definire un pubblico. Puoi selezionare un pubblico esistente di Campaign oppure utilizzare il generatore di regole per definire una query personalizzata.

<!--
The **Build audience** activity can be placed at the beginning of the workflow or after any other activity. Any activity can be placed after the **Build audience**.
-->

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

Questa attività ti consente di elaborare i set sui dati in entrata. Puoi quindi combinare più popolazioni, escluderne parte o mantenere i dati comuni a più destinazioni. Di seguito sono riportati i tipi di segmentazione disponibili:

<!--
The **Combine** activity can be placed after any other activity, but not at the beginning of the workflow. Any activity can be placed after the **Combine**.
-->

* Il **Union** consente di raggruppare il risultato di più attività in un unico target.
* Il **Intersezione** consente di mantenere solo gli elementi comuni alle diverse popolazioni in entrata nell’attività.
* Il **Esclusione** consente di escludere elementi da una popolazione in base a determinati criteri.

Per configurare il **Combina** attività:

1. Aggiungi il **Combina** a una delle transizioni di segmentazione precedenti.
1. Seleziona il tipo di segmentazione: unione, intersezione o esclusione.
1. Clic **Continua**.
1. In **Set da unire** , controlla tutte le attività precedenti a cui desideri partecipare.

Per **Union**, effettua le seguenti operazioni:

1. Seleziona il tipo di riconciliazione per definire la modalità di gestione dei duplicati:
   * Solo tasti: questa è la modalità predefinita. L’attività mantiene un solo elemento quando gli elementi delle diverse transizioni in entrata hanno la stessa chiave. È possibile utilizzare questa opzione solo se le popolazioni in entrata sono omogenee.
   * Una selezione di colonne: seleziona questa opzione per definire l’elenco di colonne alle quali viene applicata la riconciliazione dei dati. Devi innanzitutto selezionare il set principale (quello contenente i dati di origine), quindi le colonne da utilizzare per il join.

Per **Intersezione** segui questi passaggi:

1. Seleziona il tipo di riconciliazione per definire la modalità di gestione dei duplicati. Consulta la sezione **Union** sopra.
1. Seleziona l’opzione Genera completamento.

Per **Esclusione**, effettua le seguenti operazioni:

1. In **Set da unire** , seleziona la sezione **Set primario** dalle transizioni in entrata. Questo è il set da cui gli elementi sono esclusi. Gli altri set confrontano gli elementi prima che vengano esclusi dal set primario.
1. Seleziona l’opzione Genera completamento.












Intersection: consente di mantenere solo gli elementi comuni alle diverse popolazioni in entrata nell’attività.

Esclusione: consente di escludere elementi da una popolazione in base a determinati criteri.

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

