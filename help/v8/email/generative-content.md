---
audience: end-user
title: Testo con l’Assistente AI
description: Introduzione all’Assistente IA in Campaign
badge: label="Beta"
exl-id: d9d35c1d-13db-4d2c-82f8-1629fd1e5848
hide: true
hidefromtoc: true
source-git-commit: 23c43fad6076fc1dd1eaec2aee1664773ac7ce09
workflow-type: tm+mt
source-wordcount: '1097'
ht-degree: 22%

---

# Generazione di e-mail con l’Assistente IA {#generative-content}

>[!BEGINSHADEBOX]

**Sommario**

* [Introduzione all’Assistente IA](generative-gs.md)
* **[Generazione di e-mail con l’Assistente AI](generative-content.md)**
* [Generazione di SMS con l’Assistente IA](generative-sms.md)
* [Generazione di notifiche push con l’Assistente IA](generative-push.md)

>[!ENDSHADEBOX]

Dopo aver creato e personalizzato le e-mail, utilizza l’Assistente di intelligenza artificiale di Journey Optimizer in Campaign basato sull’intelligenza artificiale generativa per portare il contenuto al livello successivo.

L’Assistente AI può aiutarti a ottimizzare l’impatto delle consegne suggerendo contenuti diversi che hanno maggiori probabilità di risuonare con il pubblico.

