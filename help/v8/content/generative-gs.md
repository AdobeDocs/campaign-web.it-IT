---
audience: end-user
title: Introduzione a Genera contenuto
description: Introduzione alla generazione di contenuti
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
TQID: https://experienceleague.adobe.com/jpw4u-Vy7M2Q9qRyQ2J3rJ-Mr8UKLUpxhw39tglbbNc
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
source-git-commit: d4e22ba88bcb6dc74d22e8a927c1640f21d75d3e
workflow-type: tm+mt
source-wordcount: 887
ht-degree: 20%

---

# Utilizzare Genera contenuto {#generative-gs}

>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="Genera contenuto"
>abstract="Dopo aver creato e personalizzato la consegna, utilizza l’intelligenza artificiale per migliorare i contenuti. Questa funzione semplifica il processo di personalizzazione e il miglioramento dei contenuti e ti consente di perfezionarli descrivendo cosa desideri generare."

>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="Definire il contesto con Genera contenuto in Campaign"
>abstract="Per utilizzare il contenuto selezionato come input per la generazione di contenuti, attiva il pulsante di attivazione **Migliora con il contesto corrente**. Puoi anche caricare le risorse del tuo marchio per utilizzarle come origine. Se non utilizzi il contenuto selezionato, è necessari caricare e selezionare le risorse del brand."

>[!CONTEXTUALHELP]
>id="acw_emagica_generate"
>title="Condizioni per l’IA generativa di Adobe"
>abstract="L’accesso a questa funzione è soggetto al consenso alle linee guida per l’utente dell’IA generativa di Adobe Experience Cloud. Verifica l’accuratezza degli output generati da questa funzione e assicurati che siano appropriati al tuo caso d’uso."
>additional-url="https://www.adobe.com/it/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Linee guida per l’utente sull’intelligenza artificiale generativa di Adobe"

>[!INFO]
>
>Immergiti in un&#39;esperienza pratica con [la nostra anteprima live delle funzionalità](https://experienceleague.adobe.com/it/apps/journey-optimizer/ai-assistant-content-accelerator), progettata per consentirti di esplorarne le funzionalità in prima persona e comprenderne appieno le funzionalità.

Man mano che il settore del marketing diventa più competitivo, i brand cercano modi efficienti per generare contenuti di impatto in tempi rapidi. Generate Content in Adobe Campaign Web (Genera contenuto in Web), basato su Microsoft Azure OpenAI e Adobe Firefly, è la funzionalità di generazione di contenuti di intelligenza artificiale di Adobe che trasforma il modo in cui gli esperti di marketing creano contenuti professionali e coerenti con il brand attraverso canali diversi, come e-mail, SMS e notifiche push. Con modelli GenAI avanzati e una profonda conoscenza delle linee guida del brand, Generate Content genera automaticamente contenuti personalizzati, coinvolgenti ed efficaci in base all’obiettivo di marketing, ottimizzando i contenuti per stili, layout, toni e altro ancora delineati dal brand.

Genera contenuto supporta la generazione **in più lingue** consentendo di raggiungere e coinvolgere diversi tipi di pubblico globali. Genera contenuto è disponibile nelle seguenti lingue:

<table style="table-layout:fixed; margin-top: 0px; margin-bottom: 0px;">
  <tbody>
    <tr style="border: 0;background-color: #FFFFFF;">
      <td>
        <ul>
          <li>Cinese (Hong Kong)</li>
          <li>Cinese (semplificato)</li>
          <li>Cinese (Taiwan)</li>
          <li>Olandese</li>
        </ul>
      </td>
      <td>
        <ul>
          <li>Francese</li>
          <li>Tedesco</li>
          <li>Italiano</li>
          <li>Giapponese</li>
        </ul>
      </td>
      <td>
        <ul>
          <li>Norvegese</li>
          <li>Portoghese</li>
          <li>Spagnolo</li>
          <li>Svedese</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

Genera contenuto semplifica la creazione e l’esecuzione di campagne di marketing su canali diversi, come e-mail, SMS e notifiche push, consentendo di risparmiare tempo, migliorando l’efficienza e ottenendo risultati migliori.

