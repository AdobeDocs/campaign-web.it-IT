---
audience: end-user
title: Contenuto generativo
description: Introduzione all’Assistente IA in Campaign
badge: label="Beta"
exl-id: d9d35c1d-13db-4d2c-82f8-1629fd1e5848
hide: true
hidefromtoc: true
source-git-commit: fe687647b0a3d4969373ced400c49b364e878acd
workflow-type: tm+mt
source-wordcount: '1369'
ht-degree: 24%

---

# Generazione di e-mail con l’Assistente IA {#generative-content}

>[!BEGINSHADEBOX]

**Sommario**

* [Introduzione all’Assistente IA](generative-gs.md)
* Generazione di e-mail con l’Assistente IA
* [Generazione di SMS con l’Assistente IA](generative-sms.md)
* [Generazione di notifiche push con l’Assistente IA](generative-push.md)

>[!ENDSHADEBOX]

>[!NOTE]
>
>Prima di iniziare a utilizzare questa funzionalità, leggi l’articolo sui relativi [Guardrail e limitazioni](generative-gs.md#generative-guardrails).

Dopo aver creato e personalizzato le e-mail, utilizza l’Assistente all’intelligenza artificiale in Campaign basato sull’intelligenza artificiale generativa per portare il contenuto al livello successivo.

L’Assistente AI può aiutarti a ottimizzare l’impatto delle consegne generando e-mail intere, contenuto di testo mirato e persino immagini personalizzate per far risuonare il messaggio al tuo pubblico. In questo modo è possibile ottimizzare le campagne e-mail per un coinvolgimento migliore.

Con le campagne e-mail, puoi utilizzare l’assistente AI per generare e-mail, testo o immagini completi. Esplora le schede seguenti per scoprire come utilizzare l’Assistente IA in Campaign.

>[!BEGINTABS]

>[!TAB Generazione e-mail completa]

Nell’esempio seguente, sfrutteremo l’assistente AI per perfezionare un’e-mail esistente, personalizzandola per un evento speciale.

1. Dopo aver creato e configurato la consegna e-mail, fai clic su **[!UICONTROL Modifica contenuto]**.

   Per ulteriori informazioni su come configurare la consegna e-mail, consulta [questa pagina](../email/create-email-content.md).

1. Personalizza l’e-mail in base alle esigenze e accedi al **[!UICONTROL Assistente AI]** menu.

   ![](assets/full-email-1.png){zoomable=&quot;yes&quot;}

1. Abilita **[!UICONTROL Usa contenuto originale]** Opzione per l’Assistente AI per personalizzare i nuovi contenuti in base alla consegna, al nome della consegna e al pubblico selezionato.

   La richiesta deve essere sempre associata al contenuto corrente.

1. Ottimizza il contenuto descrivendo cosa desideri generare nel **[!UICONTROL Prompt]** campo.

   Se stai cercando assistenza per creare il tuo prompt, accedi al **[!UICONTROL Libreria dei prompt]** che offre una vasta gamma di idee per migliorare le tue consegne.

   ![](assets/full-email-2.png){zoomable=&quot;yes&quot;}

1. È possibile attivare/disattivare **[!UICONTROL Oggetto]** o **[!UICONTROL Preheader]** per includerli nella generazione delle varianti.

1. Clic **[!UICONTROL Carica risorsa marchio]** per aggiungere qualsiasi risorsa del brand contenente contenuti che possano fornire ulteriore contesto, utilizza l’Assistente per l’intelligenza artificiale o selezionane una caricata in precedenza.

   ![](assets/full-email-3.png){zoomable=&quot;yes&quot;}

1. Personalizza il prompt con le diverse opzioni:

   * **[!UICONTROL Strategia di comunicazione]**: scegli lo stile di comunicazione più adatto al testo generato.
   * **[!UICONTROL Lingua]**: seleziona la lingua in cui desideri generare il contenuto.
   * **[!UICONTROL Tono]**: il tono dell’e-mail dovrebbe risuonare con il pubblico. Che tu voglia essere informativo, giocoso o persuasivo, l’Assistente AI può adattare il messaggio di conseguenza.
   * **[!UICONTROL Lunghezza]**: scegli la lunghezza desiderata del contenuto utilizzando il cursore intervallo.

   ![](assets/full-email-4.png){zoomable=&quot;yes&quot;}

1. Una volta completato il prompt, fai clic su **[!UICONTROL Genera]**.

1. Sfoglia il generato **[!UICONTROL Varianti]** e fai clic su **[!UICONTROL Anteprima]** per visualizzare una versione a schermo intero della variante selezionata.

1. Accedi a **[!UICONTROL Perfeziona]** all&#39;interno del **[!UICONTROL Anteprima]** finestra per accedere ad altre funzioni di personalizzazione:

   * **[!UICONTROL Utilizza come contenuto di riferimento]**: la variante scelta fungerà da contenuto di riferimento per la generazione di altri risultati.

   * **[!UICONTROL Riformula]**: l’Assistente AI può riformulare il messaggio in diversi modi, mantenendo la scrittura fresca e coinvolgente per diversi tipi di pubblico.

   * **[!UICONTROL Utilizza un linguaggio più semplice]**: sfrutta l’Assistente AI per semplificare la lingua, garantendo chiarezza e accessibilità a un pubblico più ampio.

   ![](assets/full-email-5.png){zoomable=&quot;yes&quot;}

1. Una volta trovato il contenuto appropriato, fai clic su **[!UICONTROL Seleziona]**.

1. Inserisci campi di personalizzazione per personalizzare il contenuto delle e-mail in base ai dati dei profili. Quindi, fai clic su **[!UICONTROL Simula contenuto]** per controllare il rendering e controllare le impostazioni di personalizzazione con i profili di test. [Ulteriori informazioni](../preview-test/preview-content.md)

   ![](assets/full-email-6.png){zoomable=&quot;yes&quot;}

Una volta definiti il contenuto, il pubblico e la pianificazione, puoi preparare la consegna e-mail. [Ulteriori informazioni](../monitor/prepare-send.md)

>[!TAB Generazione testo]

Nell’esempio seguente, sfrutteremo l’assistente AI per migliorare il contenuto del nostro invito e-mail per il nostro evento imminente.

1. Dopo aver creato e configurato la consegna e-mail, fai clic su **[!UICONTROL Modifica contenuto]**.

   Per ulteriori informazioni su come configurare la consegna e-mail, consulta [questa pagina](../email/create-email-content.md).

1. Seleziona un **[!UICONTROL Componente testo]** per impostare come destinazione solo un contenuto specifico. e accedere al **[!UICONTROL Assistente AI]** menu.

   ![](assets/text-genai-1.png){zoomable=&quot;yes&quot;}

1. Abilita **[!UICONTROL Usa contenuto originale]** Opzione per l’Assistente AI per personalizzare i nuovi contenuti in base alla consegna, al nome della consegna e al pubblico selezionato.

   La richiesta deve essere sempre associata al contenuto corrente.

1. Ottimizza il contenuto descrivendo cosa desideri generare nel **[!UICONTROL Prompt]** campo.

   Se stai cercando assistenza per creare il tuo prompt, accedi al **[!UICONTROL Libreria dei prompt]** che offre una vasta gamma di idee per migliorare le tue consegne.

   ![](assets/text-genai-2.png){zoomable=&quot;yes&quot;}

1. Clic **[!UICONTROL Carica risorsa marchio]** per aggiungere qualsiasi risorsa del brand contenente contenuti che possano fornire ulteriore contesto all’Assistente AI.

   ![](assets/text-genai-3.png){zoomable=&quot;yes&quot;}

1. Personalizza il prompt con le diverse opzioni:

   * **[!UICONTROL Strategia di comunicazione]**: seleziona l’approccio di comunicazione desiderato per il testo generato.
   * **[!UICONTROL Lingua]**: scegli la lingua per il contenuto della variante.
   * **[!UICONTROL Tono]**: assicurati che il testo sia appropriato per il pubblico e lo scopo.
   * **[!UICONTROL Lunghezza]**: seleziona la lunghezza del contenuto utilizzando il cursore intervallo.

   ![](assets/text-genai-4.png){zoomable=&quot;yes&quot;}

1. Una volta completato il prompt, fai clic su **[!UICONTROL Genera]**.

1. Sfoglia il generato **[!UICONTROL Varianti]** e fai clic su **[!UICONTROL Anteprima]** per visualizzare una versione a schermo intero della variante selezionata.

1. Accedi a **[!UICONTROL Perfeziona]** all&#39;interno del **[!UICONTROL Anteprima]** finestra per accedere ad altre funzioni di personalizzazione:

   * **[!UICONTROL Utilizza come contenuto di riferimento]**: la variante scelta fungerà da contenuto di riferimento per la generazione di altri risultati.

   * **[!UICONTROL Elaborare]**: l’Assistente AI può aiutarti a espandere argomenti specifici, fornendo ulteriori dettagli per una migliore comprensione e coinvolgimento.

   * **[!UICONTROL Riepiloga]**: informazioni lunghe possono sovraccaricare i destinatari delle e-mail. Utilizza l’Assistente per l’intelligenza artificiale per condensare i punti chiave in riepiloghi chiari e concisi che catturino l’attenzione e li incoraggino a leggere ulteriormente.

   * **[!UICONTROL Riformula]**:L’Assistente AI può riformulare il messaggio in diversi modi, mantenendo la scrittura fresca e coinvolgente per diversi tipi di pubblico.

   * **[!UICONTROL Utilizza un linguaggio più semplice]**: sfrutta l’Assistente AI per semplificare la lingua, garantendo chiarezza e accessibilità a un pubblico più ampio.

   ![](assets/text-genai-5.png){zoomable=&quot;yes&quot;}

1. Una volta trovato il contenuto appropriato, fai clic su **[!UICONTROL Seleziona]**.

1. Inserisci campi di personalizzazione per personalizzare il contenuto delle e-mail in base ai dati dei profili. Quindi, fai clic su **[!UICONTROL Simula contenuto]** per controllare il rendering e controllare le impostazioni di personalizzazione con i profili di test. [Ulteriori informazioni](../preview-test/preview-content.md)

   ![](assets/text-genai-7.png){zoomable=&quot;yes&quot;}

Una volta definiti il contenuto, il pubblico e la pianificazione, puoi preparare la consegna e-mail. [Ulteriori informazioni](../monitor/prepare-send.md)

>[!TAB Generazione di immagini]

Nell’esempio seguente, scopri come sfruttare l’Assistente AI per ottimizzare e migliorare le risorse, garantendo un’esperienza più semplice da usare.

1. Dopo aver creato e configurato la consegna e-mail, fai clic su **[!UICONTROL Modifica contenuto]**.

   Per ulteriori informazioni su come configurare la consegna e-mail, consulta [questa pagina](../email/create-email-content.md).

1. Compila i **[!UICONTROL Dettagli di base]** per la consegna. Al termine, fai clic su **[!UICONTROL Modifica contenuto e-mail]**.

1. Seleziona la risorsa da modificare con l’Assistente AI.

1. Dal menu di destra, seleziona **[!UICONTROL Assistente AI]**.

   ![](assets/image-genai-1.png){zoomable=&quot;yes&quot;}

1. Ottimizza il contenuto descrivendo cosa desideri generare nel **[!UICONTROL Prompt]** campo.

   Se stai cercando assistenza per creare il tuo prompt, accedi al **[!UICONTROL Libreria dei prompt]** che offre una vasta gamma di idee per migliorare le tue consegne.

   ![](assets/image-genai-2.png){zoomable=&quot;yes&quot;}

1. Clic **[!UICONTROL Carica risorsa marchio]** per aggiungere qualsiasi risorsa del brand contenente contenuti che possano fornire ulteriore contesto all’Assistente AI.

   La richiesta deve essere sempre associata a un contesto specifico.

1. Personalizza il prompt con le diverse opzioni:

   * **[!UICONTROL Proporzioni]**: determina la larghezza e l’altezza della risorsa. È possibile scegliere tra rapporti comuni, ad esempio 16:9, 4:3, 3:2 o 1:1, oppure immettere una dimensione personalizzata.
   * **[!UICONTROL Colore e tonalità]**: l’aspetto complessivo dei colori all’interno di un’immagine e l’umore o l’atmosfera che trasmette.
   * **[!UICONTROL Tipo di contenuto]**: categorizza la natura dell’elemento visivo, distinguendo tra diverse forme di rappresentazione visiva come foto, grafica o arte.
   * **[!UICONTROL Illuminazione]**: si riferisce al fulmine presente in un’immagine, che ne forma l’atmosfera ed evidenzia elementi specifici.
   * **[!UICONTROL Composizione]**: si riferisce alla disposizione degli elementi nel fotogramma di un’immagine

   ![](assets/image-genai-3.png){zoomable=&quot;yes&quot;}

1. Una volta completata la configurazione del prompt, fai clic su **[!UICONTROL Genera]**.

1. Sfoglia **[!UICONTROL Suggerimenti varianti]** per trovare la risorsa desiderata.

   Fai clic su **[!UICONTROL Anteprima]** per visualizzare una versione a schermo intero della variante selezionata.

   ![](assets/image-genai-5.png){zoomable=&quot;yes&quot;}

1. Scegli **[!UICONTROL Mostra simili]** se desideri visualizzare le immagini correlate a questa variante.

1. Una volta trovato il contenuto appropriato, fai clic su **[!UICONTROL Seleziona]**.

   ![](assets/image-genai-6.png){zoomable=&quot;yes&quot;}

1. Dopo aver definito il contenuto del messaggio, fai clic sul pulsante **[!UICONTROL Simula contenuto]** per controllare il rendering e verificare le impostazioni di personalizzazione con i profili di test.  [Ulteriori informazioni](../preview-test/preview-content.md)

   ![](assets/image-genai-7.png){zoomable=&quot;yes&quot;}

1. Una volta definiti il contenuto, il pubblico e la pianificazione, puoi preparare la consegna e-mail. [Ulteriori informazioni](../monitor/prepare-send.md)

>[!ENDTABS]


## Video dimostrativo {#video}

Scopri come utilizzare l’Assistente AI per generare contenuti e-mail, testo e immagini completi.

>[!VIDEO](https://video.tv.adobe.com/v/3428984)

