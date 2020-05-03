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
ms.openlocfilehash: 40fc1ec1f5b2abc587e1b5224dc7fe0a5a656f33
ms.sourcegitcommit: 3890a23390edd0b5fdb2cf33613ec0778566cf97
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/01/2020
ms.locfileid: "43992118"
---
# <a name="use-preferences-to-manage-privacy-controls-for-office-on-ios-devices"></a>Utilizați preferințele pentru a gestiona controalele de confidențialitate ale Office pe dispozitivele iOS

Există noi setări de preferințe pentru Office pe dispozitivele iOS care vă permit să controlați setările asociate cu:

- ***Date de diagnosticare*** care sunt colectate și trimise la Microsoft despre software-ul client Office utilizat

- ***Experiențe conectate*** care utilizează funcționalitatea în cloud pentru a vă furniza caracteristici îmbunătățite de Office dvs. și utilizatorilor dvs.

Pentru mai multe informații despre datele de diagnosticare și experiențele conectate, consultați [Prezentare generală a controalelor de confidențialitate](overview-privacy-controls.md).

Aceste setări de preferințe se aplică la următoarele aplicații:
- Versiunea 2.30 și versiunile ulterioare de Word pentru iOS, Excel pentru iOS și PowerPoint pentru iOS.
- Versiunea 16.30 și versiunile ulterioare de OneNote pentru iOS.
- Versiunea 1.17 și versiunile ulterioare de Visio Viewer pentru iOS.

> [!NOTE]
> Pentru mai multe informații despre setări similare pentru Office pe calculatoare care rulează macOS, consultați [Utilizați preferințele pentru a gestiona controalele de confidențialitate pentru Office pentru Mac](mac-privacy-preferences.md).


## <a name="setting-device-preferences"></a>Setarea preferințelor dispozitivelor
Aceste noi setări de preferințe pot fi, de asemenea, setate la nivel de dispozitiv de către un server de Management a dispozitivelor mobile (MDM) atunci când este instalată aplicația Office. Multe servere MDM le permit administratorilor IT să adauge un dicționar de configurare opțional atunci când serverul trimite comanda `InstallApplication` MDM către un dispozitiv iOS. Consultați documentația serverului MDM pentru mai multe detalii.

Dicționarul este reprezentat ca un set de perechi de chei/valori în format XML. De exemplu:

```xml
<dict>
    <key>DiagnosticDataTypePreference</key>
    <string>BasicDiagnosticData</string>
</dict>
```

Odată trimis către dispozitiv, dicționarul de configurare se va afla sub cheia `com.apple.managed.configuration`, de unde va fi citit atunci când se lansează aplicația Office.

> [!NOTE]
> De asemenea, puteți utiliza serviciul de politici cloud pentru Office și aceste patru setări de politică:
> - Configurați nivelul datelor de diagnosticare pentru software-ul client trimise de Office la Microsoft
> - Permiteți utilizarea de experiențe conectate în Office care analizează conținut
> - Permiteți utilizarea de experiențe conectate în Office care descarcă conținut online
> - Permiteți utilizarea de experiențe conectate opționale, suplimentare în Office
>
> Pentru mai multe informații despre utilizarea serviciului de politici cloud pentru Office, consultați [Prezentarea generală a serviciului de politici cloud pentru Office](../overview-office-cloud-policy-service.md).

## <a name="preference-setting-for-diagnostic-data"></a>Setarea de preferințe pentru datele de diagnosticare 

