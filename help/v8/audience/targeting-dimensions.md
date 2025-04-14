---
title: Dimensioni di targeting
description: Ulteriori informazioni sulle dimensioni di targeting in Adobe Campaign Web
exl-id: b910649a-7300-4f99-8f40-3a8965572ee9
source-git-commit: 93a79b471c236e5bf67da0dbd0d76274598dcb0e
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 22%

---

# Dimensioni di targeting {#targeting-dimensions}

>[!CONTEXTUALHELP]
>id="acw_orchestration_build_audience_dimension"
>title="Selezionare una dimensione targeting"
>abstract="La dimensione di targeting consente di definire la popolazione target dell’operazione: destinatari, beneficiari del contratto, operatore, abbonati e altro ancora. Per impostazione predefinita, per le e-mail e gli SMS, la destinazione è selezionata dalla tabella incorporata Destinatari. Per le notifiche push, la dimensione di destinazione predefinita è Applicazioni in abbonamento."

La dimensione di targeting, nota anche come mappatura target, è il tipo di dati che un’operazione gestisce. Definisce la popolazione target, ad esempio profili, beneficiari del contratto, operatori o abbonati.

## Dimensioni di targeting dei flussi di lavoro {#workflow}

La dimensione di targeting di un flusso di lavoro è definita dalla prima attività **[!UICONTROL Genera pubblico]** e viene utilizzata in tutte le attività successive fino alla fine del flusso di lavoro. Ad esempio, quando esegui una query sui profili dal database, la transizione in uscita contiene dati di tipo &quot;destinatario&quot;, che vengono trasmessi all’attività successiva.

Cambiare la dimensione di targeting in un flusso di lavoro utilizzando [Cambia attività dimensione](../workflows/activities/change-dimension.md). Ciò consente di eseguire query sul database su una tabella specifica, ad esempio acquisti o abbonamenti, e quindi di modificare la dimensione di targeting in Destinatari per inviare le consegne ai profili corrispondenti.

Quando si seleziona una dimensione di targeting (nelle impostazioni del flusso di lavoro o in attività come **Genera pubblico**, **Riconciliazione** o **Modifica dimensione**), per impostazione predefinita viene visualizzato un elenco degli schemi comunemente utilizzati. Per visualizzare tutti gli schemi disponibili, attiva il pulsante **[!UICONTROL Mostra tutti gli schemi]**. La selezione delle opzioni viene salvata per ogni utente.

![Schermata che mostra l&#39;interfaccia della dimensione di targeting con il pulsante &quot;Mostra tutti gli schemi&quot; abilitato.](assets/targeting-dimension-show-all.png){zoomable="yes"}

## Dimensioni di targeting {#list}

Per impostazione predefinita, i modelli di consegna e-mail e SMS sono destinati ai profili. La dimensione di destinazione utilizza i campi della tabella **nms:recipient**. Per le notifiche push, la dimensione target predefinita è **Applicazioni in abbonamento nms:appSubscriptionRcp**, collegata alla tabella dei destinatari.

Utilizza altre mappature di destinazione incorporate nei flussi di lavoro e nelle consegne, come elencato di seguito:

| Nome | Utilizza per consegnare a | Schema |
|-----------------------|-------------------------------------------------------|-------------------------|
| Destinatari | Profili/destinatari (tabella dei destinatari incorporata) | nms:recipient |
| Visitatori | Visitatori i cui profili sono stati raccolti tramite riferimento (viral marketing per ex) | mns:visitor |
| Abbonamenti | Profili abbonati a un servizio di informazioni, ad esempio una newsletter | nms:subscription |
| Abbonamenti visitatore | Visitatori abbonati a un servizio di informazioni | nms:visitorSub |
| Operatori | Operatori Adobe Campaign | nms:operator |
| File esterno | Consegna tramite un file contenente tutte le informazioni richieste | Nessuno schema collegato, nessuna destinazione immessa |
| Applicazioni in abbonamento | Profili abbonati a un’applicazione | nms:appSubscriptionRcp |

Inoltre, crea nuove mappature di destinazione in base a esigenze specifiche. Esegui questa operazione solo dalla console client. Per ulteriori informazioni, consulta la [documentazione di Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html?lang=it#new-mapping){target="_blank"}.