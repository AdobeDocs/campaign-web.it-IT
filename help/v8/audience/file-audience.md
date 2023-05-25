---
audience: end-user
title: Eseguire il targeting dei destinatari da un file
description: Scopri come utilizzare i destinatari da un file esterno per creare il pubblico delle e-mail
badge: label="Alpha" type="Positive"
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: fd9a5724aa9b97bffc6d143853742e0107bd3483
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 22%

---

# Caricare i destinatari da un file {#audience-from-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_select"
>title="Selezione file"
>abstract="Seleziona il file locale da caricare. I formati supportati sono TXT e CSV. Allinea il formato del file con il file di esempio collegato di seguito."

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_columns"
>title="Definizione colonne"
>abstract="Controlla il formato delle colonne da inserire dal file locale."

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_formatting"
>title="Formattazione dei parametri"
>abstract="Verifica i parametri di formattazione per il file."

Puoi caricare i contatti da un file esterno. Questa funzionalità è disponibile solo per le consegne e-mail. I formati di file supportati sono: testo (TXT) e valore separato da virgole (CSV). I profili non vengono aggiunti al database, ma tutti i campi nel file di input sono disponibili per la personalizzazione.

>[!NOTE]
>
>Puoi creare un flusso di lavoro di importazione per aggiungere o aggiornare più profili nel database. Ulteriori informazioni


Per eseguire il targeting dei profili da un file locale direttamente dall’interfaccia, effettua le seguenti operazioni:

1. Nella finestra di creazione della consegna e-mail, da **Pubblico** , fare clic sul pulsante **Seleziona pubblico** e scegliere il pulsante **Seleziona da file** opzione.

   ![](assets/select-from-file.png)

1. Seleziona il file locale da caricare.
1. Visualizza l’anteprima e controlla come vengono mappati i dati nella sezione centrale della schermata.
1. Scegli la colonna che contiene l’indirizzo e-mail del **Campo indirizzo** a discesa. Se tali informazioni sono presenti nel file di input, è inoltre possibile selezionare la colonna di inserita nell&#39;elenco Bloccati del sistema di selezione.
1. Regola le impostazioni delle colonne e la formattazione dei dati dalle opzioni disponibili.
1. Fai clic su **Conferma** una volta che le impostazioni sono corrette.

Durante la creazione e la personalizzazione del contenuto del messaggio, puoi selezionare i campi dal file di input nell’editor di personalizzazione.

![](assets/select-external-perso.png)

>[!CAUTION]
>
>Non è possibile utilizzare [gruppi di controllo](control-group.md) durante il caricamento della popolazione target da un file esterno.

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
