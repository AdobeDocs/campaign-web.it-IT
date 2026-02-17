---
title: Informazioni sugli schemi
description: Scopri come utilizzare gli schemi.
exl-id: 1433a441-1673-45a2-9fec-be9550fbba0d
source-git-commit: 28f7bcf5f65671136be25c79b414f149532b749f
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 6%

---

# Informazioni sugli schemi {#schemas}

>[!CONTEXTUALHELP]
>id="acw_schema"
>title="Schemi"
>abstract="Adobe Campaign utilizza schemi basati su XML per definire la struttura fisica e logica dei dati all’interno dell’applicazione. Da questa schermata è possibile visualizzare tutti gli schemi esistenti, accedere ai dettagli degli schemi, configurare moduli personalizzati e creare o estendere schemi direttamente dall&#39;interfaccia utente Web."

**[!DNL Adobe Campaign]** utilizza schemi basati su XML per definire la struttura fisica e logica dei dati all’interno dell’applicazione. Uno schema è un documento XML collegato a una tabella di database che definisce:

* Struttura della tabella SQL, inclusi nome della tabella, campi e relazioni.
* Struttura dei dati XML, inclusi elementi, attributi, gerarchia, tipi, valori predefiniti ed etichette.

Gli schemi svolgono un ruolo chiave in:

* Mappatura dei dati dell&#39;applicazione alle tabelle del database.
* Definizione delle relazioni tra gli oggetti dati.
* Specifica la struttura e le proprietà di ciascun campo.

Ogni entità in Adobe Campaign dispone di uno schema dedicato che garantisce la coerenza e l’organizzazione dei dati.

L’interfaccia degli schemi consente di:

* [Accesso e personalizzazione degli schemi](schemas-browse-access.md) - Visualizzazione degli schemi disponibili, esplorazione dei relativi dettagli e personalizzazione della visualizzazione dello schermo
* [Configura colonne elenco](schemas-list-columns.md) - Configura quali colonne vengono visualizzate per impostazione predefinita nelle visualizzazioni elenco.
* [Modifica campi personalizzati](schemas-custom-fields.md) - Configura i campi personalizzati da visualizzare nelle schermate di dettaglio e organizzali in sezioni.
* [Aggiungi elenchi raccolta](schemas-collection-lists.md) - Aggiungi elenchi raccolta per visualizzare i dati correlati nelle schermate del profilo.
* [Crea e gestisci schemi](schemas-create-publish.md#create-schemas) - Crea nuovi schemi ed estendi quelli esistenti
* [Pubblicare e sincronizzare gli schemi](schemas-create-publish.md#publish) - Sincronizzare le modifiche allo schema con la struttura del database.
* [Operazioni con i moduli personalizzati](schemas-custom-forms.md) - Creazione, modifica e gestione di record negli schemi personalizzati tramite i moduli di immissione dati.

>[!NOTE]
>
>Per gestire gli schemi è necessario disporre dei diritti di amministratore.

Informazioni dettagliate sugli schemi sono disponibili nella [documentazione della console Campaign](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/schemas){target="_blank"}.
