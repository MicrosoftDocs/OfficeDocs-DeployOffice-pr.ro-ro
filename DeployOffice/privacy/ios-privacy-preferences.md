---
title: Utilizați preferințele pentru a gestiona controalele de confidențialitate ale Office pe dispozitivele iOS
ms.author: danbrown
author: pbowden-msft
manager: laurawi
audience: ITPro
ms.topic: article
ms.service: o365-proplus-itpro
localization_priority: Priority
ms.collection: Ent_O365
ms.custom:
- Ent_Office_ProPlus
- Ent_Office_Privacy
- Ent_Office_Mac
description: Furnizează administratorilor Office informații despre cum să gestioneze setările de confidențialitate pe dispozitive iOS.
hideEdit: true
ms.openlocfilehash: d1a14d2e1bfe45710255467fcbce9ac4af2c9cb7
ms.sourcegitcommit: 903d6bac7d8b7d8003863ac778c0b5bbdfa7a62a
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/21/2019
ms.locfileid: "37604295"
---
# <a name="use-preferences-to-manage-privacy-controls-for-office-on-ios-devices"></a><span data-ttu-id="30616-103">Utilizați preferințele pentru a gestiona controalele de confidențialitate ale Office pe dispozitivele iOS</span><span class="sxs-lookup"><span data-stu-id="30616-103">Use preferences to manage privacy controls for Office on iOS devices</span></span>

<span data-ttu-id="30616-104">Există noi setări de preferințe pentru Office pe dispozitivele iOS care vă permit să controlați setările asociate cu:</span><span class="sxs-lookup"><span data-stu-id="30616-104">There are new preference settings for Office on iOS devices that allow you to control settings related to the following:</span></span>

- <span data-ttu-id="30616-105">***Date de diagnosticare*** care sunt colectate și trimise la Microsoft despre software-ul client Office utilizat</span><span class="sxs-lookup"><span data-stu-id="30616-105">***Diagnostic data*** that is collected and sent to Microsoft about Office client software being used.</span></span>

- <span data-ttu-id="30616-106">***Experiențe conectate*** care utilizează funcționalitatea în cloud pentru a vă furniza caracteristici îmbunătățite de Office dvs. și utilizatorilor dvs.</span><span class="sxs-lookup"><span data-stu-id="30616-106">***Connected experiences*** that use cloud-based functionality to provide enhanced Office features to you and your users.</span></span>

<span data-ttu-id="30616-107">Pentru mai multe informații despre datele de diagnosticare și experiențele conectate, consultați [Prezentare generală a controalelor de confidențialitate](overview-privacy-controls.md).</span><span class="sxs-lookup"><span data-stu-id="30616-107">For more information about diagnostic data and connected experiences, see [Overview of privacy controls](overview-privacy-controls.md).</span></span>

<span data-ttu-id="30616-108">Aceste setări de preferințe se aplică la următoarele aplicații:</span><span class="sxs-lookup"><span data-stu-id="30616-108">These preference settings apply to the following applications:</span></span>
- <span data-ttu-id="30616-109">Versiunea 2.30 și versiunile ulterioare de Word pentru iOS, Excel pentru iOS și PowerPoint pentru iOS.</span><span class="sxs-lookup"><span data-stu-id="30616-109">Version 2.30 and later of Word for iOS, Excel for iOS, and PowerPoint for iOS.</span></span>
- <span data-ttu-id="30616-110">Versiunea 16.30 și versiunile ulterioare de OneNote pentru iOS.</span><span class="sxs-lookup"><span data-stu-id="30616-110">Version 16.30 and later of OneNote for iOS.</span></span>
- <span data-ttu-id="30616-111">Versiunea 1.17 și versiunile ulterioare de Visio Viewer pentru iOS.</span><span class="sxs-lookup"><span data-stu-id="30616-111">Version 1.17 and later of Visio Viewer for iOS.</span></span>

> [!NOTE]
> <span data-ttu-id="30616-112">Pentru mai multe informații despre setări similare pentru Office pe calculatoare care rulează macOS, consultați [Utilizați preferințele pentru a gestiona controalele de confidențialitate pentru Office pentru Mac](mac-privacy-preferences.md).</span><span class="sxs-lookup"><span data-stu-id="30616-112">For information about similar settings for Office on computers running Windows, see [Use policy settings to manage privacy controls for Office 365 ProPlus](mac-privacy-preferences.md).</span></span>


