---
title: Utilizzare filtri preimpostati
description: Scopri come creare e gestire filtri preimpostati in Adobe Campaign Web
exl-id: f6b73792-063d-4371-93e1-efa2aa02ee28
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '785'
ht-degree: 60%

---

# Utilizzare filtri preimpostati {#predefined-filters}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card4"
>title="Gestione dei filtri preimpostati"
>abstract="L’interfaccia utente di Campaign Web offre un’interfaccia intuitiva per gestire e personalizzare facilmente i filtri predefiniti in base alle esigenze specifiche. Crea una sola volta e salva per un utilizzo futuro."

>[!CONTEXTUALHELP]
>id="acw_predefined-filters-dashboard"
>title="Filtri preimpostati"
>abstract="L’interfaccia utente di Campaign Web offre un’interfaccia intuitiva per gestire e personalizzare facilmente i filtri predefiniti in base alle esigenze specifiche. Crea una sola volta e salva per un utilizzo futuro."

I filtri predefiniti sono filtri personalizzati creati e salvati per utilizzi futuri. Fungono da scelte rapide durante le operazioni di filtro con Query Modeler. Ad esempio, possono essere utilizzati per filtrare un elenco di dati o creare il pubblico di una consegna.

Puoi utilizzare i filtri incorporati esistenti per accedere a un sottoinsieme specifico dei dati o creare filtri predefiniti personalizzati e salvarli.

![Interfaccia del menu dei filtri predefiniti](assets/predefined-filters-menu.png){zoomable="yes"}

## Creare un filtro preimpostato {#create-predefined-filter}

>[!CONTEXTUALHELP]
>id="acw_predefined-filters-creation"
>title="Creare un filtro preimpostato"
>abstract="Immetti un’etichetta per il filtro preimpostato e seleziona la tabella a cui si applica. Apri le opzioni aggiuntive per aggiungere una descrizione e imposta questo filtro come preferito. Quindi utilizza il pulsante “Crea regola” per definire le condizioni del filtro"

>[!CONTEXTUALHELP]
>id="acw_predefined-filters-rules"
>title="Creare le regole del filtro preimpostato"
>abstract="Per definire le condizioni del filtro personalizzato, fai clic sul pulsante “Crea regola”."

### Creare un filtro dal query modeler {#create-from-rule-builder}

Salva un filtro personalizzato da [modeler query](../query/query-modeler-overview.md) per renderlo disponibile per un utilizzo futuro. Segui questi passaggi:

1. Apri il query modeler e definisci le condizioni del filtro. Nell’esempio seguente, i destinatari che vivono a Madrid e si sono iscritti a una newsletter vengono filtrati.
1. Fai clic sul pulsante **Seleziona o salva filtro** e seleziona **Salva come filtro**.

   ![Salva interfaccia filtro predefinita](assets/predefined-filters-save.png){zoomable="yes"}

