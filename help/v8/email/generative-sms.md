---
audience: end-user
title: SMS con l’assistente AI in Campaign
description: Introduzione all’Assistente IA in Campaign
badge: label="Beta"
hide: true
hidefromtoc: true
exl-id: db0459e5-8759-42d9-8945-8c9667450527
source-git-commit: fe687647b0a3d4969373ced400c49b364e878acd
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 20%

---

# Generazione di SMS con l’Assistente IA {#generative-sms}

>[!BEGINSHADEBOX]

**Tabella dei contenuti**

* [Introduzione all’Assistente IA](generative-gs.md)
* [Generazione di e-mail con l’Assistente IA](generative-content.md)
* Generazione di SMS con l’Assistente IA
* [Generazione di notifiche push con l’Assistente IA](generative-push.md)

>[!ENDSHADEBOX]

Dopo aver creato e personalizzato i messaggi SMS in base alle esigenze del pubblico, porta la tua comunicazione a un livello successivo con l’aiuto dell’Assistente AI in Campaign, basato su una tecnologia di intelligenza artificiale innovativa.

Questo comodo strumento offre suggerimenti intelligenti per perfezionare i contenuti, garantendo una riproduzione efficace dei messaggi e massimizzando il coinvolgimento.

>[!NOTE]
>
>Prima di iniziare a utilizzare questa funzionalità, leggi l’articolo sui relativi [Guardrail e limitazioni](generative-gs.md#generative-guardrails).

1. Dopo aver creato e configurato la consegna SMS, fai clic su **[!UICONTROL Modifica contenuto]**.

   Per ulteriori informazioni su come configurare la consegna SMS, consulta [questa pagina](../sms/create-sms.md).

1. Compila i **[!UICONTROL Dettagli di base]** per la consegna. Al termine, fai clic su **[!UICONTROL Modifica contenuto]**.

1. Personalizza il messaggio SMS in base alle esigenze. [Ulteriori informazioni](../sms/content-sms.md)

1. Accedere al menu **[!UICONTROL Mostra Assistente AI]**.

   ![](assets/sms-genai-1.png){zoomable="yes"}

1. Abilita l&#39;opzione **[!UICONTROL Usa contenuto originale]** affinché l&#39;Assistente AI personalizzi nuovi contenuti in base alla consegna, al nome della consegna e al pubblico selezionato.

   >[!IMPORTANT]
   >
   > La richiesta deve essere sempre associata al contenuto corrente.

1. Ottimizzare il contenuto descrivendo cosa si desidera generare nel campo **[!UICONTROL Prompt]**.

   Se stai cercando assistenza per creare il prompt, accedi alla **[!UICONTROL Libreria prompt]** che fornisce una vasta gamma di idee per migliorare le consegne.

   ![](assets/sms-genai-2.png){zoomable="yes"}

1. Seleziona **[!UICONTROL Carica risorsa marchio]** per aggiungere qualsiasi risorsa marchio contenente contenuto che possa fornire ulteriore contesto all&#39;Assistente IA.

1. Personalizza il prompt con le diverse opzioni:

   * **[!UICONTROL Strategia di comunicazione]**: selezionare l&#39;approccio di comunicazione desiderato per il testo generato.
   * **[!UICONTROL Lingua]**: scegli la lingua per il contenuto della variante.
   * **[!UICONTROL Tono]**: verifica che il testo sia appropriato per il pubblico e lo scopo.
   * **[!UICONTROL Lunghezza]**: seleziona la lunghezza del contenuto utilizzando il cursore di intervallo.

   ![](assets/sms-genai-3.png){zoomable="yes"}

1. Una volta completato il prompt, fai clic su **[!UICONTROL Genera]**.

1. Sfoglia le **[!UICONTROL Varianti]** generate e fai clic su **[!UICONTROL Anteprima]** per visualizzare una versione a schermo intero della variante selezionata.

1. Passa all&#39;opzione **[!UICONTROL Perfeziona]** nella finestra **[!UICONTROL Anteprima]** per accedere ad altre funzioni di personalizzazione e perfezionare la variante in base alle tue preferenze:

   * **[!UICONTROL Utilizza come contenuto di riferimento]**: la variante scelta fungerà da contenuto di riferimento per generare altri risultati.

   * **[!UICONTROL Usa un linguaggio più semplice]**: l&#39;assistente AI ti aiuta a scrivere messaggi chiari e concisi che tutti possono comprendere.

   * **[!UICONTROL Riformulazione]**: l&#39;Assistente AI riformula il messaggio per mantenere il coinvolgimento per diversi tipi di pubblico.

   ![](assets/sms-genai-4.png){zoomable="yes"}

1. Una volta trovato il contenuto appropriato, fai clic su **[!UICONTROL Seleziona]**.

1. Inserisci campi di personalizzazione per personalizzare il contenuto SMS in base ai dati dei profili. [Ulteriori informazioni sulla personalizzazione dei contenuti](../personalization/personalize.md)

   ![](assets/sms-genai-5.png){zoomable="yes"}

1. Dopo aver definito il contenuto del messaggio, fai clic sul pulsante **[!UICONTROL Simula contenuto]** per controllare il rendering e verifica le impostazioni di personalizzazione con i profili di test. [Ulteriori informazioni](../preview-test/preview-content.md)

   ![](assets/sms-genai-6.png){zoomable="yes"}

Una volta definiti il contenuto, il pubblico e la pianificazione, sei pronto per preparare la consegna SMS. [Ulteriori informazioni](../monitor/prepare-send.md)
