---
audience: end-user
title: Avvisi di consegna
description: Scopri come utilizzare gli avvisi sulla consegna.
badge: label="Disponibilità limitata"
exl-id: b91ef82b-f3e9-4704-87a2-0e3f75104572
source-git-commit: a28bc98d1735232d8aa0b0daaeca3969913e548c
workflow-type: tm+mt
source-wordcount: '1146'
ht-degree: 24%

---

# Dashboard di avvisi di consegna {#delivery-alerting-dashboards}

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_dashboards"
>title="Dashboard di avvisi di consegna"
>abstract="Avvisi di consegna è un sistema di gestione degli avvisi che consente ai gruppi di utenti di ricevere automaticamente le notifiche e-mail con le informazioni sulle esecuzioni della propria consegna. Le dashboard di avvisi di consegna ti consentono di specificare chi riceverà gli avvisi e-mail, scegliere e configurare i criteri di avviso da utilizzare per l’invio e accedere alla cronologia di tutte le notifiche inviate."

Le dashboard di avviso di consegna ti consentono di specificare chi riceverà gli avvisi e-mail, scegliere e configurare i criteri di avviso da utilizzare per inviare tali avvisi e accedere alla cronologia di tutte le notifiche inviate. Sono accessibili dal menu **Avvisi di consegna** nel riquadro di navigazione a sinistra, nella scheda **Dashboard**.

