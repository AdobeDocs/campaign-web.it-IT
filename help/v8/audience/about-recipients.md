---
title: Monitorare e gestire i profili
description: Scopri come monitorare e gestire i profili in Campaign Web.
badge: label="Disponibilità limitata"
source-git-commit: e61878f325575377865186fb9cb63b831ac843fd
workflow-type: tm+mt
source-wordcount: '662'
ht-degree: 9%

---

# Monitorare e gestire i profili {#profiles}

>[!CONTEXTUALHELP]
>id="acw_homepage_rn4"
>title="Visualizzazione 360 dei profili"
>abstract="Crea nuovi profili e monitorali tramite rapporti e strumenti potenti. Accedi agli attributi, alle interazioni e ai registri dei profili. Utilizza le opzioni di filtro per sfogliare l’elenco dei profili, modificarne e aggiornarne il profilo."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new.html" text="Consulta le note sulla versione"

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Profili"
>abstract="Un profilo è un soggetto destinato a ricevere i messaggi inviati da Adobe Campaign. Da questo elenco, puoi visualizzare i dettagli dei profili in base alle autorizzazioni di cui disponi. Utilizza le opzioni di filtro per sfogliare l’elenco. Puoi modificare e aggiornare un piccolo set di attributi dei profili."

## Introduzione ai profili {#gs}

Un profilo in Adobe Campaign Web è una persona memorizzata nel database che funge da componente chiave per la creazione di tipi di pubblico per le consegne e l’aggiunta di dati di personalizzazione al contenuto. Nel database sono memorizzati vari tipi di profili, ad esempio Profili di test, progettati per testare le consegne prima che vengano inviate al pubblico finale. [Scopri come utilizzare i profili di test](test-profiles.md)

I profili possono essere aggiunti solo dalla console client di Campaign. Tuttavia, sono accessibili in Adobe Campaign Web dalla sezione **Profili** nella barra di navigazione a sinistra. È inoltre possibile accedervi da **Esplora** visualizzazione, in cui è possibile sfogliare, creare cartelle, sottocartelle e verificare le autorizzazioni associate.

Puoi filtrare l’elenco dei profili utilizzando il campo di ricerca o i filtri disponibili nella sezione **Mostra filtri** pulsante.

![](assets/profiles-list.png)

>[!NOTE]
>
>A seconda delle autorizzazioni, potresti non avere accesso all’elenco completo dei profili memorizzati nel database. Ulteriori informazioni sulle autorizzazioni sono disponibili in [questa sezione](../get-started/permissions.md).

## Accedere e modificare gli attributi dei profili {#access}

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_details"
>title="Dettagli di base"
>abstract="Questa sezione offre informazioni approfondite sui dettagli di base del profilo. Per modificare qualsiasi informazione, apporta le modifiche direttamente nel rispettivo campo e fai clic sul pulsante **Salva** nell&#39;angolo superiore destro dello schermo."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_contactinformation"
>title="Dati di contatto"
>abstract="Questa sezione offre informazioni approfondite sulle informazioni di contatto del profilo. Per modificare qualsiasi informazione, apporta le modifiche direttamente nel rispettivo campo e fai clic sul pulsante **Salva** nell&#39;angolo superiore destro dello schermo."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_address"
>title= "Address"
>abstract="Questa sezione offre informazioni approfondite sull’indirizzo postale del profilo e sulla qualità dell’indirizzo. Per modificare qualsiasi informazione, apporta le modifiche direttamente nel rispettivo campo e fai clic sul pulsante **Salva** nell&#39;angolo superiore destro dello schermo."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_account"
>title="Dettagli account"
>abstract="Questa sezione offre informazioni approfondite sui dettagli dell’account del profilo. Per modificare qualsiasi informazione, apporta le modifiche direttamente nel rispettivo campo e fai clic sul pulsante **Salva** nell&#39;angolo superiore destro dello schermo."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_nolongercontact"
>title="Destinatari da non contattare più"
>abstract="Questa sezione offre informazioni approfondite sulle preferenze di contatto del profilo. Per modificare qualsiasi informazione, apporta le modifiche direttamente nel rispettivo campo e fai clic sul pulsante **Salva** nell&#39;angolo superiore destro dello schermo."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_customfields"
>title="Campi personalizzati"
>abstract="I campi personalizzati sono attributi specifici personalizzati in base alle tue esigenze e configurati per la tua istanza. Per modificare qualsiasi informazione, apporta le modifiche direttamente nel rispettivo campo e fai clic sul pulsante **Salva** nell&#39;angolo superiore destro dello schermo."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_othersfields"
>title="Altri"
>abstract="Questa sezione fornisce attributi incorporati aggiuntivi. Per modificare qualsiasi informazione, apporta le modifiche direttamente nel rispettivo campo e fai clic sul pulsante **Salva** nell&#39;angolo superiore destro dello schermo."

>[!CONTEXTUALHELP]
>id="acw_recipients_subscription_list"
>title="Elenco iscrizioni dei destinatari"
>abstract="Questa scheda elenca tutti i servizi a cui il profilo è abbonato."

Per accedere ai dettagli di un profilo, fai clic sul nome nell’elenco dei profili.

![](assets/profiles-details.png)

Da questa schermata, puoi accedere alle informazioni dettagliate sul profilo:

* Il **[!UICONTROL Dettagli]** Questa scheda ti consente di sfogliare gli attributi incorporati e personalizzati del profilo. Per modificare un attributo, apporta le modifiche desiderate nel campo desiderato e fai clic sul pulsante **[!UICONTROL Salva]** pulsante.
* Il **[!UICONTROL Iscrizioni]** fornisce informazioni sui servizi a cui il profilo è abbonato. [Scopri come utilizzare i servizi di iscrizione](manage-services.md)
* Il **[!UICONTROL Registri]** Questo pulsante, situato nell’angolo superiore destro della schermata, ti consente di visualizzare una cronologia delle interazioni del profilo tramite i registri di invio, esclusione e tracciamento, nonché le proposte presentate al profilo.
