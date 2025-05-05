---
audience: end-user
title: Introduzione all’Assistente AI
description: Introduzione all’Assistente AI
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
source-git-commit: 5f7fe214c1c89b1ee25cea6d512bd1a55b5522ec
workflow-type: tm+mt
source-wordcount: '732'
ht-degree: 18%

---

# Utilizzare l’Assistente AI {#generative-gs}

>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="Assistente IA"
>abstract="Dopo aver creato e personalizzato la consegna, utilizza l’Assistente AI per migliorare i contenuti. Questa funzione semplifica il processo di personalizzazione e il miglioramento dei contenuti e ti consente di perfezionarli descrivendo cosa desideri generare."

>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="Definire il contesto con l’Assistente IA in Campaign"
>abstract="Per utilizzare il contenuto selezionato come input per la generazione di contenuti, attiva l’interruttore **Migliora con il contesto corrente**. Puoi anche caricare le risorse del tuo marchio per utilizzarle come origine. Se non utilizzi il contenuto selezionato, è necessari caricare e selezionare le risorse del brand."

>[!CONTEXTUALHELP]
>id="acw_emagica_generate"
>title="Condizioni per l’IA generativa di Adobe"
>abstract="L’accesso a questa funzione è soggetto al consenso alle linee guida per l’utente dell’IA generativa di Adobe Experience Cloud. Verifica l’accuratezza degli output generati da questa funzione e assicurati che siano appropriati al tuo caso d’uso."
>additional-url="https://www.adobe.com/it/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Linee guida per l’utente sull’intelligenza artificiale generativa di Adobe"

>[!INFO]
>
>Immergiti in un&#39;esperienza pratica con [la nostra anteprima live delle funzionalità](https://experienceleague.adobe.com/it/apps/journey-optimizer/ai-assistant-content-accelerator), progettata per consentirti di esplorarne le funzionalità in prima persona e comprenderne appieno le funzionalità.

Man mano che il settore del marketing diventa più competitivo, i brand cercano modi efficienti per generare contenuti di impatto in tempi rapidi. L’Assistente per l’intelligenza artificiale in Adobe Campaign Web, con tecnologia Microsoft Azure OpenAI e Adobe Firefly, è la funzionalità di generazione di contenuti di intelligenza artificiale di Adobe che trasforma il modo in cui gli esperti di marketing creano contenuti professionali e coerenti con il brand tra canali diversi, come e-mail, SMS e notifiche push. Con modelli GenAI avanzati e una profonda conoscenza delle linee guida del brand, AI Assistant genera automaticamente contenuti personalizzati, coinvolgenti ed efficaci in base all’obiettivo di marketing, ottimizzando i contenuti per stili, layout, toni e altro ancora delineati dal brand.

AI Assistant semplifica la creazione e l’esecuzione di campagne di marketing su canali diversi, come e-mail, SMS e notifiche push, risparmiando tempo, migliorando l’efficienza e ottenendo risultati migliori.

>[!IMPORTANT]
>
>* Prima di utilizzare questa funzionalità, controlla le [protezioni e limitazioni](#generative-guardrails) correlate.
>
>* È necessario accettare un [contratto utente](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html) prima di utilizzare l&#39;Assistente IA in Adobe Campaign Web. Per ulteriori informazioni, contatta il rappresentante Adobe.

## Accedi all’Assistente di AI {#generative-access}

L’Assistente IA per e-mail, notifiche push e SMS è ora disponibile in General Availability (GA) e per tutti gli utenti. Di seguito sono riportati i passaggi e le autorizzazioni necessari per concedere l’accesso agli utenti.

+++ Scopri come assegnare le autorizzazioni relative alla generazione dei contenuti

1. **Crea profilo prodotto** - In [Admin Console](https://stage.adminconsole.adobe.com/), crea un profilo prodotto con il seguente pattern specifico:
   `Campaign - <instance-name> - AIAssistant`

1. **Aggiungi utenti** - Aggiungi l&#39;utente richiesto a quel profilo di prodotto,\
   o\
   **Crea gruppo di utenti**, aggiungi tale gruppo di utenti al profilo di prodotto, quindi aggiungi gli utenti a tale profilo di prodotto.

Scopri come definire le autorizzazioni in Campaign in [questa sezione](../get-started/permissions.md).

+++

## Guardrail e limitazioni {#generative-guardrails}

Di seguito sono elencate le linee guida generali per l’utilizzo dell’Assistente IA in Adobe Campaign Web per la generazione di e-mail:

* La qualità del contenuto generato dipende in larga misura dall’obiettivo di marketing o dal prompt definito. Utilizzate un prompt ben definito per consentire al modello GenAI di interpretare con precisione.
* Carica le risorse del brand per garantire contenuti precisi on-brand. In caso contrario, il contenuto si basa su informazioni disponibili pubblicamente. Il contenuto caricato può essere nei seguenti formati: PDF, JPEG, PNG o file ZIP (con formati di file supportati).
* La dimensione massima per le risorse marchio caricate è di 50 MB. File di grandi dimensioni o numerose immagini possono aumentare il tempo di elaborazione.
* Utilizza [modelli e-mail incorporati](../email/create-email-templates.md), modelli specifici per il brand o modelli personalizzati per creare contenuti e-mail tramite l&#39;Assistente all&#39;intelligenza artificiale. Si consigliano modelli e-mail con un massimo di 8-10 immagini.
* Segnala eventuali output problematici utilizzando le icone thumb-up, thumbs-down o flag durante la selezione delle varianti.
* L’utilizzo di AI Assistant è soggetto alle linee guida per l’utente di Adobe Experience Cloud Generative AI. [Ulteriori informazioni](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html).
* Come parte dell’impegno di Adobe per la trasparenza nell’utilizzo di strumenti di intelligenza artificiale generativi nella creazione di contenuti multimediali, Adobe applica Content Credentials quando vengono scaricati o esportati contenuti o progetti che includono una risorsa generata da Firefly. [Ulteriori informazioni](https://helpx.adobe.com/it/firefly/using/content-credentials.html).

Le seguenti limitazioni si applicano all’Assistente IA in Adobe Campaign Web:

* L’Assistente IA in Adobe Campaign Web è attualmente supportato solo in inglese. Gli input non in inglese possono produrre risultati incoerenti o errati. Al momento non sarà possibile affrontare o migliorare le questioni sollevate da risposte non in lingua inglese.
* Disponibile solo per i canali e-mail, push e SMS.
* Il contenuto GenAI potrebbe non essere sempre accurato. Condividi il tuo feedback affinché gli ingegneri possano perfezionare i modelli.
* Puoi caricare più risorse per il brand, ma puoi sfruttarne una sola per una generazione specifica.

## Funzionalità di generazione dei contenuti dell’Assistente AI {#generative-features}

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-content.md">
<img alt="[Generazione di e-mail con l’Assistente AI]" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
<a href="generative-content.md"><strong>Generazione di e-mail con Assistente AI</strong></a>
</div>
<p>
</td>
<td>
<a href="generative-sms.md">
<img alt="[Generazione di SMS con Assistente IA]" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div><a href="generative-sms.md"><strong>Generazione di SMS con Assistente AI</strong>
</div>
<p>
</td>
<td>
<a href="generative-push.md">
<img alt="[Generazione di notifiche push con Assistente IA]" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
<a href="generative-push.md"><strong>Generazione notifiche push con Assistente IA</strong></a>
</div>
<p></td>
</tr></table>