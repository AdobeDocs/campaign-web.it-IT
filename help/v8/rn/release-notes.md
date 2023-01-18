---
audience: end-user
title: Note sulla versione di Campaign Web v8
description: Note sulla versione di Campaign Web v8
exl-id: 3d8c07be-665e-46af-ba5d-f04b25b40880
source-git-commit: 54bcb9b0ba8704cde8beaf1b0400eaa01bba0b15
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 0%

---

# Note sulla versione {#release-notes}

![](../assets/do-not-localize/badge.png)

In questa pagina sono elencate tutte le funzioni e i miglioramenti più recenti per Campaign Web v8.

## Rilascio Alpha{#alpha-release}

Questa nuova interfaccia web di Campaign è attualmente disponibile solo per **Professionisti Alpha** con le seguenti funzionalità:

**Esperienza moderna, intuitiva e unificata**

La nuova interfaccia utente Web di Campaign offre una nuova esperienza utente, allineata con tutte le soluzioni e le app Adobe Experience Cloud. Offre:

* Accesso alla nuova interfaccia e ad altre soluzioni Adobe con una sessione utente singola e condivisa
* Nuova esperienza di navigazione, con tutti i menu e le cartelle disponibili nella barra a sinistra
* Switcher di soluzione e organizzazione dalla barra superiore
* Integrazione unificata della shell, con accesso diretto alla community, al centro assistenza e al supporto
<!--
No search and pulse notifications in Alpha
-->

Ulteriori informazioni sulla nuova interfaccia in [questa pagina](../get-started/user-interface.md).

**Creare, avviare e misurare la campagna e-mail**

Utilizza la nuova interfaccia utente web di Campaign per:

* Progettare contenuti e-mail personalizzati con e-mail designer - [Ulteriori informazioni](../content/edit-content.md)
* Definire i tipi di pubblico target con il generatore di regole - [Ulteriori informazioni](../audience/about-audiences.md)
* Anteprima, verifica e invia i tuoi messaggi e-mail - [Ulteriori informazioni](../monitor/prepare-send.md)
* Monitora i risultati di invio e misurazione con report incorporati - [Ulteriori informazioni](../reporting/reports.md)

<!--
add info somewhere to remind users that
* they still have access to their console (+ link to v8 console doc)
* they keep their existing data (example: will be able to use their existing delivery templates to create deliveries)
-->

>[!NOTE]
>
>Tieni presente che le campagne cross-channel e le funzionalità di gestione del flusso di lavoro saranno disponibili con la versione beta.

## Aggiornamenti terminologici

In qualità di utente di Campaign esistente, tieni presente che alcuni concetti sono stati rinominati per allinearsi agli standard terminologici più recenti. Queste modifiche si applicano solo all’interfaccia utente web di Campaign e non vengono riportate nella console client. Sono riassunti di seguito.

* Le bozze sono ora **Verifica e-mail**: per inviare una bozza, utilizza **Test** nell’interfaccia utente di e-mail delivery. Il target del target delle bozze ora è indicato come **Profili di test**
* Gli indirizzi di seed vengono ora utilizzati come **Profili di test**: invia l’e-mail di test agli indirizzi di seed, che sono destinatari aggiuntivi e fittizi nel database
* L’analisi della consegna è ora **preparazione alla consegna**. Quando devi avviare l’analisi, fai clic sul pulsante **Preparare** pulsante
* L’anteprima e-mail è ora disponibile tramite la funzione **Simulazione del contenuto** pulsante
* Gli elenchi sono ora **Tipi di pubblico**
