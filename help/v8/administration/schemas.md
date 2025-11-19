---
title: Utilizzare gli schemi
description: Scopri come utilizzare gli schemi.
exl-id: 1433a441-1673-45a2-9fec-be9550fbba0d
source-git-commit: 934a37cfebfacd2df0b7610285252d883611f252
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 14%

---

# Utilizzare gli schemi {#schemas}

>[!CONTEXTUALHELP]
>id="acw_schema"
>title="Schemi"
>abstract="**[!DNL Adobe Campaign]** utilizza schemi basati su XML per definire la struttura fisica e logica dei dati all’interno dell’applicazione. Da questa schermata, puoi visualizzare tutti gli schemi esistenti e accedere ai dettagli di uno schema selezionandone il nome nell’elenco. I filtri sono disponibili per aiutarti a perfezionare l’elenco, ad esempio per visualizzare solo gli schemi modificabili."

## Informazioni sugli schemi {#about}

**[!DNL Adobe Campaign]** utilizza schemi basati su XML per definire la struttura fisica e logica dei dati all’interno dell’applicazione. Uno schema è un documento XML collegato a una tabella di database che definisce:

* Struttura della tabella SQL, inclusi nome della tabella, campi e relazioni.
* Struttura dei dati XML, inclusi elementi, attributi, gerarchia, tipi, valori predefiniti ed etichette.

Gli schemi svolgono un ruolo chiave in:

* Mappatura dei dati dell&#39;applicazione alle tabelle del database.
* Definizione delle relazioni tra gli oggetti dati.
* Specifica la struttura e le proprietà di ciascun campo.

Ogni entità in Adobe Campaign dispone di uno schema dedicato che garantisce la coerenza e l’organizzazione dei dati.

Informazioni dettagliate sugli schemi sono disponibili nella [documentazione della console Campaign](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/schemas){target="_blank"}.

## Accedere agli schemi nell’interfaccia utente web {#access}

Gli schemi sono accessibili dal menu **[!UICONTROL Amministrazione]** > **[!UICONTROL Schemi]**.

![Schemi con la schermata dell&#39;elenco che mostra gli schemi e i filtri disponibili](assets/schemas-list.png)

Da questa schermata puoi visualizzare tutti gli schemi esistenti. I filtri sono disponibili per aiutarti a perfezionare l’elenco, ad esempio per visualizzare solo gli schemi modificabili.

Per aprire uno schema, selezionarne il nome. Viene visualizzata una vista di schema dettagliata.

![Schermata dei dettagli dello schema che mostra le proprietà e il contenuto dello schema](assets/schema-details.png)

### Panoramica dello schema {#overview}

La scheda **[!UICONTROL Panoramica]** fornisce una visualizzazione generale dello schema:

* Nella sezione **[!UICONTROL Proprietà]** vengono visualizzate informazioni chiave, ad esempio il nome dello schema, lo spazio dei nomi e il nome della tabella associata.

* La sezione **[!UICONTROL Definizione schema]** mostra i dettagli sulla definizione dello schema, inclusa la chiave primaria utilizzata per la riconciliazione dei dati e i relativi collegamenti ad altre tabelle.

  Fai clic sul pulsante **[!UICONTROL Anteprima schema]** per visualizzare i diversi campi e collegamenti che compongono lo schema. Questo consente di controllare la struttura completa di uno schema. Se lo schema è stato esteso con campi personalizzati, puoi visualizzarne tutte le estensioni.

* La sezione **[!UICONTROL Content]** visualizza il contenuto XML dello schema, consentendo di passare dall&#39;origine alla sintassi generata.

### Dati schema {#data}

La scheda **[!UICONTROL Dati]** fornisce informazioni sui dati dello schema.

![Scheda dati dello schema che mostra la struttura dati e gli attributi](assets/schemas-data.png)

## Configurare la definizione della schermata {#screen-definition}

### Modifica campi personalizzati {#fields}

I campi personalizzati sono attributi aggiuntivi aggiunti a schemi predefiniti tramite la console Adobe Campaign. Consentono di personalizzare gli schemi includendo nuovi attributi in base alle esigenze dell’organizzazione.

I campi personalizzati possono essere visualizzati in varie schermate, ad esempio nei dettagli del profilo nell’interfaccia web di Campaign. Puoi controllare quali campi sono visibili e come appaiono nell’interfaccia. A tale scopo, fare clic sul pulsante **[!UICONTROL Screen edition]** nel menu **[!UICONTROL Schemi]**.

![Schermata dei campi personalizzati con attributi modificabili](assets/schemas-custom.png)

Fai clic su **[!UICONTROL Anteprima]** per visualizzare i campi personalizzati in una schermata di esempio.

Per informazioni dettagliate su come modificare i campi personalizzati in uno schema, consulta questa sezione: [Configurare i campi personalizzati](../administration/custom-fields.md).

### Aggiungere elenchi di raccolte {#collection-lists}

Questa sezione **Elenco di elenchi personalizzati** ti consente di definire i collegamenti alle raccolte, ad esempio gli acquisti. I dati correlati vengono quindi visualizzati nelle schermate del profilo tramite una scheda dedicata.

>[!NOTE]
>
>Attualmente, questa funzionalità è disponibile solo per lo schema Destinatari.

1. Per aggiungere un elenco di raccolte all&#39;interfaccia, fare clic sul pulsante con i puntini di sospensione e scegliere **Seleziona elenchi personalizzati**.

   ![Creazione elenchi di raccolte](assets/schemas-collection1.png)

1. Seleziona uno degli elenchi personalizzati disponibili, ad esempio acquisti, quindi fai clic su **Conferma**.

   ![Creazione elenchi di raccolte](assets/schemas-collection2.png)

1. Passare al menu **Profili** e filtrare i profili che hanno effettuato acquisti.

   ![Creazione elenchi di raccolte](assets/schemas-collection3.png)

1. Fai clic su un profilo. Viene visualizzata la nuova scheda. Se necessario, puoi aggiungere altre colonne.

   ![Creazione elenchi di raccolte](assets/schemas-collection4.png)
