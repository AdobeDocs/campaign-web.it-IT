---
audience: end-user
product: campaign
title: Metadati C2PA in Designer e-mail e Designer pagine di destinazione
description: Scopri cosa succede ai metadati C2PA già allegati a un’immagine mentre si sposta attraverso l’e-mail e il designer di pagine di destinazione nell’interfaccia utente web di Adobe Campaign.
topic: Content Management
role: User
level: Beginner
source-git-commit: 645352d9e2ba12d5430ddf1b62852077344c3016
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 4%
---

# Metadati C2PA in Designer e-mail e Designer pagine di destinazione {#c2pa-email-landing-page-designer}

>[!BEGINSHADEBOX]

**In questa pagina:** Scopri cosa succede ai metadati C2PA già allegati a un&#39;immagine mentre si sposta tramite la finestra di progettazione delle pagine di destinazione e e-mail nell&#39;interfaccia utente Web di Adobe Campaign.

>[!ENDSHADEBOX]

>[!INFO]
>
>Nuove leggi stanno emergendo sulla trasparenza generativa dell’intelligenza artificiale e Adobe sta lavorando per soddisfare i requisiti applicabili in tutte le giurisdizioni. I metadati C2PA sono lo strumento di provenienza utilizzato da Adobe per soddisfare i requisiti di queste normative.

Il designer dell’e-mail e della pagina di destinazione non genera o modifica le immagini di per sé. Fa riferimento a immagini già generate o modificate con l’intelligenza artificiale generativa in un altro strumento Adobe, ad esempio Generate Content (Genera contenuto), Adobe Express, Firefly o in un modello partner. I metadati C2PA già allegati a tali immagini vengono mantenuti e invariati durante la generazione, la pubblicazione e l’invio.

## I metadati C2PA vengono conservati durante la generazione e l&#39;invio {#c2pa-preserved}

La tabella seguente riepiloga cosa accade ai metadati C2PA in ogni fase della creazione e dell’invio di contenuti con il designer delle e-mail e delle pagine di destinazione.

| Azione | Cosa succede | Conservazione dei metadati C2PA? | Esempio |
| --- | --- | --- | --- |
| **Inserire un&#39;immagine in un modello** | La finestra di progettazione aggiunge un riferimento a un’immagine già generata o modificata con IA generativa altrove, ad esempio Genera contenuto, Adobe Express, Firefly o un modello partner. Il file di immagine stesso non viene modificato. | Sì, invariato | Un banner generato da Firefly viene inserito in un modello e-mail. |
| **Ridimensionare, riposizionare o aggiungere testo alternativo** | Vengono visualizzate solo le proprietà nella modifica HTML del modello. Il file di immagine non viene codificato di nuovo. | Sì, invariato | Un’immagine viene ridimensionata per rientrare in un layout mobile e viene fornito testo alternativo. |
| **Pubblica** | L’e-mail o la pagina di destinazione viene pubblicata e l’immagine viene memorizzata per la consegna. | Sì, invariato | Viene pubblicata una campagna e le relative immagini vengono memorizzate per l’invio. |
| **Inviare un&#39;e-mail o visualizzare una pagina di destinazione** | L’immagine viene consegnata alla casella in entrata del destinatario o visualizzata nella pagina live. | Sì, invariato | Un destinatario apre l’e-mail e scarica l’immagine; le credenziali corrispondono ancora a quelle originali. |

## Tipi di contenuto e ambito {#c2pa-content-types}

* **Immagini**: coperte. I metadati C2PA già allegati a un’immagine vengono mantenuti mentre vengono inseriti, regolati, pubblicati e consegnati, come mostrato sopra.
* **Video, audio, testo**: non applicabile. Il designer di e-mail e pagine di destinazione non genera o modifica questi tipi di contenuto con IA generativa.

## Cosa succede quando il contenuto si sposta {#c2pa-content-moves}

I metadati C2PA viaggiano con l’immagine nella finestra di progettazione delle e-mail e delle pagine di destinazione nell’interfaccia utente di Adobe Campaign Web, dall’editor all’archiviazione, fino alla casella in entrata del destinatario o alla pagina live. Nessuna credenziale creata, modificata o rimossa in nessuna di queste operazioni.

Se un’immagine non contiene metadati C2PA di IA per l’intelligenza artificiale generativi, poiché non è stata generata o modificata con intelligenza artificiale generativa, qui non viene visualizzata alcuna credenziale. Questo è previsto, non un errore.

## Verifica delle credenziali in corso {#c2pa-checking-credential}

Non esiste ancora un modo per ispezionare un Content Credential direttamente all’interno dell’e-mail o del designer della pagina di destinazione.

## Risorse aggiuntive

* [Utilizzare Genera contenuti](generative-gs.md)
* [Trasparenza dei contenuti di IA generativa](https://experienceleague.adobe.com/en/docs/cx-enterprise-ai/experience-cloud-ai/overview/content-transparency)