![Schermata che mostra l&#39;elenco delle dashboard di avviso nel menu Avvisi consegna.](assets/alerting-dashboard-list.png)

>[!AVAILABILITY]
>
>Questa funzionalità è a disponibilità limitata (LA). È limitata ai clienti che eseguono la migrazione **da Adobe Campaign Standard ad Adobe Campaign v8** e non possono essere distribuiti in nessun altro ambiente.

## Creare una dashboard di consegna {#dashboards}

>[!CONTEXTUALHELP]
>id="acw_delery_alerting_dashboard_create"
>title="Creare una dashboard per gli avvisi di consegna"
>abstract="La creazione di un dashboard di avviso di consegna consente di specificare chi riceverà gli avvisi e-mail, scegliere e configurare i criteri di avviso da utilizzare e accedere alla cronologia di tutte le notifiche inviate."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_create_general"
>title="Parametri generali degli avvisi di consegna"
>abstract="Specifica le proprietà generali della dashboard di avvisi di consegna. Il campo **Seleziona gruppo di avvisi** consente di specificare il **gruppo di operatori** che deve ricevere gli avvisi inviati da questa dashboard."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_create_criteria_add"
>title="Criteri per gli avvisi di consegna"
>abstract="In questa sezione, aggiungi i criteri che desideri utilizzare per inviare avvisi da questa dashboard. Scegli un criterio predefinito o creane uno personalizzato da allineare a esigenze specifiche."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_create_criteria_parameters"
>title="Parametri dei criteri"
>abstract="I criteri hanno valori di parametri predefiniti che definiscono come devono essere applicati. In questa sezione è possibile modificare questi valori in base alle proprie esigenze."

Per creare un dashboard di consegna, segui questi passaggi:

1. Passa al menu **Avvisi di consegna** nel riquadro di navigazione a sinistra e fai clic su **Crea dashboard di consegna**.

   ![Schermata che mostra l&#39;opzione Crea dashboard di consegna nel menu Avvisi di consegna.](assets/alerting-dashboard.png)

1. Denomina il dashboard nel campo **Etichetta**. Il campo **Nome interno** è compilato automaticamente e di sola lettura.

1. Nel campo **Seleziona gruppo di avvisi**, specifica il **gruppo di operatori** per ricevere gli avvisi inviati da questo dashboard. Tutti i membri del gruppo di operatori selezionato riceveranno gli avvisi.

   Ulteriori informazioni sulle autorizzazioni e sui gruppi di operatori nella [documentazione di Adobe Campaign v8 (console)](https://experienceleague.adobe.com/it/docs/campaign/campaign-v8/admin/permissions/gs-permissions){target="_blank"}

1. Nella sezione **Criteri di avviso di consegna**, aggiungi i criteri che desideri utilizzare per inviare gli avvisi. Scegli un criterio predefinito o creane uno personalizzato da allineare a esigenze specifiche. [Scopri come utilizzare i criteri](../msg/delivery-alerting-criteria.md)

1. I criteri hanno valori di parametro predefiniti che definiscono come devono essere applicati. È possibile modificare questi valori in base alle proprie esigenze dalla sezione **Parametri dei criteri**.

   ![Schermata che mostra la sezione Parametri dei criteri nel dashboard di consegna.](assets/alerting-criteria-parameters.png)

   Ad esempio, per impostazione predefinita, il parametro del criterio **Dimensione minima destinazione consegna** è impostato su 50, il che significa che una consegna verrà inclusa nell&#39;avviso inviato da questo dashboard solo se viene eseguita su almeno 50 profili. Puoi modificare questo parametro se desideri includere le consegne con targeting inferiore a 50 profili.

   Espandi la sezione seguente per ulteriori informazioni su ciascun parametro di criterio:

   +++Parametri dei criteri disponibili

   * **Dimensione minima destinazione consegna**: ad esempio, se si immette 100 in questo campo, viene inviata una notifica solo per le consegne con una destinazione uguale o superiore a 100 destinatari. Questo parametro si applica a tutti i criteri.
   * **Periodo di monitoraggio prima e dopo la data di contatto (in ore)**: numero di ore prima e dopo l&#39;ora corrente. Vengono prese in considerazione solo le consegne con una data di contatto in questo intervallo di tempo. Questo parametro si applica a tutti i criteri. Per impostazione predefinita, il valore di questo campo è impostato su 24 ore.
   * **Rapporto massimo di errori di mancato recapito non permanente**: viene inviata una notifica per tutte le consegne con un rapporto di errore di mancato recapito non permanente maggiore del valore specificato. Per impostazione predefinita, il valore di questo campo è 0,05 (5%).
   * **Rapporto massimo di errori di mancato recapito permanenti**: viene inviata una notifica per tutte le consegne con un rapporto di errore di mancato recapito permanente maggiore del valore specificato. Per impostazione predefinita, il valore di questo campo è 0,05 (5%).
   * **Soglia minima di tempo per la consegna con stato &#39;Avvio in sospeso&#39; (in minuti)**: viene inviata una notifica per tutte le consegne con stato Avvio in sospeso più lungo della durata specificata in questo campo. Lo stato Avvio in sospeso indica che i messaggi non sono ancora stati considerati dal sistema.
   * **Tempo minimo richiesto per il calcolo della velocità effettiva (in minuti)**: solo le consegne avviate (con stato In corso) per una durata superiore a quella specificata vengono prese in considerazione per il criterio Consegne con bassa velocità effettiva.
   * **Percentuale massima di messaggi elaborati per il calcolo della velocità effettiva**: solo le consegne con una percentuale di messaggi elaborati inferiore alla percentuale specificata vengono prese in considerazione per il criterio Consegne con bassa velocità effettiva.
   * **Velocità effettiva minima prevista (in messaggi inviati all&#39;ora)**: solo le consegne con una velocità effettiva inferiore al valore specificato vengono prese in considerazione per il criterio Consegne con velocità effettiva bassa.
   * **Rapporto minimo di elaborazione richiesto per il criterio &quot;Consegne in corso&quot;**: vengono prese in considerazione solo le consegne con una percentuale di messaggi elaborati superiore alla percentuale specificata.

   +++

1. Per impostazione predefinita, le dashboard di avviso sono disabilitate, il che significa che gli avvisi e-mail collegati a questa dashboard non vengono inviati. Per attivare immediatamente il dashboard, attivare/disattivare l&#39;opzione **Enabled** nella sezione **General** accanto al campo di selezione del gruppo di avvisi.

   Puoi anche salvare la dashboard e abilitarla in un secondo momento.

   ![Schermata che mostra l&#39;opzione Attiva/Disattiva nelle impostazioni del dashboard di consegna.](assets/alerting-dashboard-enable.png)

1. Per salvare il dashboard degli avvisi, fare clic sul pulsante **Salva**.

Viene visualizzato il dashboard degli avvisi con dati vuoti. Quando sei pronto ad attivarlo e inviare notifiche, fai clic sul pulsante **Impostazioni** e attiva l&#39;opzione **Abilitato**, se non lo hai già fatto in precedenza.

Ora, ogni volta che una consegna soddisfa i criteri definiti in questo dashboard, viene inviata una notifica di avviso al gruppo di operatori specificato.

## Gestire le dashboard di avviso

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_dashboard_alerts"
>title="Avvisi di consegna inviati"
>abstract="Questa sezione ti consente di visualizzare le informazioni relative agli ultimi avvisi inviati."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_dashboard_history"
>title="Cronologia degli avvisi di consegna"
>abstract="Il riquadro **Cronologia** contiene tutti gli avvisi inviati da questa dashboard. Fare clic su un elemento per accedere agli avvisi corrispondenti inviati in un determinato momento."

Tutti i dashboard di avviso creati sono accessibili dal menu **Avvisi di consegna**, nella scheda **Dashboard**.

![Schermata che mostra l&#39;elenco delle dashboard di avviso nel menu Avvisi consegna.](assets/alerting-dashboard-list.png)

Puoi duplicare o eliminare un dashboard utilizzando il pulsante **Altre azioni** accanto al nome.

Per accedere a una vista dettagliata di un dashboard, fare clic sul nome nell&#39;elenco. Da questa schermata, puoi visualizzare l’ultimo avviso inviato. Tutti gli avvisi inviati sono elencati nel riquadro a sinistra. Fare clic su un elemento per accedere agli avvisi corrispondenti inviati in un determinato momento.

![Schermata che mostra la visualizzazione dettagliata di un dashboard di avvisi.](assets/alerting-dashboard-details.png)

Per modificare il dashboard, fare clic sul pulsante **Impostazioni** nell&#39;angolo superiore destro e apportare le modifiche desiderate.