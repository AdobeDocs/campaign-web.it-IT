---
title: Creare e utilizzare filtri preimpostati
description: Scopri come creare e gestire filtri preimpostati nell’interfaccia web di Adobe Campaign
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
badge: label="Beta"
exl-id: f6b73792-063d-4371-93e1-efa2aa02ee28
source-git-commit: f4ffb1e033dae3d631772ef602e48e336c8c0f16
workflow-type: ht
source-wordcount: '786'
ht-degree: 100%

---

# Utilizzare filtri preimpostati {#predefined-filters}

>[!CONTEXTUALHELP]
>id="acw_homepage_card3"
>title="Gestione dei filtri preimpostati"
>abstract="Campaign Web ora offre un’interfaccia semplice e intuitiva per gestire e personalizzare filtri preimpostati, al fine di soddisfare esigenze specifiche. Crea una sola volta e salva per un utilizzo futuro."

>[!CONTEXTUALHELP]
>id="acw_predefined-filters-dashboard"
>title="Filtri preimpostati"
>abstract="Campaign Web ora offre un’interfaccia semplice e intuitiva per gestire e personalizzare filtri preimpostati, al fine di soddisfare esigenze specifiche. Crea una sola volta e salva per un utilizzo futuro."

I filtri preimpostati sono filtri personalizzati che vengono creati e salvati per essere disponibili per un utilizzo futuro. Possono essere utilizzati come scelte rapide durante qualsiasi operazione di filtro insieme al generatore di regole, ad esempio quando si filtra un elenco di dati o si crea il pubblico di una consegna.

Puoi utilizzare i filtri preimpostati esistenti per accedere a un sottoinsieme specifico dei tuoi dati o creare filtri preimpostati personalizzati e salvarli.

![](assets/predefined-filters-menu.png)

