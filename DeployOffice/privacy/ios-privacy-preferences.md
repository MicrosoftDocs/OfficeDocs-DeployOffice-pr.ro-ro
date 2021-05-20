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
ms.openlocfilehash: 000fd2c5e13ed51abf3afba6e7a1433c9d4b912f
ms.sourcegitcommit: 9b5f18c543c286c95e546e22fc8edb60ef541030
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/20/2021
ms.locfileid: "52578348"
---
# <a name="use-preferences-to-manage-privacy-controls-for-office-on-ios-devices"></a><span data-ttu-id="e664d-103">Utilizați preferințele pentru a gestiona controalele de confidențialitate ale Office pe dispozitivele iOS</span><span class="sxs-lookup"><span data-stu-id="e664d-103">Use preferences to manage privacy controls for Office on iOS devices</span></span>

> [!NOTE]
> <span data-ttu-id="e664d-104">Pentru o listă de produse Office care sunt reglementate prin aceste informații de confidențialitate, consultați [Controale de confidențialitate disponibile pentru produsele Office](products-versions-privacy-controls.md).</span><span class="sxs-lookup"><span data-stu-id="e664d-104">For a list of Office products covered by this privacy information, see [Privacy controls available for Office products](products-versions-privacy-controls.md).</span></span>

<span data-ttu-id="e664d-105">Există noi setări de preferințe pentru Office pe dispozitivele iOS care vă permit să controlați setările asociate cu:</span><span class="sxs-lookup"><span data-stu-id="e664d-105">There are new preference settings for Office on iOS devices that allow you to control settings related to the following:</span></span>

- <span data-ttu-id="e664d-106">***Date de diagnosticare*** care sunt colectate și trimise la Microsoft despre software-ul client Office utilizat</span><span class="sxs-lookup"><span data-stu-id="e664d-106">***Diagnostic data*** that is collected and sent to Microsoft about Office client software being used.</span></span>

- <span data-ttu-id="e664d-107">***Experiențe conectate*** care utilizează funcționalitatea în cloud pentru a vă furniza caracteristici îmbunătățite de Office dvs. și utilizatorilor dvs.</span><span class="sxs-lookup"><span data-stu-id="e664d-107">***Connected experiences*** that use cloud-based functionality to provide enhanced Office features to you and your users.</span></span>

<span data-ttu-id="e664d-108">Pentru mai multe informații despre datele de diagnosticare și experiențele conectate, consultați [Prezentare generală a controalelor de confidențialitate](overview-privacy-controls.md).</span><span class="sxs-lookup"><span data-stu-id="e664d-108">For more information about diagnostic data and connected experiences, see [Overview of privacy controls](overview-privacy-controls.md).</span></span>

> [!NOTE]
> <span data-ttu-id="e664d-109">Pentru mai multe informații despre setări similare pentru Office pe calculatoare care rulează macOS, consultați [Utilizați preferințele pentru a gestiona controalele de confidențialitate pentru Office pentru Mac](mac-privacy-preferences.md).</span><span class="sxs-lookup"><span data-stu-id="e664d-109">For information about similar settings for Office on computers running macOS, see [Use preferences to manage privacy controls for Office for Mac](mac-privacy-preferences.md)</span></span>


## <a name="setting-device-preferences"></a><span data-ttu-id="e664d-110">Setarea preferințelor dispozitivelor</span><span class="sxs-lookup"><span data-stu-id="e664d-110">Setting device preferences</span></span>
<span data-ttu-id="e664d-111">Aceste noi setări de preferințe pot fi, de asemenea, setate la nivel de dispozitiv de către un server de Management a dispozitivelor mobile (MDM) atunci când este instalată aplicația Office.</span><span class="sxs-lookup"><span data-stu-id="e664d-111">These new preference settings can also be set at the device level by a Mobile Device Management (MDM) server when the Office application is installed.</span></span> <span data-ttu-id="e664d-112">Multe servere MDM le permit administratorilor IT să adauge un dicționar de configurare opțional atunci când serverul trimite comanda `InstallApplication` MDM către un dispozitiv iOS.</span><span class="sxs-lookup"><span data-stu-id="e664d-112">Many MDM servers allow IT administrators to add an optional configuration dictionary when the server sends the `InstallApplication` MDM command to an iOS device.</span></span> <span data-ttu-id="e664d-113">Consultați documentația serverului MDM pentru mai multe detalii.</span><span class="sxs-lookup"><span data-stu-id="e664d-113">Refer to your MDM server documentation for more details.</span></span>

