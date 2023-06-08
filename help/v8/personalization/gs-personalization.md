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
source-git-commit: b8b1cb62c11b66eaade5937fa798d58a9c376127
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 33%

---


# Introduzione ai contenuti dinamici

Per ottenere il massimo da ogni campagna di marketing, Adobe Campaign offre un modo per fornire contenuti dinamici personalizzati che parlano ai clienti a loro livello. In base ai dati del profilo, utilizza le funzionalità di personalizzazione per creare un’esperienza personalizzata per diversi gruppi e singoli utenti: puoi adattare i messaggi a ogni destinatario specifico sfruttando i dati e le informazioni di cui disponi su di essi. Può essere il nome, gli interessi, dove vivono, cosa hanno comprato, e molto altro.

Utilizza Campaign per creare contenuti dinamici e inviare messaggi personalizzati. Le funzionalità di personalizzazione possono essere combinate per migliorare i messaggi e creare un’esperienza utente personalizzata.

Per rendere dinamico il contenuto del messaggio, inserisci:

* **Campi di personalizzazione**

   I campi di personalizzazione vengono utilizzati per la personalizzazione di primo livello dei messaggi. Puoi selezionare qualsiasi campo disponibile nel database dall’editor di personalizzazione. Per una consegna, puoi selezionare qualsiasi campo correlato al destinatario, al messaggio o alla consegna. Questi attributi di personalizzazione possono essere inseriti nella riga dell’oggetto o nel corpo dei messaggi.

   ![](assets/perso-subject-line.png)

   Per inserire nel contenuto la città del destinatario, utilizza la seguente sintassi: &lt;%= recipient.location.city %>.

* **Contenuto condizionale**

   Configura il contenuto condizionale per aggiungere contenuto ad esempio in base al profilo del destinatario. I blocchi di testo e/o le immagini vengono inseriti quando viene soddisfatta una particolare condizione. Puoi definire la versione alternativa del contenuto quando la condizione non è true.

* **Blocchi di contenuto incorporati**

   Campaign viene fornito con un set di blocchi di personalizzazione contenenti un rendering specifico da inserire nelle consegne. Ad esempio, puoi aggiungere un logo, un messaggio di saluto o un collegamento alla pagina speculare di un messaggio e-mail. I blocchi di contenuto sono disponibili da una voce dedicata nell’editor di personalizzazione.

   ![](assets/perso-content-blocks.png)

## Dove posso aggiungere contenuti dinamici?

Adobe Campaign V8 Web fornisce un editor di espressioni in cui è possibile selezionare, disporre, personalizzare e convalidare tutti i dati per creare un’esperienza personalizzata per il contenuto.

L’editor di espressioni è disponibile per tutti i canali, in tutti i campi con l’icona Apri finestra di dialogo per personalizzazione, ad esempio il campo dell’oggetto o i collegamenti e-mail e i componenti di contenuto testo/pulsante.

![](assets/expression-editor-access.png)

![](assets/expression-editor-access-email.png)

![](assets/perso-link-insert-icon.png)

Inoltre, durante la progettazione di un’e-mail è possibile accedere a un generatore di contenuti condizionali dedicato. [Scopri come creare contenuti condizionali nelle e-mail](conditions.md)

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
