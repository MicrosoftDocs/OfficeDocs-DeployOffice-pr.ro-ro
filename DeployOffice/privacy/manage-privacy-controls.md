---
title: Utilizați setările de politică pentru a gestiona controale de confidențialitate pentru Office 365 ProPlus
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.audience: ITPro
ms.topic: article
ms.service: o365-proplus-itpro
localization_priority: Priority
ms.collection:
- Ent_O365
- M365-modern-desktop
ms.custom:
- Ent_Office_ProPlus
- Ent_Office_Privacy
description: Administratorii Office oferă informații despre gestionarea controalelor de confidențialitate în Office 365 ProPlus, utilizând setările de politică.
hideEdit: true
ms.openlocfilehash: 069b21632044354afded61ccc9b1d099cd9cda98
ms.sourcegitcommit: 8dd9721bd618ae6e4d27f2c45c5dc8e3219858ac
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/20/2019
ms.locfileid: "34250395"
---
# <a name="use-policy-settings-to-manage-privacy-controls-for-office-365-proplus"></a>Utilizați setările de politică pentru a gestiona controale de confidențialitate pentru Office 365 ProPlus

Microsoft se angajează să vă furnizeze informațiile și controalele de care aveți nevoie pentru a face alegeri privind modul de colectare și de utilizare a datelor dvs. atunci când utilizați Office 365 ProPlus.

Începând cu versiunea 1904 pentru Office 365 ProPlus, există noi setări de politică care vă permit să controlați setările asociate cu:

- ***Date de diagnosticare*** care sunt colectate și trimise la Microsoft despre software-ul client Office utilizat

- ***Experiențe conectate*** care utilizează funcționalitatea în cloud pentru a vă furniza caracteristici îmbunătățite de Office dvs. și utilizatorilor dvs.

Iată cele cinci noi setări de politică:

- Configurați nivelul datelor de diagnosticare pentru software-ul client trimise de Office la Microsoft
- Permiteți utilizarea de experiențe conectate în Office care analizează conținut
- Permiteți utilizarea de experiențe conectate în Office care descarcă conținut online
- Permiteți utilizarea de experiențe conectate opționale, suplimentare în Office
- Permiteți utilizarea de experiențe conectate în Office

