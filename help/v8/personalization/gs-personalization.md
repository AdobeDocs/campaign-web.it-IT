---
title: Introduzione ai contenuti dinamici
description: Scopri come rendere i contenuti dinamici utilizzando la personalizzazione, i contenuti condizionali e i blocchi di contenuto incorporati.
audience: automating
content-type: reference
topic-tags: workflow-general-operation
context-tags: workflow,overview;workflow,main
feature: Workflows
role: Data Architect
level: Intermediate
source-git-commit: e241226cacbc366aa884eb7781ce60188913d7b1
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 10%

---


# Introduzione ai contenuti dinamici

In qualità di addetto al marketing, è fondamentale rivolgersi ai clienti realmente interessati alle offerte e coinvolgerli fornendo contenuti efficaci e pertinenti. Data la varietà di destinatari che si incontrano, la creazione di più contenuti di marketing da presentare a persone diverse può richiedere tempo e comportare uno spreco. Qui entra in gioco il contenuto dinamico.

Le funzionalità di contenuto dinamico web di Adobe Campaign ti consentono di personalizzare il contenuto in base alle informazioni raccolte sui destinatari. Utilizzando i contenuti dinamici, potrai essere sicuro che le tue attività di marketing siano più rilevanti, evitando di marketing di prodotti o servizi indesiderati o non necessari. Questo approccio rende i contenuti più accattivanti e aumenta la probabilità che vengano letti. Inoltre, ti consente di personalizzare il contenuto, facendo sentire i destinatari come se stessero ricevendo informazioni da una persona invece che da una macchina.

## Come rendere dinamico il contenuto?

Per rendere dinamico il contenuto del messaggio, inserisci costrutti JavaScript nell’editor di espressioni web di Campaign. Al momento dell’invio dei messaggi, Adobe Campaign interpreta tali espressioni per fornire il contenuto corretto a ciascuno dei destinatari:

* **Personalizzare i messaggi** per ogni destinatario specifico sfruttando i dati del profilo come il nome, gli interessi, dove vive, cosa ha acquistato e molto altro. Puoi selezionare qualsiasi campo disponibile nel database dall’editor di personalizzazione relativo al destinatario, al messaggio o alla consegna. Questi attributi di personalizzazione possono essere inseriti nella riga dell’oggetto o nel corpo dei messaggi. Per inserire nel contenuto la città del destinatario, utilizza la seguente sintassi: &lt;%= recipient.location.city %>.

  ![](assets/perso-subject-line.png){width="800" align="center"}

* **Creare contenuti condizionali** adattare le consegne a ciascun destinatario e mostrare solo il contenuto rilevante per un determinato cliente in base alle informazioni di cui disponi su di esso. Questo consente di visualizzare blocchi di testo e/o immagini specifici in base alle condizioni. Ad esempio, adatta un banner e-mail in base all’abbonamento dei destinatari a un servizio specifico.

  ![](assets/condition-sample.png){width="800" align="center"}

* **Utilizzare i blocchi di personalizzazione** per risparmiare tempo e sfruttare contenuti personalizzati riutilizzabili nei messaggi. Campaign viene fornito con un set di blocchi di personalizzazione contenenti un rendering specifico da inserire nelle consegne. Ad esempio, puoi aggiungere un logo, un messaggio di saluto o un collegamento alla pagina speculare di un messaggio e-mail. I blocchi di contenuto sono disponibili da una voce dedicata nell’editor di personalizzazione.

  ![](assets/content-blocks.png){width="800" align="center"}

## Accedere all’editor di espressioni {#access}

Adobe Campaign V8 Web fornisce un editor di espressioni in cui è possibile selezionare, disporre, personalizzare e convalidare tutti i dati per creare un’esperienza personalizzata per il contenuto. L’editor di espressioni è disponibile per tutti i canali, in tutti i campi con **[!UICONTROL Apri finestra di dialogo per personalizzazione]** come il campo dell’oggetto, i collegamenti e-mail e i componenti di contenuto testo/pulsante.

Di seguito sono riportati alcuni esempi su come accedere all’editor di espressioni a seconda del contenuto che desideri rendere dinamico:

* *Accesso all’editor di espressioni dal campo Nome mittente*

  ![](assets/expression-editor-access.png){width="800" align="center"}

* *Accesso all’editor di espressioni da un componente di testo e-mail*

  ![](assets/expression-editor-access-email.png){width="800" align="center"}

* *Accesso all’editor di espressioni da un collegamento in un messaggio e-mail*

  ![](assets/perso-link-insert-icon.png){width="800" align="center"}

>[!NOTE]
>
>Oltre all’editor di espressioni, puoi anche sfruttare un generatore di contenuti condizionali dedicato durante la progettazione di un’e-mail. [Scopri come creare contenuti condizionali nelle e-mail](conditions.md)

## Approfondiamo

Ora che sai come rendere dinamici i contenuti, è ora di approfondire queste sezioni della documentazione per iniziare a lavorare con la funzione.

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="personalize.md">
<img alt="Personalizzazione dei contenuti" src="assets/do-not-localize/dynamic-personalization.jpg">
</a>
<div>
<a href="personalize.md"><strong>Aggiungere personalizzazione</strong></a>
</div>
<p>
</td>
<td>
<a href="conditions.md">
<img alt="Lead" src="assets/do-not-localize/dynamic-conditional.jpg">
</a>
<div><a href="conditions.md"><strong>Aggiungere contenuto condizionale</strong>
</div>
<p>
</td>
<td>
<a href="content-blocks.md">
<img alt="Infrequente" src="assets/do-not-localize/dynamic-content-blocks.jpg">
</a>
<div>
<a href="content-blocks.md"><strong>Aggiungere blocchi di contenuto incorporati</strong></a>
</div>
<p></td>
</tr></table>
