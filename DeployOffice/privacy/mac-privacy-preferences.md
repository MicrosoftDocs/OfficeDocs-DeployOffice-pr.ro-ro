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
ms.openlocfilehash: 01bb31f3b6c307ec1dc4762b54fea17185dcf27d
ms.sourcegitcommit: 0fd23324ba1364fa1f8dd1578adf25946adde90f
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/07/2019
ms.locfileid: "36246314"
---
# <a name="use-preferences-to-manage-privacy-controls-for-office-for-mac"></a>Utilizați preferințele pentru a gestiona controalele de confidențialitate ale Office pentru Mac

Începând cu versiunea 16.28 pentru Office pentru Mac, există noi setări de preferințe care vă permit să controlați setările asociate cu:

- ***Date de diagnosticare*** care sunt colectate și trimise la Microsoft despre software-ul client Office utilizat

- ***Experiențe conectate*** care utilizează funcționalitatea în cloud pentru a vă furniza caracteristici îmbunătățite de Office dvs. și utilizatorilor dvs.

În plus, există o nouă setare de preferințe corelată cu o casetă de dialog **Notificare de date necesare** pentru Microsoft actualizare automată (MAU).

Pentru mai multe informații despre datele de diagnosticare și experiențele conectate, consultați [Prezentare generală a controalelor de confidențialitate](overview-privacy-controls.md).

> [!NOTE]
> Pentru mai multe informații despre setări similare pentru Office pe computere care rulează Windows, consultați [Utilizați setările de politică pentru a gestiona controalele de confidențialitate pentru Office 365 ProPlus](manage-privacy-controls.md)

## <a name="setting-preferences"></a>Setarea preferințelor

Aceste noi setări de preferințe sunt CFPreferences API compatibile și pot fi setate utilizând `defaults`comanda din terminal sau impuse printr-un profil de configurare sau un server de gestionare a dispozitivelor mobile (MDM). Atunci când sunt impuse preferințele, utilizatorul nu poate modifica valorile și toate controalele din aplicație vor apărea dezactivate.

## <a name="preference-setting-for-diagnostic-data"></a>Setarea de preferințe pentru datele de diagnosticare 

