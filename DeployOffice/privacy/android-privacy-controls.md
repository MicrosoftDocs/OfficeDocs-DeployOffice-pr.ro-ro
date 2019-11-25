---
title: Utilizați setările de politică pentru a gestiona controale de confidențialitate pentru Office pe dispozitivele Android
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
audience: ITPro
ms.topic: article
ms.service: o365-proplus-itpro
localization_priority: Priority
ms.collection: Ent_O365
ms.custom:
- Ent_Office_ProPlus
- Ent_Office_Privacy
description: Furnizează administratorilor Office informații despre cum să gestioneze setările de confidențialitate pentru Office pe dispozitive Android.
hideEdit: true
ms.openlocfilehash: 36ae9878d03845c24e3717dfac970b2b961279dc
ms.sourcegitcommit: acb22296532bbfdfcad4dc1e7162f812997fbdd1
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 11/08/2019
ms.locfileid: "38068446"
---
# <a name="use-policy-settings-to-manage-privacy-controls-for-office-on-android-devices"></a><span data-ttu-id="85864-103">Utilizați setările de politică pentru a gestiona controale de confidențialitate pentru Office pe dispozitivele Android</span><span class="sxs-lookup"><span data-stu-id="85864-103">Use policy settings to manage privacy controls for Office 365 ProPlus</span></span>

<span data-ttu-id="85864-104">Există noi setări de politică pentru Office pe dispozitivele Android care vă permit să controlați setările asociate cu:</span><span class="sxs-lookup"><span data-stu-id="85864-104">There are new preference settings for Office on iOS devices that allow you to control settings related to the following:</span></span>

- <span data-ttu-id="85864-105">***Date de diagnosticare*** care sunt colectate și trimise la Microsoft despre software-ul client Office utilizat</span><span class="sxs-lookup"><span data-stu-id="85864-105">***Diagnostic data*** that is collected and sent to Microsoft about Office client software being used.</span></span>

- <span data-ttu-id="85864-106">***Experiențe conectate*** care utilizează funcționalitatea în cloud pentru a vă furniza caracteristici îmbunătățite de Office dvs. și utilizatorilor dvs.</span><span class="sxs-lookup"><span data-stu-id="85864-106">***Connected experiences*** that use cloud-based functionality to provide enhanced Office features to you and your users.</span></span>

<span data-ttu-id="85864-107">Pentru mai multe informații despre datele de diagnosticare și experiențele conectate, consultați [Prezentare generală a controalelor de confidențialitate](overview-privacy-controls.md).</span><span class="sxs-lookup"><span data-stu-id="85864-107">For more information about diagnostic data and connected experiences, see [Overview of privacy controls](overview-privacy-controls.md).</span></span>

<span data-ttu-id="85864-108">Aceste setări de politică se aplică la următoarele aplicații:</span><span class="sxs-lookup"><span data-stu-id="85864-108">These preference settings apply to the following applications:</span></span>
- <span data-ttu-id="85864-109">Versiunea 16.0.12226.10000 și versiunile ulterioare de Word pentru Android, Excel pentru Android și PowerPoint pentru Android.</span><span class="sxs-lookup"><span data-stu-id="85864-109">Version 16.0.12226.10000 and later of Word for Android, Excel for Android, and PowerPoint for Android.</span></span>
- <span data-ttu-id="85864-110">Versiunea 16.0.12228.20004 și versiunile ulterioare de OneNote pentru Android.</span><span class="sxs-lookup"><span data-stu-id="85864-110">Version 16.0.12228.20004 and later of OneNote for Android.</span></span>

