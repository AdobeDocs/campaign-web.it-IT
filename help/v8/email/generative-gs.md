---
audience: end-user
title: Introduzione all’assistente ai contenuti
description: Introduzione all’assistente ai contenuti
badge: label="Alpha"
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
hide: true
hidefromtoc: true
source-git-commit: efb5d5d9ea3b3559c57d6a0b2a250f075dabf831
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 100%

---

# Introduzione all’assistente ai contenuti {#generative-gs}

<!--
>[!CONTEXTUALHELP]
>id="acw_emagica_generate"
>title="Adobe Generative AI terms"
>abstract="Access to this feature is subject to your agreement to the Adobe Experience Cloud Generative AI User Guidelines, and the following:
* Any prompts, context, or supplemental information, or other input you provide to this feature (a) must be tied to specific context, which can include your branding materials, website content, data, schemas for such data, templates, or other trusted documents, and (b) must not contain any personal information (personal information includes anything that can be linked back to a specific invidual).
* You should review any output from this feature for accuracy and ensure that it is appropriate for your use case."
>additional-url="https://www.adobe.com/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Adobe Generative AI User Guidelines"
-->

>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="Assistente contenuto"
>abstract="Dopo aver creato e personalizzato la consegna, puoi migliorarne i contenuti utilizzando la funzione Assistente contenuto. Questa semplifica il processo di personalizzazione e miglioramento dei contenuti consentendoti di perfezionarli descrivendo cosa desideri generare."


>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="Definire il contesto per la generazione di contenuti"
>abstract="Per utilizzare il contenuto selezionato come input per la generazione di contenuti, attiva l’interruttore **Migliora con il contenuto corrente**. Puoi anche caricare le risorse del tuo marchio per utilizzarle come origine. Se non utilizzi il contenuto selezionato, devi obbligatoriamente caricare e selezionare le risorse di un marchio."

La funzione Assistente contenuto, basata su IA generativa, è uno strumento prezioso per migliorare il contenuto delle e-mail. Semplifica la personalizzazione e il miglioramento dei contenuti, ottimizzando le consegne e-mail per il tuo pubblico in modo da renderle più efficaci.

Questa funzione genera in automatico dicontenuti e-mail completi, consentendoti di risparmiare tempo e di ottenere contenuti di qualità e coerenti. Utilizzando la IA generativa, puoi creare e-mail coinvolgenti senza difficoltà, migliorando l’efficacia e l’efficienza delle comunicazioni.


La funzione Assistente contenuto di Campaign può essere sfruttata nelle e-mail per: [generare immagini](generative-image.md), [generare contenuti di testo](generative-content.md), [generare l’intero contenuto HTML](generative-email.md).

>[!NOTE]
>
>Questa funzionalità è disponibile in versione Alpha ed è soggetta a modifiche senza preavviso. Verrà attivata all’inizio di ottobre.

## Guardrail e limitazioni {#generative-guardrails}

Di seguito sono elencate alcune linee guida generali su come utilizza Assistente contenuto nella generazione di e-mail:

* La qualità del contenuto generato è fortemente influenzata dalla finalità dell’iniziativa di marketing e dal prompt che inserisci nelle impostazioni. Inserisci un prompt chiaro e preciso nelle impostazioni, per consentire al modello GenAI di interpretarle con precisione. 
* Per ottenere contenuti accurati e in linea con i requisiti del marchio, carica una risorsa del marchio. In caso contrario, il contenuto verrà generato sulla base di informazioni di pubblico dominio. Puoi caricare contenuti nei seguenti formati: file PDF, immagini JPEG o PNG, o file ZIP (contenenti formati di file supportati).
* La risorsa del marchio caricata dovrebbe essere di diemnsione inferiore a 10 MB.È possibile utilizzare anche file di dimensioni maggiori o numerose immagini, ma questo comporterà tempi di elaborazione più lunghi.
* Per creare il contenuto dell’e-mail, utilizza un modello creato in Adobe Campaign o, preferibilmente, uno dei [modelli e-mail incorporati](../email/create-email-templates.md). Si consiglia di utilizzare un modello e-mail con un massimo di 8-10 immagini.


La funzione Assistente contenuto di Campaign è soggetta alle seguenti limitazioni:

* È supportata solo la lingua inglese.
* È disponibile solo per il canale E-mail.
* Il contenuto GenAI potrebbe non essere sempre accurato: condividi il tuo feedback in modo che i nostri tecnici possano perfezionare i modelli.
* Puoi caricare più risorse del tuo marchio, ma puoi sfruttarne una sola per una generazione specifica.



<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-content.md">
<img alt="Generazione di testo" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
<a href="generative-content.md"><strong>Generazione di testo con Assistente contenuto</strong></a>
</div>
<p>
</td>
<td>
<a href="generative-image.md">
<img alt="Generazione di immagini" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div><a href="generative-image.md"><strong>Generazione di immagini con Assistente contenuto</strong>
</div>
<p>
</td>
<td>
<a href="generative-email.md">
<img alt="Generazione di e-mail" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
<a href="generative-email.md"><strong>Generazione di e-mail con Assistente contenuto</strong></a>
</div>
<p></td>
</tr></table>
