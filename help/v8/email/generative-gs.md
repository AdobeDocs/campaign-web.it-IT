---
audience: end-user
title: Introduzione all’Assistente IA
description: Introduzione all’Assistente AI
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
source-git-commit: 3729a6159affbbb30d2cdab91d1e42dbf9df9c86
workflow-type: tm+mt
source-wordcount: '777'
ht-degree: 37%

---

# Utilizzare l’Assistente AI {#generative-gs}


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

>[!INFO]
>
>Immergiti in un&#39;esperienza pratica con [la nostra anteprima live delle funzionalità](https://experienceleague.adobe.com/it/apps/journey-optimizer/ai-assistant-content-accelerator), progettata per consentirti di esplorarne le funzionalità in prima persona e comprenderne appieno le funzionalità.


Man mano che il settore Marketing diventa più competitivo, i brand cercano modi efficienti per generare contenuti di impatto in modo efficiente e rapido. L’Assistente per l’intelligenza artificiale in Adobe Campaign Web, basato su Microsoft Azure OpenAI e Adobe Firefly, è la funzionalità di generazione di contenuti di intelligenza artificiale di Adobe che rivoluziona il modo in cui gli esperti di marketing creano contenuti professionali e coerenti con il brand su canali diversi, come e-mail, SMS e push. Con modelli GenAI avanzati e una profonda comprensione delle linee guida del brand, AI Assistant genera automaticamente contenuti personalizzati, coinvolgenti ed efficaci in base all’obiettivo di marketing, con contenuti ottimizzati per stili, layout, toni e altro ancora delineati dal brand.

L’Assistente IA rende la creazione e l’esecuzione di campagne di marketing su canali diversi come e-mail, SMS e push intuitivi, semplici e senza problemi, risparmiando tempo, migliorando l’efficienza e ottenendo risultati migliori.

>[!IMPORTANT]
>
>* Prima di iniziare a utilizzare questa funzionalità, leggi l’articolo sui relativi [Guardrail e limitazioni](#generative-guardrails).
>
>* È necessario accettare un [contratto utente](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html) prima di poter utilizzare l&#39;Assistente IA in Adobe Campaign Web. Per ulteriori informazioni, contatta il rappresentante Adobe.

## Accedere all’Assistente AI {#generative-access}

L’Assistente AI per e-mail, notifiche push e SMS è ora in Disponibilità generale (GA) e disponibile per tutti gli utenti. Di seguito sono riportati i passaggi e le autorizzazioni necessari per concedere l’accesso agli utenti.

+++  Scopri come assegnare le autorizzazioni relative alla generazione di contenuti

1. **Crea profilo prodotto** - In [Admin Console](https://stage.adminconsole.adobe.com/) crea un profilo prodotto con il seguente pattern specifico:
   `Campaign - <instance-name> - AIAssistant`

1. **Aggiungi utenti** - Aggiungi l&#39;utente richiesto a tale profilo di prodotto,
o
   **Crea gruppo di utenti**, aggiungi il gruppo di utenti al profilo di prodotto e aggiungi gli utenti a tale profilo.

Scopri come definire le autorizzazioni in Campaign in [questa sezione](../get-started/permissions.md).

+++

## Guardrail e limitazioni {#generative-guardrails}

Di seguito sono elencate le linee guida generali per l’utilizzo dell’Assistente IA in Adobe Campaign Web per la generazione di e-mail:

* La qualità del contenuto generato è fortemente influenzata dalla finalità dell’iniziativa di marketing e dal prompt che inserisci nelle impostazioni. Inserisci un prompt chiaro e preciso nelle impostazioni, per consentire al modello GenAI di interpretarle con precisione. 
* Per ottenere contenuti accurati e in linea con i requisiti del marchio, carica una risorsa del marchio. In caso contrario, il contenuto verrà generato sulla base di informazioni di pubblico dominio. Puoi caricare contenuti nei seguenti formati: file PDF, immagini JPEG o PNG, o file ZIP (contenenti formati di file supportati).
* La dimensione massima per la risorsa del brand caricata è di 50 MB.È possibile utilizzare anche file di dimensioni maggiori o numerose immagini, ma questo comporterà tempi di elaborazione più lunghi.
* Utilizza [modelli e-mail incorporati](../email/create-email-templates.md), modello specifico per il brand o modello personalizzato per creare il contenuto delle e-mail tramite l&#39;assistente di intelligenza artificiale. Si consiglia di utilizzare modelli e-mail con un massimo di 8-10 immagini.
* Assicurati di segnalare eventuali output problematici utilizzando le icone thumb up, thumb down o flag durante la selezione delle varianti.
* L’utilizzo dell’assistente IA è soggetto alle linee guida per l’utente di Adobe Experience Cloud Generative AI. [Ulteriori informazioni](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html)
* Come parte dell’impegno di Adobe per promuovere la trasparenza nell’utilizzo di strumenti di intelligenza artificiale generativi nella creazione di contenuti multimediali, Adobe applicherà Content Credentials quando vengono scaricati o esportati contenuti o progetti che includono una risorsa generata da Firefly. [Ulteriori informazioni](https://helpx.adobe.com/firefly/using/content-credentials.html)

Le seguenti limitazioni si applicano all’Assistente IA in Adobe Campaign Web:

* L’Assistente IA in Adobe Campaign Web è attualmente supportato solo in inglese. Gli input non in inglese possono produrre risultati incoerenti o errati. Le questioni sollevate da risposte non in lingua inglese non saranno al momento affrontate né migliorate.
* Disponibile solo per i canali e-mail, push e SMS.
* Il contenuto GenAI potrebbe non essere sempre accurato: condividi il tuo feedback in modo che i nostri ingegneri possano perfezionare i modelli.
* Puoi caricare più risorse per il brand, ma puoi sfruttarne una sola per una generazione specifica.

## Funzionalità di generazione dei contenuti dell’Assistente AI {#generative-features}

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
