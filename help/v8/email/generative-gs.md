---
audience: end-user
title: Introduzione all’Assistente IA
description: Introduzione con l'assistente AI
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '745'
ht-degree: 8%

---

# Utilizzare l’Assistente IA {#generative-gs}

>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="Assistente IA"
>abstract="Dopo aver creato e personalizzato la consegna, usa l&#39;Assistente AI per migliorare la tua contenuto. Questa funzione semplifica i miglioramenti personalizzazione e contenuto consentendo di ottimizzare il contenuto descrivendo ciò che si desidera generare."

>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="Definire il contesto con l’Assistente IA in Campaign"
>abstract="Per utilizzare il contenuto selezionato come input per la generazione di contenuto, attivare l&#39;interruttore **Migliora con contenuto** corrente. Puoi anche caricare le risorse del tuo marchio per utilizzarle come origine. Se non si utilizza il contenuto selezionato, il caricamento e la selezione di marchio risorse sono obbligatori."

>[!CONTEXTUALHELP]
>id="acw_emagica_generate"
>title="Termini di IA generativa di Adobe"
>abstract="L&#39;accesso a questa funzione dipende dall&#39;accettazione delle Adobe Experience Cloud Generative AI User Guidelines. Esamina l&#39;accuratezza di qualsiasi output di questa funzione e assicurati che sia appropriato per il tuo caso d&#39;uso."
>additional-url="https://www.adobe.com/it/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Linee guida per l’utente sull’intelligenza artificiale generativa di Adobe"

>[!INFO]
>
>Immergiti in un&#39;esperienza pratica con [la nostra anteprima](https://experienceleague.adobe.com/it/apps/journey-optimizer/ai-assistant-content-accelerator) delle funzionalità dal vivo, progettata per consentirti di esplorare le sue funzionalità in prima persona e comprendere appieno le sue capacità.

Man mano che l&#39;industria marketing diventa più competitiva, i marchi cercano modi efficienti per generare rapidamente contenuto di impatto. AI Assistant in Adobe Campaign Web, basato su Microsoft Azure OpenAI e Adobe Systems Firefly, è la funzionalità di generazione di contenuto AI di Adobe Systems che trasforma il modo in cui gli esperti di marketing creano contenuto professionali e coerenti in marchio su tutti i canali like e-mail, SMS e notifiche push. Con modelli GenAI avanzati e una profonda comprensione delle linee guida marchio, AI Assistant genera automaticamente contenuto personalizzate, coinvolgenti ed efficaci in base all&#39;obiettivo marketing, ottimizzando contenuto per stili, layout, toni e altro marchio ancora.

AI Assistant semplifica la creazione e l&#39;esecuzione di campagne marketing su tutti i canali like e-mail, SMS e notifiche push, risparmiando tempo, migliorando l&#39;efficienza e ottenendo risultati migliori.

>[!IMPORTANT]
>
>* Prima di utilizzare questa funzionalità, esamina i Guardrail e le Limitazioni](#generative-guardrails) correlati[.
>
>* È necessario accettare un [accordo](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html) utente prima di usare l&#39;Assistente AI in Adobe Campaign Web. Per ulteriori informazioni, contatta il rappresentante Adobe.

## Accedere all&#39;Assistente AI {#generative-access}

L&#39;Assistente AI per e-mail, notifiche push e SMS è ora disponibile in Disponibilità generale (GA) e disponibile per tutti gli utenti. Le autorizzazioni necessarie e i passaggi necessari per concedere accesso agli utenti sono descritti di seguito.

+++ Scopri come assegnare le autorizzazioni relative alla generazione di contenuti

1. **Crea Profilo** di prodotto: in [Admin Console](https://stage.adminconsole.adobe.com/), crea un profilo di prodotto con il seguente pattern specifico:
   `Campaign - <instance-name> - AIAssistant`

1. **Aggiungi utenti** : aggiungi il utente richiesto al profilo di prodotto,\
   o\
   **Crea gruppo** di utenti e aggiungi tale gruppo di utente al profilo di prodotto, quindi aggiungi gli utenti al profilo di prodotto.

Scopri come definire le autorizzazioni nei Campaign di [questa sezione](../get-started/permissions.md).

+++

## Guardrail e limitazioni {#generative-guardrails}

Le linee guida generali per l&#39;utilizzo dell&#39;Assistente AI in Adobe Campaign Web per la generazione di e-mail sono elencate di seguito:

* La qualità del contenuto generato dipende fortemente dall&#39;obiettivo o dal prompt marketing definito. Utilizza un prompt ben definito affinché il modello GenAI interpreti accuratamente.
* Caricate marchio risorse per garantire un&#39;contenuto accurata e marchio. In caso contrario, contenuto si basa su informazioni disponibili pubblicamente. I contenuto caricati possono essere nei seguenti formati: PDF, JPEG, PNG o ZIP (con i formati di file supportati).
* La dimensione massima per l&#39;risorse di marchio caricata è 50 MB. File di grandi dimensioni o numerose immagini possono aumentare il tempo di elaborazione.
* Usa [modelli](../email/create-email-templates.md) e-mail integrati, modelli specifici per marchio o modelli personalizzati per creare i tuoi contenuto e-mail utilizzando l&#39;Assistente AI. Si consigliano modelli di e-mail con un massimo di 8-10 immagini.
* Segnala eventuali output problematici utilizzando le icone pollice su, pollice giù o contrassegno quando selezioni le varianti.
* L&#39;utilizzo dell&#39;Assistente AI è soggetto alle Linee guida per l&#39;utente dell&#39;IA Adobe Experience Cloud generativa. [Ulteriori informazioni](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html).
* Come parte dell&#39;impegno di Adobe Systems per la trasparenza nell&#39;uso degli strumenti di intelligenza artificiale generativa nella creazione di media, Adobe Systems applica le credenziali di contenuto quando viene scaricato o esportato contenuto o un progetto che include un risorsa generato da Firefly. [Ulteriori informazioni](https://helpx.adobe.com/firefly/using/content-credentials.html).

Le seguenti limitazioni si applicano ad AI Assistant in Adobe Campaign Web:

* AI Assistant in Adobe Campaign Web è attualmente supportato solo in Inglese. Gli input non Inglese possono produrre risultati incoerenti o errati. I problemi derivanti da risposte non Inglese non saranno affrontati o migliorati in questo momento.
* Disponibile solo per i canali e-mail, push e SMS.
* I contenuto GenAI potrebbero non essere sempre accurati. Condividi il tuo feedback in modo che gli ingegneri possano perfezionare i modelli.
* Puoi caricare più marchio risorse ma puoi sfruttare solo uno per una generazione specifica.

## Funzionalità di generazione contenuto di AI Assistant {#generative-features}

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-content.md">
<img alt="[Generazione di e-mail con AI Assistant]" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
<a href="generative-content.md"><strong>Generazione di e-mail con AI Assistant</strong></a>
</div>
<p>
</td>
<td>
<a href="generative-sms.md">
<img alt="[Generazione SMS con AI Assistant]" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div><a href="generative-sms.md"><strong>Generazione di SMS con AI Assistant</strong>
</div>
<p>
</td>
<td>
<a href="generative-push.md">
<img alt="[Invia notifica generazione con AI Assistant]" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
<a href="generative-push.md"><strong>Spingere la generazione di notifica con AI Assistant</strong></a>
</div>
<p></td>
</tr></table>