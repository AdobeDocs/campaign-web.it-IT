---
title: Dimensioni di targeting
description: Ulteriori informazioni sulle dimensioni di targeting in Adobe Campaign Web
exl-id: b910649a-7300-4f99-8f40-3a8965572ee9
source-git-commit: 3879f217f3a6a1cae0d6c924733d2ef1fd4ab9e7
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 51%

---

# Dimensioni di targeting {#targeting-dimensions}

>[!CONTEXTUALHELP]
>id="acw_orchestration_build_audience_dimension"
>title="Selezionare una dimensione targeting"
>abstract="La dimensione targeting consente di definire la popolazione target dell’operazione: destinatari, beneficiari del contratto, operatore, iscritti, ecc. Per impostazione predefinita, per le e-mail e gli SMS, la destinazione è selezionata dalla tabella incorporata Destinatari. Per le notifiche push, la dimensione di destinazione predefinita è Applicazioni in abbonamento."

La dimensione targeting, detta anche mappatura target, è il tipo di dati gestito da un’operazione. Consente di definire la popolazione target: profili, beneficiari del contratto, operatori, abbonati, ecc.

## Dimensioni di targeting dei flussi di lavoro {#workflow}

La dimensione targeting di un flusso di lavoro è definita dalla prima attività **[!UICONTROL Crea pubblico]** e viene utilizzata in tutte le ulteriori attività fino alla fine del flusso di lavoro. Ad esempio, se esegui una query sui profili dal database, la transizione in uscita conterrà dati di tipo &quot;destinatario&quot; e verrà trasmessa all’attività successiva.

Tieni presente che puoi cambiare la dimensione targeting in un flusso di lavoro utilizzando un’attività [Cambia dimensione](../workflows/activities/change-dimension.md). Ciò ti consente, ad esempio, di eseguire query sul database su una tabella specifica, ad esempio acquisti o abbonamenti, e quindi di modificare la dimensione di targeting in Destinatari per inviare le consegne ai profili corrispondenti.

Durante la selezione di una dimensione di targeting (nelle impostazioni del flusso di lavoro o in attività come **Creare un pubblico**, **Reconciliation** o **Cambia dimensione**), nell’elenco viene visualizzata per impostazione predefinita una selezione di schemi comunemente utilizzati. Per visualizzare tutti gli schemi disponibili, attiva **[!UICONTROL Mostra tutti gli schemi]** pulsante. La selezione delle opzioni viene salvata per ogni utente.

![](assets/targeting-dimension-show-all.png){zoomable=&quot;yes&quot;}

## Dimensioni di targeting {#list}

Per impostazione predefinita, i modelli di consegna e-mail e SMS sono destinati ai profili. La loro dimensione target utilizza quindi i campi della tabella **nms:recipient**. Per le notifiche push, la dimensione target predefinita è **Applicazioni in abbonamento nms:appSubscriptionRcp**, collegata alla tabella dei destinatari.

Puoi anche utilizzare altre mappature target integrate nei flussi di lavoro e nelle consegne, elencate di seguito:

| Nome | Utilizza per | Schema |
|---|---|---|
| Destinatari | Consegna a profili/destinatari (tabella dei destinatari incorporata) | nms:recipient |
| Visitatori | Consegnare ai visitatori i cui profili sono stati raccolti tramite riferimento (marketing virale) per es. | mns:visitor |
| Abbonamenti | Distribuisci ai profili abbonati a un servizio di informazioni, ad esempio una newsletter | nms:subscription |
| Abbonamenti visitatore | Consegnare ai visitatori abbonati o iscritti a un servizio informativo | nms:visitorSub |
| Operatori | Consegnare agli operatori Adobe Campaign | nms:operator |
| File esterno | Consegnare tramite un file contenente tutte le informazioni necessarie per la consegna | Nessuno schema collegato, nessuna destinazione immessa |
| Applicazioni in abbonamento | Consegna ai profili abbonati a un’applicazione | nms:appSubscriptionRcp |

Inoltre, puoi creare una nuova mappatura target in base alle tue esigenze. Questa operazione viene eseguita solo dalla console client. Per ulteriori informazioni, consulta la [documentazione di Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html?lang=it#new-mapping){target="_blank"}.
