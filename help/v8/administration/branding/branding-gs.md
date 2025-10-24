---
title: Branding
description: Scopri tutti gli strumenti disponibili per gestire le tue identità di branding
audience: administration
context-tags: branding,overview;branding,main
role: Admin
level: Experienced
exl-id: f6438303-5ae8-47c6-8c34-8e586f4b6fe7
source-git-commit: 1ed20f88d9a11dcac7aa4a3aa93e3058b18c04ff
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 14%

---

# Introduzione al branding {#branding-gs}

>[!AVAILABILITY]
>
>Questa funzionalità è disponibile solo su richiesta, per le nuove implementazioni. Per ottenere l’accesso, contatta il tuo rappresentante Adobe.


>[!IMPORTANT]
>
>I brand non possono essere creati o modificati dagli utenti finali: queste operazioni devono essere eseguite dall’amministratore tecnico di Adobe Campaign. Per qualsiasi richiesta, contatta l’Assistenza cliente di Adobe.

Ogni azienda dispone di linee guida per il brand che definiscono sia gli elementi visivi che i dettagli tecnici. Adobe Campaign ti consente di gestire queste linee guida a livello centrale, in modo da poter presentare ai clienti un’immagine del brand coerente in tutte le attività, dai loghi nelle e-mail agli URL e ai domini utilizzati nelle campagne.

Gli amministratori tecnici possono creare e gestire più marchi all’interno di Adobe Campaign. Questo ti consente di definire tutti gli elementi che compongono la tua brand identity, compresi i loghi e anche le impostazioni di tracciamento delle e-mail. Una volta creati, questi marchi possono essere facilmente collegati alle consegne.

In Campaign puoi aggiungere nuove entità della tua organizzazione o creare un nuovo tipo di e-mail da inviare in un sottodominio diverso. A tale scopo, segui i passaggi indicati di seguito:

1. **Configura un nuovo sottodominio**. Per utilizzare un nuovo sottodominio da parte di Adobe, devi innanzitutto configurarlo. Puoi eseguire questa operazione tramite [Pannello di controllo Campaign della campagna](https://experienceleague.adobe.com/docs/control-panel/using/subdomains-and-certificates/subdomains-branding.html?lang=it) o rivolgerti al tuo contatto tecnico Adobe. Ulteriori informazioni sulla configurazione del sottodominio [in questa pagina](https://experienceleague.adobe.com/en/docs/deliverability-learn/deliverability-best-practice-guide/additional-resources/campaign/ac-domain-name-setup).

   >[!NOTE]
   >
   >Il Pannello di controllo è accessibile a tutti gli utenti amministratori. I passaggi per concedere a un utente l’accesso come amministratore sono descritti in[questa pagina](https://experienceleague.adobe.com/docs/control-panel/using/discover-control-panel/managing-permissions.html?lang=it#discover-control-panel).

1. **Crea un modello di consegna** - Una volta che il nuovo brand è disponibile, è consigliabile creare almeno un nuovo modello di consegna vuoto che faccia riferimento a questo nuovo brand. [Ulteriori informazioni](branding-assign.md).

1. **Verifica le linee guida per il recapito messaggi** - Prima di iniziare a utilizzare il nuovo dominio, discuti la strategia con il team di recapito messaggi di Adobe. Aiuteranno a definire le best practice, ad esempio se è necessario creare una nuova affinità per suddividere gli IP tra domini e/o se è necessario definire un piano di aumento graduale.

## Nota di compatibilità {#compatibility-note}

Il nuovo modello di branding centralizzato non è compatibile con la configurazione di [branding legacy](https://experienceleague.adobe.com/docs/campaign-classic/using/transactional-messaging/configure-transactional-messaging/additional-configurations.htmml#configuring-multibranding){target="_blank"} precedentemente utilizzata nella console client.

Nell&#39;approccio legacy, i clienti hanno implementato il branding estendendo il modulo extAccount e utilizzando la scheda **Branding**.

![](assets/branding-legacy.png)

Se l&#39;ambiente esistente utilizza questa configurazione legacy, non è possibile migrare direttamente al nuovo modello di branding centralizzato. Per adottare il nuovo sistema è necessaria una reimplementazione completa delle impostazioni di branding.