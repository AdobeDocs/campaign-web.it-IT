---
audience: end-user
title: Contenuto generativo
description: Scopri come generare le immagini con l’Assistente AI
source-git-commit: c51877d1926e1a8a6766ea1a5aa00f826071a3fc
workflow-type: tm+mt
source-wordcount: '1152'
ht-degree: 4%

---

# Generare immagini con l’Assistente AI {#generative-image}

>[!IMPORTANT]
>
>Prima di iniziare a utilizzare questa funzionalità, leggi le [protezioni e limitazioni](generative-gs.md#generative-guardrails) correlate.
></br>
>
>È necessario accettare un [contratto utente](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html){target="_blank"} prima di utilizzare l&#39;Assistente IA in Adobe Campaign Web. Per ulteriori informazioni, contatta il rappresentante Adobe.

Utilizza l’Assistente AI in Adobe Campaign Web per creare contenuti visivi coinvolgenti che migliorino i messaggi tra e-mail, pagine di destinazione e notifiche push. Ai Assistant consente di generare e ottimizzare le immagini, assicurando il coinvolgimento visivo dei contenuti e l’allineamento con il marchio.

## Per e-mail e pagine di destinazione {#email-web-channels}

L’Assistente AI può generare esperienze visive complete per le consegne e-mail e le pagine di destinazione. Questa funzionalità consente di produrre immagini sul marchio che catturano l’attenzione e che risuonano con il pubblico in diversi punti di contatto digitali.

### Accedere e configurare {#access-configure}

Per iniziare a generare le immagini con l’Assistente AI, configura innanzitutto la consegna e apri l’editor di contenuti. Segui i passaggi seguenti per preparare l’area di lavoro e accedere al pannello dell’Assistente IA.

1. Crea e configura la consegna:

   * **E-mail**: dopo aver creato e configurato la consegna e-mail, fai clic su **[!UICONTROL Modifica contenuto]**. [Ulteriori informazioni](../email/create-email-content.md)
   * **Pagina di destinazione**: dopo aver creato e configurato la pagina di destinazione, fai clic su **[!UICONTROL Modifica contenuto]**. [Ulteriori informazioni](../landing-pages/create-lp.md)

1. Selezionare la risorsa che si desidera modificare con l&#39;Assistente AI e accedere al menu **[!UICONTROL Assistente AI]**.

   ![Schermata che mostra la selezione di componenti di testo in Adobe Campaign Web](assets/image-genai-1.png){zoomable="yes"}

### Genera contenuto {#generate-content}

Scopri come creare prompt efficaci e configurare le impostazioni delle immagini per generare immagini visivamente coinvolgenti con l’Assistente AI. Personalizza parametri quali proporzioni, intensità visiva e illuminazione per creare immagini in linea con gli obiettivi del tuo marchio e della tua campagna.

1. Abilita l&#39;opzione **[!UICONTROL Stile riferimento]** affinché l&#39;Assistente AI personalizzi nuovi contenuti in base al contenuto selezionato.

1. Seleziona il tuo **[!UICONTROL marchio]** per garantire che i contenuti generati dall&#39;intelligenza artificiale siano in linea con le specifiche del tuo marchio. [Ulteriori informazioni](brands.md) sui marchi.

1. Ottimizzare il contenuto descrivendo cosa si desidera generare nel campo **[!UICONTROL Prompt]**.

   Se hai bisogno di assistenza per creare il prompt, accedi alla **[!UICONTROL Libreria prompt]**, che fornisce una vasta gamma di idee per migliorare le consegne. [Ulteriori informazioni sulle best practice per i prompt](ai-assistant-prompting-guide.md)

   ![Schermata che mostra la libreria dei prompt per la generazione di immagini in Adobe Campaign Web](assets/image-genai-2.png){zoomable="yes"}

1. Personalizza la richiesta utilizzando l&#39;opzione **[!UICONTROL Impostazioni immagine]**:

   * **[!UICONTROL Proporzioni]**: determina la larghezza e l&#39;altezza della risorsa. Scegliere tra i rapporti comuni, ad esempio 16:9, 4:3, 3:2 o 1:1, oppure immettere una dimensione personalizzata.
   * **[!UICONTROL Tipo di contenuto]**: categorizza la natura dell&#39;elemento visivo, distinguendo tra diverse forme di rappresentazione visiva come foto, immagini o immagini.
   * **[!UICONTROL Intensità visiva]**: controlla l&#39;impatto dell&#39;immagine regolandone l&#39;intensità. Un&#39;impostazione più bassa (2) crea un aspetto più morbido, mentre un&#39;impostazione più alta (10) rende l&#39;immagine più vibrante.
   * **[!UICONTROL Colore e tono]**: regola l&#39;aspetto complessivo dei colori e dell&#39;umore o dell&#39;atmosfera veicolati.
   * **[!UICONTROL Illuminazione]**: modifica l&#39;illuminazione nell&#39;immagine per modellarne l&#39;atmosfera ed evidenziare elementi specifici.
   * **[!UICONTROL Composizione]**: dispone gli elementi all&#39;interno della cornice dell&#39;immagine.

     ![Schermata che mostra le opzioni delle impostazioni immagine in Adobe Campaign Web](assets/image-genai-4.png){zoomable="yes"}

1. Dal menu **[!UICONTROL Contenuto di riferimento]**, fai clic su **[!UICONTROL Carica file]** per aggiungere qualsiasi risorsa del marchio contenente contenuto che possa fornire un&#39;Assistente di IA per l&#39;analisi del contesto aggiuntivo o selezionarne una caricata in precedenza.

   I file precedentemente caricati sono disponibili nel menu a discesa **[!UICONTROL Contenuto di riferimento caricato]**. È sufficiente attivare o disattivare le risorse da includere nella generazione.

1. Una volta completata la configurazione del prompt, fai clic su **[!UICONTROL Genera]**.

### Perfezionare e finalizzare {#refine-finalize}

Dopo aver generato le varianti di immagine, puoi esaminare i risultati, verificare l’allineamento del brand e selezionare l’opzione migliore per il contenuto.

1. Sfoglia le **[!UICONTROL Varianti]** generate.

1. Fai clic sull&#39;icona percentuale per visualizzare il **[!UICONTROL punteggio di allineamento del brand]** e identificare eventuali disallineamenti con il brand.

   Ulteriori informazioni sul [Punteggio di allineamento del marchio](../content/brands-score.md).

   ![](assets/image-genai-3.png){zoomable="yes"}

1. Fai clic su **[!UICONTROL Anteprima]** per visualizzare una versione a schermo intero della variante selezionata o su **[!UICONTROL Applica]** per sostituire il contenuto corrente.

1. Scegliere **[!UICONTROL Genera simili]** se si desidera visualizzare le immagini correlate a questa variante.

1. Apri la scheda **[!UICONTROL Allineamento marchio]** per vedere come il contenuto si allinea alle [linee guida per il marchio](../content/brands.md).

1. Fai clic su **[!UICONTROL Seleziona]** una volta trovato il contenuto appropriato.

1. Dopo aver definito il contenuto del messaggio, fai clic sul pulsante **[!UICONTROL Simula contenuto]** per controllare il rendering e verificare le impostazioni di personalizzazione con i profili di test. [Ulteriori informazioni](../preview-test/preview-content.md)

1. Rivedi e attiva il contenuto:
   * **E-mail**: una volta definiti il contenuto, il pubblico e la pianificazione, puoi preparare la consegna e-mail. [Ulteriori informazioni](../monitor/prepare-send.md)
   * **Pagina di destinazione**: quando la pagina di destinazione è pronta, puoi pubblicarla per renderla disponibile per l&#39;utilizzo in un messaggio. [Ulteriori informazioni](../landing-pages/create-lp.md)

## Per canali mobili {#mobile-channels}

L’Assistente AI ti consente di generare immagini coinvolgenti per le notifiche push, consentendoti di creare comunicazioni mobili visivamente coinvolgenti che catturano l’attenzione e risuonano con il pubblico.

### Accedere e configurare {#mobile-access-configure}

Per iniziare a generare immagini per le notifiche push con l’Assistente AI, configura innanzitutto la consegna e apri l’Assistente AI.

1. Dopo aver creato e configurato la consegna delle notifiche push, fai clic su **[!UICONTROL Modifica contenuto]**. [Ulteriori informazioni](../push/create-push.md)

1. Accedere al menu **[!UICONTROL Mostra Assistente AI]**.

   ![Schermata che mostra il menu Mostra Assistente AI](assets/push-img-1.png){zoomable="yes"}

### Genera contenuto {#mobile-generate-content}

Dopo aver effettuato l’accesso a AI Assistant, puoi regolare le impostazioni di generazione per creare immagini in linea con il tuo marchio e supportare gli obiettivi delle notifiche push. Configura i parametri di prompt e immagine per generare visualizzazioni ottimizzate per gli schermi mobili.

1. Seleziona il tuo **[!UICONTROL marchio]** per garantire che i contenuti generati dall&#39;intelligenza artificiale siano in linea con le specifiche del tuo marchio. [Ulteriori informazioni](brands.md) sui marchi.

1. Ottimizzare il contenuto descrivendo cosa si desidera generare nel campo **[!UICONTROL Prompt]**.

   Se stai cercando assistenza per creare il prompt, accedi alla **[!UICONTROL Libreria prompt]** che fornisce una vasta gamma di idee per migliorare le campagne. [Ulteriori informazioni sulle best practice per i prompt](ai-assistant-prompting-guide.md)

   ![Assistente AI con campo Prompt e opzioni](assets/push-img-2.png){zoomable="yes"}

1. Seleziona **[!UICONTROL Immagine]** per generare solo le risorse.

1. Scegli le **[!UICONTROL impostazioni immagine]**:

   * **[!UICONTROL Tipo di contenuto]**: categorizza la natura dell&#39;elemento visivo, distinguendo tra diverse forme di rappresentazione visiva come foto, immagini o immagini.
   * **[!UICONTROL Intensità visiva]**: controlla l&#39;impatto dell&#39;immagine regolandone l&#39;intensità. Un&#39;impostazione più bassa (2) crea un aspetto più morbido e più contenuto, mentre un&#39;impostazione più alta (10) rende l&#39;immagine più vibrante e visivamente potente.
   * **[!UICONTROL Illuminazione]**: regola l&#39;illuminazione nell&#39;immagine per modellarne l&#39;atmosfera ed evidenziare elementi specifici.
   * **[!UICONTROL Composizione]**: dispone gli elementi all&#39;interno della cornice dell&#39;immagine.

     ![Schermata che mostra le opzioni delle impostazioni immagine](assets/push-img-3.png){zoomable="yes"}

1. Dal menu **[!UICONTROL Contenuto di riferimento]**, fai clic su **[!UICONTROL Carica file]** per aggiungere qualsiasi risorsa del marchio contenente contenuto che possa fornire un&#39;Assistente di IA per l&#39;analisi del contesto aggiuntivo o selezionarne una caricata in precedenza.

   I file precedentemente caricati sono disponibili nel menu a discesa **[!UICONTROL Contenuto di riferimento caricato]**. È sufficiente attivare o disattivare le risorse da includere nella generazione.

1. Una volta completato il prompt, fai clic su **[!UICONTROL Genera]**.

### Perfezionare e finalizzare {#mobile-refine-finalize}

Dopo aver generato le varianti di immagine per i messaggi mobili, puoi perfezionare i risultati per garantire che soddisfino esattamente le tue esigenze.

1. Dopo la generazione, sfoglia le **[!UICONTROL Varianti]**.

1. Fai clic sull&#39;icona percentuale per visualizzare il **[!UICONTROL punteggio di allineamento del brand]** e identificare eventuali disallineamenti con il brand.

   Ulteriori informazioni sul [Punteggio di allineamento del marchio](../content/brands-score.md).

   ![](assets/push-img-4.png){zoomable="yes"}

1. Fai clic su **[!UICONTROL Anteprima]** per sfogliare le **[!UICONTROL Varianti]**.

1. Apri la scheda **[!UICONTROL Allineamento marchio]** per vedere come il contenuto si allinea alle [linee guida per il marchio](brands.md).

1. Una volta trovato il contenuto appropriato, fai clic su **[!UICONTROL Seleziona]**.

Una volta definiti il contenuto, il pubblico e la pianificazione, prepara la consegna push. [Ulteriori informazioni](../monitor/prepare-send.md)
