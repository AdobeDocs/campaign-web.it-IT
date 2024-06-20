---
audience: end-user
title: Avvisi di consegna
description: Scopri come utilizzare gli avvisi sulla consegna.
source-git-commit: 8c7893dfaa394158ba98172b4025e05e4ab3343c
workflow-type: tm+mt
source-wordcount: '1050'
ht-degree: 2%

---

# Dashboard di avvisi sulla consegna {#delivery-alerting-dashboards}

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_dashboards"
>title="Dashboard di avvisi sulla consegna"
>abstract="Avvisi di consegna è un sistema di gestione degli avvisi che consente ai gruppi di utenti di ricevere automaticamente le notifiche e-mail con le informazioni sulle esecuzioni della consegna. Le dashboard di avviso di consegna ti consentono di specificare chi riceverà gli avvisi e-mail, scegliere e configurare i criteri di avviso da utilizzare per inviare tali avvisi e accedere alla cronologia di tutte le notifiche inviate."

Le dashboard di avviso di consegna ti consentono di specificare chi riceverà gli avvisi e-mail, scegliere e configurare i criteri di avviso da utilizzare per inviare tali avvisi e accedere alla cronologia di tutte le notifiche inviate. Sono accessibili dalla sezione **Avvisi sulla consegna** nel riquadro di navigazione a sinistra, sotto il **Dashboard** scheda.

![](assets/alerting-dashboard-list.png)

## Creare un dashboard di consegna {#dashboards}

>[!CONTEXTUALHELP]
>id="acw_delery_alerting_dashboard_create"
>title="Creare una dashboard per gli avvisi di consegna"
>abstract="La creazione di un dashboard di avviso sulla consegna consente di specificare chi riceverà gli avvisi e-mail, scegliere e configurare i criteri di avviso da utilizzare per inviare tali avvisi e accedere alla cronologia di tutte le notifiche inviate."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_create_general"
>title="Parametri generali degli avvisi di consegna"
>abstract="Specifica le proprietà generali del dashboard di avvisi di consegna. Il **Seleziona gruppo di avvisi** campo consente di specificare **gruppo di operatori** per ricevere gli avvisi inviati da questo dashboard."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_create_criteria_add"
>title="Criteri per gli avvisi di consegna"
>abstract="In questa sezione, aggiungi i criteri che desideri utilizzare per inviare avvisi da questo dashboard. Scegli un criterio predefinito o creane uno personalizzato da allineare a esigenze specifiche."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_create_criteria_parameters"
>title="Parametri dei criteri"
>abstract="I criteri hanno valori di parametri predefiniti che definiscono come devono essere applicati. In questa sezione è possibile modificare questi valori in base alle proprie esigenze."

Per creare un dashboard di consegna, segui questi passaggi:

1. Accedi a **Avvisi sulla consegna** nel riquadro di navigazione a sinistra e fare clic su **Creare un dashboard di consegna**.

   ![](assets/alerting-dashboard.png)

1. Denomina il dashboard in **Etichetta** campo. Il **Nome interno** viene compilato automaticamente e di sola lettura.

1. In **Seleziona gruppo di avvisi** , specificare il **gruppo di operatori** per ricevere gli avvisi inviati da questo dashboard. Tutti i membri del gruppo di operatori selezionato riceveranno gli avvisi.

   Ulteriori informazioni sulle autorizzazioni e sui gruppi di operatori in [Documentazione di Adobe Campaign v8 (console)](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/gs-permissions){target="_blank"}

1. In **Criteri di avviso sulla consegna** , aggiungere i criteri che si desidera utilizzare per inviare gli avvisi. Scegli un criterio predefinito o creane uno personalizzato da allineare a esigenze specifiche. [Scopri come utilizzare i criteri](../msg/delivery-alerting-criteria.md)

