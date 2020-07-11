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
ms.openlocfilehash: 6465a5b5e2103070170bdec8cd64b8bc044d46a3
ms.sourcegitcommit: f441b1a5f8853c0941b3e23c7781c89abf0be641
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/09/2020
ms.locfileid: "45087859"
---
# <a name="use-preferences-to-manage-privacy-controls-for-office-on-ios-devices"></a><span data-ttu-id="9063a-103">Utilizați preferințele pentru a gestiona controalele de confidențialitate ale Office pe dispozitivele iOS</span><span class="sxs-lookup"><span data-stu-id="9063a-103">Use preferences to manage privacy controls for Office on iOS devices</span></span>

<span data-ttu-id="9063a-104">Există noi setări de preferințe pentru Office pe dispozitivele iOS care vă permit să controlați setările asociate cu:</span><span class="sxs-lookup"><span data-stu-id="9063a-104">There are new preference settings for Office on iOS devices that allow you to control settings related to the following:</span></span>

- <span data-ttu-id="9063a-105">***Date de diagnosticare*** care sunt colectate și trimise la Microsoft despre software-ul client Office utilizat</span><span class="sxs-lookup"><span data-stu-id="9063a-105">***Diagnostic data*** that is collected and sent to Microsoft about Office client software being used.</span></span>

- <span data-ttu-id="9063a-106">***Experiențe conectate*** care utilizează funcționalitatea în cloud pentru a vă furniza caracteristici îmbunătățite de Office dvs. și utilizatorilor dvs.</span><span class="sxs-lookup"><span data-stu-id="9063a-106">***Connected experiences*** that use cloud-based functionality to provide enhanced Office features to you and your users.</span></span>

<span data-ttu-id="9063a-107">Pentru mai multe informații despre datele de diagnosticare și experiențele conectate, consultați [Prezentare generală a controalelor de confidențialitate](overview-privacy-controls.md).</span><span class="sxs-lookup"><span data-stu-id="9063a-107">For more information about diagnostic data and connected experiences, see [Overview of privacy controls](overview-privacy-controls.md).</span></span>

<span data-ttu-id="9063a-108">Aceste setări de preferințe se aplică la următoarele aplicații:</span><span class="sxs-lookup"><span data-stu-id="9063a-108">These preference settings apply to the following applications:</span></span>
- <span data-ttu-id="9063a-109">Versiunea 2.30 și versiunile ulterioare de Word pentru iOS, Excel pentru iOS și PowerPoint pentru iOS.</span><span class="sxs-lookup"><span data-stu-id="9063a-109">Version 2.30 and later of Word for iOS, Excel for iOS, and PowerPoint for iOS.</span></span>
- <span data-ttu-id="9063a-110">Versiunea 4.30.0 și versiunile ulterioare de Outlook pentru iOS.</span><span class="sxs-lookup"><span data-stu-id="9063a-110">Version 4.30.0 and later of Outlook for iOS</span></span>
- <span data-ttu-id="9063a-111">Versiunea 16.30 și versiunile ulterioare de OneNote pentru iOS.</span><span class="sxs-lookup"><span data-stu-id="9063a-111">Version 16.30 and later of OneNote for iOS.</span></span>
- <span data-ttu-id="9063a-112">Versiunea 11.19.11 și versiunile ulterioare de OneDrive pentru iOS.</span><span class="sxs-lookup"><span data-stu-id="9063a-112">Version 11.19.11 and later of OneDrive for iOS.</span></span>
- <span data-ttu-id="9063a-113">Versiunea 1.17 și versiunile ulterioare de Visio Viewer pentru iOS.</span><span class="sxs-lookup"><span data-stu-id="9063a-113">Version 1.17 and later of Visio Viewer for iOS.</span></span>

> [!NOTE]
> <span data-ttu-id="9063a-114">Pentru mai multe informații despre setări similare pentru Office pe calculatoare care rulează macOS, consultați [Utilizați preferințele pentru a gestiona controalele de confidențialitate pentru Office pentru Mac](mac-privacy-preferences.md).</span><span class="sxs-lookup"><span data-stu-id="9063a-114">For information about similar settings for Office on computers running macOS, see [Use preferences to manage privacy controls for Office for Mac](mac-privacy-preferences.md)</span></span>


