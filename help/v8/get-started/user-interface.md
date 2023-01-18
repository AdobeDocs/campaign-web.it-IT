---
audience: end-user
title: Scopri l’interfaccia
description: Interfaccia utente Web di Campaign v8
exl-id: 0908c827-aa91-469f-824b-8e3de543876d
source-git-commit: b203d1e2adb1b41cdc4adf398934707f6093b317
workflow-type: tm+mt
source-wordcount: '1297'
ht-degree: 1%

---

# Scopri l’interfaccia {#user-interface}

![](../assets/do-not-localize/badge.png)

>[!CONTEXTUALHELP]
>id="acw_homepage_learnmore"
>title="Scopri l’interfaccia"
>abstract="La nuova interfaccia web Campaign v8 offre un’esperienza utente integrata, intuitiva e coerente."

La nuova interfaccia web Campaign v8 offre un’esperienza utente moderna e intuitiva per semplificare la progettazione e la distribuzione delle campagne di marketing. Questa nuova interfaccia è integrata con Adobe Experience Platform.

<!--
Key concepts when browsing the user interface are common with Adobe Experience Platform. Refer to [Adobe Experience Platform documentation](https://experienceleague.adobe.com/docs/experience-platform/landing/platform-ui/ui-guide.html#adobe-experience-platform-ui-guide) for more details.
-->

>[!NOTE]
>
>Questa documentazione viene spesso aggiornata per riflettere le ultime modifiche nell’interfaccia utente del prodotto. Tuttavia, alcune schermate possono differire leggermente dall’interfaccia utente.


<!--
* console + web interface (overview, why use each of them)
* web UI made up of read-only lists that can be configured, show how to add columns
-->

## Menu di navigazione a sinistra

Sfoglia i collegamenti a sinistra per accedere alle funzionalità web di Campaign v8. Diversi collegamenti presentano elenchi di oggetti che possono essere ordinati e filtrati. Puoi anche configurare le colonne per visualizzare tutte le informazioni necessarie. Vedi questo [sezione](#list-screens). Tutte le schermate elenco sono di sola lettura, ad eccezione dell’elenco di consegna e-mail. Non è possibile fare clic su una voce dell’elenco per modificarla o visualizzarla in Alfa. Tutti gli elenchi saranno modificabili nelle versioni future. Gli elementi visualizzati nel menu di navigazione a sinistra dipendono dalle autorizzazioni utente.

![](assets/home.png)

### Home

Questa schermata include collegamenti chiave e risorse per un accesso rapido alle funzionalità Web principali di Campaign v8. La **Recenti** fornisce collegamenti alle consegne create e modificate di recente. Questo elenco mostra le relative date e lo stato di creazione e modifica.

<!--
* Banner
* KPIs on email channel (cross-deliveries): open rate, delivery rate, etc
* Recent items
* Learning cards
-->

Accedi alle pagine della guida della chiave Web v8 di Campaign dalla sezione inferiore della home page.

<!--
show global KPIs, recent items + left menu to access features)
CONTROL PANEL not alpha
Global report not alpha
-->

### Explorer

>[!CONTEXTUALHELP]
>id="acw_explorer"
>title="Explorer"
>abstract="La **Esplora risorse** visualizza la stessa gerarchia di cartelle di quella presente nella console client. Sfoglia tutti i componenti, le cartelle e gli schemi di Campaign v8. Tutte le schermate elenco sono di sola lettura, ad eccezione dell’elenco di consegna e-mail."

La **Esplora risorse** visualizza la stessa gerarchia di cartelle di quella presente nella console client. Sfoglia tutti i componenti, le cartelle e gli schemi di Campaign v8. Tutte le schermate elenco sono di sola lettura, ad eccezione dell’elenco di consegna e-mail.

Gli elementi visualizzati in Esplora risorse dipendono dalle autorizzazioni dell&#39;utente.

Come in qualsiasi schermata dell’elenco, puoi configurare le colonne per personalizzare la visualizzazione e visualizzare tutte le informazioni necessarie. Vedi questo [sezione](#list-screens).

Per ulteriori informazioni su Campaign Explorer, consulta questo [documentazione](https://experienceleague.adobe.com/docs/campaign/campaign-v8/new/ac-ui/campaign-ui.html#ac-explorer-ui){target="_blank"}.
<!--
Explorer' menu in web UI to navigate through console content: console navtree second view in addition to the left menu lists with filters. The Explorer gives the real folder hierarchy from the console. Make sure you find your deliveries in sub-folders. All lists can be accessed in read-only. No Create/Edit. You can configure lists (colums). All schema fields, linked tables are available. 

If you need to view your lists of recipients (age, gender), transactions or live transactional messages. To view each/edit -> console.

Navtree view depends on permissions (same as console).
-->

### Gestione delle campagne

>[!CONTEXTUALHELP]
>id="acw_campaigns_list"
>title="Campagne"
>abstract="Elenco delle campagne. Puoi visualizzare informazioni utili, ad esempio le date di inizio/fine/ultima modifica e il relativo stato. È possibile filtrare l’elenco in base allo stato o alle date di inizio/fine. Sono disponibili anche i modelli di campagna. Questi elenchi sono di sola lettura."

>[!CONTEXTUALHELP]
>id="acw_deliveries_list"
>title="Consegne"
>abstract="Scorri l’elenco delle consegne. Puoi visualizzarne lo stato, l’ultima data di modifica e i KPI chiave. Puoi filtrare l’elenco per stato, data di contatto o canale. Fai clic su una consegna e-mail per aprire il relativo dashboard. Gli altri elementi sono di sola lettura. Sono disponibili anche i modelli di consegna."

* **Campagne** - Elenco delle campagne. Per impostazione predefinita, puoi visualizzarne le date di inizio/fine/ultima modifica e il relativo stato. È possibile filtrare l’elenco in base allo stato o alle date di inizio/fine. Sono disponibili anche i modelli di campagna. Questi elenchi sono di sola lettura.

* **Consegne** - Scorri l’elenco delle consegne. Per impostazione predefinita, puoi visualizzarne lo stato, la data dell’ultima modifica e i KPI chiave. Puoi filtrare l’elenco per stato, data di contatto o canale. Fai clic su una consegna e-mail per aprire il relativo dashboard per ottenere una panoramica dei dettagli della consegna. Le consegne su altri canali sono di sola lettura. I modelli di consegna sono disponibili anche in modalità di sola lettura. Puoi utilizzare la console Client per modificarli. Vedi questo [documentazione](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/create-templates.html){target="_blank"}.

   Utilizza la **Altre azioni** per eliminare o duplicare una consegna.

   ![](assets/more-actions.png){width="70%" align="left"}

### Gestione clienti

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Destinatari"
>abstract="Accedi al database dei destinatari. Puoi visualizzare informazioni utili quali indirizzo e-mail, nome e cognome. Questo elenco è di sola lettura."

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="Tipi di pubblico"
>abstract="Questo è il tuo elenco di tipi di pubblico. Puoi visualizzarne il tipo, l’origine, le date di creazione/ultima modifica e l’etichetta. È possibile filtrare l’elenco in base all’origine. Questo elenco è di sola lettura."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list"
>title="Elenchi di iscrizioni"
>abstract="Sfoglia gli elenchi degli abbonamenti. Puoi visualizzarne il tipo, la modalità e l’etichetta. Questo elenco è di sola lettura."

>[!CONTEXTUALHELP]
>id="acw_targeting_workflow_list"
>title="Flussi di lavoro di targeting"
>abstract="Accedi all’elenco dei flussi di lavoro di Campaign. Puoi visualizzarne lo stato, le date e l’ambiente dell’ultima/successiva elaborazione. Puoi filtrare l’elenco per stato, data dell’ultima elaborazione e tipo di flusso di lavoro. Sono disponibili anche i modelli di flusso di lavoro . Questi elenchi sono di sola lettura."

* **Destinatari** - Accedere al database dei destinatari. Per impostazione predefinita, puoi visualizzarne l’indirizzo e-mail, il nome e il cognome. Questo elenco è di sola lettura.
* **Tipi di pubblico** - Questo è il tuo elenco di tipi di pubblico. Per impostazione predefinita, puoi visualizzarne il tipo, l’origine, le date di creazione/ultima modifica e l’etichetta. È possibile filtrare l’elenco in base all’origine. Questo elenco è di sola lettura.
* **Elenco sottoscrizioni** - Sfoglia gli elenchi degli abbonamenti. Per impostazione predefinita, puoi visualizzarne il tipo, la modalità e l’etichetta. Questo elenco è di sola lettura.
* **Workflow di targeting** - Accedi all’elenco dei flussi di lavoro di Campaign. Per impostazione predefinita, è possibile visualizzarne lo stato, le date dell’ultima/successiva elaborazione e l’ambiente. Puoi filtrare l’elenco per stato, data dell’ultima elaborazione e tipo di flusso di lavoro. Sono disponibili anche i modelli di flusso di lavoro . Questi elenchi sono di sola lettura.

### Gestione delle decisioni

>[!CONTEXTUALHELP]
>id="acw_offers_list"
>title="Offerte"
>abstract="Scorri l’elenco delle offerte di interazione. Per impostazione predefinita, puoi visualizzarne lo stato, le date di inizio/fine e l’ambiente. Puoi filtrare l’elenco per stato e per date di inizio/fine. Sono disponibili anche modelli di offerta. Questi elenchi sono di sola lettura."

* **Offerte** - Scorri l’elenco delle offerte di interazione. Per impostazione predefinita, puoi visualizzarne lo stato, le date di inizio/fine e l’ambiente. Puoi filtrare l’elenco per stato e per date di inizio/fine. Sono disponibili anche modelli di offerta. Questi elenchi sono di sola lettura.

## Barra superiore

La barra superiore dell’interfaccia consente di:

* condividere il tuo feedback come tester Alpha
* passare da un’organizzazione all’altra e alle istanze
* passare da un&#39;applicazione Adobe Experience Cloud all&#39;altra
* accedere alle pagine della guida, contattare il supporto e condividere i commenti. Puoi cercare articoli e video della guida dal campo di ricerca.

![](assets/unified-shell.png){width="70%" align="left"}
<!--
Org / Sub-org switcher to switch between instances. Only one for Alpha. Later: intermerdiate screen with Control Panel (beta). if v8 + ACS with one card per ACS instance. Maybe quickly explain the menu for Alpha?
-->

## Configurare le schermate elenco {#list-screens}

Diversi collegamenti dal menu di navigazione a sinistra, ad esempio **Consegne** o **Campagne**, mostra gli elenchi degli oggetti. Queste schermate elenco sono di sola lettura, ad eccezione dell’elenco di consegna e-mail.

Per trovare gli elementi più rapidamente, puoi utilizzare la barra di ricerca o filtrare l’elenco in base a criteri contestuali.

![](assets/filter.png){width="70%" align="left"}

Gli elenchi vengono visualizzati in colonne. Puoi visualizzare ulteriori informazioni modificando la configurazione delle colonne. A questo scopo, fai clic sull’icona nell’angolo in alto a destra dell’elenco. È possibile aggiungere o rimuovere colonne e modificare l’ordine in cui vengono visualizzate.

![](assets/columns.png){width="70%" align="left"}

Per ordinare gli elementi dell’elenco, fai clic su qualsiasi intestazione di colonna. Viene visualizzata una freccia (Su o Giù) che indica che l’elenco è ordinato in quella colonna. Per le colonne numeriche o di data, la freccia Su indica che l’elenco è ordinato in ordine crescente, mentre la freccia Giù indica un ordine decrescente. Per le colonne stringa o alfanumeriche, i valori sono elencati in ordine alfabetico.

## Aiuto contestuale e guida all’onboarding

Nell’interfaccia è disponibile una guida contestuale. Quando disponibile, fai clic sul pulsante **?** per visualizzare le informazioni della guida e i relativi collegamenti alla documentazione.

![](assets/context-help.png){width="70%" align="left"}

È inoltre disponibile una guida all’onboarding per aiutarti a iniziare con Campaign v8 Web. Fai clic sull’icona nell’angolo in basso a destra, scegli uno degli scenari dettagliati disponibili e segui semplicemente le istruzioni.

![](assets/onboarding.png){width="70%" align="left"}

## Browser supportati {#browsers}

Campaign v8 Web è progettato per funzionare in modo ottimale nell’ultima versione di Google Chrome, Safari e Microsoft Edge. È possibile che si verifichino problemi durante l’utilizzo di alcune funzioni nelle versioni precedenti o in altri browser.

## Preferenze della lingua {#language-pref}

L’interfaccia utente è attualmente disponibile nelle seguenti lingue:

* Inglese (USA) - IT-IT
* Francese - FR
* Tedesco - DE
* Italiano - IT
* Spagnolo - ES
* Portoghese (brasiliano) - PTBR
* Giapponese - JP
* Coreano - KR
* Cinese semplificato - CHS
* Cinese tradizionale - CHT

La lingua predefinita dell’interfaccia è determinata dalla lingua preferita specificata nel profilo utente.

Per modificare la lingua:

* Fai clic su **Preferenze** dal tuo avatar, in alto a destra.
   ![](assets/preferences.png)
* Quindi fai clic sulla lingua visualizzata sotto il tuo indirizzo e-mail
* Seleziona la lingua preferita e fai clic su **Salva**. È possibile selezionare una seconda lingua nel caso in cui il componente utilizzato non sia localizzato nella prima lingua.
   ![](assets/select-language.png)

<!--
## Supported browsers {#browsers}

Adobe Campaign interface is designed to work optimally in the latest version of Google Chrome. You might have trouble using certain features on older versions or other browsers.
-->