---
title: Utilizzare gli schemi
description: Scopri come utilizzare gli schemi.
exl-id: 1433a441-1673-45a2-9fec-be9550fbba0d
source-git-commit: 24691b7d6e71e0a6986a1e1fdd0d709cf869e9dd
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 26%

---

# Utilizzare gli schemi {#schemas}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn3"
>title="Utilizzare gli schemi"
>abstract="Ora puoi accedere ai dettagli di uno schema selezionandone il nome nell’elenco. La modifica dei campi personalizzati è accessibile anche dal pulsante **Modifica dettagli personalizzati**."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=it" text="Consulta le note sulla versione"



>[!CONTEXTUALHELP]
>id="acw_schema"
>title="Schemi"
>abstract="**[!DNL Adobe Campaign]** utilizza schemi basati su XML per definire la struttura fisica e logica dei dati all’interno dell’applicazione. Da questa schermata, puoi visualizzare tutti gli schemi esistenti e accedere ai dettagli di uno schema selezionandone il nome nell’elenco. I filtri sono disponibili per aiutarti a perfezionare l’elenco, ad esempio per visualizzare solo gli schemi modificabili."

## Informazioni sugli schemi {#about}

**[!DNL Adobe Campaign]** utilizza schemi basati su XML per definire la struttura fisica e logica dei dati all’interno dell’applicazione. Uno schema è un documento XML collegato a una tabella di database che definisce:

* Struttura della tabella SQL (nome della tabella, campi, relazioni).
* Struttura dei dati XML (elementi, attributi, gerarchia, tipi, valori predefiniti, etichette).

Gli schemi svolgono un ruolo chiave in:

* Mappatura dei dati dell&#39;applicazione alle tabelle del database.
* Definizione delle relazioni tra gli oggetti dati.
* Specifica la struttura e le proprietà di ciascun campo.

Ogni entità in Adobe Campaign dispone di uno schema dedicato che garantisce la coerenza e l’organizzazione dei dati.

Informazioni dettagliate sugli schemi sono disponibili nella [documentazione della console Campaign](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/schemas){target="_blank"}

## Accedere agli schemi nell’interfaccia utente web {#access}

Gli schemi sono accessibili dal menu **[!UICONTROL Amministrazione]** > **[!UICONTROL Schemi]**.

![](assets/schemas-list.png)

Da questa schermata puoi visualizzare tutti gli schemi esistenti. I filtri sono disponibili per aiutarti a perfezionare l’elenco, ad esempio per visualizzare solo gli schemi modificabili.

Per aprire uno schema, selezionarne il nome. Viene visualizzata una vista di schema dettagliata.

![](assets/schema-details.png)

### Panoramica dello schema {#overview}

La scheda **[!UICONTROL Panoramica]** fornisce una visualizzazione generale dello schema:

* Nella sezione **[!UICONTROL Proprietà]** vengono visualizzate informazioni chiave, ad esempio il nome dello schema, lo spazio dei nomi e il nome della tabella associata.

* La sezione **[!UICONTROL Definizione schema]** mostra dettagli sulla definizione dello schema, come la chiave primaria utilizzata per la riconciliazione dei dati e i relativi collegamenti con altre tabelle.

  Fai clic sul pulsante **[!UICONTROL Anteprima schema]** per visualizzare i diversi campi e collegamenti che compongono lo schema. Questo consente di controllare la struttura completa di uno schema. Se lo schema è stato esteso con campi personalizzati, puoi visualizzarne tutte le estensioni.

* La sezione **[!UICONTROL Content]** visualizza il contenuto XML dello schema, consentendo di passare dall&#39;origine alla sintassi generata.

### Dati schema {#data}

La scheda **[!UICONTROL Dati]** fornisce informazioni sui dati dello schema.

![](assets/schemas-data.png)

## Modifica campi personalizzati {#fields}

I campi personalizzati sono attributi aggiuntivi aggiunti a schemi predefiniti tramite la console Adobe Campaign. Consentono di personalizzare gli schemi includendo nuovi attributi in base alle esigenze dell’organizzazione.

I campi personalizzati possono essere visualizzati in varie schermate, ad esempio nei dettagli del profilo, nell’interfaccia web di Campaign. Puoi controllare quali campi sono visibili e come appaiono nell’interfaccia. A tale scopo, fare clic sul pulsante **[!UICONTROL Modifica dettagli personalizzati]** nel menu **[!UICONTROL Schemi]**.

![](assets/schemas-custom.png)

Informazioni dettagliate su come modificare i campi personalizzati in uno schema, consulta questa sezione: [Configurare i campi personalizzati](../administration/custom-fields.md).
