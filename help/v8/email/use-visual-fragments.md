---
audience: end-user
title: Aggiungi frammenti visivi alle e-mail
description: Scopri come aggiungere frammenti visivi alle e-mail
badge: label="Disponibilità limitata"
exl-id: 6d6f38f9-9d3e-47cb-beb8-177b5a5d8306
source-git-commit: 3b602342885c16c09b5bc97015fa039c153c9ded
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 9%

---

# Aggiungi frammenti visivi alle e-mail {#use-visual-fragments}

Puoi utilizzare un frammento visivo in una [consegna e-mail](get-started-email-designer.md) o in un [modello di contenuto](use-email-templates.md). I passaggi sono descritti di seguito. Scopri come creare e gestire i frammenti in [questa sezione](fragments.md).

>[!AVAILABILITY]
>
>Questa funzionalità è a disponibilità limitata (LA). È limitata ai clienti che eseguono la migrazione **da Adobe Campaign Standard ad Adobe Campaign v8** e non possono essere distribuiti in nessun altro ambiente.

## Utilizzare un frammento {#use-fragment}

Per inserire un frammento in un contenuto e-mail, effettua le seguenti operazioni:

1. Apri qualsiasi contenuto e-mail o modello utilizzando [E-mail Designer](get-started-email-designer.md).

1. Seleziona l&#39;icona **[!UICONTROL Frammenti]** dalla barra a sinistra.

   ![](assets/fragments-in-designer.png)

1. Viene visualizzato l’elenco di tutti i frammenti visivi creati nella sandbox corrente. Puoi eseguire le seguenti azioni:

   * Cerca un frammento specifico iniziando a digitarne l’etichetta.
   * Ordina i frammenti in ordine crescente o decrescente.
   * Modifica la modalità di visualizzazione dei frammenti (scheda o elenco).

   >[!NOTE]
   >
   >I frammenti sono ordinati per data di creazione: i frammenti visivi aggiunti di recente vengono visualizzati per primi nell’elenco.

   Se alcuni frammenti sono stati modificati o aggiunti durante la modifica del contenuto, fai clic sull&#39;icona **Aggiorna** per aggiornare l&#39;elenco con le modifiche più recenti.

1. Trascina un frammento dall’elenco nell’area in cui desideri inserirlo. Come qualsiasi altro componente, puoi spostare il frammento all’interno del contenuto.

1. Seleziona il frammento per visualizzarne le opzioni nel riquadro a destra.

   ![](assets/fragment-right-pane.png)

   Dalla scheda **[!UICONTROL Impostazioni]** puoi effettuare le seguenti operazioni:

   * Scegli i dispositivi su cui vuoi visualizzare il frammento.
   * Fai clic sul pulsante **Modifica contenuto** per aprire il contenuto di questo frammento. [Ulteriori informazioni](../email/fragments.md#edit-fragments)

     Puoi personalizzare ulteriormente il frammento utilizzando la scheda **[!UICONTROL Stili]**.

1. Se necessario, puoi interrompere l’ereditarietà con il frammento originale. [Ulteriori informazioni](#break-inheritance)
Puoi anche eliminare il frammento dal contenuto o duplicarlo. Queste azioni possono essere eseguite direttamente dal menu contestuale visualizzato sopra il frammento.

1. Aggiungi tutti i frammenti desiderati e **[!UICONTROL Salva]** le modifiche.

## Interrompi ereditarietà {#break-inheritance}

Quando modifichi un frammento visivo, le modifiche vengono sincronizzate. Vengono propagati automaticamente a tutte le consegne e-mail e ai modelli di contenuto contenenti tale frammento.

I frammenti aggiunti a un messaggio e-mail o a un modello di contenuto vengono sincronizzati per impostazione predefinita.

Tuttavia, puoi interrompere l’ereditarietà dal frammento originale. In tal caso, il contenuto del frammento viene copiato nella progettazione corrente e le modifiche non vengono più sincronizzate.

Per interrompere l’ereditarietà, effettua le seguenti operazioni:

1. Seleziona il frammento.

1. Fai clic sull’icona Sblocca nella barra degli strumenti contestuale.

   ![](assets/fragment-break-inheritance.png)

1. Il frammento diventa un elemento autonomo non più collegato al frammento originale. Modificalo come qualsiasi altro componente del contenuto. [Ulteriori informazioni](content-components.md)
