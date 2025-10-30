---
audience: end-user
title: Notifica push con Assistente IA
description: Introduzione all’Assistente AI
exl-id: a361f75d-63c2-4fdc-993c-f8414b18e13e
source-git-commit: 127c65a466c41e1aba8408aa9cf41c2d89c93801
workflow-type: tm+mt
source-wordcount: '589'
ht-degree: 3%

---

# Generazione di notifiche push con Assistente IA {#generative-push}

>[!IMPORTANT]
>
>Prima di iniziare a utilizzare questa funzionalità, leggi le [protezioni e limitazioni](generative-gs.md#generative-guardrails) correlate.
>&#x200B;></br>
>
>È necessario accettare un [contratto utente](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html) prima di utilizzare l&#39;Assistente IA in Adobe Campaign Web. Per ulteriori informazioni, contatta il rappresentante Adobe.

L’Assistente AI consente di ottimizzare l’impatto delle consegne suggerendo contenuti diversi in base alle esigenze del pubblico.

Nell’esempio seguente, l’Assistente AI viene utilizzato per creare messaggi convincenti per creare un’esperienza del cliente più coinvolgente.

1. Dopo aver creato e configurato la consegna delle notifiche push, fai clic su **[!UICONTROL Modifica contenuto]**.

   Per ulteriori informazioni sulla configurazione della consegna push, consulta [questa pagina](../push/create-push.md).

1. Accedere al menu **[!UICONTROL Mostra Assistente AI]**.

   ![Schermata che mostra il menu Mostra Assistente AI](assets/push-genai-1.png){zoomable="yes"}

1. Abilita l&#39;opzione **[!UICONTROL Usa contenuto originale]** per l&#39;Assistente AI per personalizzare nuovi contenuti in base al contenuto selezionato.

1. Ottimizzare il contenuto descrivendo cosa si desidera generare nel campo **[!UICONTROL Prompt]**.

   Se hai bisogno di assistenza per creare il prompt, accedi alla **[!UICONTROL Libreria prompt]**, che fornisce una vasta gamma di idee per migliorare le consegne.

   ![Schermata che mostra l&#39;interfaccia della libreria di richieste](assets/push-genai-2.png){zoomable="yes"}

1. Scegli il campo da generare: **[!UICONTROL Titolo]**, **[!UICONTROL Sottotitolo]**, **[!UICONTROL Messaggio]** e/o **[!UICONTROL Immagine]**.

1. Personalizza la richiesta utilizzando l&#39;opzione **[!UICONTROL Impostazioni testo]**:

   * **[!UICONTROL Strategia di comunicazione]**: scegli lo stile di comunicazione più adatto al testo generato.
   * **[!UICONTROL Tono]**: regola il tono dell&#39;e-mail in modo che risuonino con il pubblico. Che tu voglia essere informativo, giocoso o persuasivo, l’Assistente AI adatta il messaggio di conseguenza.

   ![Schermata che mostra le opzioni delle impostazioni del testo](assets/push-genai-3.png){zoomable="yes"}

1. Scegli le **[!UICONTROL impostazioni immagine]**:

   * **[!UICONTROL Tipo di contenuto]**: categorizza la natura dell&#39;elemento visivo, distinguendo tra diverse forme di rappresentazione visiva come foto, immagini o immagini.
   * **[!UICONTROL Intensità visiva]**: controlla l&#39;impatto dell&#39;immagine regolandone l&#39;intensità. Un&#39;impostazione più bassa (2) crea un aspetto più morbido e più contenuto, mentre un&#39;impostazione più alta (10) rende l&#39;immagine più vibrante e visivamente potente.
   * **[!UICONTROL Illuminazione]**: regola l&#39;illuminazione nell&#39;immagine per modellarne l&#39;atmosfera ed evidenziare elementi specifici.
   * **[!UICONTROL Composizione]**: dispone gli elementi all&#39;interno della cornice dell&#39;immagine.

   ![Schermata che mostra le opzioni delle impostazioni immagine](assets/push-genai-4.png){zoomable="yes"}

1. Dal menu **[!UICONTROL Risorse per i marchi]**, fai clic su **[!UICONTROL Carica risorsa per i marchi]** per aggiungere eventuali risorse per i marchi contenenti contenuto che fornisca ulteriore contesto all&#39;Assistente di intelligenza artificiale, oppure selezionane una caricata in precedenza.

   I file precedentemente caricati sono disponibili nel menu a discesa **[!UICONTROL Risorse del brand caricate]**. Attiva/disattiva le risorse da includere nella generazione.

1. Una volta completato il prompt, fai clic su **[!UICONTROL Genera]**.

1. Sfoglia le **[!UICONTROL Varianti]** generate e fai clic su **[!UICONTROL Anteprima]** per visualizzare una versione a schermo intero della variante selezionata oppure su **[!UICONTROL Applica]** per sostituire il contenuto corrente.

1. Fai clic sull&#39;icona percentuale per visualizzare il **[!UICONTROL punteggio di allineamento del brand]** e identificare eventuali disallineamenti con il brand.

   Ulteriori informazioni sul [Punteggio di allineamento del marchio](../content/brands-score.md).

   ![](assets/push-genai-6.png){zoomable="yes"}

1. Passa all&#39;opzione **[!UICONTROL Perfeziona]** nella finestra **[!UICONTROL Anteprima]** per accedere ad altre funzioni di personalizzazione:

   * **[!UICONTROL Utilizza come contenuto di riferimento]**: utilizza la variante scelta come contenuto di riferimento per generare altri risultati.
   * **[!UICONTROL Riformula]**: riformula il messaggio in diversi modi per mantenere la scrittura fresca e coinvolgente per diversi tipi di pubblico.
   * **[!UICONTROL Usa un linguaggio più semplice]**: semplifica la lingua per garantire chiarezza e accessibilità a un pubblico più ampio.

   Puoi anche modificare il **[!UICONTROL Tono]** e la **[!UICONTROL Strategia di comunicazione]** del tuo testo.

   ![Schermata che mostra le opzioni di ottimizzazione](assets/push-genai-5.png){zoomable="yes"}

1. Apri la scheda **[!UICONTROL Allineamento marchio]** per vedere come il contenuto si allinea alle [linee guida per il marchio](../content/brands.md).

1. Fai clic su **[!UICONTROL Seleziona]** una volta trovato il contenuto appropriato.

1. Inserisci campi di personalizzazione per personalizzare il contenuto delle e-mail in base ai dati del profilo. Quindi, fai clic sul pulsante **[!UICONTROL Simula contenuto]** per controllare il rendering e controllare le impostazioni di personalizzazione con i profili di test. [Ulteriori informazioni](../preview-test/preview-content.md)

Quando definisci il contenuto, il pubblico e la pianificazione, prepara la consegna push. [Ulteriori informazioni](../monitor/prepare-send.md)