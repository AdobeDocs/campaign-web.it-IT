---
audience: end-user
title: Contenuto generativo
description: Scopri come generare esperienze di contenuto complete con l’Assistente IA in Journey Optimizer.
exl-id: d9d35c1d-13db-4d2c-82f8-1629fd1e5848
source-git-commit: 2066f29b0867f82f2130361c8ccdb15889085886
workflow-type: tm+mt
source-wordcount: '1606'
ht-degree: 3%

---

# Generare contenuti completi con l’Assistente AI {#generative-full-content}

>[!IMPORTANT]
>
>Prima di iniziare a utilizzare questa funzionalità, leggi le [protezioni e limitazioni](generative-gs.md#generative-guardrails) correlate.
></br>
>
>È necessario accettare un [contratto utente](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html){target="_blank"} prima di utilizzare l&#39;Assistente IA in Adobe Campaign Web. Per ulteriori informazioni, contatta il rappresentante Adobe.

Utilizza l’Assistente AI in Adobe Campaign Web per generare esperienze di contenuti complete nei canali e-mail, pagine di destinazione e notifiche push. Ai Assistant consente di ottimizzare l’impatto delle consegne creando contenuti completi che suonano con il pubblico.

## Per e-mail e pagina di destinazione {#email-web-channels}

L’Assistente AI può produrre esperienze di contenuto complete per le consegne e-mail e le pagine di destinazione, generando sia testo che immagini. Questa robusta funzionalità consente di creare contenuti coinvolgenti e on-brand che si connettono con il pubblico in tutti i punti di contatto digitali.

### Accedere e configurare {#access-configure}

Prima di iniziare a creare contenuti con l’Assistente AI, è necessario configurare la consegna e aprire l’editor di contenuti. Utilizza i passaggi seguenti per preparare l’area di lavoro e accedere al pannello dell’Assistente AI.

1. Crea e configura la consegna:

   * **E-mail**: dopo aver creato e configurato la consegna e-mail, fai clic su **[!UICONTROL Modifica contenuto]**. [Ulteriori informazioni](../email/create-email-content.md)
   * **Pagina di destinazione**: dopo aver creato e configurato la pagina di destinazione, fai clic su **[!UICONTROL Modifica contenuto]**. [Ulteriori informazioni](../landing-pages/create-lp.md)

1. Personalizza il layout in base alle esigenze e accedi al menu **[!UICONTROL Assistente AI]**.

   ![Pannello Assistente IA che mostra la selezione del brand e il campo di prompt](assets/full-email-1.png){zoomable="yes"}

### Genera contenuto {#generate-content}

Con l’Assistente AI aperto, ora puoi configurare le impostazioni di generazione per creare contenuti che corrispondano agli obiettivi del tuo marchio e della tua campagna. Personalizza i parametri di testo e immagine, aggiungi risorse del brand e fornisci prompt per guidare l’intelligenza artificiale nella generazione di varianti rilevanti per il pubblico.

1. Seleziona il tuo **[!UICONTROL marchio]** per garantire che i contenuti generati dall&#39;intelligenza artificiale siano in linea con le specifiche del tuo marchio. [Ulteriori informazioni](brands.md) sui marchi.

1. Ottimizzare il contenuto descrivendo cosa si desidera generare nel campo **[!UICONTROL Prompt]**.

   Se hai bisogno di assistenza per creare il prompt, accedi alla **[!UICONTROL Libreria prompt]**, che fornisce una vasta gamma di idee per migliorare le consegne. [Ulteriori informazioni sulle best practice per i prompt](ai-assistant-prompting-guide.md)

   ![Schermata che mostra la libreria di richieste in Adobe Campaign Web](assets/full-email-2.png){zoomable="yes"}

1. **Per le e-mail**, puoi attivare/disattivare le opzioni **[!UICONTROL Oggetto]** e **[!UICONTROL Preheader]** per includerle nella generazione delle varianti.

1. Personalizza la richiesta utilizzando l&#39;opzione **[!UICONTROL Impostazioni testo]**:

   * **[!UICONTROL Strategia di comunicazione]**: scegli lo stile di comunicazione più adatto al testo generato.
   * **[!UICONTROL Lingue]**: scegli la lingua del contenuto generato.
   * **[!UICONTROL Tono]**: assicurati che il tono dell&#39;e-mail risuoni con il pubblico. Che tu voglia essere informativo, giocoso o persuasivo, l’Assistente AI adatta il messaggio di conseguenza.

     ![Schermata che mostra le opzioni delle impostazioni di testo in Adobe Campaign Web](assets/full-email-4.png){zoomable="yes"}

1. Scegli le **[!UICONTROL impostazioni immagine]**:

   * **[!UICONTROL Tipo di contenuto]**: categorizza la natura dell&#39;elemento visivo, distinguendo tra diverse forme di rappresentazione visiva come foto, immagini o immagini.
   * **[!UICONTROL Intensità visiva]**: controlla l&#39;impatto dell&#39;immagine regolandone l&#39;intensità. Un&#39;impostazione più bassa (2) crea un aspetto più morbido, mentre un&#39;impostazione più alta (10) rende l&#39;immagine più vibrante.
   * **[!UICONTROL Colore e tono]**: regola l&#39;aspetto complessivo dei colori e dell&#39;umore o dell&#39;atmosfera veicolati.
   * **[!UICONTROL Illuminazione]**: modifica l&#39;illuminazione nell&#39;immagine per modellarne l&#39;atmosfera ed evidenziare elementi specifici.
   * **[!UICONTROL Composizione]**: dispone gli elementi all&#39;interno della cornice dell&#39;immagine.

1. Dal menu **[!UICONTROL Contenuto di riferimento]**, fai clic su **[!UICONTROL Carica file]** per aggiungere qualsiasi risorsa del marchio contenente contenuto che possa fornire un&#39;Assistente di IA per l&#39;analisi del contesto aggiuntivo o selezionarne una caricata in precedenza.

   I file precedentemente caricati sono disponibili nel menu a discesa **[!UICONTROL Contenuto di riferimento caricato]**. È sufficiente attivare o disattivare le risorse da includere nella generazione.

   ![Schermata che mostra le opzioni delle impostazioni dei marchi in Adobe Campaign Web](assets/full-email-3.png){zoomable="yes"}

1. Una volta completato il prompt, fai clic su **[!UICONTROL Genera]**.

### Perfezionare e finalizzare {#refine-finalize}

Dopo aver generato le varianti di contenuto, puoi perfezionare i risultati per garantire che soddisfino esattamente le tue esigenze. Rivedi l’allineamento del brand, regola il tono e la lingua e prepara il contenuto per l’attivazione nella consegna.

1. Dopo la generazione, sfoglia le **[!UICONTROL Varianti]**.

1. Fai clic sull&#39;icona percentuale per visualizzare il **[!UICONTROL punteggio di allineamento del brand]** e identificare eventuali disallineamenti con il brand.

   Ulteriori informazioni sul [Punteggio di allineamento del marchio](brands-score.md).

   ![](assets/full-email-7.png){zoomable="yes"}

1. Fai clic su **[!UICONTROL Anteprima]** per visualizzare una versione a schermo intero della variante selezionata o su **[!UICONTROL Applica]** per sostituire il contenuto corrente.

1. Passa all&#39;opzione **[!UICONTROL Perfeziona]** nella finestra **[!UICONTROL Anteprima]** per accedere ad altre funzioni di personalizzazione:

   * **[!UICONTROL Riformulazione]**: riscrivere il messaggio conservandone il significato. Questa opzione consente di generare una formulazione alternativa, migliorare il flusso o regolare la formulazione senza modificare il messaggio principale.

   * **[!UICONTROL Usa un linguaggio più semplice]**: sfrutta l&#39;Assistente AI per semplificare la lingua, garantendo chiarezza e accessibilità a un pubblico più ampio.

   * **[!UICONTROL Traduci]**: semplifica la lingua per garantire chiarezza e accessibilità a un pubblico più ampio.

   * **[!UICONTROL Cambia tono]**: regola il tono del messaggio per adattarlo al tuo stile di comunicazione, rendendolo più amichevole, professionale, urgente o ispiratore.

   * **[!UICONTROL Modifica strategia di comunicazione]**: modifica l&#39;approccio di messaggistica in base agli obiettivi, ad esempio la creazione di messaggi urgenti o l&#39;enfasi sull&#39;aspetto interessante.

     ![Perfeziona il menu visualizzando le opzioni](assets/full-email-5.png){zoomable="yes"}

1. Apri la scheda **[!UICONTROL Allineamento marchio]** per vedere come il contenuto si allinea alle [linee guida per il marchio](brands.md).

1. Una volta trovato il contenuto appropriato, fai clic su **[!UICONTROL Seleziona]**.

1. Inserisci campi di personalizzazione per personalizzare il contenuto in base ai dati dei profili. Quindi, fai clic sul pulsante **[!UICONTROL Simula contenuto]** per controllare il rendering e controlla le impostazioni di personalizzazione con i profili di test. [Ulteriori informazioni](../preview-test/preview-content.md)

1. Rivedi e attiva il contenuto:
   * **E-mail**: una volta definiti il contenuto, il pubblico e la pianificazione, puoi preparare la consegna e-mail. [Ulteriori informazioni](../monitor/prepare-send.md)
   * **Pagina di destinazione**: quando la pagina di destinazione è pronta, puoi pubblicarla per renderla disponibile per l&#39;utilizzo in un messaggio. [Ulteriori informazioni](../landing-pages/create-lp.md)

## Per canali mobili {#mobile-channels}

L’Assistente AI supporta anche la generazione di contenuti per le notifiche push per dispositivi mobili, consentendoti di creare titoli, messaggi e immagini coinvolgenti per le app mobili. Questo consente di mantenere una comunicazione coerente e di alta qualità su tutti i punti di contatto dei clienti, compresi i dispositivi mobili.

### Accedere e configurare {#mobile-access-configure}

Per utilizzare l’Assistente AI per le notifiche push, configura innanzitutto la consegna push e apri l’editor di contenuti. I passaggi seguenti ti guideranno attraverso la preparazione della consegna e l’accesso agli strumenti di AI Assistant.

1. Dopo aver creato e configurato la consegna delle notifiche push, fai clic su **[!UICONTROL Modifica contenuto]**.

   Per ulteriori informazioni sulla configurazione della consegna push, consulta [questa pagina](../push/create-push.md).

1. Personalizza la notifica push in base alle esigenze. [Ulteriori informazioni](../push/content-push.md)

1. Accedere al menu **[!UICONTROL Mostra Assistente AI]**.

   ![Schermata che mostra il menu Mostra Assistente AI](assets/push-genai-1.png){zoomable="yes"}

### Genera contenuto {#mobile-generate-content}

Dopo aver effettuato l’accesso all’Assistente AI per le notifiche push, puoi configurare le impostazioni di generazione per creare contenuti coinvolgenti per dispositivi mobili. Definisci le preferenze di testo e immagine, seleziona le risorse del brand e utilizza i prompt per generare varianti di notifica push che coinvolgono gli utenti mobili.

1. Seleziona il tuo **[!UICONTROL marchio]** per garantire che i contenuti generati dall&#39;intelligenza artificiale siano in linea con le specifiche del tuo marchio. [Ulteriori informazioni](brands.md) sui marchi.

1. Ottimizzare il contenuto descrivendo cosa si desidera generare nel campo **[!UICONTROL Prompt]**.

   Se stai cercando assistenza per creare il prompt, accedi alla **[!UICONTROL Libreria prompt]** che fornisce una vasta gamma di idee per migliorare la consegna. [Ulteriori informazioni sulle best practice per i prompt](ai-assistant-prompting-guide.md)

   ![Assistente AI con campo Prompt e opzioni](assets/push-genai-2.png){zoomable="yes"}

1. Scegli il campo da generare: **[!UICONTROL Titolo]**, **[!UICONTROL Sottotitolo]**, **[!UICONTROL Messaggio]** e/o **[!UICONTROL Immagine]**.

1. Personalizza la richiesta con l&#39;opzione **[!UICONTROL Impostazioni testo]**:

   * **[!UICONTROL Strategia di comunicazione]**: scegli lo stile di comunicazione più adatto al testo generato.
   * **[!UICONTROL Lingue]**: scegli la lingua del contenuto generato.
   * **[!UICONTROL Tono]**: il tono delle notifiche push dovrebbe risuonare con il pubblico. Che tu voglia essere informativo, giocoso o persuasivo, AI Assistant può adattare il messaggio di conseguenza.

     ![Pannello impostazioni testo per notifiche push](assets/push-genai-3.png){zoomable="yes"}

1. Scegli le **[!UICONTROL impostazioni immagine]**:

   * **[!UICONTROL Tipo di contenuto]**: categorizza la natura dell&#39;elemento visivo, distinguendo tra diverse forme di rappresentazione visiva come foto, immagini o immagini.
   * **[!UICONTROL Intensità visiva]**: controlla l&#39;impatto dell&#39;immagine regolandone l&#39;intensità. Un&#39;impostazione più bassa (2) crea un aspetto più morbido e più contenuto, mentre un&#39;impostazione più alta (10) rende l&#39;immagine più vibrante e visivamente potente.
   * **[!UICONTROL Illuminazione]**: regola l&#39;illuminazione nell&#39;immagine per modellarne l&#39;atmosfera ed evidenziare elementi specifici.
   * **[!UICONTROL Composizione]**: dispone gli elementi all&#39;interno della cornice dell&#39;immagine.

     ![Impostazioni immagine per le notifiche push](assets/push-genai-4.png){zoomable="yes"}

1. Dal menu **[!UICONTROL Contenuto di riferimento]**, fai clic su **[!UICONTROL Carica file]** per aggiungere qualsiasi risorsa del marchio contenente contenuto che possa fornire un&#39;Assistente di IA per l&#39;analisi del contesto aggiuntivo o selezionarne una caricata in precedenza.

   I file precedentemente caricati sono disponibili nel menu a discesa **[!UICONTROL Contenuto di riferimento caricato]**. È sufficiente attivare o disattivare le risorse da includere nella generazione.

1. Una volta completato il prompt, fai clic su **[!UICONTROL Genera]**.

### Perfezionare e finalizzare {#mobile-refine-finalize}

Dopo aver esaminato le varianti di notifica push generate, puoi lucidare il contenuto alla perfezione. Utilizza gli strumenti di ottimizzazione per regolare lingua e tono, verificare l’allineamento del brand e personalizzare il contenuto prima di attivare la campagna push.

1. Sfoglia le **[!UICONTROL Varianti]** generate.

1. Fai clic sull&#39;icona percentuale per visualizzare il **[!UICONTROL punteggio di allineamento del brand]** e identificare eventuali disallineamenti con il brand.

   Ulteriori informazioni sul [Punteggio di allineamento del marchio](brands-score.md).

   ![Varianti di notifica push generate con punteggio di allineamento del marchio](assets/push-genai-6.png){zoomable="yes"}

1. Fai clic su **[!UICONTROL Anteprima]** per visualizzare una versione a schermo intero della variante selezionata oppure fai clic su **[!UICONTROL Applica]** per sostituire il contenuto corrente.

1. Passa all&#39;opzione **[!UICONTROL Perfeziona]** nella finestra **[!UICONTROL Anteprima]** per accedere ad altre funzioni di personalizzazione:

   * **[!UICONTROL Utilizza come contenuto di riferimento]**: utilizza la variante scelta come contenuto di riferimento per generare altri risultati.
   * **[!UICONTROL Riformula]**: riformula il messaggio in diversi modi per mantenere la scrittura fresca e coinvolgente per diversi tipi di pubblico.
   * **[!UICONTROL Usa un linguaggio più semplice]**: semplifica la lingua per garantire chiarezza e accessibilità a un pubblico più ampio.
   * **[!UICONTROL Traduci]**: semplifica la lingua per garantire chiarezza e accessibilità a un pubblico più ampio.

   Puoi anche modificare il **[!UICONTROL Tono]** e la **[!UICONTROL Strategia di comunicazione]** del tuo testo.

   ![Opzioni di ottimizzazione per le notifiche push](assets/push-genai-5.png){zoomable="yes"}

1. Apri la scheda **[!UICONTROL Allineamento marchio]** per vedere come il contenuto si allinea alle [linee guida per il marchio](brands.md).

1. Una volta trovato il contenuto appropriato, fai clic su **[!UICONTROL Seleziona]**.

1. Inserisci campi di personalizzazione per personalizzare il contenuto delle e-mail in base ai dati del profilo. Quindi, fai clic sul pulsante **[!UICONTROL Simula contenuto]** per controllare il rendering e controllare le impostazioni di personalizzazione con i profili di test. [Ulteriori informazioni](../preview-test/preview-content.md)

Quando definisci il contenuto, il pubblico e la pianificazione, prepara la consegna push. [Ulteriori informazioni](../monitor/prepare-send.md)

## Video dimostrativo {#video}

Scopri come utilizzare l’Assistente AI per generare contenuti e-mail, testo e immagini completi.

>[!VIDEO](https://video.tv.adobe.com/v/3428984)