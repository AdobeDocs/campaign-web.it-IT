---
title: Utilizzare destinatari e tipi di pubblico
description: Scopri come utilizzare i destinatari e i tipi di pubblico in Campaign Web
badge: label="Beta"
exl-id: 71a1ec92-cd79-4654-9ae3-9a92a01c6279
source-git-commit: 5183dd0045c7f13e79f65eca5b31dfd4cde2f31d
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 93%

---

# Utilizzare destinatari e tipi di pubblico {#about-recipients}

## Destinatari e pubblico {#about}

In Adobe Campaign, la popolazione target di una consegna è un “pubblico”. Un pubblico è un insieme di persone che condividono comportamenti e/o caratteristiche simili. Questa raccolta di persone può essere generata, selezionata o caricata [come descritto di seguito](#audiences).

Nella maggior parte dei casi, il pubblico è costituito da profili, memorizzati come [destinatari](#recipients) in Adobe Campaign. Puoi anche lavorare con altre mappature target modificando la dimensione come spiegato [in questa sezione](#targeting-dimensions).

## Dimensioni di targeting {#targeting-dimensions}

La dimensione targeting, detta anche mappatura target, è il tipo di dati gestito da un’operazione. Consente di definire la popolazione target: destinatari, beneficiari del contratto, operatori, abbonati, ecc.

La dimensione targeting di un flusso di lavoro è definita dalla prima attività **[!UICONTROL Crea pubblico]** e viene utilizzata in tutte le ulteriori attività fino alla fine del flusso di lavoro. Ad esempio, se esegui una query sui destinatari del database, la transizione in uscita conterrà dati di tipo destinatario e verrà trasmessa all’attività successiva.

Tieni presente che puoi cambiare la dimensione targeting in un flusso di lavoro utilizzando un’attività [Cambia dimensione](../workflows/activities/change-dimension.md). In questo modo, ad esempio, puoi eseguire query sul database per una tabella specifica, come acquisti o abbonamenti, e quindi cambiare la dimensione targeting in Destinatari per inviare le consegne ai destinatari corrispondenti.

Per impostazione predefinita, i modelli di consegna e-mail e SMS hanno come target i **[!UICONTROL Destinatari]**. La loro dimensione target utilizza quindi i campi della tabella **nms:recipient**. Per le notifiche push, la dimensione target predefinita è **Applicazioni in abbonamento nms:appSubscriptionRcp**, collegata alla tabella dei destinatari.

Puoi anche utilizzare altre mappature target integrate nei flussi di lavoro e nelle consegne, elencate di seguito:

| Nome | Utilizza per | Schema |
|---|---|---|
| Destinatari | Consegnare ai destinatari (tabella dei destinatari incorporata) | nms:recipient |
| Visitatori | Consegnare ai visitatori i cui profili sono stati raccolti tramite riferimento (marketing virale) per es. | mns:visitor |
| Abbonamenti | Consegnare ai destinatari abbonati o iscritti a un servizio informativo, ad esempio una newsletter | nms:subscription |
| Abbonamenti visitatore | Consegnare ai visitatori abbonati o iscritti a un servizio informativo | nms:visitorSub |
| Operatori | Consegnare agli operatori Adobe Campaign | nms:operator |
| File esterno | Consegnare tramite un file contenente tutte le informazioni necessarie per la consegna | Nessuno schema collegato, nessuna destinazione immessa |
| Applicazioni in abbonamento | Consegnare ai destinatari abbonati o iscritti a un’applicazione | nms:appSubscriptionRcp |

Inoltre, puoi creare una nuova mappatura target in base alle tue esigenze. Questa operazione viene eseguita dalla console client. Per ulteriori informazioni, consulta la [documentazione di Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html?lang=it#new-mapping){target="_blank"}
