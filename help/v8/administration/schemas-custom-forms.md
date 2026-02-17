---
title: Utilizzare i moduli personalizzati
description: Scopri come creare, modificare e gestire i record negli schemi personalizzati utilizzando i moduli di immissione dati.
source-git-commit: be4876090ecaac853aaa88948505c444bef27ec2
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# Utilizzare i moduli personalizzati {#custom-forms}

I moduli personalizzati sono interfacce di immissione dati che consentono di gestire record in schemi personalizzati direttamente dall&#39;interfaccia utente Web. Ogni modulo personalizzato corrisponde a uno schema personalizzato specifico e fornisce una vista a elenco per sfogliare i record e una vista di dettaglio per creare, modificare ed eliminare i record.

I moduli personalizzati si basano sulla definizione del modulo dello schema (definizione dello schermo), che configura quali campi vengono visualizzati e come sono organizzati.

>[!NOTE]
>
>I moduli personalizzati sono disponibili solo per gli schemi che hanno una definizione di modulo configurata.

## Creare e pubblicare gli schemi personalizzati {#form-schema}

Devi innanzitutto creare e pubblicare gli schemi personalizzati. Per istruzioni dettagliate, consulta questa [sezione](schemas-create-publish.md).

Di seguito è riportato il modello dati utilizzato per questo esempio:

* Un destinatario effettua diversi acquisti
* Un acquisto è collegato a un prodotto
* Un prodotto è collegato a un marchio

Per questo caso d’uso, vengono creati tre schemi: Schemi Purchases, Products e Brand. Ecco un esempio:

![Moduli personalizzati](assets/schemas-forms.png)

## Configurare la definizione della schermata {#form-screen-schema}

Definisci quali campi vengono visualizzati e come sono organizzati. Per istruzioni dettagliate, consulta questa [sezione](schemas-browse-access.md#screen-def).

Di seguito è riportato un esempio per lo schema Marchio in cui viene aggiunto l’elenco personalizzato Prodotti. Il modulo visualizza quindi l’elenco dei prodotti collegati al brand.

![Moduli personalizzati](assets/schemas-forms2.png)

Per lo schema Prodotti, viene aggiunto l’elenco personalizzato Acquisti. E per lo schema Purchases, i campi Product e Recipient.

## Creare voci di navigazione {#form-screen-entries}

Creare cartelle in Esplora risorse per accedere al modulo personalizzato. Per istruzioni dettagliate, consulta questa [sezione](schemas-create-publish.md#navigation).

![Moduli personalizzati](assets/schemas-forms3.png)

Nella vista a elenco vengono visualizzati tutti i record per tale schema. Se nello schema è configurata una definizione di modulo, l&#39;elenco è modificabile ed è possibile creare, modificare ed eliminare record.
![Moduli personalizzati](assets/schemas-forms4.png)

Puoi quindi:

* **Visualizza e modifica record**: fare clic su un record nella visualizzazione elenco per aprirlo nella visualizzazione dettagli e modificare direttamente i campi.
* **Crea nuovi record**: fai clic sul pulsante **[!UICONTROL Crea]** e compila i campi obbligatori. Per i campi collegati, utilizza l’icona di ricerca per selezionare tra i record correlati disponibili.
* **Elimina record**: selezionare un record e utilizzare l&#39;azione di eliminazione disponibile nella visualizzazione dettagli record o elenco.
* **Visualizza dati correlati in schede**: accedi ai record correlati tramite schede dedicate nella visualizzazione dettagli (ad esempio, visualizza tutti i prodotti collegati a un brand o tutti gli acquisti collegati a un prodotto).
* **Applica filtri**: utilizza il pannello dei filtri per perfezionare la visualizzazione elenco e trovare record specifici in base a qualsiasi campo nello schema.
* **Personalizza colonne elenco**: configura quali colonne vengono visualizzate per impostazione predefinita nelle visualizzazioni elenco tramite la definizione dello schermo.
