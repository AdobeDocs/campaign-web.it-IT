---
audience: end-user
title: Avvisi di consegna
description: Scopri come utilizzare gli avvisi di consegna.
exl-id: b91ef82b-f3e9-4704-87a2-0e3f75104572
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '1115'
ht-degree: 22%

---

# Dashboard di avvisi di consegna {#delivery-alerting-dashboards}

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_dashboards"
>title="Dashboard di avvisi di consegna"
>abstract="Avvisi di consegna è un sistema di gestione degli avvisi che consente ai gruppi di utenti di ricevere automaticamente le notifiche e-mail con le informazioni sulle esecuzioni della propria consegna. Le dashboard di avvisi di consegna ti consentono di specificare chi riceverà gli avvisi e-mail, scegliere e configurare i criteri di avviso da utilizzare per l’invio e accedere alla cronologia di tutte le notifiche inviate."

I dashboard di avvisi di recapito consentono di specificare chi riceverà gli avvisi e-mail, scegliere e configurare i criteri di avviso da utilizzare per inviare tali avvisi e accesso la cronologia di tutte le notifiche inviate. Sono accessibili dal **menu Avvisi di** recapito nel riquadro navigazione sinistro, sotto la **scheda Dashboard** .

![Schermata che mostra l&#39;elenco dei dashboard di avviso nel menu Avvisi di consegna.](assets/alerting-dashboard-list.png)

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

Per creare un dashboard di consegna, seguire questi passaggi:

1. Passare al **menu Avvisi di** recapito nel riquadro navigazione sinistro e fare clic su **Crea dashboard** di consegna.

   ![Schermata che mostra l&#39;opzione del dashboard di consegna Crea nel menu Avvisi di consegna.](assets/alerting-dashboard.png)

1. Denomina il **dashboard nel campo Etichetta** . Il **campo Nome** interno viene popolato automaticamente e di sola lettura.

1. **Nel campo Seleziona gruppo** di avvisi, specificare il gruppo **di** operatori che riceverà gli avvisi inviati da questo dashboard. Tutti i membri del gruppo di operatori selezionato riceveranno gli avvisi.

   Scopri ulteriori informazioni su autorizzazioni e gruppi di operatori nella [documentazione di Adobe Campaign v8 (console)](https://experienceleague.adobe.com/it/docs/campaign/campaign-v8/admin/permissions/gs-permissions){target="_blank"}

1. **Nella sezione Criteri** avvisi di recapito aggiungere i criteri che si desidera utilizzare per inviare gli avvisi. Scegli tra criteri predefiniti o crea i tuoi criteri per allinearli a esigenze specifiche. [Scopri come utilizzare i criteri](../msg/delivery-alerting-criteria.md)

1. I criteri hanno valori di parametri predefiniti che definiscono come devono essere applicati. Puoi modificare questi valori in base alle tue esigenze dalla sezione Parametri **criteri**.

   ![Schermata che mostra la sezione Parametri criteri nel dashboard di consegna.](assets/alerting-criteria-parameters.png)

   Ad esempio, per impostazione predefinita, il **parametro Criteri di dimensione minima** destinazione consegna è impostato su 50, il che significa che una consegna verrà inclusa nell&#39;avviso inviato da questo dashboard solo se ha come destinazione almeno 50 profili. È possibile modificare questo parametro se si desidera includere consegne targeting meno di 50 profili.

   Espandi la sezione seguente per ulteriori informazioni su ciascun parametro di criteri:

   +++Parametri criteri disponibili

   * **Consegna destinazione dimensione** minima: Ad esempio, se inserisci 100 in questo campo, un notifica viene inviato solo per consegne con un destinazione pari o superiore a 100 destinatari. Questo parametro si applica a tutti i criteri.
   * **Periodo di monitoraggio prima e dopo la data di contatto (in ore)**: numero di ore prima e dopo l&#39;ora corrente. Vengono prese in considerazione solo le consegne con una data di contatto in questo intervallo di tempo. Questo parametro si applica a tutti i criteri. Per impostazione predefinita, il valore di questo campo è impostato su 24 ore.
   * **Rapporto massimo di errori** di soft bounce: viene inviato un notifica per tutte le consegne con un soft bounce error ratio maggiore del valore specificato. Per impostazione predefinita, il valore di questo campo è impostato su 0,05 (5%).
   * **Rapporto massimo di errori** di hard bounce: viene inviato un notifica per tutte le consegne con un hard bounce error ratio maggiore del valore specificato. Per impostazione predefinita, il valore di questo campo è impostato su 0,05 (5%).
   * **Tempo minimo soglia per la consegna nello stato &quot;Inizia in sospeso&quot; (in minuti):** viene inviato un notifica per tutte le consegne con uno stato Inizia in sospeso per un periodo superiore alla durata specificata in questo campo, Inizia stato in sospeso significa che i messaggi non sono ancora stati presi in account dal sistema.
   * **Tempo minimo richiesto per il calcolo della velocità effettiva (in minuti):** solo le consegne avviate (con stato In corso) per un periodo superiore alla durata specificata vengono prese in account per il criterio Consegne con bassa velocità effettiva.
   * **Percentuale massima di messaggi elaborati per il calcolo della velocità effettiva**: solo le consegne con una percentuale di messaggi elaborati inferiore alla percentuale specificata vengono prese in account per il criterio Recapito con bassa velocità effettiva.
   * **Velocità effettiva minima prevista (nei messaggi inviati all&#39;ora):** solo le consegne con una velocità effettiva inferiore al valore specificato vengono prese in account per il criterio Recapito con bassa velocità effettiva.
   * **Rapporto minimo di elaborazione richiesto per il criterio** &quot;Consegne in corso&quot;: vengono prese in account considerazione solo le consegne con una percentuale di messaggi elaborati superiore alla percentuale specificata.

   +++

1. Per impostazione predefinita, i dashboard di avviso sono disabilitati, il che significa che gli avvisi e-mail collegati a questo dashboard non vengono inviati. Per abilitare immediatamente la dashboard, attivare o disattivare l&#39;opzione **Abilitato** nella **sezione Generale** , accanto al campo di selezione del gruppo di avvisi.

   È inoltre possibile salvare il dashboard e abilitarlo in un secondo momento.

   ![Schermata che mostra l&#39;opzione di attivazione/disattivazione nelle impostazioni del dashboard di consegna.](assets/alerting-dashboard-enable.png)

1. Per salvare il dashboard degli avvisi, fare clic sulla **pulsante Salva** .

Il dashboard degli avvisi si apre con dati vuoti. Quando sei pronto per attivarlo e inviare notifiche, fai clic sul **pulsante Impostazioni** e attiva l&#39;opzione **Abilitato** se non lo hai fatto in precedenza.

Ora, ogni volta che una consegna soddisfa i criteri definiti in questo dashboard, viene inviato un notifica di avviso al gruppo di operatori specificato.

## Gestire le dashboard di avviso

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_dashboard_alerts"
>title="Avvisi di consegna inviati"
>abstract="Questa sezione ti consente di visualizzare le informazioni relative agli ultimi avvisi inviati."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_dashboard_history"
>title="Cronologia degli avvisi di consegna"
>abstract="Il riquadro **Cronologia** contiene tutti gli avvisi inviati da questa dashboard. Fare clic su un elemento per accedere agli avvisi corrispondenti inviati in un determinato momento."

Tutti i dashboard di avviso creati sono accessibili dal **menu Avvisi di** consegna, nella **scheda Dashboard** .

![Schermata che mostra l&#39;elenco dei dashboard di avviso nel menu Avvisi di consegna.](assets/alerting-dashboard-list.png)

È possibile duplicare o eliminare una dashboard utilizzando la **pulsante Altre azioni** accanto al nome.

Per accesso una vista dettagliata di una dashboard, fate clic sul suo nome dall&#39;elenco. Da questa schermata è possibile visualizzare l&#39;ultimo avviso inviato. Tutti gli avvisi inviati sono elencati nel riquadro a sinistra. Fare clic su un elemento per accedere agli avvisi corrispondenti inviati in un determinato momento.

![Schermata che mostra la vista dettagliata di un dashboard di avviso.](assets/alerting-dashboard-details.png)

Per modificare il dashboard, fare clic sulla **pulsante Impostazioni** nell&#39;angolo in alto a destra e apportare le modifiche desiderate.