---
audience: end-user
title: Notifica push con l’Assistente IA in Campaign
description: Introduzione all’Assistente IA in Campaign
badge: label="Beta"
hide: true
hidefromtoc: true
exl-id: a361f75d-63c2-4fdc-993c-f8414b18e13e
source-git-commit: 886fd47b52d08b0a1bfcbeca03929d48b5bc2a3f
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 34%

---

# Generazione di notifiche push con l’Assistente AI {#generative-push}

>[!BEGINSHADEBOX]

**Sommario**

* [Introduzione all’Assistente IA](generative-gs.md)
* [Generazione di e-mail con l’Assistente AI](generative-content.md)
* [Generazione di SMS con l’Assistente AI](generative-sms.md)
* **[Generazione di notifiche push con l’Assistente AI](generative-push.md)**

>[!ENDSHADEBOX]

Dopo aver creato e personalizzato le e-mail, utilizza l’Assistente all’intelligenza artificiale in Campaign basato sull’intelligenza artificiale generativa per portare il contenuto al livello successivo.

L’Assistente AI può aiutarti a ottimizzare l’impatto delle consegne suggerendo contenuti diversi che hanno maggiori probabilità di risuonare con il pubblico.

>[!NOTE]
>
>Prima di iniziare a utilizzare questa funzionalità, leggi l’articolo sui relativi [Guardrail e limitazioni](generative-gs.md#guardrails-and-limitations).

1. Dopo aver creato e configurato la consegna delle notifiche push, fai clic su **[!UICONTROL Modifica contenuto]**.

   Per ulteriori informazioni su come configurare la consegna push, consulta [questa pagina](../push/create-push.md).

1. Compila i **[!UICONTROL Dettagli di base]** per la consegna. Al termine, fai clic su **[!UICONTROL Modifica contenuto]**.

1. Personalizza la notifica push in base alle esigenze. [Ulteriori informazioni](../push/content-push.md)

1. Accedere a **[!UICONTROL Mostra Assistente IA]** menu.

   ![](assets/push-genai-1.png){zoomable=&quot;yes&quot;}

1. Ottimizza il contenuto descrivendo cosa desideri generare nel **[!UICONTROL Prompt]** campo.

   Se stai cercando assistenza per creare il tuo prompt, accedi al **[!UICONTROL Libreria dei prompt]** che offre una vasta gamma di idee per migliorare le tue consegne.

   ![](assets/push-genai-2.png){zoomable=&quot;yes&quot;}

1. Abilita **[!UICONTROL Migliora con il contesto corrente]** Opzione per l’Assistente AI per personalizzare i nuovi contenuti in base alla consegna, al nome della consegna e al pubblico selezionato.

   >[!IMPORTANT]
   >
   > Il prompt deve sempre essere associato a un contesto specifico caricando una risorsa del brand o abilitando **[!UICONTROL Migliora il contenuto corrente]** opzione.

   ![](assets/push-genai-3.png){zoomable=&quot;yes&quot;}

1. Seleziona **[!UICONTROL Carica risorsa marchio]** per aggiungere qualsiasi risorsa del brand contenente contenuti che possano fornire ulteriore contesto all’Assistente AI.

1. Scegliere il campo da generare: **[!UICONTROL Titolo]**, **[!UICONTROL Sottotitolo]** o **[!UICONTROL Messaggio]**.

1. Seleziona la **[!UICONTROL Strategia di comunicazione]** più adatta alle tue esigenze. Questa influisce sul tono e sullo stile del testo generato.

1. Scegli la **[!UICONTROL Lingua]** e il **[!UICONTROL Tono]** da applicare al testo generato. Il testo generato sarà quindi appropriato per il pubblico e lo scopo a cui è destinato.

   ![](assets/push-genai-4.png){zoomable=&quot;yes&quot;}

1. Una volta completato il prompt, fai clic su **[!UICONTROL Genera]**.

1. Sfoglia le **[!UICONTROL Varianti]** generate, individua il contenuto apprpriato e fai clic su **[!UICONTROL Applica]**.

   Fai clic su **[!UICONTROL Anteprima]** per visualizzare una versione a schermo intero della variante selezionata.

   ![](assets/push-genai-5.png){zoomable=&quot;yes&quot;}

1. Inserisci campi di personalizzazione per personalizzare il contenuto push in base ai dati dei profili. [Ulteriori informazioni sulla personalizzazione dei contenuti](../personalization/personalize.md)

   ![](assets/push-genai-6.png){zoomable=&quot;yes&quot;}

1. Dopo aver definito il contenuto del messaggio, fai clic sul pulsante **[!UICONTROL Simula contenuto]** per controllare il rendering e verifica le impostazioni di personalizzazione con i profili di test. [Ulteriori informazioni](../preview-test/preview-content.md)

   ![](assets/push-genai-7.png){zoomable=&quot;yes&quot;}

1. Una volta definiti il contenuto, il pubblico e la pianificazione, sei pronto per preparare la consegna push. [Ulteriori informazioni](../monitor/prepare-send.md)
