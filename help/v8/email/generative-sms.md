---
audience: end-user
title: SMS con l’Assistente AI
description: Introduzione all’Assistente AI
exl-id: db0459e5-8759-42d9-8945-8c9667450527
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '897'
ht-degree: 6%

---

# Generazione di SMS con l’Assistente IA {#generative-sms}

>[!IMPORTANT]
>
>Prima di iniziare a utilizzare questa funzionalità, leggi le [protezioni e limitazioni](generative-gs.md#generative-guardrails) correlate.
></br>
>
>È necessario accettare un [contratto utente](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html) prima di utilizzare l&#39;Assistente IA in Adobe Campaign Web. Per ulteriori informazioni, contatta il rappresentante Adobe.

Una volta creati e personalizzati i messaggi SMS per soddisfare il pubblico, eleva la tua comunicazione con l’Assistente AI in Adobe Campaign Web, basato su una tecnologia di intelligenza artificiale innovativa.

Questo strumento offre suggerimenti intelligenti per perfezionare i contenuti, garantendo una riproduzione efficace dei messaggi e massimizzando il coinvolgimento.

>[!BEGINTABS]

>[!TAB Generazione SMS completa]

1. Dopo aver creato e configurato la consegna SMS, fai clic su **[!UICONTROL Modifica contenuto]**.

   Per ulteriori informazioni sulla configurazione della consegna SMS, consulta [questa pagina](../sms/create-sms.md).

1. Compila i **[!UICONTROL Dettagli di base]** per la consegna. Al termine, fare clic su **[!UICONTROL Modifica contenuto]**.

1. Accedere al menu **[!UICONTROL Mostra Assistente AI]**.

   ![Schermata che mostra il menu Mostra Assistente AI](assets/sms-genai-1.png){zoomable="yes"}

1. Ottimizzare il contenuto descrivendo cosa si desidera generare nel campo **[!UICONTROL Prompt]**.

   Se hai bisogno di assistenza per creare il prompt, accedi alla **[!UICONTROL Libreria prompt]**, che fornisce una vasta gamma di idee per migliorare le consegne.

   ![Schermata che mostra la libreria dei prompt](assets/sms-genai-2.png){zoomable="yes"}

1. Personalizza la richiesta utilizzando l&#39;opzione **[!UICONTROL Impostazioni testo]**:

   * **[!UICONTROL Strategia di comunicazione]**: scegli lo stile di comunicazione più adatto al testo generato.
   * **[!UICONTROL Tono]**: assicurati che il tono dell&#39;e-mail risuoni con il pubblico. Che tu voglia essere informativo, giocoso o persuasivo, l’Assistente AI adatta il messaggio di conseguenza.
   * **Lunghezza testo**: utilizza il cursore per selezionare la lunghezza desiderata del testo.

   ![Schermata che mostra le opzioni delle impostazioni del testo](assets/sms-genai-3.png){zoomable="yes"}

1. Dal menu **[!UICONTROL Risorse per i marchi]**, fai clic su **[!UICONTROL Carica risorsa per i marchi]** per aggiungere eventuali risorse per i marchi contenenti contenuto che fornisca ulteriore contesto all&#39;Assistente IA, oppure selezionane una caricata in precedenza.

   I file precedentemente caricati sono disponibili nel menu a discesa **[!UICONTROL Risorse del brand caricate]**. Attiva/disattiva le risorse da includere nella generazione.

1. Una volta completato il prompt, fai clic su **[!UICONTROL Genera]**.

1. Sfoglia le **[!UICONTROL Varianti]** generate e fai clic su **[!UICONTROL Anteprima]** per visualizzare una versione a schermo intero della variante selezionata.

   ![Schermata che mostra le varianti generate](assets/sms-genai-4.png){zoomable="yes"}

1. Passa all&#39;opzione **[!UICONTROL Perfeziona]** nella finestra **[!UICONTROL Anteprima]** per accedere ad altre funzioni di personalizzazione e perfezionare la variante in base alle tue preferenze:

   * **[!UICONTROL Utilizza come contenuto di riferimento]**: la variante scelta funge da contenuto di riferimento per la generazione di altri risultati.
   * **[!UICONTROL Usa un linguaggio più semplice]**: l&#39;Assistente AI ti consente di scrivere messaggi chiari e concisi che tutti possono comprendere.
   * **[!UICONTROL Riformula]**: l&#39;Assistente AI riformula il messaggio per mantenerlo coinvolgente per diversi tipi di pubblico.

   Puoi anche modificare il **[!UICONTROL Tono]** e la **[!UICONTROL Strategia di comunicazione]** del tuo testo.

   ![Schermata che mostra le opzioni di ottimizzazione](assets/sms-genai-5.png){zoomable="yes"}

1. Fai clic su **[!UICONTROL Seleziona]** una volta trovato il contenuto appropriato.

1. Inserisci campi di personalizzazione per personalizzare il contenuto SMS in base ai dati di profilo. [Ulteriori informazioni sulla personalizzazione dei contenuti](../personalization/personalize.md).

   ![Schermata con campi di personalizzazione](assets/sms-genai-5.png){zoomable="yes"}

1. Dopo aver definito il contenuto del messaggio, fai clic sul pulsante **[!UICONTROL Simula contenuto]** per controllare il rendering e verificare le impostazioni di personalizzazione con i profili di test. [Ulteriori informazioni](../preview-test/preview-content.md).

   ![Schermata che mostra la simulazione del contenuto](assets/sms-genai-6.png){zoomable="yes"}

Quando definisci il contenuto, il pubblico e la pianificazione, prepara la consegna SMS. [Ulteriori informazioni](../monitor/prepare-send.md).

>[!TAB Generazione solo testo]

1. Dopo aver creato e configurato la consegna SMS, fai clic su **[!UICONTROL Modifica contenuto]**.

   Per ulteriori informazioni sulla configurazione della consegna SMS, consulta [questa pagina](../sms/create-sms.md).

1. Compila i **[!UICONTROL Dettagli di base]** per la consegna. Al termine, fare clic su **[!UICONTROL Modifica contenuto]**.

1. Personalizza il messaggio SMS in base alle esigenze. [Ulteriori informazioni](../sms/content-sms.md).

1. Accedi al menu **[!UICONTROL Assistente AI]** accanto al campo **[!UICONTROL Messaggio]**.

   ![Schermata che mostra il menu dell&#39;Assistente AI](assets/sms-text-1.png){zoomable="yes"}

1. Abilita l&#39;opzione **[!UICONTROL Usa contenuto di riferimento]** per l&#39;Assistente AI per personalizzare nuovi contenuti in base al contenuto selezionato.

1. Ottimizzare il contenuto descrivendo cosa si desidera generare nel campo **[!UICONTROL Prompt]**.

   Se hai bisogno di assistenza per creare il prompt, accedi alla **[!UICONTROL Libreria prompt]**, che fornisce una vasta gamma di idee per migliorare le campagne.

   ![Schermata che mostra la libreria dei prompt](assets/sms-text-2.png){zoomable="yes"}

1. Personalizza la richiesta utilizzando l&#39;opzione **[!UICONTROL Impostazioni testo]**:

   * **[!UICONTROL Strategia di comunicazione]**: selezionare l&#39;approccio di comunicazione desiderato per il testo generato.
   * **[!UICONTROL Lingua]**: scegli la lingua per il contenuto della variante.
   * **[!UICONTROL Tono]**: verifica che il testo sia appropriato per il tuo pubblico e il tuo scopo.
   * **[!UICONTROL Lunghezza]**: seleziona la lunghezza del contenuto utilizzando il cursore di intervallo.

   ![Schermata che mostra le opzioni delle impostazioni del testo](assets/sms-text-3.png){zoomable="yes"}

1. Dal menu **[!UICONTROL Risorse per i marchi]**, fai clic su **[!UICONTROL Carica risorsa per i marchi]** per aggiungere eventuali risorse per i marchi contenenti contenuto che fornisca ulteriore contesto all&#39;Assistente IA, oppure selezionane una caricata in precedenza.

   I file precedentemente caricati sono disponibili nel menu a discesa **[!UICONTROL Risorse del brand caricate]**. Attiva/disattiva le risorse da includere nella generazione.

1. Una volta completato il prompt, fai clic su **[!UICONTROL Genera]**.

1. Sfoglia le **[!UICONTROL Varianti]** generate e fai clic su **[!UICONTROL Anteprima]** per visualizzare una versione a schermo intero della variante selezionata.

1. Passa all&#39;opzione **[!UICONTROL Perfeziona]** nella finestra **[!UICONTROL Anteprima]** per accedere ad altre funzioni di personalizzazione e perfezionare la variante in base alle tue preferenze:

   * **[!UICONTROL Utilizza come contenuto di riferimento]**: la variante scelta funge da contenuto di riferimento per la generazione di altri risultati.
   * **[!UICONTROL Riformula]**: l&#39;Assistente di intelligenza artificiale può riformulare il messaggio in diversi modi, mantenendo la scrittura fresca e coinvolgente per diversi tipi di pubblico.
   * **[!UICONTROL Usa un linguaggio più semplice]**: sfrutta l&#39;Assistente AI per semplificare la lingua, garantendo chiarezza e accessibilità a un pubblico più ampio.

   Puoi anche modificare il **[!UICONTROL Tono]** e la **[!UICONTROL Strategia di comunicazione]** del tuo testo.

   ![Schermata che mostra le opzioni di ottimizzazione](assets/sms-text-4.png){zoomable="yes"}

1. Fai clic su **[!UICONTROL Seleziona]** una volta trovato il contenuto appropriato.

1. Inserisci campi di personalizzazione per personalizzare il contenuto SMS in base ai dati di profilo. [Ulteriori informazioni sulla personalizzazione dei contenuti](../personalization/personalize.md).

1. Dopo aver definito il contenuto del messaggio, fai clic sul pulsante **[!UICONTROL Simula contenuto]** per controllare il rendering e verificare le impostazioni di personalizzazione con i profili di test. [Ulteriori informazioni](../preview-test/preview-content.md).

   ![Schermata che mostra la simulazione del contenuto](assets/sms-text-5.png){zoomable="yes"}

Quando definisci il contenuto, il pubblico e la pianificazione, prepara la consegna SMS. [Ulteriori informazioni](../monitor/prepare-send.md).

>[!ENDTABS]