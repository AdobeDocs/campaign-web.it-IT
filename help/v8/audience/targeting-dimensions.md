---
title: Dimensioni di targeting
description: Ulteriori informazioni sulle dimensioni di targeting in Adobe Campaign Web
badge: label="Disponibilità limitata"
source-git-commit: 9fd523a04ac4bfb2d760202b1f7e9bd9e7097dfe
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 71%

---

# Dimensioni di targeting {#targeting-dimensions}

La dimensione targeting, detta anche mappatura target, è il tipo di dati gestito da un’operazione. Consente di definire la popolazione target: profili, beneficiari del contratto, operatori, abbonati, ecc.

La dimensione targeting di un flusso di lavoro è definita dalla prima attività **[!UICONTROL Crea pubblico]** e viene utilizzata in tutte le ulteriori attività fino alla fine del flusso di lavoro. Ad esempio, se esegui una query sui profili dal database, la transizione in uscita conterrà dati di tipo &quot;destinatario&quot; e verrà trasmessa all’attività successiva.

Tieni presente che puoi cambiare la dimensione targeting in un flusso di lavoro utilizzando un’attività [Cambia dimensione](../workflows/activities/change-dimension.md). Ciò ti consente, ad esempio, di eseguire query sul database su una tabella specifica, ad esempio acquisti o abbonamenti, e quindi di modificare la dimensione di targeting in Destinatari per inviare le consegne ai profili corrispondenti.

Per impostazione predefinita, i modelli di consegna e-mail e SMS sono destinati ai profili. La loro dimensione target utilizza quindi i campi della tabella **nms:recipient**. Per le notifiche push, la dimensione target predefinita è **Applicazioni in abbonamento nms:appSubscriptionRcp**, collegata alla tabella dei destinatari.

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