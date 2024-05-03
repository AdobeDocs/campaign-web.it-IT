---
audience: end-user
title: Aggiungi frammenti visivi alle e-mail
description: Scopri come aggiungere frammenti visivi alle e-mail
hide: true
hidefromtoc: true
source-git-commit: 341e2a5ab073405d3be19068f85b9ea917b32a69
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 4%

---

# Aggiungi frammenti visivi alle e-mail {#use-visual-fragments}

È possibile utilizzare un frammento visivo in una [consegna e-mail](get-started-email-designer.md), o in un [modello di contenuto](use-email-templates.md). I passaggi sono descritti di seguito.


>[!NOTE]
>
>Scopri come creare e gestire i frammenti in [questa sezione](fragments.md).


## Utilizzare un frammento {#use-fragment}

Per inserire un frammento in un contenuto e-mail, effettua le seguenti operazioni:

1. Apri qualsiasi contenuto e-mail o modello utilizzando [E-mail Designer](get-started-email-designer.md).

1. Seleziona la **[!UICONTROL Frammenti]** dalla barra a sinistra.

   ![](assets/fragments-in-designer.png)

1. Viene visualizzato l’elenco di tutti i frammenti visivi creati nella sandbox corrente. Puoi eseguire le seguenti azioni:

   * Cerca un frammento specifico iniziando a digitarne l’etichetta.
   * Ordina i frammenti in ordine crescente o decrescente.
   * Modifica la modalità di visualizzazione dei frammenti (scheda o elenco).

   >[!NOTE]
   >
   >I frammenti sono ordinati per data di creazione: i frammenti visivi aggiunti di recente vengono visualizzati per primi nell’elenco.

   Se alcuni frammenti sono stati modificati o aggiunti durante la modifica del contenuto, fai clic sul pulsante **Aggiorna** per aggiornare l’elenco con le modifiche più recenti.

1. Trascina un frammento dall’elenco nell’area in cui desideri inserirlo. Come qualsiasi altro componente, puoi spostare il frammento all’interno del contenuto.

1. Seleziona il frammento per visualizzarne le opzioni nel riquadro a destra.

   ![](assets/fragment-right-pane.png)

   Dalla sezione **[!UICONTROL Impostazioni]** , è possibile:

   * Scegli i dispositivi su cui vuoi visualizzare il frammento.
   * Apri il frammento in una nuova scheda per modificarlo, se necessario. [Ulteriori informazioni](../email/fragments.md#edit-fragments)

   Puoi personalizzare ulteriormente il frammento utilizzando **[!UICONTROL Stili]** scheda.

1. Se necessario, puoi interrompere l’ereditarietà con il frammento originale. [Ulteriori informazioni](#break-inheritance)
Puoi anche eliminare il frammento dal contenuto o duplicarlo. Queste azioni possono essere eseguite direttamente dal menu contestuale visualizzato sopra il frammento.

1. Aggiungi tutti i frammenti desiderati e **[!UICONTROL Salva]** le tue modifiche.

## Interrompi ereditarietà {#break-inheritance}

Quando modifichi un frammento visivo, le modifiche vengono sincronizzate. Vengono propagati automaticamente a tutte le consegne e-mail e ai modelli di contenuto contenenti tale frammento.

I frammenti aggiunti a un messaggio e-mail o a un modello di contenuto vengono sincronizzati per impostazione predefinita.

Tuttavia, puoi interrompere l’ereditarietà dal frammento originale. In tal caso, il contenuto del frammento viene copiato nella progettazione corrente e le modifiche non vengono più sincronizzate.

Per interrompere l’ereditarietà, effettua le seguenti operazioni:

1. Seleziona il frammento.

1. Fai clic sull’icona Sblocca nella barra degli strumenti contestuale.

   ![](assets/fragment-break-inheritance.png)

1. Il frammento diventa un elemento autonomo non più collegato al frammento originale. Modificalo come qualsiasi altro componente del contenuto. [Ulteriori informazioni](content-components.md)