## <a name="setting-device-preferences"></a><span data-ttu-id="9063a-115">Setarea preferințelor dispozitivelor</span><span class="sxs-lookup"><span data-stu-id="9063a-115">Setting device preferences</span></span>
<span data-ttu-id="9063a-116">Aceste noi setări de preferințe pot fi, de asemenea, setate la nivel de dispozitiv de către un server de Management a dispozitivelor mobile (MDM) atunci când este instalată aplicația Office.</span><span class="sxs-lookup"><span data-stu-id="9063a-116">These new preference settings can also be set at the device level by a Mobile Device Management (MDM) server when the Office application is installed.</span></span> <span data-ttu-id="9063a-117">Multe servere MDM le permit administratorilor IT să adauge un dicționar de configurare opțional atunci când serverul trimite comanda `InstallApplication` MDM către un dispozitiv iOS.</span><span class="sxs-lookup"><span data-stu-id="9063a-117">Many MDM servers allow IT administrators to add an optional configuration dictionary when the server sends the `InstallApplication` MDM command to an iOS device.</span></span> <span data-ttu-id="9063a-118">Consultați documentația serverului MDM pentru mai multe detalii.</span><span class="sxs-lookup"><span data-stu-id="9063a-118">Refer to your MDM server documentation for more details.</span></span>

<span data-ttu-id="9063a-119">Dicționarul este reprezentat ca un set de perechi de chei/valori în format XML.</span><span class="sxs-lookup"><span data-stu-id="9063a-119">The dictionary is represented as a set of key/value pairs in XML format.</span></span> <span data-ttu-id="9063a-120">De exemplu:</span><span class="sxs-lookup"><span data-stu-id="9063a-120">For example:</span></span>

```xml
<dict>
    <key>DiagnosticDataTypePreference</key>
    <string>BasicDiagnosticData</string>
</dict>
```

<span data-ttu-id="9063a-121">Odată trimis către dispozitiv, dicționarul de configurare se va afla sub cheia `com.apple.managed.configuration`, de unde va fi citit atunci când se lansează aplicația Office.</span><span class="sxs-lookup"><span data-stu-id="9063a-121">Once sent to the device, the configuration dictionary will reside under the `com.apple.managed.configuration` key, where it will be read when the Office application is launched.</span></span>

> [!NOTE]
> <span data-ttu-id="9063a-122">De asemenea, puteți utiliza serviciul de politici cloud pentru Office și aceste patru setări de politică:</span><span class="sxs-lookup"><span data-stu-id="9063a-122">You can also use the Office cloud policy service and these 4 policy settings:</span></span>
> - <span data-ttu-id="9063a-123">Configurați nivelul datelor de diagnosticare pentru software-ul client trimise de Office la Microsoft</span><span class="sxs-lookup"><span data-stu-id="9063a-123">Configure the level of client software diagnostic data sent by Office to Microsoft</span></span>
> - <span data-ttu-id="9063a-124">Permiteți utilizarea de experiențe conectate în Office care analizează conținut</span><span class="sxs-lookup"><span data-stu-id="9063a-124">Allow the use of connected experiences in Office that analyze content</span></span>
> - <span data-ttu-id="9063a-125">Permiteți utilizarea de experiențe conectate în Office care descarcă conținut online</span><span class="sxs-lookup"><span data-stu-id="9063a-125">Allow the use of connected experiences in Office that download online content</span></span>
> - <span data-ttu-id="9063a-126">Permiteți utilizarea de experiențe conectate opționale, suplimentare în Office</span><span class="sxs-lookup"><span data-stu-id="9063a-126">Allow the use of additional optional connected experiences in Office</span></span>
>
> <span data-ttu-id="9063a-127">Setările de confidențialitate pentru Outlook pentru iOS și OneDrive pentru iOS pot fi configurate doar utilizând serviciul de politici cloud pentru Office.</span><span class="sxs-lookup"><span data-stu-id="9063a-127">Privacy settings for Outlook for iOS and OneDrive for iOS can only be configured by using the Office cloud policy service.</span></span>
>
> <span data-ttu-id="9063a-128">Pentru mai multe informații despre utilizarea serviciului de politici cloud pentru Office, consultați [Prezentarea generală a serviciului de politici cloud pentru Office](../overview-office-cloud-policy-service.md).</span><span class="sxs-lookup"><span data-stu-id="9063a-128">For more information on using the Office cloud policy service, see [Overview of the Office cloud policy service](../overview-office-cloud-policy-service.md).</span></span>