## <a name="setting-device-preferences"></a><span data-ttu-id="30616-113">Setarea preferințelor dispozitivelor</span><span class="sxs-lookup"><span data-stu-id="30616-113">Setting device preferences</span></span>
<span data-ttu-id="30616-114">Aceste noi setări de preferințe pot fi, de asemenea, setate la nivel de dispozitiv de către un server de Management a dispozitivelor mobile (MDM) atunci când este instalată aplicația Office.</span><span class="sxs-lookup"><span data-stu-id="30616-114">These new preference settings can also be set at the device level by a Mobile Device Management (MDM) server when the Office application is installed.</span></span> <span data-ttu-id="30616-115">Multe servere MDM le permit administratorilor IT să adauge un dicționar de configurare opțional atunci când serverul trimite comanda `InstallApplication` MDM către un dispozitiv iOS.</span><span class="sxs-lookup"><span data-stu-id="30616-115">Many MDM servers allow IT administrators to add an optional configuration dictionary when the server sends the `InstallApplication` MDM command to an iOS device.</span></span> <span data-ttu-id="30616-116">Consultați documentația serverului MDM pentru mai multe detalii.</span><span class="sxs-lookup"><span data-stu-id="30616-116">Refer to your MDM server documentation for more details.</span></span>

<span data-ttu-id="30616-117">Dicționarul este reprezentat ca un set de perechi de chei/valori în format XML.</span><span class="sxs-lookup"><span data-stu-id="30616-117">The dictionary is represented as a set of key/value pairs in XML format.</span></span> <span data-ttu-id="30616-118">De exemplu:</span><span class="sxs-lookup"><span data-stu-id="30616-118">For example:</span></span>

```xml
<dict>
    <key>DiagnosticDataTypePreference</key>
    <string>BasicDiagnosticData</string>
</dict>
```

<span data-ttu-id="30616-119">Odată trimis către dispozitiv, dicționarul de configurare se va afla sub cheia `com.apple.managed.configuration`, de unde va fi citit atunci când se lansează aplicația Office.</span><span class="sxs-lookup"><span data-stu-id="30616-119">Once sent to the device, the configuration dictionary will reside under the `com.apple.managed.configuration` key, where it will be read when the Office application is launched.</span></span>

## <a name="preference-setting-for-diagnostic-data"></a><span data-ttu-id="30616-120">Setarea de preferințe pentru datele de diagnosticare </span><span class="sxs-lookup"><span data-stu-id="30616-120">Preference setting for diagnostic data</span></span>

