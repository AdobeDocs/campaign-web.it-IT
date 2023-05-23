---
audience: end-user
title: Eseguire il targeting dei destinatari da un file
description: Scopri come utilizzare i destinatari da un file esterno per creare il pubblico delle e-mail
badge: label="Alpha" type="Positive"
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: a6c85aeed30726532ab6060fec5cb4b5e398d9ec
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 37%

---

# Eseguire il targeting dei destinatari da un file {#audience-from-file}

Puoi caricare i contatti da un file esterno. Questa funzionalità è disponibile solo per le consegne e-mail. I formati supportati sono: file di testo (TXT) o file con valori separati da virgola (CSV). Questi verranno poi aggiunti al database.

>[!NOTE]
>
>Puoi creare un flusso di lavoro di importazione per aggiungere o aggiornare più profili.  Ulteriori informazioni


Per eseguire il targeting dei profili da un file locale direttamente dall’interfaccia, effettua le seguenti operazioni:

1. Nella finestra di creazione della consegna e-mail, fai clic su **Seleziona pubblico** e selezionare il pulsante **Seleziona da file** opzione.

   ![](assets/select-from-file.png)

1. Seleziona il file locale da caricare.
1. Visualizza in anteprima la modalità di mappatura dei dati nella sezione centrale dello schermo.
1. Scegli la colonna che contiene l’indirizzo e-mail del **Campo indirizzo** a discesa.
1. Regola le impostazioni delle colonne e la formattazione dei dati dalle opzioni disponibili.
1. Fai clic su **Conferma** una volta che le impostazioni sono corrette.

Durante la creazione e la personalizzazione del contenuto del messaggio, puoi selezionare i campi dal file di input nell’editor di personalizzazione.

![](assets/select-external-perso.png)

## File di esempio {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="File di esempio"
>abstract="Formati di file supportati: txt, csv. Utilizza la prima riga come intestazione di colonna."


```json
{
lastname,firstname,city,birthdate,email,denylist
Smith,Hayden,Paris,23/05/1985,hayden.smith@example.com,0
Mars,Daniel,London,17/11/1999,dannymars@example.com,0
Smith,Clara,Roma,08/02/1979,clara.smith@example.com,0
Durance,Allison,San Francisco,15/12/2000,allison.durance@example.com,1
}
```
