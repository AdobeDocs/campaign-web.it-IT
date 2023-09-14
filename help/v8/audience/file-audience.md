---
audience: end-user
title: Eseguire il targeting dei destinatari da un file
description: Scopri come utilizzare i destinatari da un file esterno per creare il pubblico dell’e-mail
badge: label="Beta"
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: 56909f59e0bd9d18bb6df9610b376f6a3a1a2bad
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 62%

---

# Caricare un pubblico dell’email da un file {#audience-from-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_select"
>title="Selezione file"
>abstract="Seleziona il file locale da caricare. Sono supportati i formati TXT e CSV. Allinea il formato del file con il file di esempio collegato di seguito."

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_columns"
>title="Definizione colonne"
>abstract="Verifica il formato delle colonne da inserire dal file locale."

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_formatting"
>title="Formattazione dei parametri"
>abstract="Verifica i parametri di formattazione per il file."

Puoi caricare i contatti da un file esterno. I profili non vengono aggiunti al database, ma tutti i campi nel file di input sono disponibili per la [personalizzazione](../personalization/gs-personalization.md). Sono supportati i formati di file di testo (TXT) e i valori separati da virgole (CSV).

>[!CAUTION]
>
>* Questa funzionalità è disponibile solo per le **consegne e-mail autonome**. Non può essere utilizzata nei flussi di lavoro, né con le consegne SMS o push.
>
>* Non è possibile utilizzare i [gruppi di controllo](control-group.md) durante il caricamento della popolazione target da un file esterno.

## Carica il file {#upload}

Per eseguire il targeting dei profili da un file locale direttamente dall’interfaccia e-mail, segui questi passaggi:

1. Apri una consegna e-mail esistente oppure [crea una nuova consegna e-mail](../email/create-email.md).
1. Nella finestra di creazione della consegna e-mail, dalla sezione **Pubblico**, fai clic sul pulsante **Seleziona pubblico** e scegli l’opzione **Seleziona da file**.

   ![](assets/select-from-file.png)

1. Seleziona il file locale da caricare. Il formato deve essere allineato con il [file di esempio](#sample-file).
1. Visualizza in anteprima e verifica la modalità di mappatura dei dati nella sezione centrale dello schermo.
1. Scegli la colonna che contiene l’indirizzo e-mail dall’elenco a discesa **Campo indirizzo**. Se tali informazioni sono presenti nel file di input, è inoltre possibile selezionare la colonna dell’elenco bloccati.
1. Regola le impostazioni delle colonne e il formato dei dati dalle opzioni disponibili.
1. Fai clic su **Conferma** una volta che le impostazioni sono corrette.

Durante la creazione e la personalizzazione del contenuto del messaggio, puoi selezionare i campi dal file di input nell’[editor di personalizzazione](../personalization/gs-personalization.md).

![](assets/select-external-perso.png)

## File di esempio {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="Caricare un pubblico da un file"
>abstract="I formati di file supportati sono TXT e CSV. Utilizza la prima riga come intestazione di colonna. Allinea il formato del file al file di esempio fornito nel collegamento seguente."

Sono supportati i formati TXT e CSV. La prima riga è l’intestazione della colonna.

Allinea il formato del file con il file di esempio di seguito:

```javascript
{
lastname,firstname,city,birthdate,email,denylist
Smith,Hayden,Paris,23/05/1985,hayden.smith@example.com,0
Mars,Daniel,London,17/11/1999,danny.mars@example.com,0
Smith,Clara,Roma,08/02/1979,clara.smith@example.com,0
Durance,Allison,San Francisco,15/12/2000,allison.durance@example.com,1
}
```

## Anteprima e verifica dell’e-mail {#test}

Campaign Web consente di visualizzare in anteprima e inviare e-mail di test quando si utilizza un pubblico caricato da un file. Per farlo, segui questi passaggi:

1. Fai clic su **[!UICONTROL Pulsante Simula contenuto]** dalla schermata di modifica dei contenuti della consegna e fai clic su **[!UICONTROL Aggiungi profili di test]** pulsante.

1. Vengono visualizzati i profili contenuti nel file caricato. Seleziona i profili da utilizzare per l’anteprima del contenuto e fai clic su **[!UICONTROL Seleziona]**.

1. Nel riquadro a destra dello schermo viene visualizzata un’anteprima del contenuto della consegna. Gli elementi personalizzati vengono sostituiti dai dati del profilo selezionato nel riquadro a sinistra. [Ulteriori informazioni sull’anteprima dei contenuti della consegna](../preview-test/preview-content.md)

   ![](assets/file-upload-preview.png)

1. Per inviare e-mail di test, fai clic su **[!UICONTROL Test]** pulsante.

1. Fai clic su **[!UICONTROL Caricare profili di bozza]** e seleziona il file .txt o .csv che contiene i destinatari della bozza.

   >[!CAUTION]
   >
   >Assicurati che il formato del file corrisponda a quello utilizzato per caricare il pubblico. Eventuali errori di formato visualizzeranno un avviso.

1. Quando i destinatari della bozza vengono aggiunti e sei pronto per inviare le bozze, fai clic sul pulsante **[!UICONTROL Invia e-mail di test]** e conferma l’invio.

   ![](assets/file-upload-test.png)

1. Puoi monitorare l’invio dell’e-mail di test utilizzando il pulsante Visualizza registro e-mail di test in qualsiasi momento. [Ulteriori informazioni sul monitoraggio delle e-mail di test](../preview-test/test-deliveries.md#access-sent-test-deliveries-access-proofs)
