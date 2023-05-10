---
audience: end-user
title: Importare i destinatari da un file
description: Scopri come importare i destinatari da un file esterno
badge: label="Alpha" type="Positive"
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: ef8418294540ee0462725cdaf6824ba7ee4d9b59
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 100%

---

# Importare i destinatari da un file {#audience-from-file}

Puoi aggiungere o aggiornare i contatti dall’interfaccia di consegna caricando un file di testo (TXT) o un file di valori separati da virgole (CSV). Questi verranno poi aggiunti al database.

>[!NOTE]
>
>Puoi anche creare un flusso di lavoro di importazione per aggiungere o aggiornare più profili.


Per aggiungere profili da un file locale direttamente dall’interfaccia, effettua le seguenti operazioni:

1. Nella finestra di creazione della consegna, fai clic sul pulsante **Seleziona pubblico** e scegli l’opzione **Seleziona da file**.
1. Seleziona il file locale da caricare.
1. Definisci le impostazioni della colonna e il formato dei dati. Puoi saltare una colonna utilizzando l’interruttore **Ignora colonna**.
1. Visualizza in anteprima la modalità di mappatura dei dati nella sezione centrale dello schermo.
1. Fai clic su **Conferma** una volta che le impostazioni sono corrette.

Durante la creazione e la personalizzazione del contenuto del messaggio, puoi selezionare i campi dal file di input nell’editor di personalizzazione.

## File di esempio {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="File di esempio"
>abstract="Formati di file supportati: txt, csv. Utilizza la prima riga come intestazione di colonna."


```json
{
lastname,firstname,birthdate,email,crmID
Smith,Hayden,23/05/1989,hayden.smith@example.com,124365
Mars,Daniel,17/11/1987,dannymars@example.com,123545
Smith,Clara,08/02/1989,clara.smith@example.com,124567
Durance,Allison,15/12/1978,allison.durance@example.com,120987
}
```