> [!NOTE]
>- <span data-ttu-id="85864-111">Aceste setări de politică se aplică și versiunii 16.0.12130.20272 și versiunilor ulterioare ale previzualizării publice a [aplicației Office Mobile](https://techcommunity.microsoft.com/t5/Office-Apps-Blog/Introducing-Office-Your-new-go-to-mobile-app-for-getting-work/ba-p/977172) pentru Android.</span><span class="sxs-lookup"><span data-stu-id="85864-111">These policy settings also apply to Version 16.0.12130.20272 and later of the public preview of the [Office Mobile app](https://techcommunity.microsoft.com/t5/Office-Apps-Blog/Introducing-Office-Your-new-go-to-mobile-app-for-getting-work/ba-p/977172) for Android.</span></span>
>- <span data-ttu-id="85864-112">Prin utilizarea previzualizării publice a aplicației Office Mobile pentru Android se vor colecta jurnale de eroare care pot cuprinde conținut în unele circumstanțe.</span><span class="sxs-lookup"><span data-stu-id="85864-112">Use of the public preview of the Office Mobile app for Android will collect crash logs which may in some circumstances contain content.</span></span>
>- <span data-ttu-id="85864-113">Dacă vă îngrijorează colectarea de date din previzualizarea publică a aplicației Office Mobile pentru Android, trebuie să-i informați pe utilizatori să nu se conecteze la aplicație cu conturile de la locul de muncă sau de la școală.</span><span class="sxs-lookup"><span data-stu-id="85864-113">If you're concerned about the collection of data from the public preview of the Office Mobile app for Android, you should inform your users not to log into the application with their work or school accounts.</span></span>

## <a name="policy-settings-available-for-office-on-android-devices"></a><span data-ttu-id="85864-114">Setări de politică disponibile pentru Office pe dispozitive Android</span><span class="sxs-lookup"><span data-stu-id="85864-114">Policy settings available for Office on Android devices</span></span>

<span data-ttu-id="85864-115">Următorul tabel enumeră setările de politică disponibile pentru Office pe dispozitive Android și câte un link către informații suplimentare despre fiecare setare de politică.</span><span class="sxs-lookup"><span data-stu-id="85864-115">The following table lists which policy settings are available for Office on Android devices and a link to additional information about each policy setting.</span></span>

> [!NOTE]
>- <span data-ttu-id="85864-116">Informațiile suplimentare furnizate se referă la setările de politică pentru Office pe dispozitive care rulează Windows.</span><span class="sxs-lookup"><span data-stu-id="85864-116">The additional information provided covers the policy settings for Office on devices running Windows.</span></span> <span data-ttu-id="85864-117">Dar aceste informații se aplică și la Office pe dispozitive Android, deoarece setările de politică sunt aceleași.</span><span class="sxs-lookup"><span data-stu-id="85864-117">But the same information applies to Office on Android devices because they are the same policy settings.</span></span>
>- <span data-ttu-id="85864-118">Setarea de politică *Permiteți utilizarea de experiențe conectate în Office* disponibilă pentru Office pe dispozitive care rulează Windows nu se aplică la Office pe dispozitive Android.</span><span class="sxs-lookup"><span data-stu-id="85864-118">The *Allow the use of connected experiences in Office* policy setting that's available for Office on devices running Windows does not apply to Office on Android devices.</span></span> 


|<span data-ttu-id="85864-119">Numele setării de politică</span><span class="sxs-lookup"><span data-stu-id="85864-119">Name of policy setting</span></span>  |<span data-ttu-id="85864-120">Informații suplimentare</span><span class="sxs-lookup"><span data-stu-id="85864-120">Additional Information</span></span> |
|---------|---------|
|<span data-ttu-id="85864-121">Configurați nivelul datelor de diagnosticare pentru software-ul client trimise de Office la Microsoft</span><span class="sxs-lookup"><span data-stu-id="85864-121">Configure the level of client software diagnostic data sent by Office to Microsoft</span></span>|[<span data-ttu-id="85864-122">Setarea de politică pentru datele de diagnosticare</span><span class="sxs-lookup"><span data-stu-id="85864-122">Policy setting for diagnostic data</span></span>](manage-privacy-controls.md#policy-setting-for-diagnostic-data)         |
|<span data-ttu-id="85864-123">Permiteți utilizarea de experiențe conectate în Office care analizează conținut</span><span class="sxs-lookup"><span data-stu-id="85864-123">Allow the use of connected experiences in Office that analyze content</span></span>| [<span data-ttu-id="85864-124">Setarea de politică pentru experiențe conectate care analizează conținut</span><span class="sxs-lookup"><span data-stu-id="85864-124">Policy setting for connected experiences that analyze your content</span></span>](manage-privacy-controls.md#policy-setting-for-connected-experiences-that-analyze-your-content)        |
|<span data-ttu-id="85864-125">Permiteți utilizarea de experiențe conectate în Office care descarcă conținut online</span><span class="sxs-lookup"><span data-stu-id="85864-125">Allow the use of connected experiences in Office that download online content</span></span> |[<span data-ttu-id="85864-126">Setarea de politică pentru experiențe conectate care descarcă conținut online</span><span class="sxs-lookup"><span data-stu-id="85864-126">Policy setting for connected experiences that download online content</span></span>](manage-privacy-controls.md#policy-setting-for-connected-experiences-that-download-online-content)         |
|<span data-ttu-id="85864-127">Permiteți utilizarea de experiențe conectate opționale, suplimentare în Office</span><span class="sxs-lookup"><span data-stu-id="85864-127">Allow the use of additional optional connected experiences in Office</span></span> |[<span data-ttu-id="85864-128">Setarea de politică pentru experiențe conectate opționale</span><span class="sxs-lookup"><span data-stu-id="85864-128">Policy setting for optional connected experiences</span></span>](manage-privacy-controls.md#policy-setting-for-optional-connected-experiences)|



## <a name="use-office-cloud-policy-service-to-apply-policy-settings"></a><span data-ttu-id="85864-129">Utilizați serviciul de politică pentru cloud Office pentru a aplica setările de politică</span><span class="sxs-lookup"><span data-stu-id="85864-129">Use Office cloud policy service to apply policy settings</span></span>

<span data-ttu-id="85864-130">Pentru a aplica oricare dintre aceste 4 setări de politică pentru Office pe dispozitive Android, trebuie să utilizați serviciul de politică pentru cloud Office.</span><span class="sxs-lookup"><span data-stu-id="85864-130">To apply any of these 4 policy settings for Office on Android devices, you need to use the Office cloud policy service.</span></span> <span data-ttu-id="85864-131">Pentru mai multe informații despre utilizarea serviciului de politică pentru cloud Office, consultați [Prezentarea generală a serviciului de politică pentru cloud Office](../overview-office-cloud-policy-service.md).</span><span class="sxs-lookup"><span data-stu-id="85864-131">For more information on using the Office cloud policy service, see [Overview of the Office cloud policy service](../overview-office-cloud-policy-service.md).</span></span>

> [!NOTE]
> <span data-ttu-id="85864-132">Dacă ați utilizat anterior serviciul de politică pentru cloud Office pentru a configura aceste setări de politică pentru Office pe dispozitive care rulează Windows, aceleași setări se vor aplica și pentru Office pe dispozitive Android.</span><span class="sxs-lookup"><span data-stu-id="85864-132">If you previously used Office cloud policy service to configure these policy settings for Office on devices running Windows, those same settings will apply to Office on Android devices.</span></span> <span data-ttu-id="85864-133">Pentru ca aceasta să se întâmple, trebuie doar să vă conectați la serviciul de politică pentru cloud Office, iar acesta va aplica setările automat la Office pe dispozitive Android.</span><span class="sxs-lookup"><span data-stu-id="85864-133">For that to happen, you just need to sign in to the Office cloud policy service and the service will apply the settings automatically to Office on Android devices.</span></span>
