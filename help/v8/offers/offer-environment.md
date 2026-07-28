---
audience: end-user
title: Rivedere le impostazioni dell’ambiente dell’offerta
description: Scopri come visualizzare, configurare e distribuire un ambiente di offerta in Campaign Web
feature: Offers
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 7be45366e3ae14e6fa7e4569a37c64e6d72f534c
workflow-type: tm+mt
source-wordcount: 319
ht-degree: 2%

---

# Rivedere le impostazioni dell’ambiente dell’offerta {#offer-environment}

Un **ambiente di offerta** è il contenitore in cui si organizza il catalogo delle offerte e i relativi spazi di offerta. Esistono due tipi di ambienti:

* un ambiente **Progettazione**, in cui le offerte vengono create, configurate e approvate,
* un ambiente **Live** di sola lettura in cui le offerte approvate e distribuite sono disponibili per la selezione della consegna.

Ogni ambiente **Design** è collegato a un ambiente **Live**. Quando un&#39;offerta viene completata e approvata, viene automaticamente distribuita nell&#39;ambiente **Live** e disponibile per la consegna.

![Schermata che mostra gli ambienti.](assets/offers-env.png){zoomable="yes"}

Per impostazione predefinita, Campaign viene fornito con due ambienti **Design** e **Live** preconfigurati per eseguire il targeting della tabella dei destinatari incorporata (offerte identificate).

