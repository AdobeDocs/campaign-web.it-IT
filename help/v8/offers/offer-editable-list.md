---
audience: end-user
title: Aggiungere un elenco modificabile allo schema delle offerte
description: Scopri come esporre un collegamento di raccolta personalizzata come elenco modificabile direttamente nella schermata dei dettagli dell’offerta.
feature: Offers
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 043cc60da1938800404964aa7e698f959ef908fd
workflow-type: tm+mt
source-wordcount: 449
ht-degree: 1%

---

# Aggiungere un elenco modificabile allo schema delle offerte {#offer-editable-list}

Quando [estendi lo  [!DNL nms:offer] schema](../administration/schemas.md) con un collegamento di raccolta personalizzato, ad esempio un set di segmenti collegati a un&#39;offerta, puoi esporla come elenco modificabile direttamente nella sezione **[!UICONTROL Opzioni personalizzate]** dell&#39;offerta. Invece di gestire i record correlati tramite una schermata separata, la raccolta viene riprodotta come elenco nei dettagli dell’offerta e puoi creare nuovi record correlati in linea tramite una finestra di dialogo dedicata.

>[!NOTE]
>
>Questa funzionalità è attualmente disponibile solo per lo schema di offerta.

## Aggiungi un campo collegamento raccolta {#add-field}

1. Estendi lo schema [!DNL nms:offer] con la tua raccolta personalizzata, quindi passa al menu **[!UICONTROL Schemi]**, apri lo schema **[!UICONTROL Offerte di marketing]** e fai clic su **[!UICONTROL Modifica schermo]**. [Ulteriori informazioni](../administration/schemas-browse-access.md#screen-def).

   ![Schermata che mostra il pulsante di definizione dello schermo.](assets/offers-editable-list.png){zoomable="yes"}

1. Nella sezione **[!UICONTROL Configurazione schermata dettagli]**, fai clic sull&#39;icona dei puntini di sospensione sopra la tabella **[!UICONTROL Elenco di campi personalizzati]** e scegli **[!UICONTROL Seleziona attributi]**. [Ulteriori informazioni](../administration/schemas-custom-fields.md).

   ![Schermata che mostra il pulsante di definizione dello schermo.](assets/offers-editable-list-0.png){zoomable="yes"}

1. Sfoglia gli attributi e seleziona il collegamento alla raccolta personalizzata, identificato dalla relativa icona.

   ![Schermata che mostra il selettore attributi con un attributo di collegamento della raccolta.](assets/offers-editable-list-1.png){zoomable="yes"}

   >[!NOTE]
   >
   >I campi del collegamento di raccolta non possono essere resi obbligatori e non supportano gli attributi secondari. Per impostazione predefinita, si estendono su due colonne del modulo.

1. Conferma la selezione. Il collegamento della raccolta viene aggiunto alla tabella **[!UICONTROL Elenco di campi personalizzati]**, il cui tipo è **[!UICONTROL raccolta]**.

   ![Schermata che mostra gli attributi aggiunti.](assets/offers-editable-list-2.png){zoomable="yes"}

## Configurare l’elenco modificabile della raccolta {#configure-list}

1. Fai clic sull&#39;icona con i puntini di sospensione nella riga del campo della raccolta e scegli **[!UICONTROL Modifica]** per aprire la finestra di dialogo **[!UICONTROL Impostazioni collegamento raccolta]**.

   ![Schermata che mostra il pulsante Modifica.](assets/offers-editable-list-3.png){zoomable="yes"}

1. Nella scheda **[!UICONTROL Generale]**, impostare facoltativamente una condizione **[!UICONTROL Visibile se]** o abilitare **[!UICONTROL Sola lettura]**.

   ![Schermata che mostra la schermata dell&#39;edizione.](assets/offers-editable-list-4.png){zoomable="yes"}

1. Nella scheda **[!UICONTROL Configurazione schermo]**, fare clic su **[!UICONTROL Seleziona attributi]** e selezionare gli attributi da utilizzare quando si aggiunge un nuovo elemento all&#39;elenco, ad esempio un nome di segmento e un campo personalizzato.

   ![Schermata che mostra la scheda di configurazione dello schermo della finestra di dialogo delle impostazioni del collegamento della raccolta.](assets/offers-editable-list-5.png){zoomable="yes"}

1. Nella scheda **[!UICONTROL Layout]**, mantieni o cancella **[!UICONTROL Estendi due colonne]**.

1. Fai clic su **[!UICONTROL Conferma]**, quindi su **[!UICONTROL Salva]** la definizione dello schermo.

## Utilizzare l’elenco modificabile in un’offerta {#use-list}

1. Dal menu a sinistra, fai clic su **Offerte** e apri un&#39;offerta. [Ulteriori informazioni](create-offer.md#create)

   ![Schermata che mostra la schermata dell&#39;offerta.](assets/offers-editable-list-7.png){zoomable="yes"}

1. Accedi alle proprietà dell’offerta. Viene eseguito il rendering della raccolta come elenco nella sezione **Opzioni personalizzate**.

   ![Schermata che mostra il rendering dell&#39;elenco modificabile nella schermata dei dettagli dell&#39;offerta.](assets/offers-editable-list-6.png){zoomable="yes"}

1. Fai clic su **[!UICONTROL Aggiungi]** per visualizzare gli attributi configurati, compilali e fai clic su **[!UICONTROL Conferma]**. Il nuovo elemento viene aggiunto all’elenco.

   È possibile aggiungere più elementi allo stesso elenco e i dettagli dell’offerta possono contenere più di un elenco modificabile.

1. Fai clic su **[!UICONTROL Salva]**.

<!--
Each element added through the editable list creates a new related record. For instance, adding a segment to an offer generates the following payload:

```xml
<offer ...>
  <offerSegment segmentName="..." _operation="insert"/>
</offer>
```
-->