Datele de diagnosticare sunt utilizate pentru a menține Office securizat și actualizat, pentru a detecta, a diagnostica și a remedia problemele și, de asemenea, pentru a face îmbunătățiri de produs. Pentru mai multe informații, consultați [Datele de diagnosticare trimise din Office 365 ProPlus la Microsoft](overview-privacy-controls.md#diagnostic-data-sent-from-office-365-proplus-to-microsoft).

|||
|:-----|:-----|
|**Domeniu de preferințe**  | `com.microsoft.office` |
|**Tastă**  | `DiagnosticDataTypePreference`  |
|**Tip de date**  | Șir |
|**Valori posibile**  | `BasicDiagnosticData` *(acest lucru setează nivelul la Necesar)* <br/> `FullDiagnosticData` *(acest lucru setează nivelul la Opțional)* <br/> `ZeroDiagnosticData` *(acest lucru setează nivelul la Niciuna)* |
|**Disponibilitate** |16.28 și versiuni mai recente |

> [!NOTE]
> Dacă setați această preferință, se va aplica și pentru următoarele produse:
> - Versiunea 1.00.217856 și versiuni mai recente ale Teams pentru Mac
> - Versiunea 16.28 și versiunile ulterioare Skype for Business pentru Mac

Dacă nu setați această preferință, sunt trimise atât date de diagnostic opționale, cât și necesare către Microsoft, dacă utilizatorii cu un abonament Office 365 sunt conectați cu un cont de la locul de muncă sau de la școală sau dacă utilizatorii au o versiune cu licență în volum de Office 2019 pentru Mac. De asemenea, acești utilizatori nu pot modifica nivelul de date de diagnostic, indiferent de modul în care setați această preferință.

Pentru alți utilizatori, cum ar fi utilizatori casnici cu un abonament Office 365, sunt trimise doar date de diagnosticare necesare, cu excepția cazului în care utilizatorul alege să trimită, de asemenea, date de diagnosticare opționale, accesând **Preferințe** > **Confidențialitate**.

## <a name="preference-setting-for-connected-experiences-that-analyze-your-content"></a>Setarea de preferințe pentru experiențe conectate care analizează conținutul

Experiențele conectate care vă analizează conținutul sunt experiențe care utilizează conținutul Office pentru vă oferi recomandări de proiectare, sugestii de editare, detalii privind datele și alte caracteristici similare. De exemplu, PowerPoint Designer sau Cercetare în Word. Pentru o listă a acestor experiențe conectate, consultați [Experiențe conectate în Office](connected-experiences.md)

|||
|:-----|:-----|
|**Domeniu de preferințe**  | `com.microsoft.office` |
|**Tastă**  | `OfficeExperiencesAnalyzingContentPreference`  |
|**Tip de date**  | Boolean |
|**Valori posibile**  | `TRUE` *(activat)* <br/> `FALSE` *(dezactivat)*|
|**Disponibilitate** |16.28 și versiuni mai recente |

Dacă nu setați această preferință, experiențele conectate care analizează conținut sunt disponibile utilizatorilor. 

Dacă utilizatorul are un abonament Office 365 și este conectat cu un cont de la locul de muncă sau de la școală sau dacă utilizatorul are o versiune cu licență în volum de Office 2019 pentru Mac, atunci utilizatorul nu poate dezactiva experiențele conectate care analizează conținutul.

Pentru alți utilizatori, cum ar fi utilizatori casnici cu un abonament Office 365, utilizatorul poate alege să dezactiveze experiențe conectate care analizează conținutul accesând **Preferințe** > **Confidențialitate**.

## <a name="preference-setting-for-connected-experiences-that-download-online-content"></a>Setarea de preferințe pentru experiențe conectate care descarcă conținut online

Experiențele conectate care descarcă conținut online sunt experiențe care vă permit să căutați și să descărcați conținut online, inclusiv șabloane, imagini, modele 3D, videoclipuri și materiale de referință pentru a vă îmbunătăți documentele. De exemplu, șabloanele Office sau Pornirea rapidă PowerPoint. Pentru o listă a acestor experiențe conectate, consultați [Experiențe conectate în Office](connected-experiences.md)

|||
|:-----|:-----|
|**Domeniu de preferințe**  | `com.microsoft.office` |
|**Tastă**  | `OfficeExperiencesDownloadingContentPreference`  |
|**Tip de date**  | Boolean |
|**Valori posibile**  | `TRUE` *(activat)* <br/> `FALSE` *(dezactivat)*|
|**Disponibilitate** |16.28 și versiuni mai recente |

Dacă nu setați această preferință, experiențele conectate care descarcă conținut online sunt disponibile utilizatorilor.

Dacă utilizatorul are un abonament Office 365 și este conectat cu un cont de la locul de muncă sau de la școală sau dacă utilizatorul are o versiune cu licență în volum de Office 2019 pentru Mac, atunci utilizatorul nu poate dezactiva experiențele conectate care descarcă conținutul online.

Pentru alți utilizatori, cum ar fi utilizatori casnici cu un abonament Office 365, utilizatorul poate alege să dezactiveze experiențe conectate care descarcă conținutul online accesând **Preferințe** > **Confidențialitate**.

## <a name="preference-setting-for-optional-connected-experiences"></a>Setarea preferințelor pentru experiențe conectate opționale

În plus față de experiențele conectate menționate mai sus, există câteva experiențe conectate opționale pe care le puteți alege pentru a le permite utilizatorilor să le acceseze cu contul organizației lor, care este uneori denumit cont de la locul de muncă sau de la școală. De exemplu, caracteristicile LinkedIn ale Asistentului pentru CV în Word sau caracteristica Bară meteo în Outlook, care utilizează Meteo MSN. Pentru mai multe exemple, consultați [Prezentare generală a experiențelor conectate opționale în Office](optional-connected-experiences.md).

|||
|:-----|:-----|
|**Domeniu de preferințe**  | `com.microsoft.office` |
|**Tastă**  | `OptionalConnectedExperiencesPreference`  |
|**Tip de date**  | Boolean |
|**Valori posibile**  | `TRUE` *(activat)* <br/> `FALSE` *(dezactivat)*|
|**Disponibilitate** |16.28 și versiuni mai recente |

Dacă nu setați această preferință, date de diagnostic opționale și necesare sunt disponibile utilizatorilor cu un abonament Office 365 care sunt conectați cu un cont de la locul de muncă sau de la școală sau dacă utilizatorii au o versiune cu licență în volum de Office 2019 pentru Mac. Cu excepția cazului în care ați setat această preferință la,`FALSE` acești utilizatori pot alege să dezactiveze experiențe conectate opționale accesând **Preferințe** > **Confidențialitate**.

Pentru alți utilizatori, cum ar fi utilizatori casnici cu un abonament Office 365, nu există o opțiune de a dezactiva experiențe conectate opționale.

## <a name="preference-setting-for-most-connected-experiences"></a>Setarea preferințelor pentru majoritatea experiențelor conectate

Puteți utiliza această preferință pentru a controla dacă majoritatea experiențelor conectate sunt disponibile pentru utilizatorii dvs.

|||
|:-----|:-----|
|**Domeniu de preferințe**  | `com.microsoft.office` |
|**Tastă**  | `ConnectedOfficeExperiencesPreference`  |
|**Tip de date**  | Boolean |
|**Valori posibile**  | `TRUE` *(activat)* <br/> `FALSE` *(dezactivat)*|
|**Disponibilitate** |16.28 și versiuni mai recente |

Dacă nu setați această preferință, toate experiențele conectate sunt disponibile pentru utilizatorii dvs., cu excepția cazului în care ați stabilit una dintre celelalte preferințe pentru experiențele conectate menționate anterior, cum ar fi `OfficeExperiencesAnalyzingContentPreference`.

De exemplu, dacă setați această preferință la`FALSE`, următoarele tipuri de experiențe conectate nu vor fi disponibile pentru utilizatorii dvs.:
- Experiențe care analizează conținut
- Experiențe care descarcă conținut online
- Experiențe conectate opționale

În plus, dacă setați această preferință la `FALSE`, majoritatea altor experiențe conectate sunt, de asemenea, dezactivate, cum ar fi elaborarea în comun și stocarea online. Pentru lista acestor experiențe conectate, consultați [Experiențe conectate în Office](connected-experiences.md).

Dar chiar dacă setați această preferință la `FALSE`, funcționalitatea Office limitată va rămâne disponibilă, cum ar fi sincronizarea unei cutii poștale în Outlook, Teams și Skype for Business vor continua să funcționeze. [Servicii esențiale](essential-services.md), cum ar fi serviciul de licențiere care confirmă că aveți licență corectă pentru a utiliza Office, vor rămâne, de asemenea, disponibile.

Dacă utilizatorul are un abonament Office 365 și este conectat cu un cont de la locul de muncă sau de la școală sau dacă utilizatorul are o versiune cu licență în volum de Office 2019 pentru Mac, atunci utilizatorul nu poate dezactiva majoritatea experiențelor conectate.

Pentru alți utilizatori, cum ar fi utilizatori casnici cu un abonament Office 365, utilizatorul poate alege să dezactiveze experiențe conectate accesând **Preferințe** > **Confidențialitate**.

## <a name="preference-setting-for-the-required-data-notice-dialog-for-microsoft-autoupdate"></a>Setarea preferințelor pentru caseta de dialog notificare de date necesară pentru Microsoft actualizare automată

Prima dată când este lansată versiunea 4.12 sau o versiune mai recentă de Microsoft actualizare automată (MAU), utilizatorii vor vedea un **Dialog de notificare **a datelor necesare, care le furnizează informații despre care date sunt trimise către Microsoft de către MAU.

Dacă nu doriți ca utilizatorii dvs. să vadă această casetă de **Dialog notificare de date necesară** pentru Microsoft actualizare automată, puteți seta următoarea preferință. Indiferent de valoarea pe care ați setat-o, caseta de dialog nu va fi afișată pentru utilizatorii dvs.

|||
|:-----|:-----|
|**Domeniu de preferințe**  | `com.microsoft.autoupdate2` |
|**Tastă**  | `AcknowledgedDataCollectionPolicy`  |
|**Tip de date**  | Șir |
|**Valori posibile**  | `RequiredDataOnly` <br/> `RequiredAndOptionalData`|
|**Disponibilitate** |4.12 și versiuni mai recente |

Dacă le permiteți utilizatorilor să vadă această casetă de dialog, atunci când utilizatorul alege **OK**, valoarea`RequiredDataOnly` este scrisă în`AcknowledgedDataCollectionPolicy` și caseta de dialog nu este afișată din nou pentru utilizator.


## <a name="related-topics"></a>Subiecte asociate

- [Referință profil de configurare (documentația pentru dezvoltatori Apple)](https://go.microsoft.com/fwlink/p/?linkid=852998)
- [Implementarea preferințelor pentru Office pentru Mac](../mac/deploy-preferences-for-office-for-mac.md)
- [Setările de confidențialitate ale contului](https://support.office.com/article/3e7bc183-bf52-4fd0-8e6b-78978f7f121b#ID0EAADAAA=Mac)
