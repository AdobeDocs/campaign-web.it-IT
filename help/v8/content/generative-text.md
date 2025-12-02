---
audience: end-user
title: Contenuto generativo
description: Scopri come generare esperienze di contenuto testuale con l’Assistente IA
source-git-commit: 2066f29b0867f82f2130361c8ccdb15889085886
workflow-type: tm+mt
source-wordcount: '1441'
ht-degree: 3%

---

# Genera testo con Assistente IA {#generative-text}

>[!IMPORTANT]
>
>Prima di iniziare a utilizzare questa funzionalità, leggi le [protezioni e limitazioni](generative-gs.md#generative-guardrails) correlate.
></br>
>
>È necessario accettare un [contratto utente](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html){target="_blank"} prima di utilizzare l&#39;Assistente IA in Adobe Campaign Web. Per ulteriori informazioni, contatta il rappresentante Adobe.

Utilizza l’Assistente AI in Adobe Campaign Web per generare testo coinvolgente che risuona con il tuo pubblico. Che tu stia migliorando la copia delle e-mail, creando contenuti persuasivi per le pagine di destinazione, scrivendo messaggi di notifica push o componendo testo SMS, l’Assistente AI ti aiuta a fornire una comunicazione chiara e di impatto.

## Per e-mail e pagine di destinazione {#email-web-channels}

L’Assistente AI può generare contenuti di testo di alta qualità per le consegne e-mail e le pagine di destinazione. Questa funzionalità ti consente di creare messaggi coinvolgenti e on-brand che si connettono con il tuo pubblico attraverso punti di contatto digitali.

### Accedere e configurare {#access-configure}

Prima di poter iniziare a generare contenuti di testo con l’Assistente AI, devi impostare la consegna e accedere all’editor di contenuti. Segui questi passaggi per preparare l’area di lavoro e aprire il pannello dell’Assistente AI.

1. Crea e configura la consegna:

   * **E-mail**: dopo aver creato e configurato la consegna e-mail, fai clic su **[!UICONTROL Modifica contenuto]**. [Ulteriori informazioni](../email/create-email-content.md)
   * **Pagina di destinazione**: dopo aver creato e configurato la pagina di destinazione, fai clic su **[!UICONTROL Modifica contenuto]**. [Ulteriori informazioni](../landing-pages/create-lp.md)

1. Seleziona un **[!UICONTROL componente testo]** per eseguire il targeting di contenuto specifico e accedi al menu **[!UICONTROL Assistente IA]**.

   ![Schermata che mostra la selezione di componenti di testo in Adobe Campaign Web](assets/text-genai-1.png){zoomable="yes"}

### Genera contenuto {#generate-content}

Scopri come creare messaggi chiari, ottimizzare le impostazioni e generare testo personalizzato utilizzando l’Assistente AI, per garantire che la messaggistica sia in linea con gli obiettivi del marchio e della comunicazione.

1. Seleziona il tuo **[!UICONTROL marchio]** per garantire che i contenuti generati dall&#39;intelligenza artificiale siano in linea con le specifiche del tuo marchio. [Ulteriori informazioni](brands.md) sui marchi.

1. Ottimizzare il contenuto descrivendo cosa si desidera generare nel campo **[!UICONTROL Prompt]**.

   Se hai bisogno di assistenza per creare il prompt, accedi alla **[!UICONTROL Libreria prompt]**, che fornisce una vasta gamma di idee per migliorare le consegne. [Ulteriori informazioni sulle best practice per i prompt](ai-assistant-prompting-guide.md)

   ![Schermata che mostra la libreria dei prompt in Adobe Campaign Web](assets/text-genai-2.png){zoomable="yes"}

1. Personalizza la richiesta utilizzando l&#39;opzione **[!UICONTROL Impostazioni testo]**:

   * **[!UICONTROL Strategia di comunicazione]**: scegli lo stile di comunicazione più adatto al testo generato.
   * **[!UICONTROL Lingue]**: scegli la lingua del contenuto generato.
   * **[!UICONTROL Tono]**: assicurati che il tono dell&#39;e-mail risuoni con il pubblico. Che tu voglia essere informativo, giocoso o persuasivo, l’Assistente AI adatta il messaggio di conseguenza.
   * **Lunghezza testo**: utilizza il cursore per selezionare la lunghezza desiderata del testo.

     ![Schermata che mostra le opzioni delle impostazioni di testo in Adobe Campaign Web](assets/text-genai-4.png){zoomable="yes"}

1. Dal menu **[!UICONTROL Contenuto di riferimento]**, fai clic su **[!UICONTROL Carica file]** per aggiungere qualsiasi risorsa del marchio contenente contenuto che possa fornire un&#39;Assistente di IA per l&#39;analisi del contesto aggiuntivo o selezionarne una caricata in precedenza.

   I file precedentemente caricati sono disponibili nel menu a discesa **[!UICONTROL Contenuto di riferimento caricato]**. È sufficiente attivare o disattivare le risorse da includere nella generazione.

1. Una volta completato il prompt, fai clic su **[!UICONTROL Genera]**.

### Perfezionare e finalizzare {#refine-finalize}

Scopri come rivedere il testo generato, perfezionare e applicare la personalizzazione per finalizzare i contenuti, creando messaggi raffinati e coinvolgenti pronti per la consegna.

1. Sfoglia le **[!UICONTROL Varianti]** generate.

1. Fai clic sull&#39;icona percentuale per visualizzare il **[!UICONTROL punteggio di allineamento del brand]** e identificare eventuali disallineamenti con il brand.

   Ulteriori informazioni sul [Punteggio di allineamento del marchio](brands-score.md).

   ![](assets/text-genai-6.png){zoomable="yes"}

1. Fai clic su **[!UICONTROL Anteprima]** per visualizzare una versione a schermo intero della variante selezionata o su **[!UICONTROL Applica]** per sostituire il contenuto corrente.

1. Passa all&#39;opzione **[!UICONTROL Perfeziona]** nella finestra **[!UICONTROL Anteprima]** per accedere ad altre funzioni di personalizzazione:

   * **[!UICONTROL Utilizza come contenuto di riferimento]**: la variante scelta funge da contenuto di riferimento per la generazione di altri risultati.
   * **[!UICONTROL Elaborare]**: espandere argomenti specifici, fornendo ulteriori dettagli per una migliore comprensione e coinvolgimento.
   * **[!UICONTROL Riepiloga]**: riduci i punti chiave in riepiloghi chiari e concisi per attirare l&#39;attenzione e incoraggiare ulteriori letture.
   * **[!UICONTROL Riformula]**: riformula il messaggio in diversi modi, mantenendo la scrittura fresca e coinvolgente per diversi tipi di pubblico.
   * **[!UICONTROL Usa un linguaggio più semplice]**: semplifica la lingua per garantire chiarezza e accessibilità a un pubblico più ampio.
   * **[!UICONTROL Traduci]**: semplifica la lingua per garantire chiarezza e accessibilità a un pubblico più ampio.

   Puoi anche modificare il **[!UICONTROL Tono]** e la **[!UICONTROL Strategia di comunicazione]** del tuo testo.

   ![Schermata che mostra le opzioni di ottimizzazione in Adobe Campaign Web](assets/text-genai-5.png){zoomable="yes"}

1. Apri la scheda **[!UICONTROL Allineamento marchio]** per vedere come il contenuto si allinea alle [linee guida per il marchio](../content/brands.md).

1. Fai clic su **[!UICONTROL Seleziona]** una volta trovato il contenuto appropriato.

1. Inserisci campi di personalizzazione per personalizzare il contenuto in base ai dati del profilo. Quindi, fai clic sul pulsante **[!UICONTROL Simula contenuto]** per controllare il rendering e controllare le impostazioni di personalizzazione con i profili di test. [Ulteriori informazioni](../preview-test/preview-content.md)

1. Rivedi e attiva il contenuto:
   * **E-mail**: una volta definiti il contenuto, il pubblico e la pianificazione, puoi preparare la consegna e-mail. [Ulteriori informazioni](../monitor/prepare-send.md)
   * **Pagina di destinazione**: quando la pagina di destinazione è pronta, puoi pubblicarla per renderla disponibile per l&#39;utilizzo in un messaggio. [Ulteriori informazioni](../landing-pages/create-lp.md)

## Per canali mobili {#mobile-channels}

L’Assistente AI può generare contenuti di testo coinvolgenti per le notifiche push e i messaggi SMS, aiutandoti a creare comunicazioni mobili coinvolgenti che si connettono con il pubblico in tutti i punti di contatto mobili.

### Accedere e configurare {#mobile-access-configure}

Prima di iniziare a generare il testo con l’Assistente AI per i canali mobili, è necessario impostare la consegna e accedere all’Assistente AI.

1. Crea e configura la consegna mobile:
   * **Notifiche push**: dopo aver creato e configurato la consegna delle notifiche push, fai clic su **[!UICONTROL Modifica contenuto]**. [Ulteriori informazioni](../push/create-push.md)
   * **SMS**: dopo aver creato e configurato la consegna SMS, fai clic su **[!UICONTROL Modifica contenuto]**. [Ulteriori informazioni](../sms/create-sms.md)

1. Personalizza il messaggio in base alle esigenze:
   * **Notifiche push**: [Ulteriori informazioni](../push/content-push.md)
   * **SMS**: [Ulteriori informazioni](../sms/content-sms.md)

1. Accedere al menu **[!UICONTROL Mostra Assistente AI]**.

   ![Schermata che mostra il menu Mostra Assistente AI](assets/sms-genai-1.png){zoomable="yes"}

### Genera contenuto {#mobile-generate-content}

Dopo aver effettuato l’accesso a AI Assistant, puoi configurare le impostazioni di generazione per creare contenuti per dispositivi mobili che corrispondano agli obiettivi di brand e consegna. Personalizza i parametri di testo, aggiungi risorse del brand e fornisci prompt per guidare l’intelligenza artificiale nella generazione di varianti rilevanti.

1. Seleziona il tuo **[!UICONTROL marchio]** per garantire che i contenuti generati dall&#39;intelligenza artificiale siano in linea con le specifiche del tuo marchio. [Ulteriori informazioni](brands.md) sui marchi.

1. Ottimizzare il contenuto descrivendo cosa si desidera generare nel campo **[!UICONTROL Prompt]**.

   Se stai cercando assistenza per creare il prompt, accedi alla **[!UICONTROL Libreria prompt]** che fornisce una vasta gamma di idee per migliorare la consegna. [Ulteriori informazioni sulle best practice per i prompt](ai-assistant-prompting-guide.md)

   ![Assistente AI con campo Prompt e opzioni](assets/sms-genai-2.png){zoomable="yes"}

1. **Per le notifiche push**, scegli il campo di testo da generare: **[!UICONTROL Titolo]**, **[!UICONTROL Sottotitolo]** e/o **[!UICONTROL Messaggio]**.

1. Personalizza la richiesta con l&#39;opzione **[!UICONTROL Impostazioni testo]**:

   * **[!UICONTROL Strategia di comunicazione]**: scegli lo stile di comunicazione più adatto al testo generato.
   * **[!UICONTROL Lingue]**: scegli la lingua del contenuto generato.
   * **[!UICONTROL Tono]**: il tono dovrebbe risuonare con il tuo pubblico. Che tu voglia essere informativo, giocoso o persuasivo, AI Assistant può adattare il messaggio di conseguenza.
   * **[!UICONTROL Lunghezza]**: seleziona la lunghezza del contenuto utilizzando il cursore di intervallo.

     ![Pannello impostazioni testo](assets/sms-genai-3.png){zoomable="yes"}

1. Dal menu **[!UICONTROL Contenuto di riferimento]**, fai clic su **[!UICONTROL Carica file]** per aggiungere qualsiasi risorsa del marchio contenente contenuto che possa fornire un&#39;Assistente di IA per l&#39;analisi del contesto aggiuntivo o selezionarne una caricata in precedenza.

   I file precedentemente caricati sono disponibili nel menu a discesa **[!UICONTROL Contenuto di riferimento caricato]**. È sufficiente attivare o disattivare le risorse da includere nella generazione.

1. Una volta completato il prompt, fai clic su **[!UICONTROL Genera]**.

### Perfezionare e finalizzare {#mobile-refine-finalize}

Dopo aver generato varianti di testo per i messaggi mobili, puoi perfezionare i risultati per garantire che soddisfino esattamente le tue esigenze. Rivedi l’allineamento del brand, regola il tono e la lingua e prepara il contenuto per l’attivazione.

1. Dopo la generazione, sfoglia le **[!UICONTROL Varianti]**.

1. Fai clic sull&#39;icona percentuale per visualizzare il **[!UICONTROL punteggio di allineamento del brand]** e identificare eventuali disallineamenti con il brand.

   Ulteriori informazioni sul [Punteggio di allineamento del marchio](brands-score.md).

   ![Perfeziona menu](assets/sms-genai-4.png){zoomable="yes"}

1. Fai clic su **[!UICONTROL Anteprima]** per visualizzare una versione a schermo intero della variante selezionata oppure fai clic su **[!UICONTROL Applica]** per sostituire il contenuto corrente.

1. Passa all&#39;opzione **[!UICONTROL Perfeziona]** nella finestra **[!UICONTROL Anteprima]** per accedere ad altre funzioni di personalizzazione:

   * **[!UICONTROL Utilizza come contenuto di riferimento]**: la variante scelta fungerà da contenuto di riferimento per generare altri risultati.

   * **[!UICONTROL Riformulazione]**: riscrivere il messaggio conservandone il significato. Questa opzione consente di generare una formulazione alternativa, migliorare il flusso o regolare la formulazione senza modificare il messaggio principale.

   * **[!UICONTROL Usa un linguaggio più semplice]**: sfrutta l&#39;Assistente AI per semplificare la lingua, garantendo chiarezza e accessibilità a un pubblico più ampio.

   * **[!UICONTROL Traduci]**: semplifica la lingua per garantire chiarezza e accessibilità a un pubblico più ampio.

   * **[!UICONTROL Cambia tono]**: regola il tono del messaggio per adattarlo al tuo stile di comunicazione, rendendolo più amichevole, professionale, urgente o ispiratore.

   * **[!UICONTROL Modifica strategia di comunicazione]**: modifica l&#39;approccio di messaggistica in base agli obiettivi, ad esempio la creazione di messaggi urgenti o l&#39;enfasi sull&#39;aspetto interessante.

     ![Varianti di testo generate con il punteggio di allineamento del marchio](assets/sms-genai-5.png){zoomable="yes"}

1. Apri la scheda **[!UICONTROL Allineamento marchio]** per vedere come il contenuto si allinea alle [linee guida per il marchio](brands.md).

1. Una volta trovato il contenuto appropriato, fai clic su **[!UICONTROL Seleziona]**.

1. Inserisci campi di personalizzazione per personalizzare il contenuto in base ai dati dei profili. Quindi, fai clic sul pulsante **[!UICONTROL Simula contenuto]** per controllare il rendering e controlla le impostazioni di personalizzazione con i profili di test. [Ulteriori informazioni](../personalization/personalize.md)

1. Rivedi e attiva il contenuto:
   * **Notifica push**: una volta definiti il contenuto, il pubblico e la pianificazione, puoi preparare la consegna della notifica push. [Ulteriori informazioni](../push/send-push.md)
   * **SMS**: una volta che il tuo SMS è pronto, puoi pubblicarlo per renderlo disponibile per l&#39;utilizzo in un messaggio. [Ulteriori informazioni](../sms/send-sms.md)
