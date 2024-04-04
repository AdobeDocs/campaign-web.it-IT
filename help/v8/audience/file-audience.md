---
audience: end-user
title: Caricare un pubblico per consegne e-mail da un file
description: Scopri come caricare i profili da un file esterno per creare il pubblico delle e-mail
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: b166d06215e06d6426ab9ce9a757fcc041810df9
workflow-type: tm+mt
source-wordcount: '657'
ht-degree: 51%

---

# Caricare un pubblico dell’email da un file {#audience-from-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_select"
>title="Selezione file"
>abstract="Seleziona il file locale da caricare. Sono supportati i formati TXT e CSV. Allinea il formato del file con il file di esempio collegato di seguito."

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_columns"
>title="Definizione colonne"
>abstract="Controlla il formato delle colonne nel file esterno."

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_formatting"
>title="Formattazione dei parametri"
>abstract="Specifica la formattazione del file esterno per garantire che i dati vengano importati correttamente."

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_preview"
>title="Anteprima del file"
>abstract="Controlla l’anteprima delle colonne del file esterno. Questa schermata mostra solo un massimo di 30 record."

L’interfaccia utente web di Adobe Campaign consente di eseguire il targeting dei profili memorizzati in un file esterno. Una volta caricati i profili, tutti i campi del file di input sono disponibili per l’utilizzo per personalizzare la consegna [Scopri come personalizzare i contenuti](../personalization/personalize.md).

I profili del file di input non vengono aggiunti al database. Sono caricati e disponibili solo per questa consegna e-mail autonoma specifica.

>[!NOTE]
>
>Questa pagina descrive come caricare profili esterni da un file durante la creazione di una consegna e-mail autonoma. Per caricare dati da un file nel contesto di un flusso di lavoro, consulta [questa pagina](../workflows/activities/load-file.md).

## Da leggere {#must-read}

* Questa funzionalità è disponibile per **consegne e-mail** solo.
* Sono supportati i formati di file di testo (TXT) e i valori separati da virgole (CSV).
* Non è possibile utilizzare i [gruppi di controllo](control-group.md) durante il caricamento della popolazione target da un file esterno.

## Seleziona e configura il file di input {#upload}

Per eseguire il targeting dei profili da un file nelle e-mail, effettua le seguenti operazioni:

1. Apri una consegna e-mail esistente oppure [crea una nuova consegna e-mail](../email/create-email.md).
1. In **Pubblico** , fare clic sul pulsante **Seleziona pubblico** quindi scegliere **Seleziona da file**.

   ![](assets/select-from-file.png){zoomable=&quot;yes&quot;}

1. Selezionare il file locale da caricare. Il formato del file deve essere allineato con [file di esempio](#sample-file).
1. Visualizza in anteprima e verifica la modalità di mappatura dei dati nella sezione centrale dello schermo.

   ![](assets/select-from-file-map.png)

1. Specifica la colonna contenente l’indirizzo e-mail del **Campo indirizzo** elenco a discesa. Se tali informazioni sono presenti nel file di input, è inoltre possibile selezionare la colonna dell’elenco bloccati.
1. Regola le impostazioni delle colonne e come formattare i dati dalle opzioni disponibili.
1. Fai clic su **Conferma** una volta che le impostazioni sono corrette.

Quando crei il contenuto del messaggio, puoi aggiungere la personalizzazione sfruttando i campi del file di input. [Scopri come personalizzare il contenuto](../personalization/personalize.md)

![](assets/select-external-perso.png){zoomable=&quot;yes&quot;}

## File di esempio {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="Caricare un pubblico da un file"
>abstract="Sono supportati i formati di file TXT e CSV. Utilizza la prima riga come intestazione di colonna. Allinea il formato del file con il file di esempio fornito nel collegamento seguente."

Quando carichi un file esterno per eseguire il targeting dei profili nelle consegne, assicurati che il file di input corrisponda ai consigli seguenti:

* I formati supportati sono TXT e CSV.
* La prima riga del file è l’intestazione della colonna.
* Allinea il formato del file con il file di esempio di seguito:

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

Campaign Web consente di visualizzare in anteprima e inviare bozze quando si utilizza un pubblico caricato da un file. Per farlo, segui questi passaggi:

1. Fai clic sul **[!UICONTROL pulsante Simula contenuto]** dalla schermata di modifica dei contenuti della consegna e sul pulsante **[!UICONTROL Aggiungi profili di test]**.

1. Vengono visualizzati i profili contenuti nel file caricato. Seleziona i profili da utilizzare per l’anteprima del contenuto e fai clic su **[!UICONTROL Seleziona]**.

1. Viene visualizzata un’anteprima del contenuto della consegna nel riquadro a destra della schermata. Gli elementi personalizzati vengono sostituiti dai dati del profilo selezionato nel riquadro a sinistra. [Ulteriori informazioni sull’anteprima dei contenuti della consegna](../preview-test/preview-content.md)

   ![](assets/file-upload-preview.png){zoomable=&quot;yes&quot;}

1. Per inviare le bozze, fai clic su **[!UICONTROL Invia bozza]** pulsante.

1. Fai clic sul pulsante **[!UICONTROL Carica i profili di bozza]** e seleziona il file .txt o .csv che contiene i destinatari della bozza.

   >[!CAUTION]
   >
   >Assicurati che il formato del file corrisponda a quello utilizzato per caricare il pubblico. Per eventuali errori di formato verrà visualizzato un avviso.

1. Quando i profili di bozza vengono aggiunti e sei pronto per inviare le bozze, fai clic sul pulsante **[!UICONTROL Invia bozza]** e conferma l’invio.

   ![](assets/file-upload-test.png){zoomable=&quot;yes&quot;}

1. Puoi monitorare l’invio della bozza utilizzando **[!UICONTROL Visualizza bozze]** in qualsiasi momento. [Ulteriori informazioni sul monitoraggio delle bozze](../preview-test/test-deliveries.md#access-test-deliveries)
