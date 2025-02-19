---
audience: end-user
title: Aggiungi frammenti visivi alle e-mail
description: Scopri come aggiungere frammenti visivi alle e-mail
badge: label="Disponibilità limitata"
exl-id: 6d6f38f9-9d3e-47cb-beb8-177b5a5d8306
source-git-commit: 1f3f3afb9b21ab37aeea73057d832cea172c00bf
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 14%

---

# Aggiungi frammenti visivi alle e-mail {#use-visual-fragments}

>[!AVAILABILITY]
>
>Questa funzionalità richiede un aggiornamento a Campaign v8.6.4. Ulteriori informazioni sono disponibili nelle [Note sulla versione della console client di Campaign v8](https://experienceleague.adobe.com/it/docs/campaign/campaign-v8/releases/release-notes).

Nell&#39;interfaccia Web di Campaign, i **frammenti visivi** sono blocchi visivi predefiniti che è possibile riutilizzare in più [consegne e-mail](../email/get-started-email-designer.md) o in [modelli di contenuto](../email/use-email-templates.md). Scopri come creare e gestire frammenti di contenuto in [questa sezione](fragments.md).

![](assets/do-not-localize/fragments.gif)

## Utilizzare un frammento visivo {#use-fragment}

>[!CONTEXTUALHELP]
>id="acw_fragments_details"
>title="Opzioni frammenti"
>abstract="Questo riquadro fornisce le opzioni relative al frammento selezionato. Consente di scegliere i dispositivi su cui desideri visualizzare il frammento e di aprirne il contenuto. Per personalizzare ulteriormente il frammento, utilizza la scheda **[!UICONTROL Stili]**. Puoi interrompere anche l’ereditarietà con il frammento visivo originale."

<!-- pas vu dans l'UI-->

Per inserire un frammento visivo in un contenuto e-mail, effettua le seguenti operazioni:

1. Apri qualsiasi contenuto e-mail o modello utilizzando [E-mail Designer](../email/get-started-email-designer.md).

1. Seleziona l&#39;icona **[!UICONTROL Frammenti]** dalla barra a sinistra.

   ![](assets/fragments-in-designer.png)

1. Viene visualizzato l’elenco di tutti i frammenti visivi creati nella sandbox corrente. Puoi eseguire le seguenti azioni:

   * Cerca un frammento specifico iniziando a digitarne l’etichetta.
   * Ordina i frammenti in ordine crescente o decrescente.
   * Modifica la modalità di visualizzazione dei frammenti (scheda o elenco).

   >[!NOTE]
   >
   >I frammenti sono ordinati per data di creazione: i frammenti aggiunti di recente vengono visualizzati per primi nell’elenco.

   Se alcuni frammenti visivi sono stati modificati o aggiunti durante la modifica del contenuto, fai clic sull&#39;icona **Aggiorna** per aggiornare l&#39;elenco con le modifiche più recenti.

1. Trascina un frammento visivo dall’elenco nell’area in cui desideri inserirlo. Come qualsiasi altro componente, puoi spostare il frammento all’interno del contenuto.

1. Seleziona il frammento per visualizzarne le opzioni nel riquadro a destra.

   ![](assets/fragment-right-pane.png)

   Dalla scheda **[!UICONTROL Impostazioni]** puoi effettuare le seguenti operazioni:

   * Scegli i dispositivi su cui vuoi visualizzare il frammento.
   * Fai clic sul pulsante **Modifica contenuto** per aprire il contenuto di questo frammento. [Ulteriori informazioni](../content/fragments.md#edit-fragments)

     Puoi personalizzare ulteriormente il frammento utilizzando la scheda **[!UICONTROL Stili]**.

1. Se necessario, puoi interrompere l’ereditarietà con il frammento visivo originale. [Ulteriori informazioni](#break-inheritance)

   Puoi anche eliminare il frammento dal contenuto o duplicarlo. Queste azioni possono essere eseguite direttamente dal menu contestuale visualizzato sopra il frammento.

1. Aggiungi tutti i frammenti visivi desiderati e **[!UICONTROL Salva]** le modifiche.

### Frammento visivo in modalità di sola lettura {#fragment-readonly}

I diritti di accesso possono essere applicati ai frammenti visivi.

Se non si dispone delle autorizzazioni di modifica per un particolare frammento visivo, il modello di contenuto verrà visualizzato in **modalità di sola lettura**. In questo caso, il pulsante **[!UICONTROL Modifica contenuto]** viene sostituito dal pulsante **[!UICONTROL Visualizza contenuto]**, che consente di visualizzare il frammento senza apportare modifiche.

![](assets/fragment-readonly.png){zoomable="yes"}

Come mostrato di seguito, tutte le icone delle funzioni sono disattivate, limitando l’interazione alla sola visualizzazione.

![](assets/fragment-readonly-view.png){zoomable="yes"}

## Interrompi ereditarietà {#break-inheritance}

Quando modifichi un frammento visivo, le modifiche vengono sincronizzate. Vengono propagati automaticamente a tutte le consegne e-mail e ai modelli di contenuto contenenti tale frammento.

I frammenti aggiunti a un messaggio e-mail o a un modello di contenuto vengono sincronizzati per impostazione predefinita.

Tuttavia, puoi interrompere l’ereditarietà dal frammento originale. In tal caso, il contenuto del frammento viene copiato nella progettazione corrente e le modifiche non vengono più sincronizzate.

Per interrompere l’ereditarietà, effettua le seguenti operazioni:

1. Seleziona il frammento visivo.

1. Fai clic sull’icona Sblocca nella barra degli strumenti contestuale.

   ![](assets/fragment-break-inheritance.png)

1. Il frammento diventa un elemento autonomo non più collegato al frammento originale. Modificalo come qualsiasi altro componente del contenuto. [Ulteriori informazioni](../email/content-components.md)