<span data-ttu-id="e664d-p102">Dicționarul este reprezentat ca set de perechi de chei/valori în format XML. De exemplu:</span><span class="sxs-lookup"><span data-stu-id="e664d-p102">The dictionary is represented as a set of key/value pairs in XML format. For example:</span></span>

```xml
<dict>
    <key>DiagnosticDataTypePreference</key>
    <string>BasicDiagnosticData</string>
</dict>
```

<span data-ttu-id="e664d-116">Odată trimis către dispozitiv, dicționarul de configurare se va afla sub cheia `com.apple.managed.configuration`, de unde va fi citit atunci când se lansează aplicația Office.</span><span class="sxs-lookup"><span data-stu-id="e664d-116">Once sent to the device, the configuration dictionary will reside under the `com.apple.managed.configuration` key, where it will be read when the Office application is launched.</span></span>

> [!NOTE]
> <span data-ttu-id="e664d-117">De asemenea, puteți utiliza serviciul de politici cloud pentru Office și aceste patru setări de politică:</span><span class="sxs-lookup"><span data-stu-id="e664d-117">You can also use the Office cloud policy service and these 4 policy settings:</span></span>
> - <span data-ttu-id="e664d-118">Configurați nivelul datelor de diagnosticare pentru software-ul client trimise de Office la Microsoft</span><span class="sxs-lookup"><span data-stu-id="e664d-118">Configure the level of client software diagnostic data sent by Office to Microsoft</span></span>
> - <span data-ttu-id="e664d-119">Permiteți utilizarea de experiențe conectate în Office care analizează conținut</span><span class="sxs-lookup"><span data-stu-id="e664d-119">Allow the use of connected experiences in Office that analyze content</span></span>
> - <span data-ttu-id="e664d-120">Permiteți utilizarea de experiențe conectate în Office care descarcă conținut online</span><span class="sxs-lookup"><span data-stu-id="e664d-120">Allow the use of connected experiences in Office that download online content</span></span>
> - <span data-ttu-id="e664d-121">Permiteți utilizarea de experiențe conectate opționale, suplimentare în Office</span><span class="sxs-lookup"><span data-stu-id="e664d-121">Allow the use of additional optional connected experiences in Office</span></span>
>
> <span data-ttu-id="e664d-122">Setările de confidențialitate pentru Outlook pentru iOS și OneDrive pentru iOS pot fi configurate doar utilizând serviciul de politici cloud pentru Office.</span><span class="sxs-lookup"><span data-stu-id="e664d-122">Privacy settings for Outlook for iOS and OneDrive for iOS can only be configured by using the Office cloud policy service.</span></span>
>
> <span data-ttu-id="e664d-123">Pentru mai multe informații despre utilizarea serviciului de politici cloud pentru Office, consultați [Prezentarea generală a serviciului de politici cloud pentru Office](../overview-office-cloud-policy-service.md).</span><span class="sxs-lookup"><span data-stu-id="e664d-123">For more information on using the Office cloud policy service, see [Overview of the Office cloud policy service](../overview-office-cloud-policy-service.md).</span></span>

## <a name="preference-setting-for-diagnostic-data"></a><span data-ttu-id="e664d-124">Setarea de preferințe pentru datele de diagnosticare </span><span class="sxs-lookup"><span data-stu-id="e664d-124">Preference setting for diagnostic data</span></span>