Datele de diagnosticare sunt utilizate pentru a menține Office securizat și actualizat, pentru a detecta, a diagnostica și a remedia problemele și, de asemenea, pentru a face îmbunătățiri de produs. Pentru mai multe informații, consultați [Datele de diagnosticare trimise din Aplicații Microsoft 365 pentru întreprindere la Microsoft](overview-privacy-controls.md#diagnostic-data-sent-from-microsoft-365-apps-for-enterprise-to-microsoft).

|||
|:-----|:-----|
|**Cheie**  | `DiagnosticDataTypePreference`  |
|**Tip de date**  | Șir |
|**Valori posibile**  | `BasicDiagnosticData` *(setează nivelul la Necesare)* <br/> `FullDiagnosticData` *(setează nivelul la Opționale)* <br/> `ZeroDiagnosticData` *(setează nivelul la Niciuna)* |

Dacă nu setați această preferință, sunt trimise doar datele de diagnosticare necesare către Microsoft, dacă utilizatorii cu abonament Office 365 (sau Microsoft 365) sunt conectați cu un cont de la locul de muncă sau de la școală. De asemenea, acești utilizatori nu pot modifica nivelul de date de diagnosticare, indiferent de modul în care setați această preferință.

Pentru alți utilizatori, cum ar fi utilizatorii la domiciliu cu abonament Office 365 (sau Microsoft 365), sunt trimise doar date de diagnosticare necesare, cu excepția cazului în care utilizatorul alege să trimită și date de diagnosticare opționale, accesând **Setări** > **Setări de confidențialitate**.


## <a name="preference-setting-for-connected-experiences-that-analyze-your-content"></a>Setarea de preferințe pentru experiențe conectate care analizează conținutul

Experiențele conectate care vă analizează conținutul sunt experiențe care utilizează conținutul Office pentru vă oferi recomandări de proiectare, sugestii de editare, detalii privind datele și alte caracteristici similare. De exemplu, Idei de proiectare în PowerPoint. Pentru o listă a acestor experiențe conectate, consultați [Experiențe conectate în Office](connected-experiences.md)

|||
|:-----|:-----|
|**Cheie**  | `OfficeExperiencesAnalyzingContentPreference`  |
|**Tip de date**  | Boolean |
|**Valori posibile**  | `TRUE` *(activat)* <br/> `FALSE` *(dezactivat)*|


Dacă nu setați această preferință, experiențele conectate care analizează conținut sunt disponibile utilizatorilor.

Dacă utilizatorul are un abonament Office 365 (sau Microsoft 365) și este conectat cu un cont de la locul de muncă, atunci utilizatorul nu poate dezactiva experiențele conectate care analizează conținutul.

Pentru alți utilizatori, cum ar fi utilizatori la domiciliu cu un abonament Office 365 (sau Microsoft 365), utilizatorul poate alege să dezactiveze experiențele conectate care analizează conținutul accesând **Setări** > **Setări de confidențialitate**.

## <a name="preference-setting-for-connected-experiences-that-download-online-content"></a>Setarea de preferințe pentru experiențe conectate care descarcă conținut online

Experiențele conectate care descarcă conținut online sunt experiențe care vă permit să căutați și să descărcați conținut online, inclusiv șabloane, imagini, videoclipuri și materiale de referință pentru a vă îmbunătăți documentele. De exemplu, șabloanele Office sau inserarea unei pictograme online. Pentru o listă a acestor experiențe conectate, consultați [Experiențe conectate în Office](connected-experiences.md)

|||
|:-----|:-----|
|**Cheie**  | `OfficeExperiencesDownloadingContentPreference`  |
|**Tip de date**  | Boolean |
|**Valori posibile**  | `TRUE` *(activat)* <br/> `FALSE` *(dezactivat)*|


Dacă nu setați această preferință, experiențele conectate care descarcă conținut online sunt disponibile utilizatorilor.

Dacă utilizatorul are un abonament Office 365 (sau Microsoft 365) și este conectat cu un cont de la locul de muncă, atunci utilizatorul nu poate dezactiva experiențele conectate pentru descărcarea conținutului online.

Pentru alți utilizatori, cum ar fi utilizatori la domiciliu cu un abonament Office 365 (sau Microsoft 365), utilizatorul poate alege să dezactiveze experiențele conectate pentru descărcarea conținutului online accesând **Setări** > **Setări de confidențialitate**.

## <a name="preference-setting-for-optional-connected-experiences"></a>Setarea preferințelor pentru experiențe conectate opționale

În plus față de experiențele conectate menționate mai sus, există câteva experiențe conectate opționale pe care le puteți alege pentru a le permite utilizatorilor să le acceseze cu contul organizației lor, care este uneori denumit cont de la locul de muncă sau de la școală. De exemplu, programele de completare Office care sunt descărcate prin Magazinul Office pe dispozitivul dvs. Pentru mai multe exemple, consultați [Prezentare generală a experiențelor conectate opționale în Office](optional-connected-experiences.md).

|||
|:-----|:-----|
|**Cheie**  | `OptionalConnectedExperiencesPreference`  |
|**Tip de date**  | Boolean |
|**Valori posibile**  | `TRUE` *(activat)* <br/> `FALSE` *(dezactivat)*|


Dacă nu setați această preferință, date de diagnosticare opționale și necesare sunt disponibile utilizatorilor cu un abonament Office 365 (sau Microsoft 365) care sunt conectați cu un cont de la locul de muncă sau de la școală. Cu excepția cazului în care ați setat această preferință la FALS, acești utilizatori pot alege să dezactiveze experiențele conectate opționale accesând **Setări** > **Setări de confidențialitate**.

Pentru alți utilizatori, cum ar fi utilizatori casnici cu un abonament Office 365 (sau Microsoft 365), nu există o opțiune de a dezactiva experiențele conectate opționale.