>[!IMPORTANT]
>
>* Prima di utilizzare questa funzionalità, controlla le [protezioni e limitazioni](#generative-guardrails) correlate.
>
>* È necessario accettare un [contratto utente](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html) prima di utilizzare l&#39;intelligenza artificiale per generare contenuto in Adobe Campaign Web. Per ulteriori informazioni, contatta il rappresentante Adobe.

## Accedi a Genera contenuto {#generative-access}

Generare contenuti per e-mail, notifiche push, pagina di destinazione e SMS è ora disponibile in General Availability (GA) e per tutti gli utenti. Di seguito sono riportati i passaggi e le autorizzazioni necessari per concedere l’accesso agli utenti.

+++ Scopri come assegnare le autorizzazioni relative alla generazione dei contenuti

1. **Accedi a [Admin Console](https://adminconsole.adobe.com/)**, passa al menu **Prodotti**, quindi seleziona **Adobe Campaign Managed Cloud**.

1. Accedi all&#39;istanza per la quale desideri concedere le autorizzazioni, quindi fai clic su **Nuovo profilo** per creare un nuovo profilo di prodotto con il seguente nome specifico:

   `Campaign - <instance-name> - AIAssistant`

1. Imposta il profilo di prodotto con le autorizzazioni necessarie per generare l’accesso ai contenuti.

1. **Aggiungi utenti o gruppi di utenti**. Scegliere una delle opzioni seguenti:
   * **Aggiungi singoli utenti**: aggiungi gli utenti richiesti direttamente al profilo di prodotto.
   * **Aggiungi gruppi di utenti**: crea un gruppo di utenti, aggiungi gli utenti a tale gruppo, quindi aggiungi il gruppo di utenti al profilo di prodotto.

Scopri come definire le autorizzazioni in Campaign in [questa sezione](../get-started/permissions.md).

+++

## Guardrail e limitazioni {#generative-guardrails}

Di seguito sono elencate le linee guida generali per l’utilizzo dell’intelligenza artificiale per generare contenuti in Adobe Campaign Web per la generazione di e-mail:

* La qualità del contenuto generato dipende in larga misura dall’obiettivo di marketing o dal prompt definito. Utilizzate un prompt ben definito per consentire al modello GenAI di interpretare con precisione.
* Carica le risorse del brand per garantire contenuti precisi on-brand. In caso contrario, il contenuto si basa su informazioni disponibili pubblicamente. Il contenuto caricato può essere nei seguenti formati: PDF, JPEG, PNG o file ZIP (con formati di file supportati).
* La dimensione massima per le risorse marchio caricate è di 50 MB. File di grandi dimensioni o numerose immagini possono aumentare il tempo di elaborazione.
* Utilizza [modelli e-mail incorporati](../content/create-email-templates.md), modelli specifici per il brand o modelli personalizzati per creare contenuti e-mail utilizzando l&#39;intelligenza artificiale. Si consigliano modelli e-mail con un massimo di 8-10 immagini.
* Segnala eventuali output problematici utilizzando le icone thumb-up, thumbs-down o flag durante la selezione delle varianti.
* L’utilizzo di Genera contenuto è soggetto alle Linee guida per l’utente di Adobe Experience Cloud Generative AI. [Ulteriori informazioni](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html).
* Come parte dell’impegno di Adobe per la trasparenza nell’utilizzo di strumenti di intelligenza artificiale generativi nella creazione di contenuti multimediali, Adobe applica Content Credentials quando vengono scaricati o esportati contenuti o progetti che includono una risorsa generata da Firefly. [Ulteriori informazioni](https://helpx.adobe.com/it/firefly/using/content-credentials.html).

Le seguenti limitazioni si applicano alla generazione di contenuti in Adobe Campaign Web:

* Generate Content in Adobe Campaign Web (Genera contenuto in Web) è attualmente supportato solo in lingua inglese. Gli input non in inglese possono produrre risultati incoerenti o errati. Al momento non sarà possibile affrontare o migliorare le questioni sollevate da risposte non in lingua inglese.
* Disponibile solo per i canali e-mail, push e SMS.
* Il contenuto GenAI potrebbe non essere sempre accurato. Condividi il tuo feedback affinché gli ingegneri possano perfezionare i modelli.
* Puoi caricare più risorse per il brand, ma puoi sfruttarne una sola per una generazione specifica.

## Funzionalità di generazione dei contenuti {#generative-features}

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-full-content.md">
<img alt="[Generazione completa dei contenuti con Generazione dei contenuti]" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
<a href="generative-full-content.md"><strong>Generazione completa dei contenuti con generazione dei contenuti</strong></a>
</div>
<p>
</td>
<td>
<a href="generative-text.md">
<img alt="[Generazione di contenuti di testo con Genera contenuto]" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div><a href="generative-text.md"><strong>Generazione testo con generazione contenuto</strong>
</div>
<p>
</td>
<td>
<a href="generative-image.md">
<img alt="[Generazione di immagini con generazione di contenuti]" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
<a href="generative-image.md"><strong>Generazione immagini con generazione contenuto</strong></a>
</div>
<p></td>
</tr></table>