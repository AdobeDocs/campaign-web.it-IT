---
title: Note preliminari sulla versione dell’interfaccia utente di Campaign Web v8
description: Scopri le nuove funzioni in arrivo con la prossima versione dell’interfaccia utente di Campaign Web
hide: true
hidefromtoc: true
exl-id: a4c6ecb7-d657-46de-aa55-90c4cb45164b
source-git-commit: 2feea0c5a1b021786e58bf6a69a2018ec37ea4b1
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 100%

---

# Note preliminari sulla versione {#e-release}

L’interfaccia utente di Adobe Campaign Web offre continuamente nuove funzioni, miglioramenti alle funzioni esistenti e correzioni di bug. Nelle [note sulla versione](release-notes.md), tutte le modifiche sono consolidate alla fine di ogni mese.

**Le note preliminari sulla versione riportate di seguito sono soggette a modifiche senza preavviso fino alla data di disponibilità del rilascio**. I collegamenti, le schermate e la documentazione aggiornata sono pubblicati nella [note sulla versione](release-notes.md), alla data di rilascio.

## Note sulla versione di luglio {#24-7-release}

**Data di rilascio**: 30-31 luglio 2024

Le seguenti funzioni e i miglioramenti sono disponibili a partire dalla versione di luglio.

### Frammenti di contenuto {#24-7-1}

Ora puoi creare e utilizzare i frammenti di contenuto. Un frammento di contenuto è un componente riutilizzabile a cui è possibile fare riferimento in uno o più messaggi. Quando si modifica un frammento, viene aggiornato ogni contenuto che lo utilizza. Questa funzionalità consente di precreare più blocchi di contenuto personalizzati che possono essere utilizzati dagli utenti di marketing per assemblare rapidamente i contenuti dei messaggi in un processo di progettazione migliorato.

Sono disponibili due tipi di frammenti:

* I **frammenti di espressione** sono espressioni predefinite disponibili in una voce dedicata nell’editor di espressioni.
* I **frammenti visivi** sono blocchi visivi predefiniti che è possibile riutilizzare in più consegne e-mail o in modelli di contenuto. [Ulteriori informazioni](../content/fragments.md)

  >[!AVAILABILITY]
  >
  >I **frammenti visivi** sono in disponibilità limitata (LA). Questa funzionalità è limitata a chi esegue la migrazione **da Adobe Campaign Standard ad Adobe Campaign v8** e non può essere distribuita in nessun altro ambiente.

### Elenchi seed {#24-7-2}

Un’elenco di seed, detto anche. **Gruppo trappola**, è un elenco di indirizzi di seed. Viene utilizzato per includere indirizzi specifici nelle consegne e quindi eseguire il targeting dei profili che non corrispondono ai criteri di targeting definiti. In questo modo, i destinatari che non rientrano nel pubblico della consegna possono riceverla, come farebbe qualsiasi altro destinatario di targeting. Puoi utilizzare gli indirizzi seed quando invii le bozze o per proteggere la mailing list.

### Modelli di notifiche push avanzate {#24-7-3}

Ora puoi inviare notifiche push avanzate. La notifica push avanzata è una forma migliorata di notifica mobile che va oltre i semplici messaggi di testo incorporando elementi multimediali come immagini, pulsanti interattivi o altri contenuti rich media. Con questa versione, è ora disponibile un set di modelli per notifiche push avanzate per le app iOS e Android.

>[!AVAILABILITY]
>
>Questa funzionalità richiede un aggiornamento a Campaign v8.6.3 o v8.7.2. Ulteriori informazioni sono disponibili nelle [Note sulla versione della console client di Campaign v8](https://experienceleague.adobe.com/it/docs/campaign/campaign-v8/releases/release-notes)

### Miglioramenti {#improvements-24-7}

**Gestione cartelle**: è ora possibile gestire autorizzazioni e restrizioni sulle cartelle.
