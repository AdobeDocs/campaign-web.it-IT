---
title: Controlli e risoluzione dei problemi dopo la transizione a Campaign v8
description: Scopri cosa controllare e come risolvere i problemi comuni dopo la transizione da Campaign Standard a Campaign v8
hide: true
robots: noindex
googlebot: noindex
role: User, Admin, Developer
level: Beginner
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
  - id: ccdd4c6f-8203-4e89-85f0-79883f86f5fd
    internal-label: Campaign v8 Web User Interface
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
    internal-label: Campaigns
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
source-git-commit: 11cf5f2a6e3e77d0747a0b88758ce3fe871e66fd
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 0%
---
# Controlli e risoluzione dei problemi dopo la transizione {#post-transition-checks}

Dopo la transizione da Campaign Standard a Campaign v8, alcune consegne, flussi di lavoro e pagine di destinazione potrebbero comportarsi in modo diverso rispetto alle aspettative. La tabella seguente elenca i sintomi segnalati dagli utenti con transizione, con la causa e le azioni da intraprendere. Per l&#39;elenco completo delle differenze, vedere [Differenze tra Campaign Standard e Campaign v8](acs-v8-differences.md).

| Sintomo | Causa e cosa fare | Ulteriori informazioni |
|---|---|---|
| I collegamenti in una consegna sono URL diretti e non vengono raccolti dati di clic. | Il tracciamento è disabilitato nella consegna o nel modello di consegna su cui si basa. Controlla che **Attiva il tracciamento** sia abilitato, in particolare sui modelli delle consegne ricorrenti. | [Impostazioni di tracciamento](../../v8/advanced-settings/delivery-settings.md#tracking-tab) |
| I destinatari che hanno annullato l’abbonamento tramite il metodo &quot;mailto&quot; List-Unsubscribe non sono in quarantena. | Questo è previsto. Questi destinatari non vengono messi in quarantena. L’abbonamento al servizio associato alla consegna viene annullato oppure viene aggiunto al inserisco nell&#39;elenco Bloccati di consegna dell’se la consegna non prevede alcun servizio. Per tenere traccia di questi annullamenti di abbonamenti, controlla gli abbonamenti del servizio o la sezione **Non contattare più** del profilo. | [Quarantene](https://experienceleague.adobe.com/it/docs/campaign/campaign-v8/send/failures/quarantines){target="_blank"} |
| Una pagina di destinazione non salva un valore calcolato da uno script o memorizzato in un campo nascosto. | Le pagine di destinazione create nell’interfaccia utente di Campaign Web non supportano campi di input nascosti o JavaScript personalizzato. Crea il modulo come applicazione web nella console client. | [Pagine di destinazione](../../v8/landing-pages/get-started-lp.md) |
| **Il trasferimento di file** non trova il file generato da un&#39;attività di direct mailing. | La transizione in uscita di un’attività di direct mailing porta la popolazione target, non il file di estrazione. Aggiungi un&#39;attività **Estrazione dati**, quindi l&#39;attività **Trasferimento file**. | [Direct mail](https://experienceleague.adobe.com/it/docs/campaign/campaign-v8/send/direct-mail){target="_blank"} |
| Varie ondate di una consegna vengono inviate insieme. | Gli scaglioni sono pianificati dalla data di contatto della consegna. Se la consegna inizia dopo il tempo pianificato di alcune ondate, queste ultime vengono inviate insieme invece di essere distanziate. | [Invia con scaglioni](../../v8/advanced-settings/send-using-waves.md) |
| Una maschera di file con caratteri dopo l’asterisco non trova alcun file nell’archiviazione BLOB di Azure. | L’archiviazione BLOB di Azure filtra i file in base al prefisso del nome. È supportato solo un asterisco finale. | [Trasferisci account esterno](../../v8/administration/transfer-external-account.md) |
| Non si apre una pagina speculare di una consegna inviata prima della transizione. | Le pagine mirror delle consegne inviate da Campaign Standard prima della transizione non sono disponibili e non esiste alcuna soluzione alternativa. Le pagine mirror delle consegne inviate da Campaign v8 funzionano normalmente. | [Pagine mirror](../../v8/email/mirror-page.md) |
| Una pagina di destinazione o un blocco di contenuto che utilizza JavaScript personalizzato si comporta in modo diverso. | JavaScript personalizzato viene trasformato durante la migrazione, ma convalidato e regolato, in particolare se utilizza `queryDef`, API di Campaign JavaScript, scritture di sessioni, gestione di unità organizzative o generazione di URL personalizzati. | [Pagine di destinazione](../../v8/landing-pages/get-started-lp.md) |