<span data-ttu-id="e664d-125">Datele de diagnosticare sunt utilizate pentru a menține Office securizat și actualizat, pentru a detecta, a diagnostica și a remedia problemele și, de asemenea, pentru a face îmbunătățiri de produs.</span><span class="sxs-lookup"><span data-stu-id="e664d-125">Diagnostic data is used to keep Office secure and up-to-date, detect, diagnose and remediate problems, and also make product improvements.</span></span> <span data-ttu-id="e664d-126">Pentru mai multe informații, consultați [Datele de diagnosticare trimise din Aplicații Microsoft 365 pentru întreprindere la Microsoft](overview-privacy-controls.md#diagnostic-data-sent-from-microsoft-365-apps-for-enterprise-to-microsoft).</span><span class="sxs-lookup"><span data-stu-id="e664d-126">For more information, see [Diagnostic data sent from Microsoft 365 Apps for enterprise to Microsoft](overview-privacy-controls.md#diagnostic-data-sent-from-microsoft-365-apps-for-enterprise-to-microsoft).</span></span>

|<span data-ttu-id="e664d-127">Categorie</span><span class="sxs-lookup"><span data-stu-id="e664d-127">Category</span></span>|<span data-ttu-id="e664d-128">Detalii</span><span class="sxs-lookup"><span data-stu-id="e664d-128">Details</span></span>|
|:-----|:-----|
|<span data-ttu-id="e664d-129">**Cheie**</span><span class="sxs-lookup"><span data-stu-id="e664d-129">**Key**</span></span>  | `DiagnosticDataTypePreference`  |
|<span data-ttu-id="e664d-130">**Tip de date**</span><span class="sxs-lookup"><span data-stu-id="e664d-130">**Data Type**</span></span>  | <span data-ttu-id="e664d-131">Șir</span><span class="sxs-lookup"><span data-stu-id="e664d-131">String</span></span> |
|<span data-ttu-id="e664d-132">**Valori posibile**</span><span class="sxs-lookup"><span data-stu-id="e664d-132">**Possible values**</span></span>  | <span data-ttu-id="e664d-133">`BasicDiagnosticData` *(această valoare setează nivelul la Necesare)*</span><span class="sxs-lookup"><span data-stu-id="e664d-133">`BasicDiagnosticData` *(this value sets the level to Required)*</span></span> <br/> <span data-ttu-id="e664d-134">`FullDiagnosticData` *(această valoare setează nivelul la Opționale)*</span><span class="sxs-lookup"><span data-stu-id="e664d-134">`FullDiagnosticData` *(this value sets the level to Optional)*</span></span> <br/> <span data-ttu-id="e664d-135">`ZeroDiagnosticData` *(această valoare setează nivelul la Niciuna)*</span><span class="sxs-lookup"><span data-stu-id="e664d-135">`ZeroDiagnosticData` *(this value sets the level to Neither)*</span></span> |

<span data-ttu-id="e664d-136">Dacă nu setați această preferință, sunt trimise către Microsoft atât datele de diagnosticare necesare, cât și cele opționale, dacă utilizatorii cu abonament Office 365 (sau Microsoft 365) sunt conectați cu un cont de la locul de muncă sau de la școală.</span><span class="sxs-lookup"><span data-stu-id="e664d-136">If you don't set this preference, both required and optional diagnostic data are sent to Microsoft if users with an Office 365 (or Microsoft 365) subscription are signed in with a work or school account.</span></span> <span data-ttu-id="e664d-137">De asemenea, acești utilizatori nu pot modifica nivelul datelor de diagnosticare, indiferent de modul în care setați această preferință.</span><span class="sxs-lookup"><span data-stu-id="e664d-137">Also, these users can't change the level of diagnostic data regardless of how you set this preference.</span></span>

> [!NOTE]
> <span data-ttu-id="e664d-138">Am actualizat paragraful anterior pentru a clarifica faptul că și datele de diagnosticare opționale sunt trimise către Microsoft dacă nu setați această preferință.</span><span class="sxs-lookup"><span data-stu-id="e664d-138">We've updated the previous paragraph to clarify that optional diagnostic data is also sent to Microsoft if you don't set this preference.</span></span>

<span data-ttu-id="e664d-139">Pentru alți utilizatori, cum ar fi utilizatorii la domiciliu cu abonament Office 365 (sau Microsoft 365), sunt trimise doar date de diagnosticare necesare, cu excepția cazului în care utilizatorul alege să trimită și date de diagnosticare opționale, accesând **Setări** > **Setări de confidențialitate**.</span><span class="sxs-lookup"><span data-stu-id="e664d-139">For other users, such as home users with an Office 365 (or Microsoft 365) subscription, only required diagnostic data is sent, unless the user chooses to also send optional diagnostic data by going to **Settings** > **Privacy Settings**.</span></span>


## <a name="preference-setting-for-connected-experiences-that-analyze-your-content"></a><span data-ttu-id="e664d-140">Setarea de preferințe pentru experiențe conectate care analizează conținutul</span><span class="sxs-lookup"><span data-stu-id="e664d-140">Preference setting for connected experiences that analyze your content</span></span>

<span data-ttu-id="e664d-141">Experiențele conectate care vă analizează conținutul sunt experiențe care utilizează conținutul Office pentru vă oferi recomandări de proiectare, sugestii de editare, detalii privind datele și alte caracteristici similare.</span><span class="sxs-lookup"><span data-stu-id="e664d-141">Connected experiences that analyze your content are experiences that use your Office content to provide you with design recommendations, editing suggestions, data insights, and similar features.</span></span> <span data-ttu-id="e664d-142">De exemplu, Idei de proiectare în PowerPoint.</span><span class="sxs-lookup"><span data-stu-id="e664d-142">For example, Design Ideas in PowerPoint.</span></span> <span data-ttu-id="e664d-143">Pentru o listă a acestor experiențe conectate, consultați [Experiențe conectate în Office](connected-experiences.md)</span><span class="sxs-lookup"><span data-stu-id="e664d-143">For a list of these connected experiences, see [Connected experiences in Office](connected-experiences.md).</span></span>

|<span data-ttu-id="e664d-144">Categorie</span><span class="sxs-lookup"><span data-stu-id="e664d-144">Category</span></span>|<span data-ttu-id="e664d-145">Detalii</span><span class="sxs-lookup"><span data-stu-id="e664d-145">Details</span></span>|
|:-----|:-----|
|<span data-ttu-id="e664d-146">**Cheie**</span><span class="sxs-lookup"><span data-stu-id="e664d-146">**Key**</span></span>  | `OfficeExperiencesAnalyzingContentPreference`  |
|<span data-ttu-id="e664d-147">**Tip de date**</span><span class="sxs-lookup"><span data-stu-id="e664d-147">**Data Type**</span></span>  | <span data-ttu-id="e664d-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="e664d-148">Boolean</span></span> |
|<span data-ttu-id="e664d-149">**Valori posibile**</span><span class="sxs-lookup"><span data-stu-id="e664d-149">**Possible values**</span></span>  | <span data-ttu-id="e664d-150">`TRUE` *(activat)*</span><span class="sxs-lookup"><span data-stu-id="e664d-150">`TRUE` *(enabled)*</span></span> <br/> <span data-ttu-id="e664d-151">`FALSE` *(dezactivat)*</span><span class="sxs-lookup"><span data-stu-id="e664d-151">`FALSE` *(disabled)*</span></span>|


<span data-ttu-id="e664d-152">Dacă nu setați această preferință, experiențele conectate care analizează conținut sunt disponibile utilizatorilor.</span><span class="sxs-lookup"><span data-stu-id="e664d-152">If you don't set this preference, connected experiences that analyze content are available to users.</span></span>

<span data-ttu-id="e664d-153">Dacă utilizatorul are un abonament Office 365 (sau Microsoft 365) și este conectat cu un cont de la locul de muncă, atunci utilizatorul nu poate dezactiva experiențele conectate care analizează conținutul.</span><span class="sxs-lookup"><span data-stu-id="e664d-153">If the user has an Office 365 (or Microsoft 365) subscription and is signed in with a work or school account, then the user can't turn off connected experiences that analyze content.</span></span>

<span data-ttu-id="e664d-154">Pentru alți utilizatori, cum ar fi utilizatori la domiciliu cu un abonament Office 365 (sau Microsoft 365), utilizatorul poate alege să dezactiveze experiențele conectate care analizează conținutul accesând **Setări** > **Setări de confidențialitate**.</span><span class="sxs-lookup"><span data-stu-id="e664d-154">For other users, such as home users with an Office 365 (or Microsoft 365) subscription, the user can choose to turn off connected experiences that analyze content by going to **Settings** > **Privacy Settings**.</span></span>

## <a name="preference-setting-for-connected-experiences-that-download-online-content"></a><span data-ttu-id="e664d-155">Setarea de preferințe pentru experiențe conectate care descarcă conținut online</span><span class="sxs-lookup"><span data-stu-id="e664d-155">Preference setting for connected experiences that download online content</span></span>

<span data-ttu-id="e664d-156">Experiențele conectate care descarcă conținut online sunt experiențe care vă permit să căutați și să descărcați conținut online, inclusiv șabloane, imagini, videoclipuri și materiale de referință pentru a vă îmbunătăți documentele.</span><span class="sxs-lookup"><span data-stu-id="e664d-156">Connected experiences that download online content are experiences that allow you to search and download online content including templates, images, videos, and reference materials to enhance your documents.</span></span> <span data-ttu-id="e664d-157">De exemplu, șabloanele Office sau inserarea unei pictograme online.</span><span class="sxs-lookup"><span data-stu-id="e664d-157">For example, Office templates or inserting an online icon.</span></span> <span data-ttu-id="e664d-158">Pentru o listă a acestor experiențe conectate, consultați [Experiențe conectate în Office](connected-experiences.md)</span><span class="sxs-lookup"><span data-stu-id="e664d-158">For a list of these connected experiences, see [Connected experiences in Office](connected-experiences.md).</span></span>

|<span data-ttu-id="e664d-159">Categorie</span><span class="sxs-lookup"><span data-stu-id="e664d-159">Category</span></span>|<span data-ttu-id="e664d-160">Detalii</span><span class="sxs-lookup"><span data-stu-id="e664d-160">Details</span></span>|
|:-----|:-----|
|<span data-ttu-id="e664d-161">**Cheie**</span><span class="sxs-lookup"><span data-stu-id="e664d-161">**Key**</span></span>  | `OfficeExperiencesDownloadingContentPreference`  |
|<span data-ttu-id="e664d-162">**Tip de date**</span><span class="sxs-lookup"><span data-stu-id="e664d-162">**Data Type**</span></span>  | <span data-ttu-id="e664d-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="e664d-163">Boolean</span></span> |
|<span data-ttu-id="e664d-164">**Valori posibile**</span><span class="sxs-lookup"><span data-stu-id="e664d-164">**Possible values**</span></span>  | <span data-ttu-id="e664d-165">`TRUE` *(activat)*</span><span class="sxs-lookup"><span data-stu-id="e664d-165">`TRUE` *(enabled)*</span></span> <br/> <span data-ttu-id="e664d-166">`FALSE` *(dezactivat)*</span><span class="sxs-lookup"><span data-stu-id="e664d-166">`FALSE` *(disabled)*</span></span>|


<span data-ttu-id="e664d-167">Dacă nu setați această preferință, experiențele conectate care descarcă conținut online sunt disponibile utilizatorilor.</span><span class="sxs-lookup"><span data-stu-id="e664d-167">If you don't set this preference, connected experiences that download online content are available to users.</span></span>

<span data-ttu-id="e664d-168">Dacă utilizatorul are un abonament Office 365 (sau Microsoft 365) și este conectat cu un cont de la locul de muncă, atunci utilizatorul nu poate dezactiva experiențele conectate pentru descărcarea conținutului online.</span><span class="sxs-lookup"><span data-stu-id="e664d-168">If the user has an Office 365 (or Microsoft 365) subscription and is signed in with a work or school account, then the user can't turn off connected experiences that download online content.</span></span>

<span data-ttu-id="e664d-169">Pentru alți utilizatori, cum ar fi utilizatori la domiciliu cu un abonament Office 365 (sau Microsoft 365), utilizatorul poate alege să dezactiveze experiențele conectate pentru descărcarea conținutului online accesând **Setări** > **Setări de confidențialitate**.</span><span class="sxs-lookup"><span data-stu-id="e664d-169">For other users, such as home users with an Office 365 (or Microsoft 365) subscription, the user can choose to turn off connected experiences that download online content by going to **Settings** > **Privacy Settings**.</span></span>

## <a name="preference-setting-for-optional-connected-experiences"></a><span data-ttu-id="e664d-170">Setarea preferințelor pentru experiențe conectate opționale</span><span class="sxs-lookup"><span data-stu-id="e664d-170">Preference setting for optional connected experiences</span></span>

<span data-ttu-id="e664d-171">În plus față de experiențele conectate menționate mai sus, există câteva experiențe conectate opționale pe care le puteți alege pentru a le permite utilizatorilor să le acceseze cu contul organizației lor, care este uneori denumit cont de la locul de muncă sau de la școală.</span><span class="sxs-lookup"><span data-stu-id="e664d-171">In addition to the connected experiences mentioned above, there are some optional connected experiences that you may choose to allow your users to access with their organization account, which is sometimes referred to as a work or school account.</span></span> <span data-ttu-id="e664d-172">De exemplu, programele de completare Office care sunt descărcate prin Magazinul Office pe dispozitivul dvs.</span><span class="sxs-lookup"><span data-stu-id="e664d-172">For example, Office add-ins that are downloaded through the Office Store to your device.</span></span> <span data-ttu-id="e664d-173">Pentru mai multe exemple, consultați [Prezentare generală a experiențelor conectate opționale în Office](optional-connected-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="e664d-173">For more examples, see [Overview of optional connected experiences in Office](optional-connected-experiences.md).</span></span>

|<span data-ttu-id="e664d-174">Categorie</span><span class="sxs-lookup"><span data-stu-id="e664d-174">Category</span></span>|<span data-ttu-id="e664d-175">Detalii</span><span class="sxs-lookup"><span data-stu-id="e664d-175">Details</span></span>|
|:-----|:-----|
|<span data-ttu-id="e664d-176">**Cheie**</span><span class="sxs-lookup"><span data-stu-id="e664d-176">**Key**</span></span>  | `OptionalConnectedExperiencesPreference`  |
|<span data-ttu-id="e664d-177">**Tip de date**</span><span class="sxs-lookup"><span data-stu-id="e664d-177">**Data Type**</span></span>  | <span data-ttu-id="e664d-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="e664d-178">Boolean</span></span> |
|<span data-ttu-id="e664d-179">**Valori posibile**</span><span class="sxs-lookup"><span data-stu-id="e664d-179">**Possible values**</span></span>  | <span data-ttu-id="e664d-180">`TRUE` *(activat)*</span><span class="sxs-lookup"><span data-stu-id="e664d-180">`TRUE` *(enabled)*</span></span> <br/> <span data-ttu-id="e664d-181">`FALSE` *(dezactivat)*</span><span class="sxs-lookup"><span data-stu-id="e664d-181">`FALSE` *(disabled)*</span></span>|


<span data-ttu-id="e664d-182">Dacă nu setați această preferință, date de diagnosticare opționale și necesare sunt disponibile utilizatorilor cu un abonament Office 365 (sau Microsoft 365) care sunt conectați cu un cont de la locul de muncă sau de la școală.</span><span class="sxs-lookup"><span data-stu-id="e664d-182">If you don't set this preference, optional connected experiences are available to users with an Office 365 (or Microsoft 365) subscription that are signed in with a work or school account.</span></span> <span data-ttu-id="e664d-183">Cu excepția cazului în care ați setat această preferință la FALS, acești utilizatori pot alege să dezactiveze experiențele conectate opționale accesând **Setări** > **Setări de confidențialitate**.</span><span class="sxs-lookup"><span data-stu-id="e664d-183">Unless you have set this preference to FALSE, these users can choose to turn off optional connected experiences by going to **Settings** > **Privacy Settings**.</span></span>

<span data-ttu-id="e664d-184">Pentru alți utilizatori, cum ar fi utilizatori casnici cu un abonament Office 365 (sau Microsoft 365), nu există o opțiune de a dezactiva experiențele conectate opționale.</span><span class="sxs-lookup"><span data-stu-id="e664d-184">For other users, such as home users with an Office 365 (or Microsoft 365) subscription, there isn't an option to turn off optional connected experiences.</span></span>