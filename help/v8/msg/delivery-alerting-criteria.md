---
audience: end-user
title: Avvisi di consegna
description: Scopri come utilizzare gli avvisi sulla consegna.
hidefromtoc: true
hide: true
robots: noindex
googlebot: noindex
exl-id: fc98d4e3-7986-42bb-82d5-b4f874aa71db
source-git-commit: 19a7540af7502709b7eafdace038b5958e077173
workflow-type: tm+mt
source-wordcount: '712'
ht-degree: 24%

---

# Criteri per gli avvisi di consegna {#delivery-alerting-criteria}

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria"
>title="Dashboard dei criteri per gli avvisi di consegna"
>abstract="L’interfaccia utente di Campaign Web fornisce criteri di avviso predefiniti (consegne con bassa velocità, consegne la cui preparazione non è riuscita...) che puoi aggiungere alla dashboard. Puoi anche creare criteri personalizzati in base alle tue esigenze."

L’interfaccia utente di Campaign Web fornisce criteri di avviso predefiniti, ad esempio consegne con bassa velocità effettiva o consegne la cui preparazione non è riuscita, che puoi aggiungere al dashboard. Puoi anche creare criteri personalizzati in base alle tue esigenze.

I criteri di avviso sono accessibili dal menu **Avvisi di consegna** nel riquadro di navigazione a sinistra, nella scheda **Criteri**.

![Elenco dei criteri di avviso visualizzati nel menu Avvisi consegna](assets/alerting-criteria-list.png)

## Criteri di avviso predefiniti {#ootb-criteria}

Nell’interfaccia utente di Campaign Web sono disponibili criteri di avviso predefiniti. Tali criteri coprono una serie di scenari, elencati di seguito:

* **Consegne non riuscite**: qualsiasi consegna pianificata entro un intervallo definito, con uno stato errato.
* **Consegne con preparazione non riuscita**: qualsiasi consegna modificata all&#39;interno di un intervallo definito, per la quale la fase di preparazione (calcolo della destinazione e generazione del contenuto) non è riuscita.
* **Consegna con percentuale di errori non validi per mancati recapiti non permanenti**: qualsiasi consegna pianificata all&#39;interno di un intervallo definito, con uno stato di almeno &quot;In corso&quot; e un rapporto di errore per mancati recapiti non permanenti maggiore di una percentuale definita.
* **Consegna con percentuale di errori non validi per mancati recapiti permanenti**: qualsiasi consegna pianificata entro un intervallo definito, con uno stato di almeno &quot;In corso&quot; e un rapporto di errore non recapitato maggiore di una percentuale definita.
* **Consegne con inizio lungo in sospeso**: qualsiasi consegna pianificata all&#39;interno di un intervallo definito, con stato &quot;Inizio in sospeso&quot; per un periodo di tempo superiore a quello definito. Lo stato &quot;Avvio in sospeso&quot; indica che i messaggi non sono ancora stati presi in considerazione dal sistema.
* **Consegne con bassa velocità effettiva**: qualsiasi consegna iniziata per un periodo di tempo superiore a quello definito, con meno di una percentuale definita di messaggi elaborati e una velocità effettiva inferiore a un valore definito.
* **Consegne in corso**: qualsiasi consegna pianificata entro un intervallo definito, con lo stato &quot;In corso&quot;.

>[!NOTE]
>
>I valori predefiniti vengono applicati a tutti i parametri per i criteri di cui sopra. Questi valori possono essere personalizzati nella sezione **Parametri dei criteri** dei dashboard di avviso sulla consegna in cui vengono utilizzati. [Scopri come utilizzare i dashboard](../msg/delivery-alerting-dashboards.md)

## Creare un criterio di avviso {#criteria}

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create"
>title="Crea criteri per gli avvisi di consegna"
>abstract="Oltre ai criteri di avviso predefiniti forniti da Adobe Campaign, puoi creare criteri personalizzati in base alle tue esigenze."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_indicators"
>title="Indicatori da aggiungere negli avvisi"
>abstract="Seleziona gli indicatori da visualizzare come colonne nella sezione “Dettagli” degli avvisi e-mail."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_alert"
>title="Tipo di avviso"
>abstract="Specifica il **Tipo di avviso** per il criterio, ovvero l’etichetta e il colore da mostrare accanto al criterio di consegna nella sezione “Riepilogo” degli avvisi."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_frequency"
>title="Frequenza criterio"
>abstract="Controlla la frequenza giornaliera degli avvisi per ogni consegna che soddisfa il criterio."

Per creare un nuovo criterio, effettua le seguenti operazioni:

1. Passa al menu **Avvisi di consegna** nel riquadro di navigazione a sinistra e seleziona la scheda **Criteri**.
1. Fai clic sul pulsante **Crea criteri di avviso consegna**.
1. Fornisci un’etichetta per il criterio. Il nome interno viene popolato automaticamente e di sola lettura.
1. Utilizza il filtro di consegna **applicato da questo criterio** per perfezionare l&#39;ambito del criterio applicando a esso un filtro predefinito.

   Nell&#39;esempio seguente, il filtro **Consegne in corso (critInProgressDeliveries)** è stato selezionato, il che significa che il criterio prende in considerazione solo le consegne con lo stato &quot;In corso&quot;.

   ![Esempio di proprietà dei criteri di avviso con il filtro selezionato](assets/alerting-criteria-properties.png)

   >[!NOTE]
   >
   >Se nessuno dei filtri predefiniti soddisfa le tue esigenze, puoi crearne di personalizzati dal menu **Gestione clienti** > **Filtri predefiniti**. [Ulteriori informazioni](../get-started/predefined-filters.md)
   >
   >Questa operazione deve essere eseguita solo da utenti esperti.

1. Nella sezione **Indicatori da aggiungere negli avvisi**, scegli gli indicatori da visualizzare come colonne nella sezione &quot;Dettagli&quot; degli avvisi e-mail.

1. Specifica il **Tipo di avviso** per il criterio, ovvero l’etichetta e il colore da mostrare accanto al criterio di consegna nella sezione “Riepilogo” degli avvisi.

1. Utilizza la sezione **Frequenza criteri** per controllare la frequenza giornaliera degli avvisi per ogni consegna che soddisfa il criterio:

   * **Questo criterio di consegna verrà ripetuto in ogni notifica**: visualizza una consegna che soddisfa il criterio in ogni avviso e-mail della giornata.
   * **Questo criterio di consegna viene inviato solo alla prima occorrenza del giorno**: visualizza una consegna che soddisfa il criterio solo nel primo rapporto del giorno, senza ripeterla negli avvisi e-mail successivi.