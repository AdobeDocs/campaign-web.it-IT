---
audience: end-user
title: Creare frammenti di contenuto
description: Scopri come creare con i frammenti di contenuto
exl-id: d155d102-a5bc-4b9b-b29c-24fde4d95ceb
source-git-commit: 2d6b885642fbb6e1545f899219db05c156b069c4
workflow-type: tm+mt
source-wordcount: '916'
ht-degree: 24%

---

# Creare frammenti di contenuto {#fragments}

>[!CONTEXTUALHELP]
>id="acw_fragments_menu"
>title="Definisci il tuo frammento"
>abstract="Un frammento è un componente riutilizzabile a cui è possibile fare riferimento in una o più e-mail tra campagne. Questa funzionalità viene utilizzata per precostruire più blocchi di contenuto personalizzati che possono essere utilizzati dagli utenti di marketing per assemblare rapidamente i contenuti delle e-mail in un processo di progettazione migliorato."

>[!CONTEXTUALHELP]
>id="acw_fragments_save"
>title="Salvataggio di frammenti"
>abstract="Salvataggio di frammenti"

>[!CONTEXTUALHELP]
>id="acw_fragments_create"
>title="Definisci il tuo frammento"
>abstract="Un frammento è un componente riutilizzabile a cui è possibile fare riferimento in una o più e-mail tra campagne."

>[!CONTEXTUALHELP]
>id="acw_fragments_properties"
>title="Proprietà dei frammenti"
>abstract="Proprietà dei frammenti"

>[!CONTEXTUALHELP]
>id="acw_fragments_type"
>title="Tipo di frammento"
>abstract="Seleziona il tipo di frammento. Per il momento, sono disponibili solo i frammenti visivi per le e-mail."

>[!CONTEXTUALHELP]
>id="acw_fragments_list"
>title="Definisci il tuo frammento"
>abstract="Un frammento è un componente riutilizzabile a cui è possibile fare riferimento in una o più e-mail tra campagne. Puoi anche utilizzare i frammenti nei modelli e-mail. Per il momento, sono disponibili solo i frammenti visivi."

>[!CONTEXTUALHELP]
>id="acw_fragments_details"
>title="Dettagli dei frammenti"
>abstract="Dettagli dei frammenti"

>[!CONTEXTUALHELP]
>id="acw_create_fragment"
>title="Definisci il tuo frammento"
>abstract="Un frammento è un componente riutilizzabile a cui è possibile fare riferimento in una o più e-mail tra campagne."

Un frammento è un componente riutilizzabile a cui è possibile fare riferimento in una o più e-mail tra campagne. Quando si modifica un frammento, viene aggiornato ogni contenuto che lo utilizza.

Questa funzionalità consente di precreare più blocchi di contenuto personalizzati che possono essere utilizzati dagli utenti di marketing per assemblare rapidamente i contenuti delle e-mail in un processo di progettazione migliorato.

![](assets/fragments.gif)

Per utilizzare al meglio i frammenti:

* Crea frammenti visivi personalizzati, come descritto di seguito.
* Utilizzali il numero di volte necessario nel contenuto tramite E-mail Designer. Consulta [Aggiungere frammenti visivi alle e-mail](../email/use-visual-fragments.md).

>[!AVAILABILITY]
>
>Questa funzionalità è a disponibilità limitata (LA). È limitata ai clienti che eseguono la migrazione **da Adobe Campaign Standard ad Adobe Campaign v8** e non possono essere distribuiti in nessun altro ambiente.

## Creare un frammento visivo {#create-fragments}

Esistono due modi per creare i frammenti:

