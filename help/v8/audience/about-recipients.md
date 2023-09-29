---
title: Utilizzare destinatari e tipi di pubblico
description: Scopri come lavorare con i destinatari di Campaign Web
badge: label="Beta"
source-git-commit: 424caa898ff9d73f3520aa6d682eb1963d992069
workflow-type: tm+mt
source-wordcount: '1022'
ht-degree: 13%

---


# Utilizzare destinatari e tipi di pubblico {#about-recipients}

In Adobe Campaign, la popolazione target di una consegna è un pubblico. Un pubblico è un insieme di persone che condividono comportamenti e/o caratteristiche simili. Questa raccolta di persone può essere generata, selezionata o caricata [come descritto di seguito](#audiences). Nella maggior parte dei casi, il pubblico è costituito da profili, memorizzati come [destinatari](#recipients) in Adobe Campaign. Puoi anche lavorare con altre mappature di destinazione modificando la dimensione come spiegato [in questa sezione](#targeting-dimensions).

## Cosa sono i destinatari? {#recipients}

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Destinatari"
>abstract="Un destinatario è un profilo il cui target è la ricezione di messaggi inviati da Adobe Campaign. In Adobe Campaign, i destinatari sono i profili predefiniti target per l’invio di consegne (e-mail, SMS). Da questo elenco, puoi visualizzare il profilo del destinatario in base alle tue autorizzazioni. Utilizza le opzioni di filtro per sfogliare questo elenco. Puoi modificare e aggiornare un piccolo set di attributi del destinatario."

Un destinatario è un profilo il cui target è la ricezione di messaggi inviati da Adobe Campaign. In Adobe Campaign, i destinatari sono i profili predefiniti oggetto di targeting per l’invio di consegne (e-mail, SMS, ecc.). I dati dei destinatari memorizzati nel database consentono di creare tipi di pubblico che riceveranno una determinata consegna e di aggiungere dati di personalizzazione al contenuto della consegna. Altri tipi di profili vengono memorizzati nel database. Sono progettati per utilizzi diversi: ad esempio, i profili di seed vengono creati per testare le consegne prima che vengano inviate al pubblico finale.

I destinatari possono essere aggiunti solo dalla console client di Campaign. Tuttavia, sono visibili nel web di Campaign dalla sezione **Destinatari** ingresso della barra di navigazione a sinistra. Puoi anche modificare gli attributi del destinatario da quella schermata.

Per modificare i dati del destinatario, fai clic sui tre punti accanto al nome e scegli **Modifica...**.

![Modificare un profilo del destinatario](assets/recipient-edit.png)

Puoi aggiornare un set limitato di attributi, ovvero nome, cognome, e-mail e numero di telefono.

![Aggiornare un profilo destinatario](assets/recipient-update.png)

>[!NOTE]
>
>Questo modulo di modifica profilo limitato è disponibile solo per il test di programmi beta. Sarà migliorato nella versione futura. Consente all’utente di aggiungere rapidamente un indirizzo e-mail e un numero di telefono a qualsiasi profilo, in modo da poter testare i canali e-mail e SMS e ricevere i messaggi inviati.

Puoi filtrare i destinatari utilizzando il campo di ricerca, dalla sezione **Mostra filtri** pulsante.

Puoi anche accedere ai destinatari da **Esplora** visualizzare, sfogliare e creare cartelle e sottocartelle e verificare le autorizzazioni associate.

![Elenco destinatari dalla visualizzazione Esplora risorse](assets/recipients-from-explorer.png)

>[!NOTE]
>
>A seconda delle autorizzazioni di cui si dispone, è possibile che non si disponga dell&#39;accesso all&#39;elenco completo dei destinatari archiviati nel database. Ulteriori informazioni sulle autorizzazioni sono disponibili in [questa sezione](../get-started/permissions.md).

Inoltre, puoi gestire l’abbonamento e il suo annullamento a servizi quali le newsletter. [Scopri come utilizzare i servizi di abbonamento](manage-services.md)

Puoi creare flussi di lavoro per deduplicare, arricchire, combinare profili e creare tipi di pubblico. Per ulteriori informazioni, consulta [questa sezione](../workflows/gs-workflows.md).

## Cosa sono i tipi di pubblico? {#audiences}

Il pubblico è il target principale della consegna: i destinatari che ricevono i messaggi. Il tipo di pubblico dipende dalla mappatura target definita nel modello di consegna. [Scopri cos’è un modello di consegna](../msg/delivery-template.md).

Per definire la popolazione di un pubblico, puoi:

* [Creare nuovi tipi di pubblico](create-audience.md) dal **[!UICONTROL Tipi di pubblico]** menu,
* [Seleziona un pubblico esistente](add-audience.md) creato come elenco nella console client o proveniente da Adobe Experience Platform,
* [Crea un nuovo pubblico con il generatore di regole definendo e combinando criteri di filtro,](segment-builder.md)
* [Utilizzare un pubblico da un file esterno](file-audience.md). Questa opzione è disponibile solo per le consegne e-mail autonome e non può essere utilizzata nelle consegne delle campagne.

Quando esegui il targeting di un pubblico, puoi anche definire **gruppi di controllo** per evitare di inviare messaggi a una parte del pubblico e misurare l’impatto delle campagne. [Scopri come impostare un gruppo di controllo](control-group.md)

>[!NOTE]
>
>Quando si inviano messaggi nel contesto di un flusso di lavoro di una campagna, il pubblico viene definito in un **Creare un pubblico** attività del flusso di lavoro. In questo contesto, non puoi caricare un pubblico da un file per una consegna e-mail e il pubblico è definito solo in questa attività dedicata. Scopri come definire il pubblico della consegna in un flusso di lavoro della campagna [in questa sezione](../workflows/activities/build-audience.md)

## Dimensioni di targeting {#targeting-dimensions}

La dimensione di targeting, alias. mappatura target, è il tipo di dati gestito da un&#39;operazione. Consente di definire la popolazione target: destinatari, beneficiari del contratto, operatori, abbonati, ecc.

La dimensione di targeting di un flusso di lavoro è definita dal primo **[!UICONTROL Creare un pubblico]** e viene utilizzata in tutte le ulteriori attività fino alla fine del flusso di lavoro. Ad esempio, se esegui una query sui destinatari del database, la transizione in uscita conterrà dati di tipo destinatario e verrà trasmessa all’attività successiva.

Tieni presente che puoi cambiare la dimensione di targeting in un flusso di lavoro utilizzando una [Cambia attività dimensione](../workflows/activities/change-dimension.md). Ciò ti consente, ad esempio, di eseguire query sul database su una tabella specifica, ad esempio acquisti o abbonamenti, e quindi di modificare la dimensione di targeting in Destinatari per inviare le consegne ai destinatari corrispondenti.

Per impostazione predefinita, i modelli di consegna e-mail e SMS sono destinati a **[!UICONTROL Destinatari]**. La loro dimensione target utilizza quindi i campi del **nms:destinatario** tabella. Per le notifiche push, la dimensione di destinazione predefinita è **Applicazioni in abbonamento nms:appSubscriptionRcp**, che è collegato alla tabella dei destinatari.

Puoi anche utilizzare altre mappature di destinazione integrate nei flussi di lavoro e nelle consegne elencate di seguito:

| Nome | Utilizza per | Schema |
|---|---|---|
| Destinatari | Consegna ai destinatari (tabella dei destinatari incorporata) | nms:destinatario |
| Visitatori | Consegna ai visitatori i cui profili sono stati raccolti tramite riferimento (marketing virale) per es. | mns:visitatore |
| Abbonamenti | Consegna ai destinatari abbonati a un servizio di informazioni, ad esempio una newsletter | nms:sottoscrizione |
| Abbonamenti visitatore | Consegna ai visitatori abbonati a un servizio di informazioni | nms:visitorSub |
| Operatori | Consegna agli operatori Adobe Campaign | nms:operatore |
| File esterno | Consegna tramite un file contenente tutte le informazioni necessarie per la consegna | Nessuno schema collegato, nessuna destinazione immessa |
| Applicazioni in abbonamento | Consegna ai destinatari abbonati a un’applicazione | nms:appSubscriptionRcp |

Inoltre, puoi creare una nuova mappatura di destinazione in base alle tue esigenze. Questa operazione viene eseguita dalla console client. Ulteriori informazioni sono disponibili nella [documentazione di Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html#new-mapping){target="_blank"}.