>[!IMPORTANT]
>
>In tale versione del prodotto, durante la creazione di regole, la selezione del pubblico di una consegna o la creazione di un pubblico in un flusso di lavoro e alcuni filtri preimpostati non sono disponibili nell’interfaccia utente. Tuttavia, puoi ancora usarli. [Ulteriori informazioni](guardrails.md#predefined-filters-filters-guardrails-limitations)


## Creare un filtro preimpostato {#create-predefined-filter}

>[!CONTEXTUALHELP]
>id="acw_predefined-filters-creation"
>title="Creare un filtro preimpostato"
>abstract="Immetti un’etichetta per il filtro preimpostato e seleziona la tabella a cui si applica. Apri le opzioni aggiuntive per aggiungere una descrizione e imposta questo filtro come preferito. Quindi utilizza il pulsante “Crea regola” per definire le condizioni del filtro"

>[!CONTEXTUALHELP]
>id="acw_predefined-filters-rules"
>title="Creare le regole del filtro preimpostato"
>abstract="Per definire le condizioni del filtro personalizzato, fai clic sul pulsante “Crea regola”."

### Creare un filtro dal generatore di regole {#create-from-rule-builder}

Puoi salvare un filtro personalizzato creato dal generatore di regole al fine di renderlo disponibile per un utilizzo futuro. Segui questi passaggi:

1. Apri il generatore di regole e definisci le condizioni del filtro. Nell’esempio seguente, puoi filtrare i destinatari che vivono a Madrid.
1. Fai clic sul pulsante **Seleziona o salva filtro** e seleziona **Salva come filtro**.

   ![](assets/predefined-filters-save.png)

1. Seleziona **Crea un nuovo filtro** e immetti un nome e una descrizione per il filtro.

   ![](assets/predefined-filters-save-filter.png){width="70%" align="left"}

   Se necessario, puoi salvare il filtro come preferito. Per ulteriori informazioni, consulta [questa sezione](#fav-filter).

1. Fai clic su **Conferma** per salvare le modifiche.

Il filtro personalizzato è ora disponibile nell’elenco **Filtri preimpostati** e accessibile a tutti gli utenti di Campaign.


### Creare un filtro dall’elenco filtri {#create-filter-from-list}


Puoi creare un filtro dalla voce **Filtri preimpostati** nel menu a sinistra. Per farlo, segui i passaggi indicati di seguito:

1. Passa alla voce **Filtri preimpostati** nel menu a sinistra.
1. Fai clic sul pulsante **Crea filtro**.
1. Inserisci il nome del filtro e, dal campo **Tipo di documento**, seleziona lo schema a cui si applica. Lo schema predefinito è `Recipients(nms)`.

   Se necessario, puoi salvare il filtro come preferito. Per ulteriori informazioni, consulta [questa sezione](#fav-filter).

1. Definisci la regola per il filtro. Ad esempio, per i profili con più di 30 anni.

   ![](assets/filter-30+.png)

1. Salva le modifiche. Il filtro viene aggiunto all’elenco dei filtri preimpostati.


## Salva il filtro come preferito {#fav-filter}

Quando crei un filtro preimpostato, puoi abilitare l’opzione **Salva come preferito** se lo desideri visualizzare tra i preferiti.


Quando viene salvato un filtro come preferito, è disponibile per tutti gli utenti nella sezione **Filtri preferiti** dell’elenco di filtri creati, come illustrato di seguito:

![](assets/predefined-filters-favorite.png){width="30%" align="left"}


## Utilizza un filtro preimpostato {#use-predefined-filter}

I filtri preimpostati sono disponibili quando si definiscono le proprietà delle regole. Per accedere ai filtri preimpostati, scegli **Seleziona filtro personalizzato** nel menu a discesa del generatore di regole.

Puoi quindi accedere all’elenco completo dei filtri preimpostati disponibili per il contesto corrente.

Puoi anche utilizzare le scelte rapide per i filtri disponibili nella sezione **Filtri preferiti** del menu a discesa. Per ulteriori informazioni sui preferiti, consulta [questa sezione](#fav-filter).

Ad esempio, per creare un pubblico da un filtro preimpostato, segui questi passaggi:

1. Passa alla voce **Tipi di pubblico** nel menu a sinistra.
1. Fai clic sul pulsante **Crea pubblico**.
1. Immetti il nome del pubblico e fai clic su **Crea pubblico**.
1. Seleziona l’attività **Query** e, nel riquadro di destra, fai clic sul pulsante **Crea pubblico**.

   ![](assets//build-audience-from-filter.png)

1. Dal pulsante **Seleziona o salva filtro**, scegli l’opzione **Seleziona filtro personalizzato**.

   ![](assets/build-audience-select-custom-filter.png)

1. Passa al filtro preimpostato da usare per creare il pubblico, selezionalo e conferma.

   ![](assets/build-audience-filter-list.png)

1. Controlla le proprietà della regola per questo filtro e conferma.

   ![](assets/build-audience-check.png)

   Il filtro viene ora utilizzato come query nell’attività **Query**.

   ![](assets/build-audience-confirm.png)

1. Salva le modifiche e fai clic sul pulsante **Inizia** per creare il pubblico e renderlo disponibile nell’elenco dei tipi di pubblico.

## Gestire i filtri preimpostati {#manage-predefined-filter}

I filtri preimpostati sono tutti raggruppati nella voce dedicata del menu di navigazione a sinistra.

Da questo elenco, puoi creare un nuovo filtro come descritto in precedenza; inoltre, puoi:

* modificare un filtro esistente comprese regole e proprietà;
* duplicare un filtro preimpostato;
* eliminare un filtro preimpostato.

Puoi aggiungere un filtro preimpostato come preferito per accedervi rapidamente durante la creazione delle regole. Per ulteriori informazioni, consulta [questa sezione](#fav-filter).

<!--
## Built-in predefined filters {#ootb-predefined-filter}

Campaign comes with a set of predefined filters, built from the client console. These filters can be used to define your audiences, and rules. They must not be modified.
-->