1. Seleziona **Crea un nuovo filtro** e immetti un nome e una descrizione per il filtro.

   ![Salva interfaccia dettagli filtro](assets/predefined-filters-save-filter.png){zoomable="yes"}

   Se necessario, puoi salvare il filtro come preferito. Per ulteriori informazioni, consulta [questa sezione](#fav-filter).

1. Fai clic su **Conferma** per salvare le modifiche.

Il filtro personalizzato è ora disponibile nell’elenco **Filtri preimpostati** e accessibile a tutti gli utenti di Campaign.

### Creare un filtro dall’elenco filtri {#create-filter-from-list}

Crea un filtro dalla voce **Filtri predefiniti** nel menu a sinistra. Segui questi passaggi:

1. Individua la voce **Filtri predefiniti** nel menu a sinistra.
1. Fai clic sul pulsante **Crea filtro**.
1. Inserisci il nome del filtro e, dal campo **Tipo di documento**, seleziona lo schema a cui si applica. Lo schema predefinito è `Recipients(nms)`.

1. Definisci la regola per il filtro. Ad esempio, per i profili con più di 30 anni.

   ![Regola filtro per profili con più di 30](assets/filter-30+.png){zoomable="yes"}

1. Salva le modifiche.

   ![Nuova interfaccia salvata dal filtro](assets/new-filter.png){zoomable="yes"}

Il filtro viene aggiunto all’elenco dei filtri preimpostati. Se necessario, puoi salvare il filtro come preferito. Per ulteriori informazioni, consulta [questa sezione](#fav-filter).

## Salva il filtro come preferito {#fav-filter}

Quando crei un filtro predefinito, abilita l&#39;opzione **Salva come preferito** per visualizzare questo filtro predefinito nei preferiti.

Quando viene salvato un filtro come preferito, è disponibile per tutti gli utenti nella sezione **Filtri preferiti** dell’elenco di filtri creati, come illustrato di seguito:

![Sezione filtri preferiti](assets/predefined-filters-favorite.png){zoomable="yes"}{width="30%" align="left"}

## Utilizza un filtro preimpostato {#use-predefined-filter}

I filtri preimpostati sono disponibili quando si definiscono le proprietà delle regole. Per accedere ai filtri predefiniti, scegli l&#39;opzione **Seleziona filtro personalizzato** nell&#39;elenco a discesa del modellatore di query.

Accedere all&#39;elenco completo dei filtri predefiniti disponibili per il contesto corrente e utilizzare i collegamenti nella sezione **Filtri preferiti** del menu a discesa. Per ulteriori informazioni sui preferiti, consulta [questa sezione](#fav-filter).

Ad esempio, per creare un pubblico da un filtro preimpostato, segui questi passaggi:

1. Accedi a **Tipi di pubblico** nel menu a sinistra e fai clic sul pulsante **Crea pubblico** nell’angolo in alto a sinistra dell’elenco dei tipi di pubblico.
1. Immetti il nome del pubblico e fai clic su **Crea pubblico**.
1. Seleziona l’attività **Query** e, nel riquadro di destra, fai clic sul pulsante **Crea pubblico**.

   ![Crea interfaccia pubblico](assets/build-audience-from-filter.png){zoomable="yes"}

1. Dal pulsante **Seleziona o salva filtro**, scegli l’opzione **Seleziona filtro personalizzato**.

   ![Seleziona opzione filtro personalizzata](assets/build-audience-select-custom-filter.png){zoomable="yes"}

1. Passa al filtro preimpostato da usare per creare il pubblico, selezionalo e conferma.

   ![Interfaccia elenco filtri predefinita](assets/build-audience-filter-list.png){zoomable="yes"}

1. Controlla le proprietà della regola per questo filtro e conferma.

   Il filtro viene ora utilizzato come query nell’attività **Query**.

   ![Attività query con filtro predefinito](assets/build-audience-confirm.png){zoomable="yes"}

1. Salva le modifiche e fai clic sul pulsante **Inizia** per creare il pubblico e renderlo disponibile nell’elenco dei tipi di pubblico.

## Gestire i filtri preimpostati {#manage-predefined-filter}

Tutti i filtri preimpostati sono raggruppati nella voce dedicata del menu di navigazione a sinistra.

![Elenco di filtri predefiniti](assets/list-of-filters.png){zoomable="yes"}

Da questo elenco, puoi creare un nuovo filtro come descritto in precedenza ed eseguire le azioni elencate di seguito:

* Modifica un filtro esistente e modificane regole e proprietà.
* duplicare un filtro preimpostato;
* eliminare un filtro preimpostato.

Puoi anche aggiungere un filtro predefinito come preferito per l’accesso rapido durante la creazione dei tipi di pubblico. Per ulteriori informazioni, consulta [questa sezione](#fav-filter).

<!--
## Built-in predefined filters {#ootb-predefined-filter}

Campaign comes with a set of predefined filters, built from the client console. These filters can be used to define your audiences, and rules. They must not be modified.
-->