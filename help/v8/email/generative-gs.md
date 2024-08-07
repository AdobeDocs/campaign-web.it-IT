---
audience: end-user
title: Introduzione all’Assistente IA
description: Introduzione all’Assistente AI
badge: label="Beta"
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
hide: true
hidefromtoc: true
source-git-commit: 7de6d85036eac7289e7fcf3a82a7c11be12d9c6e
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 47%

---

# Introduzione all’Assistente IA {#generative-gs}

>[!BEGINSHADEBOX]

**Tabella dei contenuti**

* Introduzione all’Assistente IA
* [Generazione di e-mail con l’Assistente IA](generative-content.md)
* [Generazione di SMS con l’Assistente IA](generative-sms.md)
* [Generazione di notifiche push con l’Assistente IA](generative-push.md)

>[!ENDSHADEBOX]

>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="Assistente IA"
>abstract="Dopo aver creato e personalizzato la consegna, puoi utilizzare l’Assistente IA per migliorare il contenuto. Questa funzione semplifica il processo di personalizzazione e miglioramento dei contenuti consentendoti di perfezionarli descrivendo cosa desideri generare."


>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="Definire il contesto con l’Assistente IA in Campaign"
>abstract="Per utilizzare il contenuto selezionato come input per la generazione di contenuti, attiva l’interruttore **Migliora con il contenuto corrente**. Puoi anche caricare le risorse del tuo marchio per utilizzarle come origine. Se non utilizzi il contenuto selezionato, devi obbligatoriamente caricare e selezionare le risorse di un marchio."


>[!CONTEXTUALHELP]
>id="acw_emagica_generate"
>title="Termini di IA generativa di Adobe"
>abstract="L’accesso a questa funzione è soggetto al consenso dell’utente alle linee guida per l’utente di IA generativa di Adobe Experience Cloud. Verifica che ogni output generato da questa funzione sia accurato e assicurati che sia appropriato al caso d’uso."
>additional-url="https://www.adobe.com/it/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Linee guida per l’utente sull’intelligenza artificiale generativa di Adobe"

Man mano che il settore Marketing diventa più competitivo, i brand cercano modi efficienti per generare contenuti di impatto in modo efficiente e rapido. L’Assistente per l’intelligenza artificiale in Campaign, basato su Azure OpenAI, è la funzionalità di generazione di contenuti di intelligenza artificiale di Adobe che rivoluziona il modo in cui gli esperti di marketing creano contenuti professionali e coerenti con il brand su canali diversi, come e-mail, SMS e push. Con modelli GenAI avanzati e una profonda comprensione delle linee guida del brand, AI Assistant genera automaticamente contenuti personalizzati, coinvolgenti ed efficaci in base all’obiettivo di marketing, con contenuti ottimizzati per stili, layout, toni e altro ancora delineati dal brand.

Ai Assistant rende la creazione e l’esecuzione di campagne di marketing su canali diversi come e-mail, SMS e push intuitivi, semplici e senza problemi, risparmiando tempo, migliorando l’efficienza e ottenendo risultati migliori.

>[!NOTE]
>
>Questa funzionalità è disponibile nella versione Beta e soggetta a modifiche senza preavviso.

## Guardrail e limitazioni {#generative-guardrails}

Di seguito sono elencate le linee guida generali per l’utilizzo dell’Assistente IA in Campaign per la generazione di e-mail:

* La qualità del contenuto generato è fortemente influenzata dalla finalità dell’iniziativa di marketing e dal prompt che inserisci nelle impostazioni. Inserisci un prompt chiaro e preciso nelle impostazioni, per consentire al modello GenAI di interpretarle con precisione. 
* Per ottenere contenuti accurati e in linea con i requisiti del marchio, carica una risorsa del marchio. In caso contrario, il contenuto verrà generato sulla base di informazioni di pubblico dominio. Puoi caricare contenuti nei seguenti formati: file PDF, immagini JPEG o PNG, o file ZIP (contenenti formati di file supportati).
* La dimensione massima per la risorsa del brand caricata è di 50 MB.È possibile utilizzare anche file di dimensioni maggiori o numerose immagini, ma questo comporterà tempi di elaborazione più lunghi.
* Utilizza un modello di e-mail creato da Adobe Campaign, preferibilmente [modelli e-mail incorporati](../email/create-email-templates.md), un modello specifico per il brand o un modello personalizzato per creare il contenuto delle e-mail. Si consiglia di utilizzare un modello e-mail con un massimo di 8-10 immagini.
* Assicurati di segnalare eventuali output problematici utilizzando le icone thumb up, thumb down o flag durante la selezione delle varianti.
* L’utilizzo dell’assistente IA è soggetto alle linee guida per l’utente di Adobe Experience Cloud Generative AI. [Ulteriori informazioni](https://www.adobe.com/it/legal/licenses-terms/adobe-gen-ai-user-guidelines.html)

All’Assistente IA in Campaign si applicano le seguenti limitazioni:

* La lingua supportata è solo inglese.
* Disponibile solo per i canali e-mail, push e SMS.
* Il contenuto GenAI potrebbe non essere sempre accurato: condividi il tuo feedback in modo che i nostri ingegneri possano perfezionare i modelli.
* Puoi caricare più risorse per il brand, ma puoi sfruttarne una sola per una generazione specifica.

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-content.md">
<img alt="Generazione di e-mail" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
<a href="generative-content.md"><strong>Generazione di e-mail con l'Assistente AI</strong></a>
</div>
<p>
</td>
<td>
<a href="generative-sms.md">
<img alt="Generazione di SMS" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div><a href="generative-sms.md"><strong>Generazione di SMS con l'Assistente AI</strong>
</div>
<p>
</td>
<td>
<a href="generative-push.md">
<img alt="Generazione push" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
<a href="generative-push.md"><strong>Generazione di notifiche push con l'Assistente IA</strong></a>
</div>
<p></td>
</tr></table>
