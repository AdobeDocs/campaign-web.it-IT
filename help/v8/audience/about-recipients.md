---
title: Utilizzare destinatari e tipi di pubblico
description: Scopri come utilizzare i destinatari di Campaign Web
badge: label="Beta"
source-git-commit: 5183dd0045c7f13e79f65eca5b31dfd4cde2f31d
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 93%

---

# Utilizzare destinatari e tipi di pubblico {#about-recipients}

>[!CONTEXTUALHELP]
>id="acw_homepage_rn4"
>title="Visualizzazione 360 dei destinatari"
>abstract="Crea nuovi destinatari e monitorali tramite potenti rapporti e strumenti. Accedi agli attributi, alle interazioni e ai registri del destinatario. Utilizza le opzioni di filtro per sfogliare l’elenco dei destinatari, modificarne e aggiornare il profilo."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new.html" text="Consulta le note sulla versione"


>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Profili"
>abstract="Un profilo è un soggetto destinato a ricevere i messaggi inviati da Adobe Campaign. In Adobe Campaign, i destinatari sono i profili target predefiniti per l’invio di consegne (e-mail, SMS, ecc). Da questo elenco, in base alle tue autorizzazioni, puoi visualizzare il profilo del destinatario. Utilizza le opzioni di filtro per sfogliare l’elenco. Puoi modificare e aggiornare un piccolo set di attributi del destinatario."

Un destinatario è un profilo destinato a ricevere i messaggi inviati da Adobe Campaign. In Adobe Campaign, i destinatari sono i profili target predefiniti per l’invio di consegne (e-mail, SMS, ecc). I dati dei destinatari memorizzati nel database consentono di creare tipi di pubblico che riceveranno una determinata consegna e di aggiungere dati di personalizzazione al contenuto della consegna. Nel database sono presenti altri tipi di profili. Sono progettati per utilizzi diversi: ad esempio, i profili seed vengono usati per testare le consegne prima di inviarle al pubblico finale.

I destinatari possono essere aggiunti solo dalla console client di Campaign. Tuttavia, sono visibili in Campaign Web dalla voce **Destinatari** nella barra di navigazione a sinistra. Puoi anche modificare gli attributi del destinatario da quella schermata.

Per modificare i dati del destinatario, fai clic sui tre punti accanto al nome e scegli **Modifica...**.

![Modificare il profilo di un destinatario](assets/recipient-edit.png)

Puoi aggiornare un set limitato di attributi, ovvero: nome, cognome, indirizzo e-mail e numero di telefono.

![Aggiornare il profilo di un destinatario](assets/recipient-update.png)

>[!NOTE]
>
>Questo modulo di modifica del profilo limitato è fornito solo a scopo di test nel programma Beta. Sarà migliorato nella versione successiva. Consente all’utente di aggiungere rapidamente un indirizzo e-mail e un numero di telefono a qualsiasi profilo, in modo da poter testare i canali e-mail e SMS e ricevere i messaggi inviati.

Puoi filtrare i destinatari utilizzando il campo di ricerca, dal pulsante **Mostra filtri**.

Puoi anche accedere ai destinatari dalla vista **Explorer**, sfogliare e creare cartelle e sottocartelle e verificare le autorizzazioni associate.

![Elenco destinatari dalla vista Explorer](assets/recipients-from-explorer.png)

>[!NOTE]
>
>La possibilità di accedere all’elenco completo dei destinatari archiviati nel database dipende dalle autorizzazioni di cui disponi. Ulteriori informazioni sulle autorizzazioni sono disponibili in [questa sezione](../get-started/permissions.md).

Inoltre, puoi gestire l’iscrizione e l’annullamento dell’iscrizione dei destinatari a servizi quali le newsletter. Scopri come utilizzare i servizi di iscrizione in [questa pagina](manage-services.md)

Puoi creare flussi di lavoro per deduplicare, arricchire, combinare i profili e creare tipi di pubblico. Per ulteriori informazioni, consulta [questa sezione](../workflows/gs-workflows.md).
