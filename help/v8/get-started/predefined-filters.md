---
title: Creare e utilizzare filtri predefiniti
description: Scopri come creare e gestire filtri predefiniti nell’interfaccia web di Adobe Campaign
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
badge: label="Beta"
source-git-commit: 29fbfa9bb802ba1dff26dee8898fcb728309983d
workflow-type: tm+mt
source-wordcount: '786'
ht-degree: 10%

---

# Utilizzare filtri preimpostati {#predefined-filters}

>[!CONTEXTUALHELP]
>id="acw_homepage_card3"
>title="Gestione dei filtri predefiniti"
>abstract="Campaign web offre ora un’interfaccia intuitiva per gestire e personalizzare facilmente i filtri predefiniti in base alle tue esigenze specifiche. Crea una sola volta e salva per un utilizzo futuro."

>[!CONTEXTUALHELP]
>id="acw_predefined-filters-dashboard"
>title="Filtri preimpostati"
>abstract="Campaign web offre ora un’interfaccia intuitiva per gestire e personalizzare facilmente i filtri predefiniti in base alle tue esigenze specifiche. Crea una sola volta e salva per un utilizzo futuro."

I filtri predefiniti sono filtri personalizzati che vengono creati e salvati per essere disponibili in futuro. Possono essere utilizzati come scelte rapide durante qualsiasi operazione di filtro con il generatore di regole, ad esempio quando si filtra un elenco di dati o si crea il pubblico di una consegna.

Puoi utilizzare i filtri incorporati esistenti per accedere a un sottoinsieme specifico dei tuoi dati, oppure creare filtri predefiniti personalizzati e salvarli.

![](assets/predefined-filters-menu.png)

>[!IMPORTANT]
>
>In tale versione del prodotto, durante la creazione di regole, la selezione del pubblico di una consegna o la creazione di un pubblico in un flusso di lavoro e alcuni filtri preimpostati non sono disponibili nell’interfaccia utente. Tuttavia, puoi ancora usarli. [Ulteriori informazioni](guardrails.md#predefined-filters-filters-guardrails-limitations)


## Creare un filtro predefinito {#create-predefined-filter}

>[!CONTEXTUALHELP]
>id="acw_predefined-filters-creation"
>title="Creare un filtro predefinito"
>abstract="Immetti un’etichetta per il filtro predefinito e seleziona la tabella a cui si applica. Apri le opzioni aggiuntive per aggiungere una descrizione e imposta questo filtro come preferito. Quindi utilizza il pulsante &quot;Crea regola&quot; per definire le condizioni di filtro."

>[!CONTEXTUALHELP]
>id="acw_predefined-filters-rules"
>title="Creare le regole di filtro predefinite"
>abstract="Per definire le condizioni di filtro del filtro personalizzato, fai clic sul pulsante &quot;Crea regola&quot;."

### Creare un filtro dal generatore di regole {#create-from-rule-builder}

Puoi salvare un filtro personalizzato dal generatore di regole per renderlo disponibile per un utilizzo futuro. Segui questi passaggi:

1. Apri il generatore di regole e definisci le condizioni di filtro. Nell’esempio seguente, puoi filtrare i destinatari che vivono a Madrid.
1. Fai clic su **Seleziona o salva il filtro** e selezionare **Salva come filtro**.

   ![](assets/predefined-filters-save.png)

1. Seleziona **Crea un nuovo filtro** e immettere un nome e una descrizione per il filtro.

   ![](assets/predefined-filters-save-filter.png){width="70%" align="left"}

   Se necessario, puoi salvare il filtro come preferito. Per ulteriori informazioni, consulta [questa sezione](#fav-filter).

1. Clic **Conferma** per salvare le modifiche.

Il filtro personalizzato è ora disponibile nel **Filtri predefiniti** e accessibile a tutti gli utenti di Campaign.


### Creare un filtro dall’elenco dei filtri {#create-filter-from-list}


Puoi creare un filtro da **Filtri predefiniti** nel menu a sinistra. Per farlo, segui la procedura indicata di seguito:

1. Sfoglia il **Filtri predefiniti** nel menu a sinistra.
1. Fai clic su **Crea filtro** pulsante.
1. Inserisci il nome del filtro e, dalla **Tipo di documento** , seleziona lo schema a cui si applica. Lo schema predefinito è `Recipients(nms)`.

   Se necessario, puoi salvare il filtro come preferito. Per ulteriori informazioni, consulta [questa sezione](#fav-filter).

1. Definisci la regola per il filtro. Ad esempio, i profili con più di 30 anni.

   ![](assets/filter-30+.png)

1. Salva le modifiche. Il filtro viene aggiunto all’elenco di filtri predefinito.


## Salva il filtro come preferito {#fav-filter}

Quando crei un filtro predefinito, puoi abilitare **Salva come preferito** se desideri visualizzare questo filtro predefinito nei preferiti.


Quando un filtro viene salvato come preferito, è disponibile per tutti gli utenti nel **Filtri preferiti** dell’elenco di creazione del filtro, come illustrato di seguito:

![](assets/predefined-filters-favorite.png){width="30%" align="left"}


## Utilizza un filtro predefinito {#use-predefined-filter}

I filtri predefiniti sono disponibili quando si definiscono le proprietà della regola. Per accedere ai filtri predefiniti, scegli **Seleziona filtro personalizzato** nel menu a discesa del generatore di regole.

Puoi quindi accedere all’elenco completo dei filtri predefiniti disponibili per il contesto corrente.

È inoltre possibile utilizzare le scelte rapide da filtro disponibili nel **Filtri preferiti** del menu a discesa. Ulteriori informazioni sui preferiti in [questa sezione](#fav-filter).

Ad esempio, per creare un pubblico da un filtro predefinito, segui questi passaggi:

1. Sfoglia il **Tipi di pubblico** nel menu a sinistra.
1. Fai clic su **Crea pubblico** pulsante.
1. Immetti il nome del pubblico e fai clic su **Crea pubblico** pulsante.
1. Seleziona la **Query** e, nel riquadro di destra, fai clic su **Creare un pubblico** pulsante.

   ![](assets//build-audience-from-filter.png)

1. Dalla sezione **Seleziona o salva il pulsante del filtro**, scegli il **Seleziona filtro personalizzato** opzione.

   ![](assets/build-audience-select-custom-filter.png)

1. Individua il filtro predefinito da utilizzare per creare il pubblico, selezionalo e conferma.

   ![](assets/build-audience-filter-list.png)

1. Controlla le proprietà della regola per questo filtro e conferma.

   ![](assets/build-audience-check.png)

   Il filtro viene ora utilizzato come query in **Query** attività.

   ![](assets/build-audience-confirm.png)

1. Salva le modifiche e fai clic su **Inizio** per creare il pubblico e renderlo disponibile nell’elenco del pubblico.

## Gestire i filtri predefiniti {#manage-predefined-filter}

I filtri predefiniti sono tutti raggruppati nella voce dedicata del menu di navigazione a sinistra.

Da questo elenco, puoi creare un nuovo filtro come descritto in precedenza e:

* modificare un filtro esistente e modificarne regole e proprietà
* duplicare un filtro predefinito
* eliminare un filtro predefinito

Puoi aggiungere un filtro predefinito come preferito per un accesso rapido durante la creazione delle regole. Per ulteriori informazioni, consulta [questa sezione](#fav-filter).

<!--
## Built-in predefined filters {#ootb-predefined-filter}

Campaign comes with a set of predefined filters, built from the client console. These filters can be used to define your audiences, and rules. They must not be modified.
-->