* Crea un frammento da zero utilizzando il menu dedicato **[!UICONTROL Frammenti]**. [Scopri come](#create-from-scratch)

* Durante la progettazione di un contenuto, salva una parte del contenuto come frammento. [Scopri come](#save-as-fragment)

Una volta salvato, il frammento è disponibile per l’utilizzo in un’e-mail o in un modello e-mail. Indipendentemente dal fatto che sia stato creato da zero o da un contenuto esistente, ora puoi utilizzare questo frammento durante la creazione di qualsiasi contenuto all’interno di Campaign. Vedi [Aggiungi frammenti visivi](../email/use-visual-fragments.md).

### Creare un frammento da zero {#create-from-scratch}

Per creare un frammento da zero, segui la procedura riportata di seguito.

1. [Accedi all&#39;elenco di frammenti](#access-manage-fragments) tramite il menu a sinistra **[!UICONTROL Gestione contenuto]** > **[!UICONTROL Frammenti]**.

   ![](assets/fragments-list.png)

1. Seleziona **[!UICONTROL Crea frammento]**.

1. Inserisci l’etichetta del frammento.

   ![](assets/fragment-create.png)

1. Se necessario, puoi definire opzioni aggiuntive, ad esempio il nome interno del frammento, la relativa cartella e una descrizione.

   >[!NOTE]
   >
   >Per il momento, puoi creare solo frammenti visivi.

1. Fai clic sul pulsante **Crea** per configurare il contenuto del frammento.

1. Viene visualizzato [E-mail Designer](../email/get-started-email-designer.md). Modifica il contenuto in base alle esigenze, come faresti per qualsiasi e-mail all’interno di una campagna. Puoi aggiungere immagini, collegamenti, campi di personalizzazione e contenuti dinamici.

   ![](assets/fragment-designer.png)

1. Quando il frammento è pronto, fai clic su **[!UICONTROL Salva e chiudi]**. È stato aggiunto all&#39;[elenco frammenti](#access-manage-fragments).

Questo frammento è ora pronto per essere utilizzato quando si crea un [e-mail](../email/get-started-email-designer.md) o un [modello di contenuto](use-email-templates.md) all&#39;interno di Campaign. [Scopri come](../email/use-visual-fragments.md)


### Salvare un contenuto come frammento {#save-as-fragment}

Qualsiasi contenuto e-mail può essere salvato come frammento per riutilizzi futuri. Durante la progettazione di un [modello di contenuto](use-email-templates.md) o di una consegna [e-mail](../email/get-started-email-designer.md), puoi salvare una parte del contenuto come frammento visivo. A questo scopo, segui la procedura indicata di seguito:

1. In [E-mail Designer](../email/get-started-email-designer.md), fai clic sul pulsante **Altro** in alto a destra dello schermo.

1. Seleziona **[!UICONTROL Salva come frammento]** dal menu a discesa.

   ![](assets/fragment-save-as.png)

1. Viene visualizzata la schermata **[!UICONTROL Salva come frammento]**. Seleziona gli elementi da includere nel frammento, inclusi i campi di personalizzazione e il contenuto dinamico.

   >[!CAUTION]
   >
   >Potete selezionare solo le sezioni adiacenti. Non puoi selezionare una struttura vuota o un altro frammento.

   ![](assets/fragment-save-as-screen.png)

1. Fai clic su **[!UICONTROL Crea]**. Inserisci il nome del frammento e salvalo.

   ![](assets/fragment-save-confirm.png)

   Il contenuto è ora un frammento autonomo , aggiunto all&#39;[elenco frammenti](#manage-fragments) e accessibile dal menu dedicato. Ora puoi utilizzare questo frammento durante la creazione di qualsiasi [e-mail](../email/get-started-email-designer.md) o [modello di contenuto](use-email-templates.md) all&#39;interno di Campaign. [Scopri come](../email/use-visual-fragments.md)

>[!NOTE]
>
>Eventuali modifiche apportate al nuovo frammento non vengono propagate all’e-mail o al modello di origine. Allo stesso modo, quando il contenuto originale viene modificato all’interno dell’e-mail o del modello, il nuovo frammento non viene modificato.

## Gestire i frammenti {#manage-fragments}

È possibile modificare, aggiornare, duplicare o eliminare un frammento dall’elenco dei frammenti.

### Modificare e aggiornare un frammento {#edit-fragments}

Per modificare un frammento, effettua le seguenti operazioni.

1. Fare clic sul nome del frammento da modificare dall&#39;elenco **[!UICONTROL Frammenti]**.
1. Fai clic sul pulsante **Modifica contenuto** per aprire il contenuto di questo frammento.

   ![](assets/fragment-edit-content.png)

1. Apporta le modifiche necessarie e le salva.

>[!CAUTION]
>
>Qualsiasi modifica a un frammento viene propagata alle consegne e-mail o ai modelli che lo utilizzano.


### Eliminare un frammento {#delete-fragments}

Per eliminare un frammento, effettua le seguenti operazioni:

1. Individua l&#39;elenco dei frammenti e fai clic sul pulsante **[!UICONTROL Altre azioni]** accanto al frammento da eliminare.
1. Fai clic su **Elimina** e conferma.

   ![](assets/fragment-list-more-actions.png)

>[!CAUTION]
>
>Durante l’eliminazione di un frammento di contenuto, le consegne e i modelli e-mail che lo utilizzano vengono aggiornati: il frammento viene rimosso dal contenuto dell’e-mail, ma vi si fa ancora riferimento. Per mantenere il contenuto del frammento in tali consegne e modelli, è necessario interrompere l&#39;ereditarietà prima di eliminare il frammento, [come descritto in questa sezione](use-visual-fragments.md#break-inheritance).
>

### Duplicare un frammento {#duplicate-fragments}

Puoi duplicare facilmente un frammento per crearne uno nuovo. Per duplicare un frammento esistente, effettua le seguenti operazioni:

1. Individua l&#39;elenco dei frammenti e fai clic sul pulsante **[!UICONTROL Altre azioni]** accanto al frammento da eliminare.
1. Fai clic su **Duplica** e conferma.
1. Inserisci l’etichetta del nuovo frammento e salva le modifiche.

   Il frammento viene aggiunto all’elenco dei frammenti. Puoi modificarlo e configurarlo in base alle esigenze.