>[!NOTE]
>
>Prima di iniziare a utilizzare questa funzionalità, leggi l’articolo sui relativi [Guardrail e limitazioni](generative-gs.md#guardrails-and-limitations).

## Generazione di contenuti con l’Assistente AI {#generative-text}

Ecco come l’Assistente AI può aiutarti a scrivere e-mail coinvolgenti:

* **Riepiloga**: informazioni lunghe possono sovraccaricare i destinatari delle e-mail. Utilizza l’Assistente per l’intelligenza artificiale per condensare i punti chiave in riepiloghi chiari e concisi che catturino l’attenzione e li incoraggino a leggere ulteriormente.

* **Elaborare**: l’Assistente AI può aiutarti a espandere argomenti specifici, fornendo ulteriori dettagli per una migliore comprensione e coinvolgimento.

* **Semplifica lingua**: sfrutta l’Assistente AI per semplificare la lingua, garantendo chiarezza e accessibilità a un pubblico più ampio.

* **Riformula**:L’Assistente AI può riformulare il messaggio in diversi modi, mantenendo la scrittura fresca e coinvolgente per diversi tipi di pubblico.

* **Cambia tono**: il tono dell’e-mail dovrebbe risuonare con il pubblico. Che tu voglia essere informativo, giocoso o persuasivo, l’Assistente AI può adattare il messaggio di conseguenza.

Nell’esempio seguente, sfrutteremo l’assistente AI per migliorare il contenuto del nostro invito e-mail per il nostro evento imminente.

1. Dopo aver creato e configurato la consegna e-mail, fai clic su **[!UICONTROL Modifica contenuto]**.

   Per ulteriori informazioni su come configurare la consegna e-mail, consulta [questa pagina](../email/create-email-content.md).

1. Personalizza l’e-mail in base alle esigenze e accedi al **[!UICONTROL Assistente AI]** menu.

   È inoltre possibile selezionare una **[!UICONTROL Componente testo]** per impostare come destinazione solo un contenuto specifico.

   ![](assets/text-genai-1.png){zoomable=&quot;yes&quot;}

1. Abilita **[!UICONTROL Usa contenuto originale]** Opzione per l’Assistente AI per personalizzare i nuovi contenuti in base alla consegna, al nome della consegna e al pubblico selezionato.

   >[!IMPORTANT]
   >
   > Il prompt deve sempre essere associato a un contesto specifico caricando una risorsa del brand o abilitando **[!UICONTROL Migliora il contenuto corrente]** opzione.

1. Ottimizza il contenuto descrivendo cosa desideri generare nel **[!UICONTROL Prompt]** campo.

   Se stai cercando assistenza per creare il tuo prompt, accedi al **[!UICONTROL Libreria dei prompt]** che offre una vasta gamma di idee per migliorare le tue consegne.

   ![](assets/text-genai-2.png){zoomable=&quot;yes&quot;}

1. È possibile attivare/disattivare **[!UICONTROL Oggetto]** o **[!UICONTROL Preheader]** per includerli nella generazione delle varianti.

   Tieni presente che questa opzione è disponibile se non hai selezionato un componente Testo specifico.

1. Clic **[!UICONTROL Carica risorsa marchio]** per aggiungere qualsiasi risorsa del brand contenente contenuti che possano fornire ulteriore contesto all’Assistente AI.

   ![](assets/text-genai-3.png){zoomable=&quot;yes&quot;}

1. Personalizza il prompt con le diverse opzioni:

   * **[!UICONTROL Strategia di comunicazione]**: seleziona l’approccio di comunicazione desiderato per il testo generato.
   * **[!UICONTROL Lingua]**: scegli la lingua per il contenuto della variante.
   * **[!UICONTROL Tono]**: assicurati che il testo sia appropriato per il pubblico e lo scopo.
   * **[!UICONTROL Lunghezza]**: seleziona la lunghezza del contenuto utilizzando il cursore intervallo. Disponibile solo se è stato selezionato un componente Testo specifico.

   ![](assets/text-genai-4.png){zoomable=&quot;yes&quot;}

1. Una volta completato il prompt, fai clic su **[!UICONTROL Genera]**.

1. Sfoglia il generato **[!UICONTROL Varianti]** e fai clic su **[!UICONTROL Anteprima]** per visualizzare una versione a schermo intero della variante selezionata.

1. Accedi a **[!UICONTROL Perfeziona]** all&#39;interno del **[!UICONTROL Anteprima]** per accedere a funzioni di personalizzazione aggiuntive e perfezionare la variante in base alle preferenze.

   Una volta trovato il contenuto appropriato, fai clic su **[!UICONTROL Seleziona]**.

   ![](assets/text-genai-5.png){zoomable=&quot;yes&quot;}

1. Inserisci campi di personalizzazione per personalizzare il contenuto delle e-mail in base ai dati dei profili. Quindi, fai clic su **[!UICONTROL Simula contenuto]** per controllare il rendering e controllare le impostazioni di personalizzazione con i profili di test. [Ulteriori informazioni](../preview-test/preview-content.md)

   ![](assets/text-genai-7.png){zoomable=&quot;yes&quot;}

Una volta definiti il contenuto, il pubblico e la pianificazione, puoi preparare la consegna e-mail. [Ulteriori informazioni](../monitor/prepare-send.md)

## Generazione di immagini con l’Assistente AI {#generative-image}

Sfrutta l’Assistente AI per generare visualizzazioni diverse e personalizzate per le campagne e-mail. Ad esempio, può essere utilizzato per:

* **Genera**: genera una vasta gamma di immagini coinvolgenti appositamente progettate per le campagne e-mail. Il controllo granulare su impostazioni quali palette di colori, fulmini e composizione consente di risuonare con segmenti di pubblico distinti e raggiungere obiettivi specifici della campagna.

* **Genera simile**: utilizza l’Assistente AI per generare immagini simili da una variante selezionata.

* **Risorsa marchio**: ottimizza la selezione delle immagini per le campagne e-mail sfruttando sia le risorse interne del brand che le fonti esterne come Adobe Firefly.

Nell’esempio seguente, scopri come sfruttare l’Assistente AI per ottimizzare e migliorare i contenuti, garantendo un’esperienza più semplice da usare. Segui questi passaggi:

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

   >[!IMPORTANT]
   >
   > La richiesta deve essere sempre associata a un contesto specifico.

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