1. I criteri hanno valori di parametri predefiniti che definiscono come devono essere applicati. È possibile modificare questi valori in base alle proprie esigenze utilizzando **Parametri dei criteri** sezione.

   ![](assets/alerting-criteria-parameters.png)

   Ad esempio, per impostazione predefinita, il **Dimensione minima del target di consegna** il parametro criteri è impostato su 50, il che significa che una consegna verrà inclusa nell’avviso inviato da questo dashboard solo se è destinata ad almeno 50 profili. Puoi modificare questo parametro se desideri includere le consegne con targeting inferiore a 50 profili.

   Espandi la sezione seguente per ulteriori informazioni su ciascun parametro di criterio:

   +++Parametri dei criteri disponibili

   * **Dimensione minima del target di consegna**: ad esempio, se immetti 100 in questo campo, una notifica viene inviata solo per le consegne con una destinazione uguale o superiore a 100 destinatari. Questo parametro si applica a tutti i criteri.
   * **Periodo di monitoraggio prima e dopo la data di contatto (in ore)**: numero di ore prima e dopo l’ora corrente. Vengono prese in considerazione solo le consegne con una data di contatto in questo intervallo di tempo. Questo parametro si applica a tutti i criteri. Per impostazione predefinita, il valore di questo campo è impostato su 24 ore.
   * **Rapporto massimo di errori di mancato recapito non permanenti**: viene inviata una notifica per tutte le consegne con un rapporto di errore di mancato recapito non permanente maggiore del valore specificato. Per impostazione predefinita, il valore di questo campo è 0,05 (5%).
   * **Rapporto massimo di errori di mancato recapito permanenti**: viene inviata una notifica per tutte le consegne con un rapporto di errore per mancati recapiti permanenti maggiore del valore specificato. Per impostazione predefinita, il valore di questo campo è 0,05 (5%).
   * **Soglia minima di tempo per la consegna in stato &quot;Avvio in sospeso&quot; (in minuti)**: viene inviata una notifica per tutte le consegne con uno stato Avvio in sospeso più lungo della durata specificata in questo campo. Lo stato Avvio in sospeso indica che i messaggi non sono ancora stati presi in considerazione dal sistema.
   * **Tempo minimo necessario per il calcolo del throughput (in minuti)**: per il criterio Consegne con bassa velocità effettiva vengono prese in considerazione solo le consegne avviate (con stato In corso) per una durata superiore a quella specificata.
   * **Percentuale massima di messaggi elaborati per il calcolo della velocità effettiva**: per il criterio Consegne con bassa velocità effettiva vengono prese in considerazione solo le consegne con una percentuale di messaggi elaborati inferiore alla percentuale specificata.
   * **Velocità effettiva minima prevista (in messaggi inviati all’ora)**: per il criterio Consegne con velocità effettiva bassa vengono prese in considerazione solo le consegne con una velocità effettiva inferiore al valore specificato.
   * **Rapporto minimo di elaborazione richiesto per il criterio &quot;Consegne in corso&quot;**: vengono prese in considerazione solo le consegne con una percentuale di messaggi elaborati superiore alla percentuale specificata.

+++

1. Per impostazione predefinita, le dashboard di avviso sono disabilitate, il che significa che gli avvisi e-mail collegati a questa dashboard non vengono inviati. Per attivare immediatamente la dashboard, attiva/disattiva **Abilitato** opzione in **Generale** accanto al campo di selezione del gruppo di avvisi.

   Puoi anche salvare la dashboard e abilitarla in un secondo momento.

   ![](assets/alerting-dashboard-enable.png)

1. Per salvare il dashboard degli avvisi, fare clic su **Salva** pulsante.

Viene visualizzato il dashboard degli avvisi con dati vuoti. Quando sei pronto ad attivarlo e inviare notifiche, fai clic sul pulsante **Impostazioni** e attivare/disattivare **Abilitato** se non lo hai già fatto in precedenza.

Ora, ogni volta che una consegna soddisfa i criteri definiti in questo dashboard, viene inviata una notifica di avviso al gruppo di operatori specificato.

## Gestire le dashboard degli avvisi

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_dashboard_alerts"
>title="Avvisi di consegna inviati"
>abstract="Questa sezione ti consente di visualizzare le informazioni relative agli ultimi avvisi inviati."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_dashboard_history"
>title="Cronologia degli avvisi di consegna"
>abstract="Il **Cronologia** contiene tutti gli avvisi inviati da questo dashboard. Fare clic su un elemento per accedere agli avvisi corrispondenti inviati in un determinato momento."

Tutte le dashboard di avviso create sono accessibili dalla **Avvisi sulla consegna** nel menu **Dashboard** scheda.

![](assets/alerting-dashboard-list.png)

È possibile duplicare o eliminare un dashboard utilizzando **Altre azioni** accanto al nome.

Per accedere a una vista dettagliata di un dashboard, fare clic sul nome nell&#39;elenco. Da questa schermata, puoi visualizzare l’ultimo avviso inviato. Tutti gli avvisi inviati sono elencati nel riquadro a sinistra. Fare clic su un elemento per accedere agli avvisi corrispondenti inviati in un determinato momento.

![](assets/alerting-dashboard-details.png)

Per modificare il dashboard, fai clic su **Impostazioni** nell&#39;angolo superiore destro e apportare le modifiche desiderate.
