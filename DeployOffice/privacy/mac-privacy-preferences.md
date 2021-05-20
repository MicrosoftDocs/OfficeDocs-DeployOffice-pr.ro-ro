---
title: Utilizați preferințele pentru a gestiona controalele de confidențialitate ale Office pentru Mac
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
description: Oferă informații administratorilor Office despre gestionarea controalelor de confidențialitate în Office pentru Mac.
hideEdit: true
ms.openlocfilehash: b7beda7409cff00d54f36851eb21e4d66a8cacce
ms.sourcegitcommit: 9b5f18c543c286c95e546e22fc8edb60ef541030
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/20/2021
ms.locfileid: "52578384"
---
# <a name="use-preferences-to-manage-privacy-controls-for-office-for-mac"></a>Utilizați preferințele pentru a gestiona controalele de confidențialitate ale Office pentru Mac

> [!NOTE]
> Pentru o listă de produse Office care sunt reglementate de aceste informații despre confidențialitate, consultați [Controale de confidențialitate disponibile pentru produsele Office](products-versions-privacy-controls.md).

Începând cu versiunea 16.28 pentru Office pentru Mac, există noi setări de preferințe care vă permit să controlați setările asociate cu:

- ***Date de diagnosticare*** care sunt colectate și trimise la Microsoft despre software-ul client Office utilizat

- ***Experiențe conectate*** care utilizează funcționalitatea în cloud pentru a vă furniza caracteristici îmbunătățite de Office dvs. și utilizatorilor dvs.

În plus, există o nouă setare de preferințe corelată cu o casetă de dialog **Notificare de date necesare** pentru Microsoft AutoUpdate (MAU).

Pentru mai multe informații despre datele de diagnosticare și experiențele conectate, consultați [Prezentare generală a controalelor de confidențialitate](overview-privacy-controls.md).

> [!NOTE]
> - Pentru mai multe informații despre setări similare pentru Office pe computere care rulează Windows, consultați [Utilizați setările de politică pentru a gestiona controale de confidențialitate pentru Aplicații Microsoft 365 pentru întreprindere](manage-privacy-controls.md).
> - Pentru mai multe informații despre setări similare pentru Office pe dispozitive iOS, consultați [Utilizați preferințele pentru a gestiona controalele de confidențialitate pentru Office pe dispozitivele iOS](ios-privacy-preferences.md).

## <a name="setting-preferences"></a>Setarea preferințelor

Aceste noi setări de preferințe sunt compatibile cu API-ul CFPreferences și pot fi setate utilizând comanda `defaults` în terminal sau impuse printr-un profil de configurare sau un server de management al dispozitivelor mobile (MDM). Atunci când sunt impuse preferințele, utilizatorul nu poate modifica valorile și toate controalele din aplicație vor apărea dezactivate.

> [!NOTE]
> De asemenea, puteți utiliza serviciul de politici cloud pentru Office și aceste cinci setări de politică:
> - Configurați nivelul datelor de diagnosticare pentru software-ul client trimise de Office la Microsoft
> - Permiteți utilizarea de experiențe conectate în Office care analizează conținut
> - Permiteți utilizarea de experiențe conectate în Office care descarcă conținut online
> - Permiteți utilizarea de experiențe conectate opționale, suplimentare în Office
> - Permiteți utilizarea de experiențe conectate în Office
>
> Pentru mai multe informații despre utilizarea serviciului de politici cloud pentru Office, consultați [Prezentarea generală a serviciului de politici cloud pentru Office](../overview-office-cloud-policy-service.md).


## <a name="preference-setting-for-diagnostic-data"></a>Setarea de preferințe pentru datele de diagnosticare 

