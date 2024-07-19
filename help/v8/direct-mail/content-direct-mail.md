---
audience: end-user
title: Progettare una consegna direct mail
description: Scopri come progettare la consegna di direct mailing con Adobe Campaign Web
exl-id: aefba651-4125-4b1e-992f-1fe90fd95e4c
source-git-commit: 60484d08a68a5caaf91074c9ce543d8a44d44ab7
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 21%

---

# Progettare il file di estrazione {#design-direct-mail}

>[!CONTEXTUALHELP]
>id="acw_directmail_content"
>title="Contenuto del file di estrazione"
>abstract="Fai clic sul pulsante **Modifica contenuto** per iniziare a progettare il file di estrazione richiesto dal provider di direct mail. Questo consente di definire le proprietà del file, come l’etichetta e il formato, e di specificare le colonne da includere nel file."

>[!CONTEXTUALHELP]
>id="acw_directmail_properties_file"
>title="Proprietà file"
>abstract="Configura le proprietà del file di estrazione, ad esempio il nome e il formato. Puoi personalizzare il nome del file utilizzando gli attributi del database attraverso l’editor di espressioni."

>[!CONTEXTUALHELP]
>id="acw_directmail_properties_content"
>title="Contenuto"
>abstract="In questa sezione, specifica le colonne da visualizzare nel file di estrazione. Al termine, puoi ottenere un’anteprima del file di estrazione utilizzando il pulsante **Simula contenuto**."

Per progettare il contenuto del file di estrazione generato dalla consegna di direct mailing, fai clic sul pulsante **[!UICONTROL Modifica contenuto]** nella pagina di consegna, quindi configura le proprietà e il contenuto del file.

## Configurare le proprietà del file di estrazione {#properties}

1. Nel campo **[!UICONTROL Nome file]**, specifica il nome desiderato per il file di estrazione. Puoi personalizzare il nome del file utilizzando gli attributi del database. A questo scopo, fai clic sull&#39;icona **[!UICONTROL Apri finestra di dialogo per personalizzazione]** per aprire l&#39;editor espressioni. [Scopri come personalizzare i contenuti](../personalization/personalize.md)

1. Nel campo **[!UICONTROL Formato file]**, scegliere il formato desiderato per il file di estrazione: **Testo**, **Testo con colonne fisse**, **CSV (Excel)** o **XML**.

1. Espandi la sezione **[!UICONTROL Formato estrazione]** per accedere a opzioni specifiche relative al formato del file di estrazione. I valori disponibili dipendono dal formato selezionato.

+++ Opzioni di formato di estrazione disponibili

   * **[!UICONTROL Utilizza la prima riga come intestazione di colonna]** (formato Testo/CSV (Excel)): attiva questa opzione per utilizzare la prima colonna come intestazione.
   * **[!UICONTROL Separatore colonne]** (formato testo): specificare il carattere da utilizzare come separatore colonne nel file di estrazione.
   * **[!UICONTROL Delimitatore stringa]** (formato testo): specifica come delimitare le stringhe nel file di estrazione.
   * **[!UICONTROL Fine riga]** (formato testo): specifica come delimitare la fine delle righe nel file di estrazione.
   * **[!UICONTROL Codifica]**: scegli la codifica del file di estrazione.
   * **[!UICONTROL Formato data e separatori]**: specificare la modalità di formattazione delle date nel file di estrazione.
   * **[!UICONTROL Formato numero]**: specificare la modalità di formattazione dei numeri nel file di estrazione.
   * **[!UICONTROL Esporta etichette invece dei valori interni delle enumerazioni]**: attiva questa opzione se esporti valori di enumerazione e desideri recuperare le etichette delle colonne, che sono più facili da comprendere, piuttosto che gli ID interni.

+++

1. Attiva l&#39;opzione **[!UICONTROL Quantità richiesta]** per limitare il numero di destinatari per la consegna.

   ![](assets/dm-content-details.png){zoomable="yes"}

## Configurare le colonne del file di estrazione {#content}

Nella sezione **[!UICONTROL Contenuto]**, specifica le colonne da visualizzare nel file di estrazione. Per farlo, segui questi passaggi:

1. Fare clic sul pulsante **[!UICONTROL Aggiungi attributo]** per creare una nuova colonna.
1. Scegli l’attributo da visualizzare nella colonna, quindi conferma. È possibile sfruttare l&#39;editor espressioni per selezionare l&#39;attributo da utilizzare facendo clic sul pulsante **[!UICONTROL Modifica espressione]**.

   ![](assets/dm-add-attribute.png)

1. Una volta aggiunta la colonna, puoi modificarne l’etichetta e l’attributo associato utilizzando l’icona di modifica.
1. Ripeti questi passaggi per aggiungere tutte le colonne necessarie per il file di estrazione.
1. Per ordinare il file di estrazione utilizzando una delle colonne, fare clic sull&#39;icona nella colonna **[!UICONTROL Ordinamento]** e selezionare il metodo di ordinamento desiderato.
1. Per modificare la posizione di una colonna, utilizzare le frecce su e giù.

![](assets/dm-content-attributes.png)

Ora puoi visualizzare in anteprima il file di estrazione e inviare la consegna per generare il file di estrazione. [Scopri come testare e inviare messaggi di direct mailing](send-direct-mail.md)
