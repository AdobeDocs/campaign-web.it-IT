---
audience: end-user
title: Creare frammenti di contenuto
description: Scopri come creare frammenti di contenuto
exl-id: 8f37e9e6-3085-4a68-9746-8ca34cfa4242
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '1026'
ht-degree: 21%

---

# Creare frammenti di contenuto {#fragments}

>[!CONTEXTUALHELP]
>id="acw_fragments_create"
>title="Definire i frammenti di contenuto personalizzati"
>abstract="Definisci le proprietà del frammento e il tipo di frammento che desideri creare. Puoi utilizzare E-mail designer o l’editor di espressioni per configurare il contenuto del frammento."

<!-- pas vu dans l'UI-->

>[!CONTEXTUALHELP]
>id="acw_fragments_properties"
>title="Proprietà dei frammenti"
>abstract="Immetti l’etichetta del frammento. Se necessario, puoi definire opzioni aggiuntive, ad esempio, il nome interno del frammento, la relativa cartella e una descrizione."

>[!CONTEXTUALHELP]
>id="acw_fragments_type"
>title="Tipo di frammento di contenuto"
>abstract="Scegli il tipo di frammento che desideri creare. I **frammenti visivi** sono blocchi visivi predefiniti riutilizzabili in più consegne e-mail o in modelli di contenuto. I **frammenti di espressione** sono espressioni predefinite disponibili in una voce dedicata nell’editor di espressioni."

Esistono due modi per creare frammenti di contenuto:

* Crea un frammento da zero utilizzando il menu dedicato **[!UICONTROL Frammenti]**. [Scopri come](#create-from-scratch)
* Durante la progettazione di un contenuto, salva una parte del contenuto come frammento. [Scopri come](#save-as-fragment)

  >[!NOTE]
  >
  >Questa funzionalità è disponibile solo per i frammenti visivi. I frammenti di espressione vengono creati esclusivamente dal menu **Frammenti**.

Una volta salvato, il frammento di contenuto è disponibile per l’utilizzo in qualsiasi consegna o modello di contenuto.

## Creare un frammento di contenuto da zero {#create-from-scratch}

Per creare un frammento di contenuto da zero, effettua le seguenti operazioni.

1. [Accedi all&#39;elenco di frammenti](#access-manage-fragments) tramite il menu a sinistra **[!UICONTROL Gestione contenuto]** > **[!UICONTROL Frammenti]** e seleziona **[!UICONTROL Crea frammento]**.

   ![Schermata dell&#39;elenco di frammenti che mostra l&#39;opzione Crea frammento](assets/fragments-list.png)

1. Immetti l’etichetta del frammento. Se necessario, definisci opzioni aggiuntive, ad esempio il nome interno del frammento, la relativa cartella e una descrizione.

1. Scegliere il tipo di frammento da creare: **Frammento visivo** o **Frammento di espressione**. [Scopri le differenze tra i frammenti visivi e quelli di espressione](fragments.md)

   ![Schermata di creazione del frammento che mostra la selezione del tipo](assets/fragment-create.png)

   >[!AVAILABILITY]
   >
   >I frammenti visivi richiedono un aggiornamento a Campaign v8.6.4. Ulteriori informazioni sono disponibili nelle [Note sulla versione della console client di Campaign v8](https://experienceleague.adobe.com/it/docs/campaign/campaign-v8/releases/release-notes).

1. Fai clic sul pulsante **Crea**.

   * Per **frammenti visivi**, viene visualizzato [E-mail Designer](../email/get-started-email-designer.md). Modifica il contenuto in base alle esigenze, come faresti per qualsiasi e-mail all&#39;interno di una campagna, quindi fai clic sul pulsante **Salva e chiudi**. Aggiungi immagini, collegamenti, campi di personalizzazione e contenuti dinamici.

     ![Schermata Designer e-mail per frammenti visivi](assets/fragment-designer.png)

   * Per **frammenti di espressione**, viene aperto l&#39;editor espressioni. Utilizza le funzionalità di personalizzazione e authoring per creare il contenuto, quindi fai clic su **Conferma**. [Scopri come utilizzare l&#39;editor di espressioni](../personalization/personalize.md)

     ![Schermata dell&#39;editor espressioni per frammenti di espressione](assets/fragment-expression.png)

1. Quando il contenuto è pronto, fai clic su **Salva**.

Il frammento di contenuto è ora pronto per essere utilizzato quando si crea una consegna o un [modello di contenuto](../email/use-email-templates.md) all&#39;interno di Campaign. Scopri come utilizzare i frammenti visivi e di espressione in queste sezioni:
* [Aggiungere frammenti visivi alle e-mail](use-visual-fragments.md)
* [Aggiungere frammenti di espressione all’editor di espressioni](use-expression-fragments.md)

## Salvare un contenuto come frammento visivo {#save-as-fragment}

>[!CONTEXTUALHELP]
>id="acw_fragments_save"
>title="Salva come frammento"
>abstract="Per salvare un contenuto come frammento visivo, seleziona gli elementi che desideri includere nel frammento, inclusi i campi di personalizzazione e il contenuto dinamico. È possibile selezionare solo le sezioni adiacenti. Non è possibile selezionare strutture vuote o altri frammenti di contenuto. Il contenuto sarà quindi un frammento autonomo, aggiunto all’elenco dei frammenti e accessibile dal menu dedicato. Puoi utilizzare questo frammento durante la creazione di qualsiasi e-mail o modello di contenuto all’interno di una campagna."

<!--pas vu dans l'UI-->

Qualsiasi contenuto e-mail può essere salvato come frammento visivo per riutilizzi futuri. Durante la progettazione di un [modello di contenuto](../email/use-email-templates.md) o di una consegna [e-mail](../email/get-started-email-designer.md), salva una parte del contenuto come frammento visivo. A questo scopo, segui la procedura indicata di seguito:

1. In [E-mail Designer](../email/get-started-email-designer.md), fai clic sul pulsante **Altro** in alto a destra dello schermo.

1. Seleziona **[!UICONTROL Salva come frammento]** dal menu a discesa.

   ![Opzione Salva come frammento in E-mail Designer](assets/fragment-save-as.png)

1. Viene visualizzata la schermata **[!UICONTROL Salva come frammento]**. Seleziona gli elementi da includere nel frammento, inclusi i campi di personalizzazione e il contenuto dinamico.

   >[!CAUTION]
   >
   >È possibile selezionare solo le sezioni adiacenti. Non è possibile selezionare strutture vuote o altri frammenti di contenuto.

   ![Schermata Salva come frammento che mostra la selezione dell&#39;elemento](assets/fragment-save-as-screen.png)

1. Fai clic su **[!UICONTROL Crea]**. Inserisci il nome del frammento e salvalo.

   ![Salva schermata di conferma per frammenti visivi](assets/fragment-save-confirm.png)

   Il contenuto è ora un frammento autonomo, aggiunto all&#39;[elenco frammenti](#manage-fragments) e accessibile dal menu dedicato. Usa questo frammento durante la creazione di qualsiasi [e-mail](../email/get-started-email-designer.md) o [modello di contenuto](../email/use-email-templates.md) all&#39;interno di Campaign. [Scopri come](../content/use-visual-fragments.md)

>[!NOTE]
>
>Le modifiche al nuovo frammento non vengono propagate all’e-mail o al modello di origine. Allo stesso modo, quando il contenuto originale viene modificato nell’e-mail o nel modello, il nuovo frammento non viene modificato.

## Gestire i frammenti di contenuto {#manage-fragments}

È possibile modificare, aggiornare, duplicare o eliminare un frammento di contenuto dall’elenco dei frammenti.

### Modificare e aggiornare un frammento di contenuto {#edit-fragments}

Per modificare un frammento di contenuto, effettua le seguenti operazioni.

1. Fare clic sul nome del frammento da modificare dall&#39;elenco **[!UICONTROL Frammenti]**.
1. Fare clic sul pulsante **Modifica contenuto** per aprire il contenuto del frammento.

   ![Pulsante Modifica contenuto per frammenti](assets/fragment-edit-content.png)

1. Apporta le modifiche necessarie e le salva.

>[!CAUTION]
>
>Le modifiche apportate a un frammento vengono propagate alle consegne o ai modelli che lo utilizzano.

### Eliminare un frammento di contenuto {#delete-fragments}

Per eliminare un frammento di contenuto, effettua le seguenti operazioni:

1. Individua l&#39;elenco dei frammenti e fai clic sul pulsante **[!UICONTROL Altre azioni]** accanto al frammento da eliminare.
1. Fai clic su **Elimina** e conferma.

   ![Elimina opzione nell&#39;elenco frammenti](assets/fragment-list-more-actions.png)

>[!CAUTION]
>
>Quando si elimina un frammento, le consegne e i modelli che lo utilizzano vengono aggiornati. Il frammento viene rimosso dal contenuto ma vi si fa ancora riferimento. Per mantenere il contenuto del frammento in tali consegne e modelli, interrompere l&#39;ereditarietà prima di eliminare il frammento, [come descritto in questa sezione](use-visual-fragments.md#break-inheritance).

### Archiviare un frammento di contenuto {#archive}

Per pulire l’elenco dei frammenti, devi archiviare i frammenti che non sono più rilevanti per il tuo marchio. A tale scopo, fai clic sul pulsante **[!UICONTROL Altre azioni]** accanto al frammento desiderato e seleziona **[!UICONTROL Archivia]**. Il frammento viene rimosso dall’elenco dei frammenti, impedendo agli utenti di utilizzarlo in e-mail o modelli futuri.

Per accedere ai frammenti archiviati, utilizza il riquadro dei filtri per visualizzarli. Per annullare l&#39;archiviazione di un frammento, fai clic sul pulsante **[!UICONTROL Altre azioni]** e seleziona **[!UICONTROL Annulla archiviazione]**.

![Annulla archiviazione opzione per frammenti](assets/fragment-unarchive.png)

>[!NOTE]
>
>Se archivi un frammento utilizzato in un contenuto, tale contenuto non viene interessato.

### Duplicare un frammento di contenuto {#duplicate-fragments}

Puoi duplicare facilmente un frammento di contenuto per crearne uno nuovo. Per duplicare un frammento esistente, effettua le seguenti operazioni:

1. Individua l&#39;elenco dei frammenti e fai clic sul pulsante **[!UICONTROL Altre azioni]** accanto al frammento da duplicare.
1. Fai clic su **Duplica** e conferma.
1. Inserisci l’etichetta del nuovo frammento e salva le modifiche.

   Il frammento viene aggiunto all’elenco dei frammenti di contenuto. Modificala e configurala in base alle esigenze.