Aceste setări de politică pot fi implementate utilizând fie Politica de grup, fie [Serviciul de politică pentru cloud Office](https://docs.microsoft.com/DeployOffice/overview-office-client-policy-service). Dacă utilizați Politica de grup, trebuie să descărcați cea mai recentă versiune a fișierelor Șablon administrativ (ADMX/ADML) de la [Centrul de descărcare Microsoft](https://www.microsoft.com/download/details.aspx?id=49030).

Dacă utilizați instrumentul de Gestionare a politicilor de grup, toate aceste setări de politică se află în Configurație utilizator\\Politici\\Șabloane administrative\\Microsoft Office 2016\\Confidențialitate\\Centrul de autorizare.

Aceste noi setări de politică se aplică și la versiunile desktop de Project și Visio care sunt oferite cu anumite planuri de abonament, cum ar fi planul Project Online Professional sau Visio Online Plan 2. Se aplică și la Office 365 Business.

În plus, există unele setări de politică care nu se vor mai aplica la Office 365 ProPlus și există unele modificări la nivelul interfeței utilizator (UI) privind setările de confidențialitate de care trebuie să țineți cont întrucât utilizatorii dvs. ar putea să observe respectivele modificări și să pună întrebări în legătură cu ele.

Cât despre noile setări de politică, trebuie să le testați cu atenție le într-un mediu limitat, controlat pentru a vă asigura că setările pe care le configurați au efectul dorit înainte să implementați setările de politică pe scară largă în organizația dvs.

## <a name="policy-setting-for-diagnostic-data"></a>Setarea de politică pentru datele de diagnosticare 

Datele de diagnosticare sunt utilizate pentru a menține Office securizat și actualizat, pentru a detecta, a diagnostica și a remedia problemele și, de asemenea, pentru a face îmbunătățiri de produs.

Puteți utiliza setarea de politică *Configurați nivelul datelor de diagnosticare pentru software-ul client trimise de Office la Microsoft* pentru a alege ce nivel al datelor de diagnosticare să fie trimis la Microsoft.

Dacă activați această setare de politică, trebuie să alegeți ce nivel al datelor de diagnosticare să fie trimis la Microsoft. Opțiunile dvs. sunt Obligatoriu, Opțional sau Fără.

- Dacă alegeți ***Obligatoriu***, la Microsoft sunt trimise datele minime necesare pentru a păstra Office securizat, actualizat și într-o stare de funcționare conform așteptărilor pe dispozitivul pe care este instalat.

- Dacă alegeți ***Opțional***, la Microsoft sunt trimise date suplimentare care ne ajută să îmbunătățim produsele și furnizează mai multe informații care ne permit să detectăm, să diagnosticăm și să remediem problemele. Dacă alegeți să trimiteți date de diagnosticare opționale, vor fi incluse și datele de diagnosticare obligatorii.

- Dacă alegeți ***Fără***, la Microsoft nu sunt trimise date de diagnosticare despre software-ul client Office care rulează pe dispozitivul utilizatorului. Însă această opțiune, limitează semnificativ capacitatea Microsoft de a detecta, a diagnostica și a remedia problemele pe care utilizatorii dvs. le pot întâmpina când utilizează Office.

Dacă dezactivați sau nu configurați această setare de politică, atât datele de diagnosticare opționale, cât și cele obligatorii sunt trimise la Microsoft.

Pentru mai multe informații despre datele de diagnosticare, consultați linkul următor:

- [Prezentare generală a controalelor de confidențialitate pentru Office 365 ProPlus](overview-privacy-controls.md)
- [Date de diagnosticare obligatorii pentru Office](required-diagnostic-data.md)
- [Date de diagnosticare opționale pentru Office](optional-diagnostic-data.md)
- [Utilizarea Vizualizatorului de date de diagnosticare cu Office](https://support.office.com/article/cf761ce9-d805-4c60-a339-4e07f3182855)

## <a name="policy-settings-for-connected-experiences"></a>Setările de politică pentru experiențe conectate

Office 365 ProPlus constă din aplicații software client și experiențe conectate proiectate pentru a vă permite să creați, să comunicați și să colaborați mai eficient. Lucrul cu alte persoane într-un document stocat pe OneDrive pentru business sau traducerea conținutului unui document Word într-o altă limbă sunt exemple de experiențe conectate.

Înțelegem că ați dori să alegeți tipurile de experiențe conectate disponibile utilizatorilor dvs. atunci când aceștia lucrează în aplicațiile Office. Prin urmare, vă prezentăm patru noi setări de politică:

- Permiteți utilizarea de experiențe conectate în Office care analizează conținut
- Permiteți utilizarea de experiențe conectate în Office care descarcă conținut online
- Permiteți utilizarea de experiențe conectate opționale, suplimentare în Office
- Permiteți utilizarea de experiențe conectate în Office

Dacă nu utilizați aceste setări de politică, toate experiențele conectate vor fi disponibile. Acest lucru le oferă utilizatorilor dvs. toate caracteristicile și funcționalitățile accesibile prin Office 365 ProPlus. Dar înțelegem că va trebui, probabil, să dezactivați unele experiențe conectate sau chiar pe toate pentru a satisface anumite cerințe ale organizației dvs.

> [!IMPORTANT]
> În prezent, există o problemă legată de aceste 4 setări de politică pe care ne străduim să le corectăm. Momentan, pentru a dezactiva una dintre aceste setări de politică utilizând instrumentul de Gestionare a politicilor de grup, trebuie să selectați butonul radio **Activat**, apoi să alegeți **Dezactivat** din lista verticală din secțiunea **Opțiuni**. Selectarea butonului radio **Dezactivat** nu va dezactiva aceste setări de politică.

Dacă alegeți să nu le oferiți utilizatorilor dvs. unele tipuri de experiențe conectate, panglica sau comanda meniului pentru acele experiențe conectate se va estompa sau utilizatorii vor primi un mesaj de eroare atunci când încearcă să utilizeze aceste experiențe conectate. În acest caz, la Microsoft nu vor fi trimise [datele de serviciu obligatorii](required-service-data.md) pentru acele experiențe conectate.

Utilizatorii dvs. nu vor putea să aleagă dacă să activeze sau să dezactiveze aceste experiențe conectate incluse în Office 365 ProPlus dacă sunt conectați la Office cu acreditările organizației, la care se face uneori referire ca la contul de la locul de muncă sau de la școală.

### <a name="policy-setting-for-connected-experiences-that-analyze-your-content"></a>Setarea de politică pentru experiențe conectate care analizează conținut

Acestea sunt experiențe care utilizează conținutul dvs. Office pentru a vă oferi recomandări de proiectare, sugestii de editare, detalii privind datele și caracteristici similare. De exemplu, PowerPoint Designer sau Editor în Word. Pentru o listă a acestor experiențe conectate, consultați [Experiențe conectate în Office](connected-experiences.md)

Puteți utiliza setarea de politică *Permiteți utilizarea de experiențe conectate în Office care analizează conținut* pentru a controla dacă aceste tipuri de experiențe conectate sunt disponibile pentru utilizatorii dvs. Dacă nu configurați această setare de politică, aceste experiențe conectate vor fi disponibile pentru utilizatorii dvs.

Rețineți că dacă dezactivați setarea de politică *Permiteți utilizarea de experiențe conectate în Office*, experiențele conectate care analizează conținut nu vor fi disponibile pentru utilizatorii dvs.

### <a name="policy-setting-for-connected-experiences-that-download-online-content"></a>Setarea de politică pentru experiențe conectate care descarcă conținut online

Acestea sunt experiențe care vă permit să căutați și să descărcați conținut online, inclusiv șabloane, imagini, modele 3D, videoclipuri și materiale de referință pentru a vă îmbunătăți documentele. De exemplu, șabloanele Office sau Pornirea rapidă PowerPoint. Pentru o listă a acestor experiențe conectate, consultați [Experiențe conectate în Office](connected-experiences.md)

Puteți utiliza setarea de politică *Permiteți utilizarea de experiențe conectate în Office care descarcă conținut online* pentru a controla dacă aceste tipuri de experiențe conectate sunt disponibile pentru utilizatorii dvs. Dacă nu configurați această setare de politică, aceste experiențe conectate vor fi disponibile pentru utilizatorii dvs.

Rețineți că dacă dezactivați setarea de politică *Permiteți utilizarea de experiențe conectate în Office*, experiențele conectate care descarcă conținut online nu vor fi disponibile pentru utilizatorii dvs.

### <a name="policy-setting-for-optional-connected-experiences"></a>Setarea de politică pentru experiențe conectate opționale

În plus față de experiențele conectate menționate mai sus, care sunt incluse în Office 365 ProPlus, există câteva experiențe conectate opționale pe care le puteți alege pentru a le permite utilizatorilor să le acceseze cu contul organizației lor. De exemplu, caracteristicile LinkedIn ale Asistentului pentru CV în Word sau caracteristica Hărți 3D în Excel, care utilizează Bing. Pentru mai multe exemple, consultați [Prezentare generală a experiențelor conectate opționale în Office](optional-connected-experiences.md).

Aceste experiențe conectate sunt diferite, deoarece nu sunt acoperite de acordul comercial al organizației cu Microsoft. Experiențele conectate opționale sunt oferite de Microsoft direct utilizatorilor dvs. și sunt guvernate de [Contractul de furnizare a serviciilor Microsoft](https://www.microsoft.com/servicesagreement), nu de [Condițiile de utilizare a serviciilor online](https://www.microsoft.com/licensing/product-licensing/products). În unele cazuri, conținutul sau funcționalitățile de la terți sunt furnizate prin aceste experiențe conectate opționale și se pot aplica și alte condiții. Pentru mai multe informații, consultați [Prezentare generală a experiențelor conectate opționale în Office](optional-connected-experiences.md).

Puteți utiliza setarea de politică *Permiteți utilizarea de experiențe conectate opționale, suplimentare în Office* pentru a controla dacă aceste tipuri de experiențe conectate sunt disponibile pentru utilizatorii dvs. Dacă nu configurați această setare de politică, aceste experiențe conectate opționale vor fi disponibile pentru utilizatorii dvs.

Chiar dacă alegeți să puneți aceste experiențe conectate opționale la dispoziția utilizatorilor dvs., utilizatorii dvs. vor avea opțiunea de a le dezactiva ca grup, accesând **Fișier** > **Cont** > **Confidențialitate cont** > **Gestionare setări**. Utilizatorii dvs. vor avea această opțiune doar dacă sunt conectați la Office cu acreditările organizației lor (la care se face uneori referire ca la contul de la locul de muncă sau de la școală), însă nu și dacă sunt conectați cu o adresă de e-mail personală.

De asemenea, unele dintre aceste experiențe conectate opționale sunt considerate și experiențe conectate care analizează conținut sau care descarcă conținut online. De exemplu, Inserare imagini online este o experiență conectată opțională, pe platformă Microsoft Bing, dar este considerată și o experiență conectată care descarcă conținut online. Așadar, dacă dezactivați setarea de politică *Permiteți utilizarea de experiențe conectate în Office care descarcă conținut online*, Inserare imagini online nu va fi disponibilă pentru utilizatorii dvs. Aceasta nu va fi disponibilă, chiar dacă ați activat setarea de politică *Permiteți utilizarea de experiențe conectate opționale, suplimentare în Office*. Pentru mai multe informații despre care experiențe conectate analizează conținut sau descarcă conținut online, consultați [Experiențe conectate în Office](connected-experiences.md).

Există o excepție de care trebuie să ținem cont. Setarea de politică *Permiteți utilizarea de experiențe conectate opționale, suplimentare în Office* nu controlează experiențe care vă solicită să conectați contul LinkedIn la contul Microsoft de la locul de muncă sau de la școală. Pentru a controla aceste tipuri de experiențe, cum ar fi informațiile LinkedIn dintr-o [fișă de profil](https://support.office.com/article/365-e80f931f-5fc4-4a59-ba6e-c1e35a85b501) în Outlook, consultați [Conectați-vă la conturile LinkedIn și Microsoft](https://support.office.com/article/dc81cc70-4d64-4755-9f1c-b9536e34d381) și [Acord pentru conexiunile contului LinkedIn pentru o organizație Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/linkedin-integration).

### <a name="policy-setting-for-most-connected-experiences"></a>Setarea de politică pentru cele mai conectate experiențe

Puteți utiliza setarea de politică *Permiteți utilizarea de experiențe conectate în Office* pentru a controla dacă cele mai conectate experiențe accesibile prin Office 365 ProPlus sunt disponibile pentru utilizatorii dvs. Dacă dezactivați setarea de politică, următoarele tipuri de experiențe conectate nu vor fi disponibile pentru utilizatorii dvs.:

- Experiențe care analizează conținut
- Experiențe care descarcă conținut online
- Experiențe conectate opționale

În plus, dacă dezactivați această setare de politică, majoritatea altor experiențe conectate sunt, de asemenea, dezactivate, cum ar fi elaborarea în comun și stocarea online. Pentru lista acestor experiențe conectate, consultați [Experiențe conectate în Office](connected-experiences.md).

Chiar dacă dezactivați această setare de politică, funcționalitatea Office limitată va rămâne disponibilă, cum ar fi sincronizarea unei cutii poștale în Outlook, Teams și Skype for Business vor continua să funcționeze. [Servicii esențiale](essential-services.md), cum ar fi serviciul de licențiere care confirmă că aveți licență corectă pentru a utiliza Office, vor rămâne, de asemenea, disponibile.

## <a name="existing-policy-settings-that-are-replaced-by-new-policy-settings"></a>Setările de politică existente care sunt înlocuite de noile setări de politică

Există două setări de politică care nu se mai aplică la Office 365 ProPlus, începând cu versiunea 1904. Iată acele setări de politică:

- **Trimiteți informații personale**, care pot fi găsite în Configurația de utilizator\\Politici\\Șabloane administrative\\Microsoft Office 2016\\Confidențialitate\\Centrul de autorizare.

- **Opțiuni conținut online**, care pot fi găsite în Configurația de utilizator\\Politici\\Șabloane administrative\\Microsoft Office 2016\\Instrumente | Opțiuni | Generale | Opțiuni de servicii... \\Conținut online.

Începând cu versiunea 1904, configurarea acestor două setări de politică existente nu vor avea niciun efect asupra Office 365 ProPlus. Ele nu se mai aplică deoarece funcționalitatea lor este înlocuită de aceste noi setări de politică:

- Permiteți utilizarea de experiențe conectate în Office care analizează conținut
- Permiteți utilizarea de experiențe conectate în Office care descarcă conținut online
- Permiteți utilizarea de experiențe conectate opționale, suplimentare în Office
- Permiteți utilizarea de experiențe conectate în Office

Aceste noi setări de politică vă pot oferi un control mai fin al nivelului decât cele două setări de politică existente. De exemplu, dacă anterior ați utilizat setarea de politică *Trimiteți informații personale*, atât Pornirea rapidă PowerPoint, cât și Căutarea inteligentă trebuiau să fie dezactivate. Dar acum, cu noile setări de politică, dacă utilizați setarea de politică *Permiteți utilizarea de experiențe conectate în Office care analizează conținut* pentru a dezactiva acel tip de experiențe conectate, doar Căutarea inteligentă este dezactivată. Pornirea rapidă PowerPoint va fi încă disponibilă pentru utilizatorii dvs.

Setările de politică apar încă în instrumentul de Gestionare a politicilor de grup, întrucât sunt încă aplicabile la versiunile de licențiere în volum de Office 2016 și Office 2019, cum ar fi Office Professional Plus 2019.

## <a name="what-about-existing-policy-settings-that-control-connected-experiences"></a>Dar ce se poate spune despre setările de politică existente ce controlează experiențe conectate?

După cum probabil știți deja, există unele setări de politică care vă permit să controlați experiențe conectate. Iată câteva exemple de setări de politică existente:

- *Opțiuni PowerPoint Designer*, în Configurația de utilizator\\Politici\\Șabloane administrative\\Microsoft Office 2016\\Instrumente | Opțiuni | Generale | Opțiuni de servicii... \\PowerPoint Designer

- *Dezactivați pornirea rapidă*, la Configurare utilizator\\Politici\\Șabloane administrative\\Microsoft PowerPoint 2016\\Opțiuni PowerPoint\\Generale

- *Permiteți caracteristica Asistent pentru CV LinkedIn*, în Configurare utilizator\\Politici\\Șabloane administrative\\Microsoft Word 2016\\Opțiuni Word\\Generale

 Puteți utiliza încă aceste setări de politică existente, dacă doriți să dezactivați experiențe conectate individuale. Dar rețineți că dacă utilizați una dintre noile setări de politică, acea setare nouă de politică poate dezactiva o experiență conectată pe care ați activat-o utilizând o setare de politică diferită. De exemplu, dacă activați setarea de politică *Permiteți caracteristica Asistent pentru CV LinkedIn*, dar dezactivați setarea de politică *Permiteți utilizarea de experiențe conectate în Office*, Asistentul pentru CV LinkedIn nu va fi disponibil pentru utilizatorii dvs.

În general, dacă o setare de politică este configurată pentru a activa o anumită experiență conectată în timp ce o altă setare de politică este configurată simultan pentru a dezactiva acel tip de experiență conectată, atunci acea experiență conectată este dezactivată pentru utilizatorii dvs.

## <a name="privacy-related-changes-to-the-office-ui"></a>Modificări legate de confidențialitate la interfața de utilizator Office

Există unele modificări la interfața de utilizator (UI) a Office 365 ProPlus care au legătură cu confidențialitatea, pe care utilizatorii le pot observa și în privința cărora pot pune întrebări. Aceste modificări sunt un rezultat direct al noilor controale de confidențialitate și setări de politică, disponibile începând cu versiunea 1904.

### <a name="dialog-about-optional-connected-experiences"></a>Dialog despre experiențe conectate opționale

Dacă ați ales să le oferiți utilizatorilor [experiențe conectate opționale](optional-connected-experiences.md), prima dată când utilizatorii dvs. deschid o aplicație Office după ce a fost actualizată la versiunea 1904, va apărea o casetă de dialog informativă. Această casetă de dialog îi informează pe utilizatorii dvs. că le-ați oferit opțiunea de a utiliza aceste experiențe conectate opționale și le dau ocazia să știe că pot accesa **Fișier** > **Cont** > **Confidențialitate cont** pentru a modifica această setare.

### <a name="privacy-settings-removed-from-the-office-ui"></a>Setările de confidențialitate au fost eliminate din interfața de utilizator Office

Următoarele setări sunt eliminate din **Fișier** > **Opțiuni** > **Centrul de autorizare** > **Setări Centrul de autorizare...** > **Opțiuni de confidențialitate**:

- Obțineți proiecte, informații, recomandări și servicii, permițând ca Office să acceseze și să efectueze îmbunătățiri de produs pe baza conținutului Office de pe dispozitivul meu.

- Permiteți Office să se conecteze la serviciile online Microsoft pentru a furniza funcționalități relevante pentru locația și preferințele dvs.

De asemenea, în **Fișier** > **Opțiuni** > **Generale**, opțiunea de a activa serviciile inteligente Office este eliminată.

Ca administrator pentru organizația dvs., puteți controla acum setările echivalente ale acestora prin noile setări de politică descrise anterior.

### <a name="privacy-settings-added-to-the-office-ui"></a>Setări de confidențialitate adăugate la interfața de utilizator Office

Iată câteva elemente noi care au fost adăugate la interfața de utilizator Office:

- La **Fișier** > **Cont**, utilizatorii vor vedea o opțiune nouă pentru **Confidențialitate cont** > **Gestionare setări**. La **Gestionare setări** utilizatorii pot dezactiva experiențe conectate opționale, dacă le-ați pus la dispoziție opțiunea respectivă.

- La **Fișier** > **Opțiuni** > **Centru de autorizare** > **Setări centru de autorizare...** > **Opțiuni de confidențialitate,** există o opțiune pentru a permite utilizarea [Vizualizatorului de date de diagnosticare](https://support.office.com/article/cf761ce9-d805-4c60-a339-4e07f3182855) pe dispozitiv.

 
## <a name="control-privacy-settings-by-editing-the-registry"></a>Controlați setările de confidențialitate prin editarea registry

Unii administratori preferă să modifice setările direct în registry, de exemplu, utilizând un script, în loc să utilizeze Politica de grup sau serviciul politică de cloud Office. Puteți utiliza următoarele informații pentru a configura setările de confidențialitate direct în registry.


|**Setări de politică** |**Setări de registry**  |**Valori**  |
|---------|---------|---------|---------|
|Configurați nivelul datelor de diagnosticare pentru software-ul client trimise de Office la Microsoft  | SendTelemetry |1 = Obligatoriu <br/> 2 = Opțional <br/> 3=Fără|
|Permiteți utilizarea de experiențe conectate în Office care analizează conținut  | UserContentDisabled | 1 = Activat <br/> 2 = Dezactivat|
|Permiteți utilizarea de experiențe conectate în Office care descarcă conținut online  | DownloadContentDisabled | 1 = Activat <br/> 2 = Dezactivat|
|Permiteți utilizarea de experiențe conectate opționale, suplimentare în Office   |  DisconnectedState |1 = Activat <br/> 2 = Dezactivat|
|Permiteți utilizarea de experiențe conectate în Office | ControllerConnectedServicesEnabled  | 1 = Activat <br/> 2 = Dezactivat|

Pentru a crea un fișier .reg pentru setările de confidențialitate, deschideți Notepad și copiați în următoarele linii. Ajustați valorile în funcție de necesitățile dvs., apoi salvați fișierul. Asigurați-vă că numele de fișier are o extensie .reg

```
Windows Registry Editor Version 5.00

[HKEY_CURRENT_USER\Software\Policies\Microsoft\office\16.0\common\privacy]
"disconnectedstate"=dword:00000001
"usercontentdisabled"=dword:00000001
"downloadcontentdisabled"=dword:00000001
"controllerconnectedservicesenabled"=dword:00000001

[HKEY_CURRENT_USER\Software\Policies\Microsoft\office\common\clienttelemetry]
"sendtelemetry"=dword:00000002
```

De exemplu, puteți utiliza acest fișier .reg cu comanda regedit.exe într-un script pentru a configura setările de confidențialitate pentru utilizator.