Per eseguire il targeting di un’altra tabella, ad esempio i profili anonimi che visitano il sito web per interazioni in entrata, è necessario creare ambienti aggiuntivi (uno per dimensione di targeting). Consulta la [documentazione di Campaign v8](https://experienceleague.adobe.com/it/docs/campaign/campaign-v8/offers/interaction-settings/interaction-env#create-an-offer-environment){target="_blank"}.

## Accedere agli ambienti delle offerte {#offer-environment-settings}

Gli ambienti di offerta vengono memorizzati come cartelle. Per accedere e rivedere le impostazioni dell’ambiente (idoneità, gestione del peso, sicurezza), effettua le seguenti operazioni:

>[!CAUTION]
>
>Queste impostazioni possono essere modificate, ma è necessario prestare molta attenzione, in quanto le modifiche potrebbero interrompere l’implementazione esistente.

1. Dal menu di navigazione sinistro, apri **[!UICONTROL Explorer]** e individua la cartella dell&#39;ambiente delle offerte nel nodo **Ambiente di progettazione**.

1. Fare clic sul pulsante ... e selezionare **[!UICONTROL Impostazioni cartella]** per visualizzare le impostazioni dell&#39;ambiente.

   ![Schermata che mostra l&#39;opzione Impostazioni cartella di un ambiente](assets/offers-env-1.png){zoomable="yes"}

1. Esaminare le diverse sezioni. Le impostazioni delle cartelle di un gruppo di ambienti di offerta con opzioni specifiche per l’offerta.

   ![Schermata che mostra le impostazioni delle proprietà di un ambiente](assets/offers-env-2.png){zoomable="yes"}

   La maggior parte delle impostazioni rispecchia la configurazione dell’ambiente dell’offerta disponibile nella console client. Per ulteriori informazioni, consulta la [Documentazione di Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-env.html){target="_blank"}.

<!--
## Create a new offer environment {#create}

If you need to manage a separate offer catalog — for example, for a different targeting dimension — you can create a new **Design** environment directly from the Web UI.

1. From the left navigation menu, open the **[!UICONTROL Explorer]** and locate the **Offers - design** folder.

1. Create a new folder from this location, then open its properties and fill in the environment-specific settings described below.

The **[!UICONTROL Linked live environment]** field is set automatically when the environment is created — see [Type of environment](#type).

## Access the offer environment settings {#access}

Offer environments are stored as folders. To access an environment and modify its properties, follow these steps. 

1. From the left navigation menu, open the **[!UICONTROL Explorer]** and locate the offer environment folder under the **Design environment** node.

1. Click on the ... button, and select **[!UICONTROL Folder settings]** to display the environment settings.

  ![Screenshot showing the Folder settings option of an environment](assets/offers-env-1.png){zoomable="yes"}

The folder settings of an offer environment group offer-specific options into several sections. 

-->
<!-- 
Most settings mirror the offer environment configuration available in the Adobe Campaign client console.
-->
<!-- 

## Properties {#properties}

This section is common to all folders. It allows you to define the **Label** of the folder and modify the technical folder properties.  

![Screenshot showing the Properties settings of an environment](assets/offers-env-2.png){zoomable="yes"}

-->
<!--

* **[!UICONTROL Label]** — Display name of the environment.


Expand **[!UICONTROL Additional options]** to access the technical properties of the folder:

* **[!UICONTROL Internal name]** — Unique identifier of the folder. Used to reference the environment from schemas, workflows, and API calls. The internal name is set at creation and should not be changed afterwards.

* **[!UICONTROL Full name]** — Read-only path of the folder in the Explorer tree (for example, `/Offers - design/Environment - Recipient/`).

* **[!UICONTROL Template]** — Read-only name of the folder template the environment is based on (for example, **[!DNL nmsOfferEnv]** for an offer environment).

* **[!UICONTROL Created by]** / **[!UICONTROL Modified by]** — Audit fields populated automatically with the operator that created and last modified the folder.

This section gathers the offer-specific settings of the folder.

-->
<!--

## Environment {#env-section}

  ![Screenshot showing the Environment settings of an environment](assets/offers-env-3.png){zoomable="yes"}

### Type of environment {#type}

* **[!UICONTROL Type of environment]** — Switches the folder between **[!UICONTROL Design]** and **[!UICONTROL Live]**. The type is set when the environment is created. Changing it later is not recommended.

 **[!UICONTROL Linked live environment]** — Displays the read-only **[!UICONTROL Live]** environment that receives the deployed offers. Set automatically when the environment is created.

### Execution instances {#execution-instances}

* **[!UICONTROL Display execution instances]** — Opens the list of execution instances mapped to the environment. This section is only displayed when the multi-instance execution option is activated. Refer to the [Campaign v8 documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-architecture.html?lang=it#distributed-architecture){target="_blank"}.

### Targets of this environment {#targets}

  ![Screenshot showing the other Environment settings of an environment](assets/offers-env-4.png){zoomable="yes"}

* **[!UICONTROL Environment dedicated to incoming anonymous interactions]** — Activates anonymous interaction features on the environment. This relies on a target mapping for the visitor targeting dimension, which you can now create directly from the Web UI — see [Manage target mappings](../administration/target-mappings.md). Refer to the [Campaign v8 documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-env.html#create-an-offer-environment){target="_blank"} for the full anonymous interaction setup.

-->
<!--
and [Anonymous interactions](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/anonymous-interactions.html){target="_blank"}.
-->
<!--

* **[!UICONTROL Targeting dimension]** — Schema and table of the contacts targeted by the offers contained in this environment (for example, **[!DNL Recipients (nms:recipient)]**). The targeting dimension is reused by every offer and offer space of the environment.

### Storage of generated propositions {#storage}

* **[!UICONTROL Storage dimension]** — Schema and table where the propositions generated through this environment are stored (for example, **[!DNL Recipient offer propositions (nms:propositionRcp)]**).

* **[!UICONTROL Call data schema]** — Schema used to capture the data of each call to the Offer engine (for example, **[!DNL Interactions (nms:interaction)]**). For details on this schema, refer to the [Campaign v8 data model documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/dev/datamodel.html){target="_blank"}.

### Implicit identification (if the function is enabled in the space) {#implicit-identification}

* **[!UICONTROL Target mapping]** — Used to configure the **changeover process**, which lets the Offer engine switch between an identified and an anonymous environment depending on whether the contact can be identified during an inbound interaction. Leave this field empty when implicit identification is not used. Learn how to create and manage target mappings directly from the Web UI in [Manage target mappings](../administration/target-mappings.md). For the offer-specific changeover process configuration, refer to [Campaign v8 documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/anonymous-interactions.html){target="_blank"}.

-->
<!--
## Eligibility {#eligibility}

  ![Screenshot showing the other Environment settings of an environment](assets/offers-env-5.png){zoomable="yes"}

* **[!UICONTROL Presentation typology]** — Typology rule of type **[!UICONTROL Offer presentation]** referenced by the environment. Presentation typologies exclude offers based on the proposition history of a recipient. You can edit these rules directly from the Web UI's **[!UICONTROL Business rules]** screen — see [Work with business rules (typologies)](../administration/typologies.md). Refer to the [Campaign v8 documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-offer.html?lang=it#offer-presentation){target="_blank"} for the full rule reference.

* **[!UICONTROL Filters on the target]** — Filter rules that apply to every offer in the environment. Use **[!UICONTROL Add rules]** to open the rule builder and restrict the audience targeted by all offers contained in this environment.

## Offer weight {#offer-weight}

* **[!UICONTROL Display offer weight]** — Click the **Display offer weight** button to open the read-only list of offer weights included in the environment folder. Weights themselves are configured at the offer space and the offer levels — refer to [Create and publish an offer](create-offer.md#eligibility).

## Security settings and Restrictions {#security}

These two sections are generic Campaign folder controls. They are not specific to offer management.

* **[!UICONTROL Security settings]** — The **[!UICONTROL Group or operator]** table defines the operators and operator groups allowed to read, write, or delete the environment and its contents. For Interaction-specific operator roles (Offer manager, Delivery manager), refer to [Operators of the Interaction module](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-operators.html){target="_blank"}.

* **[!UICONTROL System folder]** — When enabled, marks the folder as a system folder.

* **[!UICONTROL Restrictions]** — Lets you turn the folder into a view by enabling **[!UICONTROL This folder is a view]** and clicking **[!UICONTROL Edit restrictions]** to define a filter on the records displayed in the folder.
-->
Quindi, [crea uno spazio delle offerte](offer-space.md) per definire dove e come vengono esposte le offerte.