## <a name="preference-setting-for-diagnostic-data"></a><span data-ttu-id="9063a-129">Setarea de preferințe pentru datele de diagnosticare </span><span class="sxs-lookup"><span data-stu-id="9063a-129">Preference setting for diagnostic data</span></span>

<span data-ttu-id="9063a-130">Datele de diagnosticare sunt utilizate pentru a menține Office securizat și actualizat, pentru a detecta, a diagnostica și a remedia problemele și, de asemenea, pentru a face îmbunătățiri de produs.</span><span class="sxs-lookup"><span data-stu-id="9063a-130">Diagnostic data is used to keep Office secure and up-to-date, detect, diagnose and remediate problems, and also make product improvements.</span></span> <span data-ttu-id="9063a-131">Pentru mai multe informații, consultați [Datele de diagnosticare trimise din Aplicații Microsoft 365 pentru întreprindere la Microsoft](overview-privacy-controls.md#diagnostic-data-sent-from-microsoft-365-apps-for-enterprise-to-microsoft).</span><span class="sxs-lookup"><span data-stu-id="9063a-131">For more information, see [Diagnostic data sent from Microsoft 365 Apps for enterprise to Microsoft](overview-privacy-controls.md#diagnostic-data-sent-from-microsoft-365-apps-for-enterprise-to-microsoft).</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9063a-132">**Cheie**</span><span class="sxs-lookup"><span data-stu-id="9063a-132">**Key**</span></span>  | `DiagnosticDataTypePreference`  |
|<span data-ttu-id="9063a-133">**Tip de date**</span><span class="sxs-lookup"><span data-stu-id="9063a-133">**Data Type**</span></span>  | <span data-ttu-id="9063a-134">Șir</span><span class="sxs-lookup"><span data-stu-id="9063a-134">String</span></span> |
|<span data-ttu-id="9063a-135">**Valori posibile**</span><span class="sxs-lookup"><span data-stu-id="9063a-135">**Possible values**</span></span>  | <span data-ttu-id="9063a-136">`BasicDiagnosticData` *(setează nivelul la Necesare)*</span><span class="sxs-lookup"><span data-stu-id="9063a-136">`BasicDiagnosticData` *(this sets the level to Required)*</span></span> <br/> <span data-ttu-id="9063a-137">`FullDiagnosticData` *(setează nivelul la Opționale)*</span><span class="sxs-lookup"><span data-stu-id="9063a-137">`FullDiagnosticData` *(this sets the level to Optional)*</span></span> <br/> <span data-ttu-id="9063a-138">`ZeroDiagnosticData` *(setează nivelul la Niciuna)*</span><span class="sxs-lookup"><span data-stu-id="9063a-138">`ZeroDiagnosticData` *(this sets the level to Neither)*</span></span> |

<span data-ttu-id="9063a-139">Dacă nu setați această preferință, sunt trimise doar datele de diagnosticare necesare către Microsoft, dacă utilizatorii cu abonament Office 365 (sau Microsoft 365) sunt conectați cu un cont de la locul de muncă sau de la școală.</span><span class="sxs-lookup"><span data-stu-id="9063a-139">If you don't set this preference, only required diagnostic data is sent to Microsoft if users with an Office 365 (or Microsoft 365) subscription are signed in with a work or school account.</span></span> <span data-ttu-id="9063a-140">De asemenea, acești utilizatori nu pot modifica nivelul de date de diagnosticare, indiferent de modul în care setați această preferință.</span><span class="sxs-lookup"><span data-stu-id="9063a-140">Also, these users can't change the level of diagnostic data regardless of how you set this preference.</span></span>

<span data-ttu-id="9063a-141">Pentru alți utilizatori, cum ar fi utilizatorii la domiciliu cu abonament Office 365 (sau Microsoft 365), sunt trimise doar date de diagnosticare necesare, cu excepția cazului în care utilizatorul alege să trimită și date de diagnosticare opționale, accesând **Setări** > **Setări de confidențialitate**.</span><span class="sxs-lookup"><span data-stu-id="9063a-141">For other users, such as home users with an Office 365 (or Microsoft 365) subscription, only required diagnostic data is sent, unless the user chooses to also send optional diagnostic data by going to **Settings** > **Privacy Settings**.</span></span>


## <a name="preference-setting-for-connected-experiences-that-analyze-your-content"></a><span data-ttu-id="9063a-142">Setarea de preferințe pentru experiențe conectate care analizează conținutul</span><span class="sxs-lookup"><span data-stu-id="9063a-142">Preference setting for connected experiences that analyze your content</span></span>

<span data-ttu-id="9063a-143">Experiențele conectate care vă analizează conținutul sunt experiențe care utilizează conținutul Office pentru vă oferi recomandări de proiectare, sugestii de editare, detalii privind datele și alte caracteristici similare.</span><span class="sxs-lookup"><span data-stu-id="9063a-143">Connected experiences that analyze your content are experiences that use your Office content to provide you with design recommendations, editing suggestions, data insights, and similar features.</span></span> <span data-ttu-id="9063a-144">De exemplu, Idei de proiectare în PowerPoint.</span><span class="sxs-lookup"><span data-stu-id="9063a-144">For example, Design Ideas in PowerPoint.</span></span> <span data-ttu-id="9063a-145">Pentru o listă a acestor experiențe conectate, consultați [Experiențe conectate în Office](connected-experiences.md)</span><span class="sxs-lookup"><span data-stu-id="9063a-145">For a list of these connected experiences, see [Connected experiences in Office](connected-experiences.md).</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9063a-146">**Cheie**</span><span class="sxs-lookup"><span data-stu-id="9063a-146">**Key**</span></span>  | `OfficeExperiencesAnalyzingContentPreference`  |
|<span data-ttu-id="9063a-147">**Tip de date**</span><span class="sxs-lookup"><span data-stu-id="9063a-147">**Data Type**</span></span>  | <span data-ttu-id="9063a-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="9063a-148">Boolean</span></span> |
|<span data-ttu-id="9063a-149">**Valori posibile**</span><span class="sxs-lookup"><span data-stu-id="9063a-149">**Possible values**</span></span>  | <span data-ttu-id="9063a-150">`TRUE` *(activat)*</span><span class="sxs-lookup"><span data-stu-id="9063a-150">`TRUE` *(enabled)*</span></span> <br/> <span data-ttu-id="9063a-151">`FALSE` *(dezactivat)*</span><span class="sxs-lookup"><span data-stu-id="9063a-151">`FALSE` *(disabled)*</span></span>|


<span data-ttu-id="9063a-152">Dacă nu setați această preferință, experiențele conectate care analizează conținut sunt disponibile utilizatorilor.</span><span class="sxs-lookup"><span data-stu-id="9063a-152">If you don't set this preference, connected experiences that analyze content are available to users.</span></span>

<span data-ttu-id="9063a-153">Dacă utilizatorul are un abonament Office 365 (sau Microsoft 365) și este conectat cu un cont de la locul de muncă, atunci utilizatorul nu poate dezactiva experiențele conectate care analizează conținutul.</span><span class="sxs-lookup"><span data-stu-id="9063a-153">If the user has an Office 365 (or Microsoft 365) subscription and is signed in with a work or school account, then the user can't turn off connected experiences that analyze content.</span></span>

<span data-ttu-id="9063a-154">Pentru alți utilizatori, cum ar fi utilizatori la domiciliu cu un abonament Office 365 (sau Microsoft 365), utilizatorul poate alege să dezactiveze experiențele conectate care analizează conținutul accesând **Setări** > **Setări de confidențialitate**.</span><span class="sxs-lookup"><span data-stu-id="9063a-154">For other users, such as home users with an Office 365 (or Microsoft 365) subscription, the user can choose to turn off connected experiences that analyze content by going to **Settings** > **Privacy Settings**.</span></span>

## <a name="preference-setting-for-connected-experiences-that-download-online-content"></a><span data-ttu-id="9063a-155">Setarea de preferințe pentru experiențe conectate care descarcă conținut online</span><span class="sxs-lookup"><span data-stu-id="9063a-155">Preference setting for connected experiences that download online content</span></span>

<span data-ttu-id="9063a-156">Experiențele conectate care descarcă conținut online sunt experiențe care vă permit să căutați și să descărcați conținut online, inclusiv șabloane, imagini, videoclipuri și materiale de referință pentru a vă îmbunătăți documentele.</span><span class="sxs-lookup"><span data-stu-id="9063a-156">Connected experiences that download online content are experiences that allow you to search and download online content including templates, images, videos, and reference materials to enhance your documents.</span></span> <span data-ttu-id="9063a-157">De exemplu, șabloanele Office sau inserarea unei pictograme online.</span><span class="sxs-lookup"><span data-stu-id="9063a-157">For example, Office templates or inserting an online icon.</span></span> <span data-ttu-id="9063a-158">Pentru o listă a acestor experiențe conectate, consultați [Experiențe conectate în Office](connected-experiences.md)</span><span class="sxs-lookup"><span data-stu-id="9063a-158">For a list of these connected experiences, see [Connected experiences in Office](connected-experiences.md).</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9063a-159">**Cheie**</span><span class="sxs-lookup"><span data-stu-id="9063a-159">**Key**</span></span>  | `OfficeExperiencesDownloadingContentPreference`  |
|<span data-ttu-id="9063a-160">**Tip de date**</span><span class="sxs-lookup"><span data-stu-id="9063a-160">**Data Type**</span></span>  | <span data-ttu-id="9063a-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="9063a-161">Boolean</span></span> |
|<span data-ttu-id="9063a-162">**Valori posibile**</span><span class="sxs-lookup"><span data-stu-id="9063a-162">**Possible values**</span></span>  | <span data-ttu-id="9063a-163">`TRUE` *(activat)*</span><span class="sxs-lookup"><span data-stu-id="9063a-163">`TRUE` *(enabled)*</span></span> <br/> <span data-ttu-id="9063a-164">`FALSE` *(dezactivat)*</span><span class="sxs-lookup"><span data-stu-id="9063a-164">`FALSE` *(disabled)*</span></span>|


<span data-ttu-id="9063a-165">Dacă nu setați această preferință, experiențele conectate care descarcă conținut online sunt disponibile utilizatorilor.</span><span class="sxs-lookup"><span data-stu-id="9063a-165">If you don't set this preference, connected experiences that download online content are available to users.</span></span>

<span data-ttu-id="9063a-166">Dacă utilizatorul are un abonament Office 365 (sau Microsoft 365) și este conectat cu un cont de la locul de muncă, atunci utilizatorul nu poate dezactiva experiențele conectate pentru descărcarea conținutului online.</span><span class="sxs-lookup"><span data-stu-id="9063a-166">If the user has an Office 365 (or Microsoft 365) subscription and is signed in with a work or school account, then the user can't turn off connected experiences that download online content.</span></span>

<span data-ttu-id="9063a-167">Pentru alți utilizatori, cum ar fi utilizatori la domiciliu cu un abonament Office 365 (sau Microsoft 365), utilizatorul poate alege să dezactiveze experiențele conectate pentru descărcarea conținutului online accesând **Setări** > **Setări de confidențialitate**.</span><span class="sxs-lookup"><span data-stu-id="9063a-167">For other users, such as home users with an Office 365 (or Microsoft 365) subscription, the user can choose to turn off connected experiences that download online content by going to **Settings** > **Privacy Settings**.</span></span>

## <a name="preference-setting-for-optional-connected-experiences"></a><span data-ttu-id="9063a-168">Setarea preferințelor pentru experiențe conectate opționale</span><span class="sxs-lookup"><span data-stu-id="9063a-168">Preference setting for optional connected experiences</span></span>

<span data-ttu-id="9063a-169">În plus față de experiențele conectate menționate mai sus, există câteva experiențe conectate opționale pe care le puteți alege pentru a le permite utilizatorilor să le acceseze cu contul organizației lor, care este uneori denumit cont de la locul de muncă sau de la școală.</span><span class="sxs-lookup"><span data-stu-id="9063a-169">In addition to the connected experiences mentioned above, there are some optional connected experiences that you may choose to allow your users to access with their organization account, which is sometimes referred to as a work or school account.</span></span> <span data-ttu-id="9063a-170">De exemplu, programele de completare Office care sunt descărcate prin Magazinul Office pe dispozitivul dvs.</span><span class="sxs-lookup"><span data-stu-id="9063a-170">For example, Office add-ins that are downloaded through the Office Store to your device.</span></span> <span data-ttu-id="9063a-171">Pentru mai multe exemple, consultați [Prezentare generală a experiențelor conectate opționale în Office](optional-connected-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="9063a-171">For more examples, see [Overview of optional connected experiences in Office](optional-connected-experiences.md).</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9063a-172">**Cheie**</span><span class="sxs-lookup"><span data-stu-id="9063a-172">**Key**</span></span>  | `OptionalConnectedExperiencesPreference`  |
|<span data-ttu-id="9063a-173">**Tip de date**</span><span class="sxs-lookup"><span data-stu-id="9063a-173">**Data Type**</span></span>  | <span data-ttu-id="9063a-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="9063a-174">Boolean</span></span> |
|<span data-ttu-id="9063a-175">**Valori posibile**</span><span class="sxs-lookup"><span data-stu-id="9063a-175">**Possible values**</span></span>  | <span data-ttu-id="9063a-176">`TRUE` *(activat)*</span><span class="sxs-lookup"><span data-stu-id="9063a-176">`TRUE` *(enabled)*</span></span> <br/> <span data-ttu-id="9063a-177">`FALSE` *(dezactivat)*</span><span class="sxs-lookup"><span data-stu-id="9063a-177">`FALSE` *(disabled)*</span></span>|


<span data-ttu-id="9063a-178">Dacă nu setați această preferință, date de diagnosticare opționale și necesare sunt disponibile utilizatorilor cu un abonament Office 365 (sau Microsoft 365) care sunt conectați cu un cont de la locul de muncă sau de la școală.</span><span class="sxs-lookup"><span data-stu-id="9063a-178">If you don't set this preference, optional connected experiences are available to users with an Office 365 (or Microsoft 365) subscription that are signed in with a work or school account.</span></span> <span data-ttu-id="9063a-179">Cu excepția cazului în care ați setat această preferință la FALS, acești utilizatori pot alege să dezactiveze experiențele conectate opționale accesând **Setări** > **Setări de confidențialitate**.</span><span class="sxs-lookup"><span data-stu-id="9063a-179">Unless you have set this preference to FALSE, these users can choose to turn off optional connected experiences by going to **Settings** > **Privacy Settings**.</span></span>

<span data-ttu-id="9063a-180">Pentru alți utilizatori, cum ar fi utilizatori casnici cu un abonament Office 365 (sau Microsoft 365), nu există o opțiune de a dezactiva experiențele conectate opționale.</span><span class="sxs-lookup"><span data-stu-id="9063a-180">For other users, such as home users with an Office 365 (or Microsoft 365) subscription, there isn't an option to turn off optional connected experiences.</span></span>