Datele de diagnosticare sunt utilizate pentru a menține Office securizat și actualizat, pentru a detecta, a diagnostica și a remedia problemele și, de asemenea, pentru a face îmbunătățiri de produs. Pentru mai multe informații, consultați [Datele de diagnosticare trimise din Aplicații Microsoft 365 pentru întreprindere la Microsoft](overview-privacy-controls.md#diagnostic-data-sent-from-microsoft-365-apps-for-enterprise-to-microsoft).

|Categorie|Detalii|
|:-----|:-----|
|**Domeniu de preferințe**  | `com.microsoft.office` |
|**Cheie**  | `DiagnosticDataTypePreference`  |
|**Tip de date**  | Șir |
|**Valori posibile**  | `BasicDiagnosticData` *(această valoare setează nivelul la Necesare)* <br/> `FullDiagnosticData` *(această valoare setează nivelul la Opționale)* <br/> `ZeroDiagnosticData` *(această valoare setează nivelul la Niciuna)* |
|**Disponibilitate** |16.28 și versiuni mai recente |

Dacă nu setați această preferință, sunt trimise către Microsoft atât datele de diagnostic necesare, cât și cele opționale, dacă utilizatorii cu abonament Office 365 (sau Microsoft 365) sunt conectați cu un cont de la locul de muncă sau de la școală sau dacă au o versiune de Office 2019 pentru Mac cu licență de volum. De asemenea, acești utilizatori nu pot modifica nivelul datelor de diagnosticare, indiferent de modul în care setați această preferință.

> [!NOTE]
> Am actualizat paragraful anterior pentru a clarifica faptul că și datele de diagnosticare opționale sunt trimise către Microsoft dacă nu setați această preferință.

Pentru alți utilizatori, cum ar fi utilizatorii la domiciliu cu abonament Office 365 (sau Microsoft 365), sunt trimise doar date de diagnosticare necesare, cu excepția cazului în care utilizatorul alege să trimită și date de diagnosticare opționale, accesând **Preferințe** > **Confidențialitate**.

## <a name="preference-setting-for-connected-experiences-that-analyze-your-content"></a>Setarea de preferințe pentru experiențe conectate care analizează conținutul

Experiențele conectate care vă analizează conținutul sunt experiențe care utilizează conținutul Office pentru vă oferi recomandări de proiectare, sugestii de editare, detalii privind datele și alte caracteristici similare. De exemplu, PowerPoint Designer sau Cercetare în Word. Pentru o listă a acestor experiențe conectate, consultați [Experiențe conectate în Office](connected-experiences.md)

|Categorie|Detalii|
|:-----|:-----|
|**Domeniu de preferințe**  | `com.microsoft.office` |
|**Cheie**  | `OfficeExperiencesAnalyzingContentPreference`  |
|**Tip de date**  | Boolean |
|**Valori posibile**  | `TRUE` *(activat)* <br/> `FALSE` *(dezactivat)*|
|**Disponibilitate** |16.28 și versiuni mai recente |

Dacă nu setați această preferință, experiențele conectate care analizează conținut sunt disponibile utilizatorilor. 

Dacă utilizatorul are un abonament Office 365 (sau Microsoft 365) și este conectat cu un cont de la locul de muncă sau de la școală sau dacă utilizatorul are o versiune cu licență de volum de Office 2019 pentru Mac, atunci utilizatorul nu poate dezactiva experiențele conectate care analizează conținutul.

Pentru alți utilizatori, cum ar fi utilizatori la domiciliu cu un abonament Office 365 (sau Microsoft 365), utilizatorul poate alege să dezactiveze experiențele conectate care analizează conținutul accesând **Preferințe** > **Confidențialitate**.

## <a name="preference-setting-for-connected-experiences-that-download-online-content"></a>Setarea de preferințe pentru experiențe conectate care descarcă conținut online

Experiențele conectate care descarcă conținut online sunt experiențe care vă permit să căutați și să descărcați conținut online, inclusiv șabloane, imagini, modele 3D, videoclipuri și materiale de referință pentru a vă îmbunătăți documentele. De exemplu, șabloanele Office sau Pornirea rapidă PowerPoint. Pentru o listă a acestor experiențe conectate, consultați [Experiențe conectate în Office](connected-experiences.md)

|Categorie|Detalii|
|:-----|:-----|
|**Domeniu de preferințe**  | `com.microsoft.office` |
|**Cheie**  | `OfficeExperiencesDownloadingContentPreference`  |
|**Tip de date**  | Boolean |
|**Valori posibile**  | `TRUE` *(activat)* <br/> `FALSE` *(dezactivat)*|
|**Disponibilitate** |16.28 și versiuni mai recente |

Dacă nu setați această preferință, experiențele conectate care descarcă conținut online sunt disponibile utilizatorilor.

Dacă utilizatorul are un abonament Office 365 (sau Microsoft 365) și este conectat cu un cont de la locul de muncă sau de la școală sau dacă utilizatorul are o versiune cu licență de volum de Office 2019 pentru Mac, atunci utilizatorul nu poate dezactiva experiențele conectate pentru descărcarea conținutului online.

Pentru alți utilizatori, cum ar fi utilizatori casnici cu un abonament Office 365 (sau Microsoft 365), un utilizator poate alege să dezactiveze experiențe conectate pentru descărcarea conținutului online accesând **Preferințe** > **Confidențialitate**.

## <a name="preference-setting-for-optional-connected-experiences"></a>Setarea preferințelor pentru experiențe conectate opționale

În plus față de experiențele conectate menționate mai sus, există câteva experiențe conectate opționale pe care le puteți alege pentru a le permite utilizatorilor să le acceseze cu contul organizației lor, care este uneori denumit cont de la locul de muncă sau de la școală. De exemplu, caracteristicile LinkedIn ale Asistentului pentru CV în Word sau caracteristica Bară meteo în Outlook, care utilizează Meteo MSN. Pentru mai multe exemple, consultați [Prezentare generală a experiențelor conectate opționale în Office](optional-connected-experiences.md).

|Categorie|Detalii|
|:-----|:-----|
|**Domeniu de preferințe**  | `com.microsoft.office` |
|**Cheie**  | `OptionalConnectedExperiencesPreference`  |
|**Tip de date**  | Boolean |
|**Valori posibile**  | `TRUE` *(activat)* <br/> `FALSE` *(dezactivat)*|
|**Disponibilitate** |16.28 și versiuni mai recente |

Dacă nu setați această preferință, date de diagnosticare opționale și necesare sunt disponibile utilizatorilor cu un abonament Office 365 (sau Microsoft 365) care sunt conectați cu un cont de la locul de muncă sau de la școală sau dacă utilizatorii au o versiune cu licență de volum de Office 2019 pentru Mac. Cu excepția cazului în care ați setat această preferință la `FALSE`, acești utilizatori pot alege să dezactiveze experiențele conectate opționale accesând **Preferințe** > **Confidențialitate**.

Pentru alți utilizatori, cum ar fi utilizatori casnici cu un abonament Office 365 (sau Microsoft 365), nu există o opțiune de a dezactiva experiențele conectate opționale.

## <a name="preference-setting-for-most-connected-experiences"></a>Setarea preferințelor pentru majoritatea experiențelor conectate

Puteți utiliza această preferință pentru a controla dacă majoritatea experiențelor conectate sunt disponibile pentru utilizatorii dvs.

|Categorie|Detalii|
|:-----|:-----|
|**Domeniu de preferințe**  | `com.microsoft.office` |
|**Cheie**  | `ConnectedOfficeExperiencesPreference`  |
|**Tip de date**  | Boolean |
|**Valori posibile**  | `TRUE` *(activat)* <br/> `FALSE` *(dezactivat)*|
|**Disponibilitate** |16.28 și versiuni mai recente |

Dacă nu setați această preferință, toate experiențele conectate sunt disponibile pentru utilizatorii dvs., cu excepția cazului în care ați stabilit una dintre celelalte preferințe pentru experiențele conectate menționate anterior, cum ar fi `OfficeExperiencesAnalyzingContentPreference`.

De exemplu, dacă setați această preferință la `FALSE`, următoarele tipuri de experiențe conectate nu vor fi disponibile pentru utilizatorii dvs.:
- Experiențe care analizează conținut
- Experiențe care descarcă conținut online
- Experiențe conectate opționale

În plus, dacă setați această preferință la `FALSE`, majoritatea altor experiențe conectate sunt, de asemenea, dezactivate, cum ar fi elaborarea în comun și stocarea online. Pentru lista acestor experiențe conectate, consultați [Experiențe conectate în Office](connected-experiences.md).

Dar chiar dacă setați această preferință la `FALSE`, funcționalitățile Office limitate vor rămâne disponibile, cum ar fi sincronizarea unei cutii poștale în Outlook, Teams și Skype for Business vor continua să funcționeze. [Servicii esențiale](essential-services.md), cum ar fi serviciul de licențiere care confirmă că aveți licență corectă pentru a utiliza Office, vor rămâne, de asemenea, disponibile.

Dacă utilizatorul are un abonament Office 365 (sau Microsoft 365) și este conectat cu un cont de la locul de muncă sau de la școală sau dacă utilizatorul are o versiune cu licență de volum de Office 2019 pentru Mac, atunci utilizatorul nu poate dezactiva majoritatea experiențelor conectate.

Pentru alți utilizatori, cum ar fi utilizatori casnici cu un abonament Office 365 (sau Microsoft 365), un utilizator poate alege să dezactiveze majoritatea experiențelor conectate accesând **Preferințe** > **Confidențialitate**.

## <a name="preference-setting-for-the-required-data-notice-dialog-for-microsoft-autoupdate"></a>Setarea preferințelor pentru caseta de dialog notificare de date necesară pentru Microsoft AutoUpdate

Prima dată când este lansată versiunea 4.12 sau o versiune mai recentă de Microsoft AutoUpdate (MAU), utilizatorii vor vedea un dialog **Notificare despre datele necesare**, care le furnizează informații referitoare la ce date din MAU sunt trimise către Microsoft.

Dacă nu doriți ca utilizatorii dvs. să vadă această casetă de dialog **Notificare despre datele necesare** pentru Microsoft AutoUpdate, puteți seta următoarea preferință. Indiferent de valoarea pe care ați setat-o, caseta de dialog nu va fi afișată pentru utilizatorii dvs.

|Categorie|Detalii|
|:-----|:-----|
|**Domeniu de preferințe**  | `com.microsoft.autoupdate2` |
|**Cheie**  | `AcknowledgedDataCollectionPolicy`  |
|**Tip de date**  | Șir |
|**Valori posibile**  | `RequiredDataOnly` <br/> `RequiredAndOptionalData`|
|**Disponibilitate** |4.12 și versiuni mai recente |

Dacă le permiteți utilizatorilor să vadă această casetă de dialog, atunci când utilizatorul alege **OK**, valoarea `RequiredDataOnly` este scrisă în`AcknowledgedDataCollectionPolicy` și caseta de dialog nu este afișată din nou pentru utilizator.


## <a name="related-articles"></a>Articole asociate

- [Referință privind profilul de configurare (documentația pentru dezvoltatori Apple)](https://go.microsoft.com/fwlink/p/?linkid=852998)
- [Implementarea preferințelor pentru Office pentru Mac](../mac/deploy-preferences-for-office-for-mac.md)
- [Setările de confidențialitate ale contului](https://support.office.com/article/3e7bc183-bf52-4fd0-8e6b-78978f7f121b#ID0EAADAAA=Mac)