<span data-ttu-id="30616-121">Datele de diagnosticare sunt utilizate pentru a menține Office securizat și actualizat, pentru a detecta, a diagnostica și a remedia problemele și, de asemenea, pentru a face îmbunătățiri ale produselor.</span><span class="sxs-lookup"><span data-stu-id="30616-121">Diagnostic data is used to keep Office secure and up-to-date, detect, diagnose and remediate problems, and also make product improvements.</span></span> <span data-ttu-id="30616-122">Pentru mai multe informații, consultați [Datele de diagnosticare trimise din Office 365 ProPlus către Microsoft](overview-privacy-controls.md#diagnostic-data-sent-from-office-365-proplus-to-microsoft).</span><span class="sxs-lookup"><span data-stu-id="30616-122">For more information, see [Diagnostic data sent from Office 365 ProPlus to Microsoft](overview-privacy-controls.md#diagnostic-data-sent-from-office-365-proplus-to-microsoft).</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="30616-123">**Cheie**</span><span class="sxs-lookup"><span data-stu-id="30616-123">**Key**</span></span>  | `DiagnosticDataTypePreference`  |
|<span data-ttu-id="30616-124">**Tip de date**</span><span class="sxs-lookup"><span data-stu-id="30616-124">**Data Type**</span></span>  | <span data-ttu-id="30616-125">Șir</span><span class="sxs-lookup"><span data-stu-id="30616-125">String</span></span> |
|<span data-ttu-id="30616-126">**Valori posibile**</span><span class="sxs-lookup"><span data-stu-id="30616-126">**Possible values**</span></span>  | <span data-ttu-id="30616-127">`BasicDiagnosticData` *(setează nivelul la Necesare)*</span><span class="sxs-lookup"><span data-stu-id="30616-127">`BasicDiagnosticData` *(this sets the level to Required)*</span></span> <br/> <span data-ttu-id="30616-128">`FullDiagnosticData` *(setează nivelul la Opționale)*</span><span class="sxs-lookup"><span data-stu-id="30616-128">`FullDiagnosticData` *(this sets the level to Optional)*</span></span> <br/> <span data-ttu-id="30616-129">`ZeroDiagnosticData` *(setează nivelul la Niciuna)*</span><span class="sxs-lookup"><span data-stu-id="30616-129">`ZeroDiagnosticData` *(this sets the level to Neither)*</span></span> |

<span data-ttu-id="30616-130">Dacă nu setați această preferință, se trimit doar datele necesare către Microsoft, dacă utilizatorii cu un abonament Office 365 sunt conectați cu un cont de la locul de muncă sau de la școală.</span><span class="sxs-lookup"><span data-stu-id="30616-130">Starting with new installations of Version 16.30, if you don't set this preference, only required diagnostic data is sent to Microsoft if users with an Office 365 subscription are signed in with a work or school account or if users have a volume licensed version of Office 2019 for Mac.</span></span> <span data-ttu-id="30616-131">De asemenea, acești utilizatori nu pot modifica nivelul de date de diagnostic, indiferent de modul în care setați această preferință.</span><span class="sxs-lookup"><span data-stu-id="30616-131">Also, these users can't change the level of diagnostic data regardless of how you set this preference.</span></span>

<span data-ttu-id="30616-132">Pentru alți utilizatori, cum ar fi utilizatorii la domiciliu cu abonament Office 365, sunt trimise doar date de diagnosticare necesare, cu excepția cazului în care utilizatorul alege să trimită și date de diagnosticare opționale, accesând **Setări** > **Setări de Confidențialitate**.</span><span class="sxs-lookup"><span data-stu-id="30616-132">For other users, such as home users with an Office 365 subscription, only required diagnostic data is sent, unless the user chooses to also send optional diagnostic data by going to **Preferences** > **Privacy**.</span></span>


## <a name="preference-setting-for-connected-experiences-that-analyze-your-content"></a><span data-ttu-id="30616-133">Setarea de preferințe pentru experiențe conectate care analizează conținutul</span><span class="sxs-lookup"><span data-stu-id="30616-133">Preference setting for connected experiences that analyze your content</span></span>

<span data-ttu-id="30616-134">Experiențele conectate care vă analizează conținutul sunt experiențe care utilizează conținutul Office pentru vă oferi recomandări de proiectare, sugestii de editare, detalii privind datele și alte caracteristici similare.</span><span class="sxs-lookup"><span data-stu-id="30616-134">Connected experiences that analyze your content are experiences that use your Office content to provide you with design recommendations, editing suggestions, data insights, and similar features.</span></span> <span data-ttu-id="30616-135">De exemplu, Idei de proiectare în PowerPoint.</span><span class="sxs-lookup"><span data-stu-id="30616-135">For example, Design Ideas in PowerPoint.</span></span> <span data-ttu-id="30616-136">Pentru o listă a acestor experiențe conectate, consultați [Experiențe conectate în Office](connected-experiences.md)</span><span class="sxs-lookup"><span data-stu-id="30616-136">For a list of these connected experiences, see [Connected experiences in Office](connected-experiences.md).</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="30616-137">**Cheie**</span><span class="sxs-lookup"><span data-stu-id="30616-137">**Key**</span></span>  | `OfficeExperiencesAnalyzingContentPreference`  |
|<span data-ttu-id="30616-138">**Tip de date**</span><span class="sxs-lookup"><span data-stu-id="30616-138">**Data Type**</span></span>  | <span data-ttu-id="30616-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="30616-139">Boolean</span></span> |
|<span data-ttu-id="30616-140">**Valori posibile**</span><span class="sxs-lookup"><span data-stu-id="30616-140">**Possible values**</span></span>  | <span data-ttu-id="30616-141">`TRUE` *(activat)*</span><span class="sxs-lookup"><span data-stu-id="30616-141">`TRUE` *(enabled)*</span></span> <br/> <span data-ttu-id="30616-142">`FALSE` *(dezactivat)*</span><span class="sxs-lookup"><span data-stu-id="30616-142">`FALSE` *(disabled)*</span></span>|


<span data-ttu-id="30616-143">Dacă nu setați această preferință, experiențele conectate care analizează conținut sunt disponibile utilizatorilor.</span><span class="sxs-lookup"><span data-stu-id="30616-143">If you don't set this preference, connected experiences that analyze content are available to users.</span></span>

<span data-ttu-id="30616-144">Dacă utilizatorul are un abonament Office 365 și este conectat cu un cont de la locul de muncă sau de la școală atunci utilizatorul nu poate dezactiva experiențele conectate care analizează conținutul.</span><span class="sxs-lookup"><span data-stu-id="30616-144">If the user has an Office 365 subscription and is signed in with a work or school account or if the user has a volume licensed version of Office 2019 for Mac, then the user can't turn off connected experiences that analyze content.</span></span>

<span data-ttu-id="30616-145">Pentru alți utilizatori, cum ar fi utilizatori la domiciliu cu un abonament Office 365, utilizatorul poate alege să dezactiveze experiențe conectate care analizează conținutul accesând **Setări** > **Setări de Confidențialitate**.</span><span class="sxs-lookup"><span data-stu-id="30616-145">For other users, such as home users with an Office 365 subscription, the user can choose to turn off connected experiences that analyze content by going to **Preferences** > **Privacy**.</span></span>

## <a name="preference-setting-for-connected-experiences-that-download-online-content"></a><span data-ttu-id="30616-146">Setarea de preferințe pentru experiențe conectate care descarcă conținut online</span><span class="sxs-lookup"><span data-stu-id="30616-146">Preference setting for connected experiences that download online content</span></span>

<span data-ttu-id="30616-147">Experiențele conectate care descarcă conținut online sunt experiențe care vă permit să căutați și să descărcați conținut online, inclusiv șabloane, imagini, videoclipuri și materiale de referință pentru a vă îmbunătăți documentele.</span><span class="sxs-lookup"><span data-stu-id="30616-147">Connected experiences that download online content are experiences that allow you to search and download online content including templates, images, 3D models, videos, and reference materials to enhance your documents.</span></span> <span data-ttu-id="30616-148">De exemplu, șabloanele Office sau inserarea unei pictograme online.</span><span class="sxs-lookup"><span data-stu-id="30616-148">For example, Office templates or inserting an online icon.</span></span> <span data-ttu-id="30616-149">Pentru o listă a acestor experiențe conectate, consultați [Experiențe conectate în Office](connected-experiences.md)</span><span class="sxs-lookup"><span data-stu-id="30616-149">For a list of these connected experiences, see [Connected experiences in Office](connected-experiences.md).</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="30616-150">**Cheie**</span><span class="sxs-lookup"><span data-stu-id="30616-150">**Key**</span></span>  | `OfficeExperiencesDownloadingContentPreference`  |
|<span data-ttu-id="30616-151">**Tip de date**</span><span class="sxs-lookup"><span data-stu-id="30616-151">**Data Type**</span></span>  | <span data-ttu-id="30616-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="30616-152">Boolean</span></span> |
|<span data-ttu-id="30616-153">**Valori posibile**</span><span class="sxs-lookup"><span data-stu-id="30616-153">**Possible values**</span></span>  | <span data-ttu-id="30616-154">`TRUE` *(activat)*</span><span class="sxs-lookup"><span data-stu-id="30616-154">`TRUE` *(enabled)*</span></span> <br/> <span data-ttu-id="30616-155">`FALSE` *(dezactivat)*</span><span class="sxs-lookup"><span data-stu-id="30616-155">`FALSE` *(disabled)*</span></span>|


<span data-ttu-id="30616-156">Dacă nu setați această preferință, experiențele conectate care descarcă conținut online sunt disponibile utilizatorilor.</span><span class="sxs-lookup"><span data-stu-id="30616-156">If you don't set this preference, connected experiences that download online content are available to users.</span></span>

<span data-ttu-id="30616-157">Dacă utilizatorul are un abonament Office 365 și este conectat cu un cont de la locul de muncă sau de la școală, atunci utilizatorul nu poate dezactiva experiențele conectate care descarcă conținut online.</span><span class="sxs-lookup"><span data-stu-id="30616-157">If the user has an Office 365 subscription and is signed in with a work or school account or if the user has a volume licensed version of Office 2019 for Mac, then the user can't turn off connected experiences that download online content.</span></span>

<span data-ttu-id="30616-158">Pentru alți utilizatori, cum ar fi utilizatorii la domiciliu cu un abonament Office 365, utilizatorul poate alege să dezactiveze experiențele conectate care descarcă conținut online accesând **Setări** > **Setări de confidențialitate**.</span><span class="sxs-lookup"><span data-stu-id="30616-158">For other users, such as home users with an Office 365 subscription, a user can choose to turn off connected experiences that download online content by going to **Preferences** > **Privacy**.</span></span>

## <a name="preference-setting-for-optional-connected-experiences"></a><span data-ttu-id="30616-159">Setarea preferințelor pentru experiențe conectate opționale</span><span class="sxs-lookup"><span data-stu-id="30616-159">Preference setting for optional connected experiences</span></span>

<span data-ttu-id="30616-160">În plus față de experiențele conectate menționate mai sus, există câteva experiențe conectate opționale pe care le puteți alege pentru a le permite utilizatorilor să le acceseze cu contul organizației lor, care este uneori denumit cont de la locul de muncă sau de la școală.</span><span class="sxs-lookup"><span data-stu-id="30616-160">In addition to the connected experiences mentioned above, there are some optional connected experiences that you may choose to allow your users to access with their organization account, which is sometimes referred to as a work or school account.</span></span> <span data-ttu-id="30616-161">De exemplu, programele de completare Office care sunt descărcate prin Magazinul Office pe dispozitivul dvs.</span><span class="sxs-lookup"><span data-stu-id="30616-161">For example, Office add-ins that are downloaded through the Office Store to your device.</span></span> <span data-ttu-id="30616-162">Pentru mai multe exemple, consultați [Prezentare generală a experiențelor conectate opționale în Office](optional-connected-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="30616-162">For more examples, see [Overview of optional connected experiences in Office](optional-connected-experiences.md).</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="30616-163">**Cheie**</span><span class="sxs-lookup"><span data-stu-id="30616-163">**Key**</span></span>  | `OptionalConnectedExperiencesPreference`  |
|<span data-ttu-id="30616-164">**Tip de date**</span><span class="sxs-lookup"><span data-stu-id="30616-164">**Data Type**</span></span>  | <span data-ttu-id="30616-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="30616-165">Boolean</span></span> |
|<span data-ttu-id="30616-166">**Valori posibile**</span><span class="sxs-lookup"><span data-stu-id="30616-166">**Possible values**</span></span>  | <span data-ttu-id="30616-167">`TRUE` *(activat)*</span><span class="sxs-lookup"><span data-stu-id="30616-167">`TRUE` *(enabled)*</span></span> <br/> <span data-ttu-id="30616-168">`FALSE` *(dezactivat)*</span><span class="sxs-lookup"><span data-stu-id="30616-168">`FALSE` *(disabled)*</span></span>|


<span data-ttu-id="30616-169">Dacă nu setați această preferință, datele de diagnostic opționale sunt disponibile utilizatorilor cu un abonament Office 365 care sunt conectați cu un cont de la locul de muncă sau de la școală.</span><span class="sxs-lookup"><span data-stu-id="30616-169">If you don't set this preference, optional connected experiences are available to users with an Office 365 subscription that are signed in with a work or school account or users who have a volume licensed version of Office 2019 for Mac.</span></span> <span data-ttu-id="30616-170">Cu excepția cazului în care ați setat această preferință la FALS, acești utilizatori pot alege să dezactiveze experiențele conectate opționale accesând **Setări** > **Setări de confidențialitate**.</span><span class="sxs-lookup"><span data-stu-id="30616-170">Unless you have set this preference to , these users can choose to turn off optional connected experiences by going to Preferences  Privacy.</span></span>

<span data-ttu-id="30616-171">Pentru alți utilizatori, cum ar fi utilizatori casnici cu un abonament Office 365, nu există o opțiune de a dezactiva experiențele conectate opționale.</span><span class="sxs-lookup"><span data-stu-id="30616-171">For other users, such as home users with an Office 365 subscription, there isn't an option to turn off optional connected experiences.</span></span>