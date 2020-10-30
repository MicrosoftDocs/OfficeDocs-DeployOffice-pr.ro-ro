---
title: Date de diagnosticare obligatorii pentru Office
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
audience: ITPro
ms.topic: reference
ms.service: o365-proplus-itpro
localization_priority: Priority
ms.collection: Ent_O365
ms.custom:
- Ent_Office_ProPlus
- Ent_Office_Privacy
description: Le oferă administratorilor Office informații despre datele de diagnosticare obligatorii în Office și le furnizează o listă de evenimente și câmpuri de date.
hideEdit: true
ms.openlocfilehash: 8fd62619d8aff4b5dcb10d7a4c73710282e2cdd8
ms.sourcegitcommit: 596a0a60394011aafe1119f353ac76f27e1a4d1b
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/29/2020
ms.locfileid: "48794705"
---
# <a name="required-diagnostic-data-for-office"></a>Date de diagnosticare obligatorii pentru Office

> [!NOTE]
> Pentru o listă de produse Office care sunt reglementate de aceste informații despre confidențialitate, consultați [Controale de confidențialitate disponibile pentru produsele Office](products-versions-privacy-controls.md).

Datele de diagnosticare se folosesc pentru a păstra Office în siguranță și la zi, pentru a detecta, a diagnostica și a remedia problemele și pentru a îmbunătăți produsele. Aceste date nu includ numele sau adresa de e-mail a unui utilizator, nici conținutul fișierelor acestuia sau informații despre aplicații care nu au legătură cu Office.

Aceste date de diagnostic sunt colectate și trimise către Microsoft despre software-ul client Office care rulează pe dispozitivul utilizatorului. Anumite date de diagnosticare sunt obligatorii, în timp ce altele sunt opționale. Vă oferim posibilitatea de a alege dacă să ne trimiteți datele de diagnosticare obligatorii sau opționale, utilizând controalele de confidențialitate, cum ar fi setările de politici pentru organizații. Puteți vedea datele de diagnosticare care ne sunt trimise utilizând Vizualizatorul de date de diagnosticare.

***Datele de diagnosticare obligatorii** _ sunt datele minime necesare pentru a păstra Office securizat, actualizat și într-o stare de funcționare conform așteptărilor pe dispozitivul pe care este instalat.

Datele de diagnosticare obligatorii ajută la identificarea problemelor cu Office care pot fi asociate cu o configurație de dispozitiv sau software. De exemplu, ne poate ajuta să stabilim dacă o caracteristică de Office înregistrează căderi mai frecvent într-o anumită versiune de sistem de operare, cu caracteristici nou-introduse, sau atunci când anumite caracteristici de Office sunt dezactivate. Datele de diagnosticare obligatorii ne ajută să detectăm, să diagnosticăm și să remediem aceste probleme mai rapid, astfel încât impactul asupra utilizatorilor sau organizațiilor este redus.

Pentru mai multe informații despre datele de diagnosticare, consultați linkul următor:

- [Date de diagnosticare opționale pentru Office](optional-diagnostic-data.md)
- [Utilizarea Vizualizatorului de date de diagnosticare cu Office](https://support.microsoft.com/office/cf761ce9-d805-4c60-a339-4e07f3182855)

Dacă sunteți administratorul organizației dvs., ați putea fi interesat și de următoarele:

- [Prezentare generală a controalelor de confidențialitate pentru Aplicații Microsoft 365 pentru întreprindere](overview-privacy-controls.md)
- [Utilizați setările de politică pentru a gestiona controale de confidențialitate pentru Aplicații Microsoft 365 pentru întreprindere](manage-privacy-controls.md)
- [Utilizați preferințele pentru a gestiona controalele de confidențialitate ale Office pentru Mac](mac-privacy-preferences.md)
- [Utilizați preferințele pentru a gestiona controalele de confidențialitate ale Office pe dispozitivele iOS.](ios-privacy-preferences.md)
- [Utilizați setările de politică pentru a gestiona controale de confidențialitate pentru Office pe dispozitivele Android](android-privacy-controls.md)

## <a name="categories-data-subtypes-events-and-data-fields-for-required-diagnostic-data"></a>Categorii, subtipuri de date, evenimente și câmpuri de date pentru date de diagnosticare obligatorii

Datele de diagnosticare obligatorii sunt organizate în categorii și subtipuri de date. În fiecare subtip de date există evenimente care conțin câmpuri de date specifice respectivului eveniment.

Următorul tabel furnizează o listă de categorii pentru datele de diagnosticare obligatorii. Subtipurile de date din fiecare categorie sunt enumerate împreună cu o descriere a focalizării pentru acel subtip de date. Există linkuri la fiecare secțiune de subtip de date, unde veți găsi informațiile următoare:

- O listă de evenimente din acel subtip de date
- O descriere a fiecărui eveniment
- O listă de câmpuri de date în fiecare eveniment
- O descriere a fiecărui câmp de date

| _ *Categorie**       | **Subtip de date**| **Descriere**    |
| ---------- | ------------- | ---- |
| **Inventar și instalare software** | [Inventar și instalare Office](#office-setup-and-inventory-subtype)   | Produsul instalat, versiunea și starea de instalare.  |
| | [Configurație program de completare Office](#office-add-in-configuration-subtype)  | Programele de completare software și setările lor.     |
| | [Securitatea](#security-subtype)  | Condițiile de eroare ale documentelor, caracteristicilor și programelor de completare care pot compromite securitatea, inclusiv pregătirea pentru actualizarea produselor.  |
| **Utilizarea produselor și a serviciilor**    | [Succesul caracteristicii aplicației](#application-feature-success-subtype)   | Succesul funcționalității aplicației. Limitat la deschiderea și închiderea aplicației și a documentelor, editarea fișierelor și partajarea fișierelor (colaborare). |
| | [Starea aplicației și inițializare](#application-status-and-boot-subtype)    | Stabilește dacă au avut loc anumite evenimente de caracteristici, cum ar fi pornirea sau oprirea, și dacă respectiva caracteristică rulează.   |
| | [Configurație accesibilitate Office](#office-accessibility-configuration-subtype)  | Caracteristici de accesibilitate în Office       |
| | [Confidențialitate](#privacy-subtype)| Setări de confidențialitate în Office|
| **Performanța produselor și a serviciilor**       | [Ieșire neașteptată a aplicației (cădere)](#unexpected-application-exit-crash-subtype)  | Ieșirile neașteptate ale aplicației și starea aplicației atunci când se întâmplă acest lucru.    |
|  | [Performanța caracteristicii aplicației](#application-feature-performance-subtype)  | Timpii de răspuns slabi sau performanțele scăzute pentru scenarii precum pornirea aplicației sau deschiderea unui fișier. |
|  | [Eroare de activitate a aplicației](#application-activity-error-subtype)   | Erorile în funcționalitatea unei caracteristici sau a unei experiențe de utilizator.  |
| **Conectivitatea și configurarea dispozitivelor** | [Conectivitatea și configurarea dispozitivelor](#device-connectivity-and-configuration-subtype) | Starea conexiunii la rețea și setările dispozitivelor, cum ar fi memoria. |


> [!NOTE]
> - Categoriile sunt afișate în Vizualizatorul de diagnosticare de date, dar subtipurile de date nu sunt afișate.
> - Un câmp de date marcat *Depășit* a fost sau va fi eliminat din datele de diagnosticare obligatorii. Unele dintre aceste câmpuri de date sunt dubluri care au apărut ca date de diagnosticare au fost modernizate și utilizate pentru a vă asigura că nu există întreruperi de serviciu pentru rapoarte de monitorizare de diagnosticare live.

## <a name="categories-and-data-fields-that-are-common-for-all-events"></a>Categorii și câmpuri de date comune pentru toate evenimentele

Există câteva informații despre evenimente comune pentru toate evenimentele, indiferent de categorie sau de subtipul de date. Aceste informații comune, denumite uneori *contracte de date* , sunt organizate în categorii. Fiecare categorie conține câmpuri, iar aceste câmpuri sunt metadatele și proprietățile unui eveniment individual. Puteți vizualiza aceste informații utilizând Vizualizatorul de date de diagnosticare.

Categoriile de informații colectate despre evenimente pot fi împărțite în două grupuri:

  - [Informații comune pentru toate evenimentele](#information-common-to-all-events)
  - [Informațiile care acceptă în mod specific colectarea datelor de diagnosticare](#information-that-specifically-supports-diagnostic-data-collection)

### <a name="information-common-to-all-events"></a>*Informații comune pentru toate evenimentele*

Informații comune pentru toate evenimentele colectate în următoarele categorii.

#### <a name="app"></a>Aplicație 

Informații despre aplicație. Toate câmpurile sunt constante pentru toate sesiunile versiunii unei aplicații date.

Această categorie conține următoarele câmpuri:

  - **Branch** - ramura de unde a provenit compilarea dată. Ne permite să stabilim din ce tip de ramură a provenit o compilare dată, astfel încât să putem direcționa corect remedierile.
  - **InstallType** - enumerator care identifică modul în care utilizatorul a instalat aplicația. Ne permite să stabilim dacă anumite mecanisme de instalare creează probleme care nu se văd în alte mecanisme de instalare.
  - **Name** - numele aplicației care oferă datele. Ne permite să identificăm aplicația care prezintă o problemă, astfel încât să știm cum să o rezolvăm.
  - **Platform** - clasificare largă a platformei pe care rulează aplicația. Ne permite să identificăm platformele pe care poate apărea o problemă astfel încât să o putem stabili corect ca prioritate.
  - **Version** - versiunea aplicației. Ne permite să identificăm ce versiuni de produs afișează o problemă, astfel încât să o putem stabili corect ca prioritate.

#### <a name="client"></a>Client 

Identificator care are legătură cu o instanță de Office pe un dispozitiv. Constant pentru toate sesiunile tuturor aplicațiilor unei versiuni de instalare date pentru suite de aplicație multiplă sau constant pentru toate sesiunile unei versiuni de aplicație date.

Această categorie conține următoarele câmpuri:

  - **ID** - identificator unic atribuit unui client la ora de instalare a Office. Ne permite să identificăm dacă problemele afectează un anumit set de instalări și câți utilizatori sunt afectați.

#### <a name="consent"></a>Consimțământ

Informații cu privire la consimțământul utilizatorilor pentru date de diagnosticare și experiențe de mod conectat.

Această categorie conține următoarele câmpuri:

  - **ControllerConnectedServicesSourceLocation** – indică modul în care a fost efectuată opțiunea utilizatorului pentru experiențe de mod conectat opționale

  - **ControllerConnectedServicesState** - indică dacă utilizatorul are acces la experiență de mod conectat opțională

  - **ControllerConnectedServicesStateConsentTime** - indică momentul în care utilizatorul a ales starea experiențelor de mod conectat opționale. Data va apărea ca o dată ușor de citit de către oameni sau ca dată codificată de calculator sub forma unui număr mare.

  - **DiagnosticConsentConsentTime** - indică momentul în care utilizatorul și-a exprimat consimțământul pentru datele de diagnosticare Data va apărea ca o dată ușor de citit de către oameni sau ca dată codificată de calculator sub forma unui număr mare.

  - **DiagnosticConsentLevel** - indică nivelul de consimțământ pentru datele de diagnosticare oferite de utilizator

  - **DiagnosticConsentLevelSourceLocation** – indică modul în care utilizatorul și-a exprimat consimțământul pentru datele de diagnosticare

  - **DownloadContentSourceLocation** - indică modul în care utilizatorul a efectuat alegerea de a activa sau dezactiva experiență de mod conectat care descarcă conținut online

  - **DownloadContentState** - indică dacă utilizatorul a ales să activeze sau să dezactiveze experiențe de mod conectat care descarcă online conținut

  - **DownloadContentStateSourceLocation** - indică momentul în care utilizatorul a efectuat alegerea de a activa sau dezactiva experiențe de mod conectat care descarcă conținut online Data va apărea ca o dată ușor de citit de către oameni sau ca dată codificată de calculator sub forma unui număr mare.

  - **ServiceConnectionState** - indică dacă utilizatorul a ales să utilizeze sau nu toate experiențele de mod conectat

  - **ServiceConnectionStateConsentTime** - indică momentul în care utilizatorul a ales dacă să utilizeze sau nu toate experiențele de mod conectat. Data va apărea ca o dată ușor de citit de către oameni sau ca dată codificată de calculator sub forma unui număr mare.

  - **ServiceConnectionStateSourceLocation** -indică modul în care utilizatorul a furnizat opțiunea de a utiliza sau nu toate experiențele de mod conectat

  - **UserCategoryValue –** identifică tipul de utilizatori care și-au exprimat consimțământul. Unul dintre MSAUser, AADUser sau LocalDeviceUser

  - **UserContentDependentSourceLocation** – indică modul în care a fost efectuată opțiunea utilizatorului de a activa sau de a dezactiva experiențele de mod conectat care analizează conținut

  - **UserContentDependentState** - indică dacă utilizatorul a ales să activeze sau să dezactiveze experiențe de mod conectat care analizează conținut

  - **UserContentDependentStateConsentTime** - indică momentul în care utilizatorul a optat să activeze sau să dezactiveze experiențe de mod conectat care analizează conținut. Data va apărea ca o dată ușor de citit de către oameni sau ca dată codificată de calculator sub forma unui număr mare.

#### <a name="device"></a>Dispozitiv 

Informații despre sistemul de operare și versiune.

Această categorie conține următoarele câmpuri:

  - **OsBuild** - numărul de compilare al sistemului de operare instalat pe dispozitiv. Ne permite să identificăm dacă problemele afectează pachete Service Pack sau versiuni ale unui sistem de operare dat, în mod diferit decât altele, astfel încât să putem stabili priorități în ceea ce privește problemele.

  - **OsVersion** - versiunea majoră a sistemului de operare instalat pe dispozitiv. Ne permite să stabilim dacă problemele afectează o anumită versiune a sistemului de operare, mai mult decât altele, astfel încât să putem stabili priorități în ceea ce privește problemele.

#### <a name="legacy"></a>Moștenit 

Oferă un ID aplicație și o versiune de SO pentru compatibilitate cu practicile de colectare moștenite existente.

Această categorie conține următoarele câmpuri:

  - **AppId** - valoare a enumeratorului reprezentând aplicația care trimite datele. Ne permite să identificăm aplicația care prezintă o problemă, astfel încât să știm cum să o rezolvăm.

  - **OsEnv** - enumerator care indică sistemul de operare pe care rulează pe sesiunea. Ne permite să identificăm sistemul de operare pe care apare o problemă, astfel încât să putem stabili priorități în ceea ce privește problemele.

#### <a name="release"></a>Lansare 

Informațiile referitoare la canalul de lansare. Toate câmpurile sunt constante pentru toate sesiunile tuturor aplicațiilor unei versiuni de instalare date. Identifică un grup de dispozitive aflat în întregime într-o etapă a ciclului de lansare a produsului.

Această categorie conține următoarele câmpuri:

  - **Audience** - identifică un segment de public al unui grup de public dat. Ne permite să urmărim subseturi de grupuri de public pentru a evalua prevalența și stabilirea priorităților în ceea ce privește problemele.

  - **AudienceGroup** - identifică cercul din care provin datele. Ne permite să implementăm caracteristici pe etape și să identificăm probleme potențiale înainte să ajungă la majoritatea utilizatorilor.

  - **Channel** - canalul prin care este lansat produsul. Ne permite să identificăm dacă o problemă afectează unul dintre canalele noastre de implementare în mod diferit decât altele.

  - **Fork** - identifică ramificația produsului. Permite ca un mecanism să efectueze agregarea datelor pe un set de numere de compilare pentru a identifica eventuale probleme legate de o lansare dată.

#### <a name="session"></a>Sesiune 

Informații despre sesiunea de proces. Toate câmpurile sunt constante pentru această sesiune.

Această categorie conține următoarele câmpuri:

  - **ABConfigs** - identifică setul de ediții flight care rulează într-o sesiune dată. Ne permite să identificăm edițiile flight individuale care rulează într-o sesiune, astfel încât să putem stabili dacă o ediție flight este sursa unei probleme care afectează utilizatorii.

  - **EcsETag** - indicator din sistemul flighting care reprezintă edițiile flight trimise la computer. Ne permite să identificăm ce ediții flight ar putea afecta o sesiune dată.

  - **Flags** - semnalizări de urmărire bitmask care se aplică la o sesiune întreagă, concentrate în principal în mod curent pe opțiuni de eșantionare și date de diagnosticare. Ne permite să controlăm modul în care se comportă o sesiune dată față de datele de diagnosticare pe care le generează sesiunea.

  - **Id** - identifică în mod unic o anumită sesiune de date. Ne permite să identificăm impactul problemelor prin evaluarea numărului de sesiuni care sunt afectate și dacă există caracteristici comune ale sesiunilor respective.

  - **ImpressionId** - identifică setul de ediții flight care rulează într-o sesiune dată. Ne permite să identificăm edițiile flight individuale care rulează într-o sesiune, astfel încât să putem stabili dacă o ediție flight este sursa unei probleme care afectează utilizatorii.

  - **MeasuresEnabled** - semnalizare care indică dacă datele curente ale sesiunilor sunt eșantionate sau nu. Ne permite să stabilim cum să evaluăm în mod statistic datele care sunt colectate dintr-o sesiune dată.

  - **SamplingClientIdValue** - ID-ul clientului utilizat pentru a stabili dacă face parte din eșantionare. Ne permite să stabilim de ce o sesiune individuală a fost inclusă sau exclusă din eșantionare.
  
 - **SubAppName** - pentru aplicația Office Mobile, acest câmp reprezintă aplicația subiacentă utilizată pentru a deschide un document. De exemplu, dacă deschideți un document Word în aplicația Office, acest câmp va raporta valoarea „Word”.

 - **VirtualizationType** - tipul de virtualizare dacă Office rulează într-una. Valorile posibile sunt: 
    - 0 = Fără
    - 1 = Desktop virtual Windows
    - 2 = Protecție aplicații Windows Defender
    - 3 = Sistem de operare de bază Windows

#### <a name="user"></a>Utilizator

Furnizează informațiile de entitate găzduită pentru SKU-uri de software comerciale.

Această categorie conține următoarele câmpuri:

  - **PrimaryIdentityHash** - identificator sub pseudonim care reprezintă utilizatorul curent.

  - **PrimaryIdentitySpace** - tipul de identitate conținut în PrimaryIdentityHash. Unul dintre MASCID, OrgIdCID sau UserObjectId.

  - **TenantGroup** - tipul de entitate găzduită de care aparține abonamentul. Ne permite să clasificăm problemele și să identificăm dacă este o problemă pe scară largă sau una izolată la un set de utilizatori.

  - **TenantId** - entitatea găzduită la care este asociat abonamentul unui utilizator. Ne permite să clasificăm problemele și să identificăm dacă este o problemă pe scară largă sau una izolată la un set de utilizatori sau la o anumită entitate găzduită.

### <a name="information-that-specifically-supports-diagnostic-data-collection"></a>*Informațiile care acceptă în mod specific colectarea datelor de diagnosticare*

Informațiile care acceptă în mod specific colectarea datelor de diagnosticare sunt colectate în categoriile următoare.

#### <a name="activity"></a>Activitate

Informații pentru a înțelege succesul evenimentului de colectare în sine.

Această categorie conține următoarele câmpuri:

  - **AggMode** - comunică sistemului cum să realizeze agregarea rezultatelor activității. Ne permite să reducem volumul de informații încărcate de pe computerul unui utilizator, prin agregarea rezultatelor activității într-un singur eveniment, care se trimite periodic.

  - **Count** - de câte ori s-a produs activitatea dacă numărul este de la un eveniment agregat. Ne permite să stabilim cât de des o activitate a reușit sau a eșuat pe baza modului de agregare a activității.

  - **CV** - valoare care identifică relația dintre activități și activități secundare. Ne permite să reconstruim relația dintre activități imbricate.

  - **Duration** - cât timp a fost necesar pentru executarea activității. Ne permite să identificăm problemele de performanță care au impact negativ asupra experienței utilizatorilor.

  - **Result** . **Code** - cod definit de aplicație pentru a identifica un anumit rezultat. Ne permite să stabilim detalii mai specifice ale unei erori date, cum ar fi un cod de eroare care poate fi utilizat pentru a clasifica și a remedia problemele.

  - **Result.Tag** - etichetă întreagă, care identifică locația din codul unde a fost generat rezultatul. Ne permite să identificăm clar locația din cod unde a fost generat un rezultat, care permite clasificarea eșecurilor.

  - **Result** . **Type** - tipul codului de rezultat. Identifică tipul de cod de rezultat care a fost trimis, astfel încât valoarea poate fi interpretată corect.

  - **Success** - semnalizare care indică dacă activitatea a reușit sau nu. Ne permite să determinăm dacă acțiunile pe care le aplică utilizatorul în produs sunt reușite sau nereușite. Acest lucru ne permite să identificăm problemele care au impact asupra utilizatorului.

#### <a name="application"></a>Aplicație 

Informații despre instalarea aplicației din care sunt colectate evenimentele.

Această categorie conține următoarele câmpuri:

  - **Architecture** - arhitectura aplicației. Să clasificăm erorile care pot fi specifice unei arhitecturi a aplicației.

  - **Click2RunPackageVersion** - numărul de versiune al pachetului Clic și Pornire care a instalat aplicația. Ne permite să identificăm ce versiune a programului de instalare a fost utilizată pentru a instala Office, astfel încât să putem identifica probleme asociate de configurare.

  - **DistributionChannel** - canalul în care a fost implementată aplicația. Ne permite să realizăm partiția datelor de intrare, astfel încât să putem stabili dacă problemele afectează publicul.

  - **InstallMethod -** dacă pentru versiunea de compilare curentă de Office s-a efectuat upgrade de la o compilare mai veche, dacă s-a revenit la o compilare mai veche sau dacă este o instalare nouă.

  - **IsClickToRunInstall** - semnalizare care indică dacă instalarea a fost o instalare Clic și Pornire. Ne permite să identificăm problemele care pot fi specifice mecanismului de instalare Clic și Pornire.

  - **IsDebug** - semnalizare indicând dacă compilarea de Office este una de depanare. Ne permite să identificăm dacă problemele provin de la compilări de depanare care se pot comporta diferit.

  - **IsInstalledOnExternalStorage** - semnalizare care indică dacă Office a fost instalat pe un dispozitiv de stocare extern. Ne permite să stabilim dacă problemele pot fi urmărite până într-o locație de stocare externă.

  - **IsOEMInstalled** - semnalizare care indică dacă Office a fost instalat de un producător original al echipamentului (OEM). Ne permite să stabilim dacă aplicația a fost instalată de un OEM care ne poate ajuta să clasificăm și să identificăm problemele.

  - **PreviousVersion** - versiunea de Office care a fost instalată anterior pe computer. Ne permite să revenim la o versiune anterioară, dacă cea curentă are o problemă.

  - **ProcessFileName** - denumirea numelui de fișier al aplicației. Ne permite să identificăm numele fișierului executabil, care generează date așa cum pot exista mai multe nume de fișiere pentru mai multe procese care raportează același nume de aplicație.

#### <a name="client"></a>Client

Informații despre clientul Office.

Această categorie conține următoarele câmpuri:

  - **FirstRunTime** - prima dată când s-a rulat clientul. Ne permite să înțelegem cât timp a avut clientul instalat Office.

#### <a name="device"></a>Dispozitiv

Informații despre configurarea și capacitățile dispozitivelor.

Această categorie conține următoarele câmpuri:

  - **DigitizerInfo** - informații despre digitizorul utilizat de computer. Ne permite să clasificăm datele pe baza pivotului de dispozitiv.

  - **FormFactor** - identifică ce factor de formă este dispozitivul care transmite informațiile. Ne permite să clasificăm datele pe baza pivotului de dispozitiv.

  - **FormFactorFamily** - identifică ce factor de formă este dispozitivul care transmite informațiile. Ne permite să clasificăm datele pe baza pivotului de dispozitiv.

  - **HorizontalResolution** - rezoluția orizontală a ecranului dispozitivelor. Ne permite să clasificăm datele pe baza pivotului de dispozitiv.

  - **Id** - identificator unic pentru dispozitiv. Ne permite să identificăm distribuția problemelor pe un set de dispozitive.

  - **IsEDPPolicyEnabled** - semnalizare pentru a indica dacă protecția îmbunătățită a datelor este activată pe computer. Ne permite să clasificăm datele pe baza pivotului de dispozitiv.

  - **IsTerminalServer** - semnalizare pentru a stabili dacă computerul este un server terminal. Ne permite să clasificăm datele pe baza pivotului de dispozitiv.

  - **Manufacturer** - producătorul dispozitivului. Ne permite să clasificăm datele pe baza pivotului de dispozitiv.

  - **Model** - Modelul de dispozitiv. Ne permite să clasificăm datele pe baza pivotului de dispozitiv.

  - **MotherboardUUIDHash** - cod hash al unui identificator unic pentru placa de bază. Ne permite să clasificăm datele pe baza pivotului de dispozitiv.

  - **Name** - numele dispozitivului. Ne permite să clasificăm datele pe baza pivotului de dispozitiv.
  
  - **NetworkCost** - indică costul sau tipul de rețea, de exemplu contorizată sau contorizată peste limită.
  
  - **NetworkCountry** - codul de țară al expeditorului, pe baza adresei IP necurățată a clientului.

  - **NumProcPhysCores** - numărul de nuclee fizice din computer. Ne permite să clasificăm datele pe baza pivotului de dispozitiv.

  - **OsLocale** - setarea regională a sistemului de operare care rulează. Ne permite să clasificăm datele pe baza pivotului de dispozitiv.

  - **ProcessorArchitecture** - arhitectura procesorului. Ne permite să clasificăm datele pe baza pivotului de dispozitiv.

  - **ProcessorCount** - numărul de procesoare de pe computer. Ne permite să clasificăm datele pe baza pivotului de dispozitiv.

  - **ProcSpeedMHz** - viteza procesorului. Ne permite să clasificăm datele pe baza pivotului de dispozitiv.

  - **RamMB** - volumul memoriei pe care îl are dispozitivul. Ne permite să clasificăm datele pe baza pivotului de dispozitiv.

  - **ScreenDepth** - ne permite să clasificăm datele pe baza pivotului de dispozitiv.

  - **ScreenDPI** - valoarea DPI a ecranului. Ne permite să clasificăm datele pe baza pivotului de dispozitiv.

  - **SusClientId -** ID-ul Windows Update al dispozitivului pe care rulează Office.

  - **SystemVolumeFreeSpaceMB** - spațiul liber disponibil din volumul sistemului. Ne permite să clasificăm datele pe baza pivotului de dispozitiv.

  - **SystemVolumeSizeMB** - dimensiunea volumului sistemului de pe computer. Ne permite să clasificăm datele pe baza pivotului de dispozitiv.

  - **VerticalResolution** - rezoluția verticală a ecranului dispozitivelor. Ne permite să clasificăm datele pe baza pivotului de dispozitiv.

  - **WindowErrorReportingMachineId** - identificator unic al computerului furnizat de raportarea erorilor Windows. Ne permite să clasificăm datele pe baza pivotului de dispozitiv.

  - **WindowSqmMachineId** - identificator unic pentru computer furnizat de Windows SQM. Ne permite să clasificăm datele pe baza pivotului de dispozitiv.

#### <a name="event"></a>Eveniment 

Informații specifice evenimentului, inclusiv identificatorul său unic din sesiune.

Această categorie conține următoarele câmpuri:

  - **Contract** - lista contractelor pe care le implementează evenimentul. Ne permite să evaluăm datele care fac parte din evenimentul individual, astfel încât să îl putem procesa mai eficient.

  - **CV** - valoare care ne permite să identificăm evenimentele corelate între ele. Utilizat pentru diagnosticări care ne permit să identificăm modele de comportament asociat sau evenimente asociate.

  - **Flags** - informații utilizate pentru a modifica modul în care răspunde un anumit eveniment. Utilizat pentru a gestiona modul în care un anumit eveniment este tratat cu scopul de a încărca datele în Microsoft.

  - **Id** - identificator unic pentru eveniment. Ne permite să identificăm evenimentele care sunt primite.

  - **Level** - denotă tipul de eveniment.

  - **Name** - numele evenimentului. Permite să identificăm evenimentul care a fost trimis de la client.

  - **Rule** - identificator al regulii care a generat datele dacă acestea au fost generate de o regulă. Ne permite să identificăm sursa unor date, astfel încât să putem valida și gestiona parametrii acelor evenimente

  - **RuleId** - identificator al regulii care a generat datele dacă acestea au fost generate de o regulă. Ne permite să identificăm sursa unor date, astfel încât să putem valida și gestiona parametrii acelor evenimente.

  - **RuleInterfaces** - orice interfețe care sunt implementate de o regulă specifică. Ne permite să clasificăm și să importăm datele în funcție de structura sa, care simplifică procesarea datelor.

  - **RuleVersion** - identificator al regulii care a generat datele dacă acestea au fost generate de o regulă. Ne permite să identificăm sursa unor date, astfel încât să putem valida și gestiona parametrii acelor evenimente.

  - **SampleRate** - o indicație a procentului de utilizatori care trimit această parte din date. Acest lucru ne permite să efectuăm analiza statistică a datelor, iar pentru punctele de date foarte obișnuite nu trebuie să fie trimise de toți utilizatorii.

  - **SchemaVersion** - versiunea schemei utilizate pentru a genera datele de diagnosticare. Necesar pentru a gestiona datele trimise de client. Acest lucru permite modificări în timp în care datele sunt trimise de la fiecare client.

  - **Sequence** - contor care identifică ordinea în care un eveniment a fost generat la client. Permite ca datele primite să fie ordonate, astfel încât să putem identifica pașii care este posibil să fi condus la o problemă care afectează clienții.

  - **Source** - canalul de sursă care a fost utilizat pentru a încărca datele. Obligatoriu pentru a monitoriza canalele noastre de încărcare pentru starea generală și pentru a identifica eventualele probleme la canalele de încărcare. Acest lucru ne permite să monitorizăm canale individuale de încărcare pentru a garanta că acestea rămân conforme.

  - **Time** - ora la care evenimentul a fost generat de client. Ne permite să sincronizăm și să validăm ordinea evenimentelor generate la client, precum și stabilirea măsurătorilor de performanță pentru instrucțiuni de utilizator. 

#### <a name="host"></a>Gazdă

Informații despre o aplicație care găzduiește o aplicație încorporată

Această categorie conține următoarele câmpuri:

  - **Id** - identificator unic atribuit aplicației gazdă de aplicația încorporată.

  - **SessionId** - identificator unic global pentru sesiunea gazdei.

  - **Version** - identificatorul versiunii de fișier executabil principal al gazdei.

#### <a name="legacy"></a>Moștenit

Informațiile necesare pentru compatibilitatea sistemului moștenit.

Această categorie conține următoarele câmpuri:

  - **OsBuild** - numărul de compilare specific al sistemului de operare. Ne permite să stabilim de la ce versiune de sistem de operare provin datele de diagnosticare, astfel încât să putem stabili priorități în ceea ce privește problemele.

  - **OsBuildRevision** - numărul de revizuire al compilării sistemului de operare. Ne permite să stabilim de la ce versiune de sistem de operare provin datele de diagnosticare, astfel încât să putem stabili priorități în ceea ce privește problemele.

  - **OsMinorVersion** - versiunea minoră a sistemului de operare. Ne permite să stabilim de la ce versiune de sistem de operare provin datele de diagnosticare, astfel încât să putem stabili priorități în ceea ce privește problemele.

  - **OsVersionString** - șir unificat, care reprezintă numărul de compilare al sistemului de operare. Ne permite să stabilim de la ce versiune de sistem de operare provin datele de diagnosticare, astfel încât să putem stabili priorități în ceea ce privește problemele.

#### <a name="session"></a>Sesiune

Informații despre sesiunea de proces.

Această categorie conține următoarele câmpuri:

  - **ABConfigsDelta** - urmărește diferența dintre datele curente ABConfigs și valoarea anterioară. Ne permite să urmărim care sunt noile setări flight de pe computer pentru a identifica dacă o nouă setare flight este responsabilă pentru o problemă.

  - **CollectibleClassification** - clasele de informații pe care sesiunea le poate colecta. Permite filtrarea sesiunilor pe baza datelor pe care ar trebui să le aibă.

  - **DisableTelemetry** - semnalizare care indică dacă cheia DisableTelemetry este setată. Ne permite să știm dacă o sesiune nu a raportat date de diagnosticare altele decât EssentialServiceMetadata.

  - **SamplingClientIdValue** - valoarea cheii utilizate pentru a determina eșantionarea. Ne permite să determinăm de ce o sesiune a fost eșantionată sau nu.

  - **SamplingDeviceIdValue** - valoarea cheii utilizate pentru a determina eșantionarea. Ne permite să determinăm de ce o sesiune a fost eșantionată sau nu.

  - **SamplingKey** - cheia este utilizată pentru a stabili dacă sesiunea este eșantionată sau nu. Ne permite să înțelegem cum aleg sesiunile individuale dacă să fie eșantionate sau nu.

  - **SamplingMethod** - metoda utilizată pentru a stabili politica de eșantionare. Ne permite să înțelegem ce date provin dintr-o sesiune.

  - **SamplingSessionKValue** - metadate complexe de eșantionare. Utilizate pentru a evalua semnificația statistică a datelor primite.

  - **SamplingSessionNValue** - metadate complexe de eșantionare. Utilizate pentru a evalua semnificația statistică a datelor primite.

  - **Sequence** - identificator numeric unic pentru sesiune. Permite ordonarea sesiunilor pentru analiza problemelor care puteau să apară.

  - **Start** - ora de inițializare a sesiunii de proces. Ne permite să stabilim când începe sesiunea.

  - **TelemetryPermissionLevel** - valoare care indică nivelul datelor de diagnosticare pentru care utilizatorul a optat. Ne permite să înțelegem la ce nivel de date de diagnosticare să ne așteptăm de la o sesiune.

  - **TimeZoneBiasInMinutes** - diferența în minute între UTC și ora locală. Permite normalizarea orelor UTC înapoi la ora locală.

## <a name="data-fields-that-are-common-for-onenote-events"></a>Câmpuri de date care sunt comune pentru evenimentele OneNote

Următoarele câmpuri de date sunt comune pentru toate evenimentele OneNote pe Mac, iOS și Android.

> [!NOTE]
> Atunci când utilizați Vizualizatorul de date de diagnosticare, evenimentele pentru OneNote pe Mac, iOS și Android vor apărea că au denumirea Activity, ReportData, sau Unexpected. Pentru a găsi numele real al evenimentului, selectați evenimentul și consultați câmpul EventName.

- **Activity_ActivityType** - indică tipul acestui eveniment. O activitate poate fi activitate normală sau activitate cu valoare mare.

- **Activity_AggMode** - comunică sistemului cum să realizeze agregarea rezultatelor activității. Ne permite să reducem volumul de informații încărcate de pe computerul unui utilizator, prin agregarea rezultatelor activității într-un singur eveniment, care se trimite periodic.

- **Activity_Count** - de câte ori s-a produs activitatea dacă numărul este de la un eveniment agregat. Ne permite să stabilim cât de des a reușit sau a eșuat o activitate pe baza modului de agregare a activității.

- **Activity_CV** - valoare care identifică relația dintre activități și activități secundare. Ne permite să reconstruim relația dintre activități imbricate.

- **Activity_DetachedDurationInMicroseconds** - durata de timp în care o activitate este inactivă și nu efectuează lucrări reale, dar timpul este totuși contorizat la timpul total al activității.

- **Activity_DurationInMicroseconds** - perioada necesară pentru executarea activității. Ne permite să identificăm problemele de performanță care au impact negativ asupra experienței utilizatorilor.

- **Activity_Expiration** - o dată în format numeric care indică momentul în care acest eveniment va înceta trimiterea de la clienți.

- **Activity_FailCount** - de câte ori nu a reușit această activitate

- **Activity_Name** - o denumire scurtă a unui eveniment. Permite identificarea evenimentului care a fost trimis de la client.

- **Activity_Namespace** - un spațiu de nume al unui eveniment. Permite gruparea evenimentului în grupuri.

- **Activity_Reason** - un șir care indică motivul pentru care o activitate se termină cu un anumit rezultat.

- **Activity_Result** - o semnalizare care indică dacă activitatea a reușit, nu a reușit sau a eșuat în mod neașteptat. Ne permite să determinăm dacă acțiunile pe care le aplică utilizatorul în produs sunt reușite sau nereușite. Acest lucru ne permite să identificăm problemele care au impact asupra utilizatorului.

- **Activity_State** - o semnalizare care indică dacă un eveniment este începutul unei activități a utilizatorului sau sfârșitul unei activități a utilizatorului.

- **Activity_SucceedCount** -  de câte ori a reușit această activitate.

- **ErrorCode** - indică un cod de eroare dacă este disponibil.

- **ErrorCode2** - indică un al doilea cod de eroare dacă este disponibil.

- **ErrorCode3** - indică un al treilea cod de eroare dacă este disponibil.

- **ErrorTag** -  indică eticheta asociată în codul unei erori dacă este disponibilă.

- **ErrorType** - indică tipul unei erori dacă este disponibil.

- **EventName** - un nume unic al unui eveniment OneNote. Evenimentele OneNote utilizează acest câmp particularizat pentru a specifica un nume unic din cauza unei limitări tehnice din trecut.

- **ExpFeatures** - precizează dacă un utilizator a activat sau nu un comutator de caracteristici experimentale în aplicația OneNote.

- **ExpirationDate** - o dată în format numeric care indică momentul în care acest eveniment va înceta trimiterea de la clienți

- **IsConsumer** - precizează dacă un utilizator este sau nu consumator

- **IsEdu** - precizează dacă un utilizator este sau nu utilizator în entitatea găzduită pentru educație.

- **IsIW** - precizează dacă un utilizator este sau nu utilizator întreprindere

- **IsMsftInternal** - precizează dacă un utilizator este sau nu angajat Microsoft

- **IsPremiumUser** - precizează dacă un utilizator are licență premium sau nu

- **Namespace** - un spațiu de nume al evenimentului. Permite gruparea evenimentului în grupuri.

- **Release_AppStore** - o semnalizare care indică dacă o compilare provine de la un magazin de aplicații sau nu.

- **Release_Audience** - identifică un segment de public al unui grup de public dat. Ne permite să urmărim subseturi de grupuri de public pentru a evalua prevalența și stabilirea priorităților în ceea ce privește problemele.

- **Release_AudienceGroup** - identifică cercul din care provin datele. Ne permite să implementăm caracteristici pe etape și să identificăm probleme potențiale înainte să ajungă la majoritatea utilizatorilor.

- **Release_Channel** - canalul prin care este lansat produsul. Ne permite să identificăm dacă o problemă afectează unul dintre canalele noastre de implementare în mod diferit decât altele.

- **RunningMode** - indică modul în care aplicația este lansată de utilizator sau de procesul de sistem.

- **SchemaVersion** - indică o versiune curentă a schemei de telemetrie în canalul de telemetrie OneNote.

- **Session_EcsETag** - indicator din sistemul flighting care reprezintă edițiile flight trimise la computer. Ne permite să identificăm ce ediții flight ar putea afecta o sesiune dată.

- **Session_ImpressionId** - identifică setul de ediții flight care rulează într-o sesiune dată. Ne permite să identificăm edițiile flight individuale care rulează într-o sesiune, astfel încât să putem stabili dacă o ediție flight este sursa unei probleme care afectează utilizatorii.

- **SessionCorrelationId** - identificator unic global pentru sesiunea gazdei.

- **SH_ErrorCode** - indică, dacă este disponibil, un cod de eroare atunci când o activitate nu reușește.

- **Tag** - etichetă număr întreg care identifică locația din cod unde este generat evenimentul de telemetrie.

- **UserInfo_IdType** - un șir care indică tipul de cont al unui utilizator

- **UserInfo_OMSTenantId** - entitatea găzduită la care este asociat abonamentul unui utilizator. Ne permite să clasificăm problemele și să identificăm dacă este o problemă pe scară largă sau una izolată la un set de utilizatori sau la o anumită entitate găzduită.

- **UserInfo_OtherId** - o listă de pseudonime de identificare non-primare care reprezintă conturi de utilizator.

- **UserInfo_OtherIdType** - o listă de tipuri de conturi non-primare.

## <a name="data-fields-that-are-common-for-outlook-mobile-events"></a>Câmpuri de date care sunt uzuale pentru evenimentele mobile Outlook

Outlook Mobile colectează câmpuri comune pentru fiecare dintre evenimentele noastre, pentru a ne asigura că aplicația este actualizată, securizată și funcțională, conform așteptărilor. 

Următoarele câmpuri de date sunt comune pentru toate evenimentele Outlook pentru iOS și Android.

- **aad_tenant_id** - ID-ul entității găzduite a clientului, dacă este disponibil

- **account_cid** - un identificator sub pseudonim care reprezintă utilizatorul curent.

- **account_domain** - numele de domeniu al contului

- **userPuid** - identificatorul de utilizator unic global pentru un cont Microsoft pentru consumatori.

- **account_type** - urmărește tipul de cont, cum ar fi Office 365, memoria cache din Google Cloud, Outlook.com etc.

- **action** - numele evenimentului acțiune (cum ar fi arhivare, ștergere etc.), astfel încât să putem detecta probleme cu anumite acțiuni întreprinse

- **ad_id** - identificatorul unic de publicitate

- **app_version** - versiunea curentă a aplicației instalată pentru a ne ajuta să detectăm problemele care afectează anumite versiuni de aplicație 

- **AppInfo.ETag** - un identificator unic pentru gestionarea lansării caracteristicilor noastre, pentru a ne ajuta să detectăm problemele care afectează anumite caracteristici în curs de lansare

- **AppInfo.Language** - setarea curentă a limbii dispozitivului pentru a ne ajuta să detectăm problemele care afectează anumite limbi

- **AppInfo.Version** - versiunea curentă a aplicației instalate pentru a ne ajuta să detectăm problemele care afectează anumite versiuni de aplicație

- **ci** - un Identificator unic de dispozitiv pentru o aplicație specifică, cu pseudonim

- **cid_type** - indică ce tip de cont este, cum ar fi un cont comercial sau un cont Outlook.com.

- **cloud** - unde se află cutia poștală pentru contul de pe acest dispozitiv, pentru a ajuta la detectarea problemelor specifice pentru o anumită cutie poștală în cloud, cum ar fi Office 365 sau GCC.

- **customer_type** - indică tipul de client (consumator, comercial, terț etc.), pentru a ne ajuta să detectăm problemele care afectează anumite tipuri de clienți

- **device_category** - indică ce tip de dispozitiv este (telefon, tabletă etc.), pentru a ne ajuta să detectăm problemele specifice categoriei de dispozitive

- **DeviceInfo.Id** - un identificator unic al dispozitivelor, pentru a ne ajuta să detectăm probleme specifice 

- **DeviceInfo.Make** - marca dispozitivului (de exemplu, Apple, Samsung etc.) pentru a ne ajuta să detectăm probleme specifice de marcă ale dispozitivului

- **DeviceInfo.Model** - modelul dispozitivului (de exemplu, iPhone 6s), pentru a ne ajuta să detectăm probleme specifice de model ale dispozitivului

- **DeviceInfo.NetworkType** - rețeaua utilizată pe dispozitivul curent (WiFi, date celulare etc.) pentru a ne ajuta să detectăm probleme specifice de rețea ale dispozitivului

- **DeviceInfo.OsBuild** - compilarea SO actuală a dispozitivului pentru a ne ajuta să detectăm problemele care afectează anumite compilări OS

- **DeviceInfo.OsName** - numele sistemului de operare (de exemplu, iOS), pentru a ne ajuta să detectăm problemele care afectează anumite platforme

- **DeviceInfo.OsVersion** - versiunea SO actuală a dispozitivului pentru a ne ajuta să detectăm problemele care afectează anumite versiuni OS

- **DeviceInfo.SDKUid** - identificatorul unic al dispozitivului (similar cu DeviceInfo.Id)

- **EventInfo. InitId** - ID utilizat ca parte a succedării pentru a comanda evenimentul prin intermediul conductei de telemetrie, pentru a ne ajuta să detectăm cauza principală a unei probleme de conducte

- **EventInfo.SdkVersion** - versiunea de SDK pe care o utilizăm pentru a trimite telemetria noastră, pentru a ne ajuta să detectăm cauza principală a unei probleme de conducte

- **EventInfo.Sequence** - secvența este pentru a comanda evenimentul prin intermediul conductei de telemetrie, pentru a ne ajuta să detectăm cauza principală a unei probleme de conducte

- **EventInfo.Source** - ne indică ce parte din cod a trimis evenimentul pentru a ne ajuta să detectăm cauza principală a unei probleme

- **EventInfo.Time** - data și ora la care a fost emis evenimentul de pe dispozitiv, astfel încât sistemele noastre să poată gestiona cu succes evenimentele care sosesc

- **eventpriority** - prioritatea relativă a evenimentului telemetrie față de alte evenimente, astfel încât sistemele noastre să poată gestiona cu succes evenimentele care sosesc

- **first_launch_date** - prima dată când a fost lansată aplicația pentru a ne ajuta să înțelegem când a început o problemă

- **hashed_email** - identificator sub pseudonim care reprezintă email-ul utilizatorului curent

- **is_first_session** - piste dacă aceasta este prima sesiune a aplicației pentru depanare

- **origin** - originea unei acțiuni. De exemplu, marcarea unui mesaj citit poate să provină din lista de mesaje sau o notificare de corespondență nouă, acest lucru ne ajută să detectăm probleme cauzate de originii acțiunii

- **PipelineInfo.AccountId** - un identificator sub pseudonim care reprezintă utilizatorul curent

- **PipelineInfo.ClientCountry** - țara curentă a dispozitivului pentru a detecta probleme specifice țării sau regiunii și întreruperi 

- **PipelineInfo.ClientIp** - adresa IP la care este conectat dispozitivul pentru a depana probleme de conexiune

- **PipelineInfo.IngestionTime** - Marcă de timp de când se întâmplă ingestia telemetrie pentru acest eveniment

- **Session.Id** -un Identificator unic pentru sesiunea de aplicații, pentru a vă ajuta să identificați problemele legate de sesiune

- **Session.ImpressionId** - un identificator unic pentru gestionarea lansării caracteristicilor noastre, pentru a asigura că caracteristicile sunt lansate cu succes pentru toți utilizatorii și dispozitive

- **ui_mode** - este utilizatorul în modul Light sau Dark, ne ajută să triem erorile UX cu modul întunecat

- **UserInfo.Language** - fusul orar al utilizatorului pentru a ajuta la depanarea problemelor cu textului tradus

- **UserInfo.Language** - fusul orar al utilizatorului pentru a ajuta la depanarea problemelor de calendar


În plus, următoarele câmpuri sunt comune pentru toate evenimentele pentru Outlook pentru iOS.

- **DeviceInfo.NetworkProvider** - furnizorul de rețea al dispozitivului (de exemplu, Verizon)

- **gcc_restrictions_enabled** - ne indică dacă s-au aplicat restricții GCC la aplicație, astfel încât să ne asigurăm că clienții noștri GCC utilizează aplicația în siguranță
 
- **multi_window_mode** – ne indică dacă utilizatorul pe iPad folosește mai multe ferestre pentru a ne ajuta să detectăm probleme legate de utilizarea ferestrelor multiple.

- **office_session_id** - un ID unic care urmărește sesiunea pentru serviciile Office conectate, pentru a ajuta la detectarea problemelor specifice unui serviciu Office integrat în Outlook, cum ar fi Word

- **state** - dacă aplicația a fost activă atunci când a fost trimis acest eveniment pentru a ajuta la detectarea problemelor specifice pentru stările de aplicații active sau inactive


În plus, următoarele câmpuri sunt comune pentru toate evenimentele pentru Outlook pentru Android.

- **aad_id** - un identificator Azure Active Directory cu pseudonim

- **DeviceInfo. NetworkCost** - indicarea de dispozitive costul de rețea curent, care reflectă starea de WiFi/date celulare/roaming pentru a ajuta la detectarea problemelor specifice rețelei de dispozitive

- **is_app_in_duo_split_view_mode** - acest lucru ne va spune că aplicația a fost în modul ecran scindat Duo.  Această proprietate este setată doar pentru dispozitivele Duo (doar pentru Android).

- **is_dex_mode_enabled** - dacă este activat modul Samsung DeX, pentru a ajuta la detectarea problemelor specifice modulului DeX cu dispozitive Samsung

- **is_sliding_drawer_enabled** - dacă este activată interfața glisantă pentru sertare, pentru a ajuta la detectarea problemelor provocate de interfața noastră glisantă pentru sertare

- **orientarea** - orientarea fizică a ecranului (portret/vedere), pentru a ajuta la detectarea problemelor specifice orientărilor dispozitivelor

- **os_arch** - arhitectura sistemului de operare pentru dispozitiv, pentru a ajuta la detectarea problemelor specifice sistemelor de operare ale dispozitivelor

- **process_bitness** - numărul de biți al procesului aplicației (32 sau 64 bit) pentru a va ajuta la detectarea problemelor specifice numărului de biți al dispozitivelor

- **webview_kernel_version** : versiunea kernel-ului Chromium a vizualizării web de pe dispozitiv, pentru a ne ajuta să detectăm probleme de compatibilitate legate de versiunea de vizualizare web a paginii.

- **webview_package_name** : numele de pachet a vizualizării web de pe dispozitiv, pentru a ne ajuta să detectăm probleme de compatibilitate legate de versiunea de vizualizare web a paginii.

- **webview_package_version** : numele de versiune a vizualizării web de pe dispozitiv, pentru a ne ajuta să detectăm probleme de compatibilitate legate de versiunea de vizualizare web a paginii.


## <a name="software-setup-and-inventory-data-events"></a>Evenimente despre instalare de software și date de inventar

Iată subtipurile de date din această categorie:
- [Inventar și instalare Office](#office-setup-and-inventory-subtype)
- [Configurație program de completare Office](#office-add-in-configuration-subtype)
- [Securitatea](#security-subtype)  

### <a name="office-setup-and-inventory-subtype"></a>*Subtip de instalare și inventar Office*

Produsul instalat, versiunea și starea de instalare.

#### <a name="addssoaccount"></a>add.sso.account

Acest lucru va alerta Microsoft pentru succesul sau eșecul unui utilizator la adăugarea unui cont prin sign-on unic (SSO).

Se colectează următoarele câmpuri: 

- **account_type** – tipul de cont adăugat utilizând SSO.

- **action_origin** – de unde a fost generat acest eveniment. (de exemplu, valori: sso_drawer, sso_add_account, sso_add_account_prompt, sso_settings, sso_oobe).

- **furnizor** – identificatorul pachetului de software al furnizorului pentru SSO.

- **stare** – starea curentă a contului, (exemplu de valoare: EȘUAT, ÎN AȘTEPTARE, ADĂUGAT etc.)
 
#### <a name="officeclicktorunupdatestatus"></a>Office.ClickToRun.UpdateStatus

Se aplică la toate aplicațiile win32. Ne ajută să înțelegem starea procesului de actualizare a suitei Office (succes sau eroare cu detalii despre eroare)

Se colectează următoarele câmpuri:

- **build** - versiunea de Office instalată momentan

- **channel** - canalul prin care Office a fost distribuit

- **errorCode** - codul de eroare care indică eroarea

- **errorMessage** - informații suplimentare despre eroare

- **stare** - starea curentă a actualizării

- **targetBuild** - versiunea de Office la care este actualizată

#### <a name="officecompliancefileformatballotdisplayedonfirstboot"></a>Office.Compliance.FileFormatBallotDisplayedOnFirstBoot

Arată dacă i-a fost afișată utilizatorului caseta de dialog pentru alegerea Formatului de fișier Office la prima/a doua încărcare de Word, Excel, PowerPoint pe Win32.  Urmărește dacă este afișată caseta de dialog FileFormat Ballot - evenimentul este trimis la prima/a doua încărcare de Word, Excel sau PPT Win32.

Se colectează următoarele câmpuri.

- **CountryRegion** - setarea pentru regiunea de țară a utilizatorilor în sistemul Windows

- **FileFormatBallotBoxAppIDBootedOnce** - în ce aplicație (Word, Excel, PPT) a fost procesată logica de afișare pentru formatul fișierelor.

- **FileFormatBallotBoxDisplayedOnFirstBoot** - care este rezultatul afișării dialogului despre formatul fișierelor (afișat/nu este afișat în mod neașteptat/nu este afișat din cauza licenței/nu este afișat din cauza locației).

#### <a name="officecompliancefileformatballotoption"></a>Office.Compliance.FileFormatBallotOption

Urmărește dacă este afișată caseta de dialog FileFormat Ballot - evenimentul este trimis la prima/a doua încărcare de Word, Excel sau PPT Win32.  Arată dacă a fost afișată caseta de dialog pentru alegerea Formatului de fișier Office la prima sau la a doua încărcare de Word, Excel sau PowerPoint pe Win32.

Se colectează următoarele câmpuri:

- **FileFormatBallotSelectedOption** - identifică opțiunea formatului de fișier (OOXML/ODF) care a fost selectată de utilizator prin intermediul casetei de dialog despre formatul fișierelor.


#### <a name="officecorrelationmetadatautccorrelationmetadata"></a>Office.CorrelationMetadata.UTCCorrelationMetadata

Colectează metadatele Office prin UTC pentru a compara cu date echivalente, colectate prin canalul de telemetrie Office pentru a verifica corectitudinea și gradul de completitudine al datelor.

Se colectează următoarele câmpuri:

- **abConfigs** - ID-uri listă de caracteristici pentru a identifica acele caracteristici care sunt activate la client sau golite când aceste date nu sunt colectate.

- **abFlights** - „NoNL:NoFlights” atunci când caracteristicile flight nu sunt configurate. În caz contrar „holdoutinfo = unknown”.

- **AppSessionGuid** - identificator al unei anumite sesiuni de aplicație care începe la ora de creare a procesului și persistă până la sfârșitul procesului. Este formatat ca GUID standard pe 128 de biți, dar alcătuit din 4 părți. Aceste patru părți sunt, în ordine: (1) ID-ul de proces pe 32 de biți (2) ID-ul de sesiune pe 16 biți (3) ID-ul de inițializare pe 16 biți (4) timpul de creare a procesului pe 64 de biți în UTC 100ns

- **appVersionBuild** – Numărul de versiune al aplicației.

- **appVersionMajor** - numărul de versiune majoră al aplicației.

- **appVersionMinor** - numărul de versiune minoră al aplicației.

- **appVersionRevision** - numărul de versiune pentru revizuirea aplicației.

- **audienceGroup** - numele grupului public de lansare

- **audienceId** - numele grupului public de lansare

- **channel** - canalul prin care Office a fost distribuit

- **deviceClass** - factor de formă al dispozitivului din SO

- **ecsETag** - identificator de experiment pentru proces

- **impressionId** - GUID care indică spre setul curent de caracteristici.

- **languageTag** - eticheta de limbă curentă IETF UI Office

- **officeUserID** - GUID generat aleatoriu pentru această instalare Office

- **osArchitecture** - arhitectură a sistemului de operare

- **osEnvironment** - un întreg care indică sistemul de operare (Windows, Android, iOS, Mac etc).

- **osVersionString** - identificator al sistemului de operare

- **sessionID** - GUID generat aleator pentru a identifica sesiunea de aplicație

- **UTCReplace_AppSessionGuid** - valoare booleană constantă. Întotdeauna true.

#### <a name="officeonenotefirstrunfirstrun"></a>Office.OneNote.FirstRun.FirstRun

Semnal critic utilizat pentru a ne asigura că utilizatorii noi pot lansa și rula pentru prima dată cu succes OneNote.  Telemetria se colectează pentru a asigura detectarea regresiei critice pentru aplicația OneNote și starea serviciilor. Dacă utilizatorii nu pot lansa aplicația pentru prima dată, acest lucru va declanșa un incident de severitate înaltă.

- **AfterOneDriveFrozenAccountError** - indică o eroare din OneDrive atunci când un cont este blocat.

- **Attempt** - de câte ori este necesar să încercați din nou prima experiență de rulare.

- **IsDefaultNotebookCreated** - indică dacă OneNote a creat un blocnotes implicit de utilizator sau nu.

- **IsDelayedSignIn** - indică dacă prima rulare se află în modul de conectare întârziată, în care un utilizator nu este obligat să se conecteze.

- **IsMSA** - indică dacă un cont este cont Microsoft sau nu.

#### <a name="officeonenotefirstrunfirstrunformsa"></a>Office.OneNote.FirstRun.FirstRunForMSA

Semnal critic utilizat pentru a ne asigura că utilizatorii consumatori noi (cont Microsoft) pot lansa și utiliza pentru prima dată cu succes OneNote.

Telemetria utilizată pentru a asigura detectarea regresiei critice pentru aplicația OneNote și starea serviciilor. Dacă utilizatorii nu pot lansa aplicația pentru prima dată, acest lucru va declanșa un incident de severitate înaltă.

Se colectează următoarele câmpuri:

- **Attempt** - de câte ori este necesar să încercați din nou prima experiență de rulare.

- **Error A** - un obiect eroare din OneNote care indică o eroare în timpul primei execuții, dacă aceasta există.

- **FAllowAddingGuide** - indică dacă OneNote va permite crearea unui blocnotes ghid sau nu.

- **FrozenOneDriveAccount** - indică dacă un cont OneDrive este blocat sau nu.

- **IsDefaultNotebookCreated** - indică dacă OneNote a creat un blocnotes implicit de utilizator sau nu.

- **NoInternetConnection** - indică dacă un dispozitiv nu are conexiune la internet.

- **ProvisioningFailure** - un obiect eroare OneNote care indică o eroare de asigurare a accesului, dacă aceasta există.

- **ProvisioningFinishedTime** - indică ora de sfârșit când OneNote termină asigurarea accesului la un blocnotes în timpul primei experiențe de rulare.

- **ProvisioningStartedTime** - indică ora de început când OneNote inițiază asigurarea accesului la un blocnotes în timpul primei experiențe de rulare.

- **ShowSuggestedNotebooks** - indică dacă OneNote va afișa o caracteristică de blocnotes sugerată sau nu.

#### <a name="officeonenotefirstrunfirstrunfororgid"></a>Office.OneNote.FirstRun.FirstRunForOrgId

Semnal critic utilizat pentru a ne asigura că utilizatorii noi de tip întreprindere (AAD/OrgID) pot lansa și rula pentru prima dată cu succes OneNote.  Telemetria utilizată pentru a asigura detectarea regresiei critice pentru aplicația OneNote și starea serviciilor. Dacă utilizatorii nu pot lansa aplicația pentru prima dată, acest lucru va declanșa un incident de severitate înaltă.

- **Attempt** - de câte ori este necesar să încercați din nou prima experiență de rulare.

- **Error** - un obiect eroare din OneNote care indică o eroare în timpul primei execuții, dacă aceasta există.

- **FAllowAddingGuide** - indică dacă OneNote va permite crearea unui blocnotes ghid sau nu.

- **IsDefaultNotebookCreated** - indică dacă OneNote a creat un blocnotes implicit de utilizator sau nu.

- **ProvisioningFailure** - un obiect eroare OneNote care indică o eroare de asigurare a accesului, dacă aceasta există.

- **ProvisioningFinishedTime** - indică ora de sfârșit când OneNote termină asigurarea accesului la un blocnotes în timpul primei experiențe de rulare.

- **ProvisioningStartedTime** - indică ora de început când OneNote inițiază asigurarea accesului la un blocnotes în timpul primei experiențe de rulare.

#### <a name="officeonenotefirstrunmrureadernotebookentries"></a>Office.OneNote.FirstRun.MruReaderNoteBookEntries 

Semnalul folosit pentru a raporta probleme întâlnite când se încarcă blocnotesuri la prima rulare.  Telemetria se folosește pentru a monitoriza, a detecta și a rezolva orice problemă la prima rulare.

Se colectează următoarele câmpuri: 

- **OnPremNBCount** - Numărul blocnotesurilor în serverul local

- **TotalNBCount** - Numărul total de blocnotesuri asociat cu un cont de utilizator

#### <a name="officetargetedmessagingensurecached"></a>Office.TargetedMessaging.EnsureCached 

Urmărește dacă s-a descărcat un pachet pentru pânza dinamică. Considerat o configurare de software, deoarece pachetul trebuie descărcat cu succes pentru a activa clientul, astfel încât să redea experiența corectă. Este esențial mai ales în cazul abonamentelor pentru consumatori în care utilizăm pânza pentru a-i comunica utilizatorului că licența a expirat. Utilizat pentru a urmări metadatele unui pachet de conținut dinamic descărcat și memorat în cache de produs, precum și rezultatele operațiunilor efectuate în pachet: erori de descărcare, erori de despachetare, erori de verificare a consistenței, accesări ale memoriei cache, utilizări de pachet, surse de descărcare.

Se colectează următoarele câmpuri:

  - **Data\_CacheFolderNotCreated -** semnalizare booleană care indică dacă a reușit crearea folderului cache

  - **Data\_CdnPath - adresa sursei pachetului-**

  - **Data\_EnsureCached -** semnalizare booleană care indică dacă pachetul de conținut a fost memorat în cache

  - **Data\_ExistsAlready -** semnalizare booleană care indică faptul că pachetul a fost deja descărcat înainte și că a mai fost o încercare

  - **Data\_GetFileStreamFailed -** pachetul sursă nu este disponibil în sursă

  - **Data\_GetFileStreamFailedToCreateLocalFolder -** probleme disc local care determină apariția de erori la crearea directorului

  - **Data\_GetFileStreamFromPackageFailed -** semnalizare care indică dacă pachetul a fost descărcat, dar clientul nu îl poate citi

  - **Data\_GetFileStreamFromPackageSuccess -** încercări reușite de citire a pachetului

  - **Data\_GetFileStreamSuccess -** nici probleme legate de disc, nici probleme legate de configurație care să nu permită ca fluxul de fișier să fie citit

  - **Data\_GetRelativePathsFailed -** calea relativă nu indică spre locația accesibilă

  - **Data\_HashActualValue -** valoarea hash extrasă din numele de fișier atunci când a fost utilizat pachetul

  - **Data\_HashCalculationFailed -** eroare în legătură cu calcularea unui cod hash

  - **Data\_HashMatchFailed -** nepotrivirea codului hash între numele pachetului și valorile de registry memorate în cache

  - **Data\_HashMatchSuccess -** succes la verificarea consistenței codului hash

  - **Data\_PackageDownloadRequestFailed -** pachetul nu poate fi descărcat

  - **Data\_PackageDownloadRequestNoData -** pachetul descărcat nu conține date

  - **Data\_PackageDownloadRequestSuccess -** pachet descărcat cu succes

  - **Data\_PackageExplodedSuccess -** stări încercări de despachetare

  - **Data\_PackageOpenFailed -** încercări nereușite de a deschide fișierul pachet

  - **Data\_PackageOpenSuccess -** încercări reușite de a deschide fișierul pachet

  - **Data\_SuccessHashValue -** valoarea hash extrasă din numele de fișier când a fost descărcat pachetul

  - **Data\_SuccessSource -** suprafața pentru care pachetul a fost descărcat

#### <a name="officevisiovisiosku"></a>Office.Visio.VisioSKU

Capturează Visio SKU indiferent dacă este standard sau profesional. Esențial pentru a clasifica probleme bazate pe SKU.

Se colectează următoarele câmpuri:

  - **Data\_VisioSKU** : **integer** - 0 pentru SKU Standard și 1 pentru SKU Profesional

#### <a name="onenoteapponenotelaunchednonactivated-previous-name-officeonenoteandroidapponenotelaunchednonactivated"></a>OneNote.App.OneNoteLaunchedNonActivated *(nume anterior)* , Office.OneNote.Android.App.OneNoteLaunchedNonActivated

Informații înregistrate despre starea de activare a aplicației.  Datele sunt monitorizate pentru a ne asigura că identificăm spini în problemele de activare. De asemenea analizăm datele pentru a găsi zone care necesită îmbunătățiri.

Se colectează următoarele câmpuri: 

- **INSTALL_LOCATION** - Indică dacă aplicația este preinstalată sau este descărcată din Store

#### <a name="onenoteresetstatus-previous-name-officeonenoteandroidresetstatus"></a>OneNote.ResetStatus *(nume anterior)* , Office.OneNote.Android.ResetStatus

Semnalul folosit pentru a înregistra problemele întâlnite când un utilizator încearcă să reseteze aplicația.  Telemetria este folosită pentru a monitoriza, a detecta și a rezolva problemele cauzate în timpul resetării. 

Se colectează următoarele câmpuri: 

- **Accounts** - Indică tipurile de conturi folosite pentru a se loga în aplicație

- **Generic String Type** - Revine dacă există o resetare completă a notes_light_data reset

- **LaunchPoint** -Punctul de unde este inițiată resetarea. Valori posibile: butonul de deconectare, eroare de deconectare, Intune declanșat

- **Pass** - Indică dacă s-a resetat cu succes

#### <a name="onenotesigninsignincompleted-previous-name-officeonenoteandroidsigninsignincompleted"></a>OneNote.SignIn.SignInCompleted *(nume anterior)* , Office.OneNote.Android.SignIn.SignInCompleted

Semnalul critic folosit pentru a se asigura logarea cu succes sau nu. Telemetria este colectată pentru a se asigura detectarea regresia critică pentru aplicația OneNote și buna funcționare a serviciului

Se colectează următoarele câmpuri: 

- **CompletionState** - ultima stare de conectare- reușită sau eroare. Și cazurile de eroare

- **EntryPoint** - Indică de unde a fost inițiată conectarea

- **HResult** - Cod eroare

- **Provider Package ID** -În cazul conectării automate

- **Result** - succes, nereușit, necunoscut, anulat

- **ServerType** - returnează tipul de server care oferă serviciul 

- **SignInMode** - Conectare sau înregistrare sau conectare automată sau înregistrare accelerată

#### <a name="onenotesigninsigninstarted-previous-name-officeonenoteandroidsigninsigninstarted"></a>OneNote.SignIn.SignInStarted *(nume anterior)* , Office.OneNote.Android.SignIn.SignInStarted

Semnalul utilizat pentru a indica probleme întâlnite în timp ce utilizați bara de mesaje.  Telemetria este folosită pentru a monitoriza, a detecta și a rezolva problemele cauzate în interacțiunea cu bara de mesaje

Se colectează următoarele câmpuri: 

- **EntryPoint** - Indică de unde a fost inițiată conectarea

- **Result** - Rezultat flux de conectare

- **ServerType** - Returnează tipul de server care oferă serviciul 

- **SignInMode** - Conectare sau înregistrare sau conectare automată sau înregistrare accelerată


### <a name="office-add-in-configuration-subtype"></a>*Subtip configurație program de completare Office*

Programele de completare software și setările lor.

#### <a name="exceladdindefinedfunctioncustomfunctionsallinone"></a>Excel.AddinDefinedFunction.CustomFunctionsAllInOne

Colectează informații despre comportamentul în execuție al funcțiilor din programele de completare particularizate. Menține contoare pentru încercările de execuție, finalizările reușite, erorile de infrastructură și erorile de cod ale utilizatorului. Este utilizat pentru a identifica problemele de fiabilitate din produs și pentru a rezolva problemele care afectează utilizatorii.
 
Se colectează următoarele câmpuri:

- **AsyncBegin** - numărul de funcții asincrone inițiate

- **AsyncEndAddinError** - numărul de funcții asincrone care se termină cu o eroare

- **AsyncEndInfraFailure** - numărul de funcții asincrone care se termină cu erori infra.

- **AsyncEndSuccess** - numărul de funcții asincrone care se termină cu succes

- **AsyncRemoveCancel** - numărul de funcții asincrone care au fost anulate 

- **AsyncRemoveRecycle** - numărul de funcții asincrone care au fost eliminate din cauza reciclării 

- **StreamingCycles1** - contor de cicluri în flux

#### <a name="officeextensibilityappcommandsappcmdprojectionstatus"></a>Office.Extensibility.AppCommands.AppCmdProjectionStatus

Colectează informațiile pentru a urmări care instalări de programe de completare Office au actualizat cu succes panglica versus care nu au reușit.

Utilizat pentru a remedia problemele comune de înregistrare în care programele de completare nu sunt instalate corect și nu se afișează niciodată, drept pentru care sunt inutilizabile.

Se colectează următoarele câmpuri:

  - Fără

#### <a name="officeextensibilityappcommandsaddsolution"></a>Office.Extensibility.AppCommands.AddSolution

Colectează informațiile despre instalarea programelor de completare Office care particularizează panglica.  Utilizat pentru detectarea problemelor cu modul în care programele de completare particularizate modifică panglica Office.
 
Se colectează următoarele câmpuri:

- **AppVersion** - versiunea aplicației

- **SolutionId** - ID-ul soluției

- **StoreType** - indică originea aplicației


#### <a name="officeextensibilitycatalogexchangegetentitlements"></a>Office.Extensibility.Catalog.ExchangeGetEntitlements

Date privind succesul sau nereușita în ceea ce privește regăsirea datelor privind dreptul la programul de completare în cazul programelor de completare atribuite de administratorul de entitate găzduită Office 365. Utilizat pentru măsurători ale stării, diagrame și analiza problemelor clientului.

Se colectează următoarele câmpuri:

  - **CachingResult -** rezultatul încercării de a salva valoarea returnată a apelului de serviciu

  - **ClientParameter -** identificatorul clientului trimis în apelul de serviciu

  - **EntitlementsCount -** numărul de drepturi estimate în răspunsul la apel

  - **EntitlementsParsed -** numărul de drepturi analizate din răspuns

  - **IsAllEntitlementsParsed -** dacă numărul drepturilor estimate corespunde cu numărul de drepturi analizate

  - **ServiceCallHResult -** rezultatul returnat de API apel de serviciu

  - **TelemetryId -** GUID care reprezintă un utilizator unic

  - **UsedCache -** dacă s-a utilizat răspunsul memorat în cache în loc să se efectueze un apel de serviciu

  - **VersionParameter -** numărul de versiune de Office trimis în apelul de serviciu

#### <a name="officeextensibilitycatalogexchangegetlastupdate"></a>Office.Extensibility.Catalog.ExchangeGetLastUpdate

Date privind succesul sau nereușita în ceea ce privește regăsirea necesității unor date actualizate privind programele de completare atribuite de administratorul de entitate găzduită Office 365. Utilizat pentru măsurători ale stării, diagrame și analiza problemelor clientului. ExchangeGetLastUpdate va rula întotdeauna la inițializare ca parte a codului gazdă și va determina dacă atribuirile de program de completare s-au modificat pentru un utilizator.   Dacă da, atunci osf.DLL va fi încărcat, astfel încât să putem apela ExchangeGetEntitlements pentru a obține anumite atribuiri (și ExchangeGetManifests va fi apelat pentru a regăsi orice manifest nou care este necesar).   ExchangeGetEntitlements (și ExchangeGetManifests) pot fi apelate și la cerere după ce aplicația-gazdă a rulat.   Ideea este de a nu încărca DLL-ul mare în cazul în care nu este necesar.   Fără acest eveniment în Obligatoriu, nu am putea să spunem dacă utilizatorii nu reușesc să obțină programe de completare atribuite lor dacă primul apel de serviciu nu reușește.   Este, de asemenea, semnalul principal în orice problemă de autentificare cu care ne confruntăm când comunicăm cu serviciul nostru.

Se colectează următoarele câmpuri:

  - **Abort -** dacă gazda a închis în timpul apelului de serviciu

  - **AllowPrompt -** dacă s-a permis solicitare de autentificare

  - **AuthScheme -** schema de autentificare solicitată de exchange

  - **BackEndHttpStatus -** codul http raportat când se comunică cu exchange back end-

  - **BackupUrl -** al doilea URL exchange pentru a apela

  - **BEServer -** numele serverului back-end exchange

  - **CalculatedBETarget -** numele complet al computerului exchange back-end

  - **Call(n)\_TokenAuthError -** eroare de autentificare la încercare de apel de serviciu nth

  - **Call(n)\_TokenIsValid -** dacă simbolul de autentificare la încercarea de serviciu nth a fost valid

  - **CallMethod -** șir care indică ce cale a luat codul

  - **ConfigSvcReady -** dacă serviciul de configurare a fost deja inițializat

  - **Data -** valoare returnată de serverul exchange

  - **DiagInfo -** informații returnate de serverul Exchange

  - **End\_TicketAuthError -** orice eroare în obținerea biletului de autentificare după apelul de serviciu

  - **End\_TokenIsValid -** dacă biletul de autentificare este valabil după apelul de serviciu

  - **EndingIdentityState -** starea raportată a obiectelor de identitate după efectuarea apelurilor de serviciu

  - **EwsHandler -** valoare returnată de la exchange

  - **FEServer -** exchange front end care servisează solicitarea

  - **HResult -** codul rezultat

  - **HttpStatus -** codul stării Http returnat de la exchange

  - **IsSupportedAuthResponse -** dacă tipul de autentificare este unul pe care îl putem utiliza

  - **LastUpdateValueRegistry -** valoarea hash preluată de la registry

  - **LastUpdateValueRetrieved -** valoarea hash returnată de la apelul de serviciu

  - **MSDiagnostics -** valoarea returnată de la exchange

  - **MsoHttpResult -** valoarea enumeratorului returnată de la API http

  - **NeedRefresh -** acesta este un câmp true sau false, care indică dacă datele programului de completare au fost învechite și trebuie să le actualizăm.

  - **PrimaryUrl -** URL principal pentru a efectua apelul de serviciu către

  - **RequestId -** valoarea returnată de la exchange

  - **RequestTryCount -** de câte ori am încercat să facă efectuăm apelul de serviciu

  - **RequestTryCount -** de câte ori am încercat să comunicăm cu exchange

  - **ResultChain -** seriile codului de rezultat de la fiecare încercare a apelului de serviciu

  - **StartingIdentityState -** starea raportată a obiectelor de identitate înainte de efectuarea apelurilor de serviciu

  - **TelemetryId -** GUID care reprezintă un utilizator unic, dacă trebuie să efectuați alte apeluri de serviciu

#### <a name="officeextensibilitycatalogexchangegetmanifests"></a>Office.Extensibility.Catalog.ExchangeGetManifests

Date privind succesul sau nereușita în ceea ce privește regăsirea datelor manifestelor programului de completare pentru programele de completare atribuite de administratorul de entitate găzduită Office 365. Utilizat pentru măsurători ale stării, diagrame și analiza problemelor clientului.

Se colectează următoarele câmpuri:

  - **CachedManifestsParsed** - numărul de manifeste găsite în cache

  - **IsAllReturnedManifestsParsed** - dacă toate manifestele care au fost returnate au putut fi analizate

  - **ManifestsRequested** - numărul de manifeste necesare

  - **ManifestsReturned** – numărul de manifeste returnate de pe server

  - **ManifestsToRetrieve** – numărul de manifeste de obținut de pe server

  - **ReturnedManifestsParsed** - numărul de manifeste returnate de server care au fost analizate cu succes

  - **TelemetryId** - GUID care reprezintă un utilizator unic

#### <a name="officeextensibilityuxfensureloadosfdll"></a>Office.Extensibility.UX.FEnsureLoadOsfDLL 

Urmărește eroarea de încărcare Osf.DLL. Detectează eroarea de încărcare DLL care împiedică rularea caracteristicii.

Se colectează următoarele câmpuri:

  - Fără

#### <a name="officeextensibilityuxfensureloadosfuidll"></a>Office.Extensibility.UX.FEnsureLoadOsfUIDLL 

Urmărește eroarea de încărcare OsfUI.DLL. Detectează eroarea de încărcare DLL care împiedică rularea caracteristicii.

Se colectează următoarele câmpuri:

  - Fără

#### <a name="officeextensibilityuxfensureosfshareddllload"></a>Office.Extensibility.UX.FEnsureOsfSharedDLLLoad 

Urmărește eroarea de încărcare OsfShared.DLL. Detectează eroarea de încărcare DLL care împiedică rularea caracteristicii.

Se colectează următoarele câmpuri:

  - Fără

#### <a name="officeextensibilityvbatelemetrycomobjectinstantiated"></a>Office.Extensibility.VBATelemetryComObjectInstantiated

Colectează informații despre invocarea serverului de automatizare sau a clientului în soluții VBA. Utilizată pentru a înțelege interacțiunea dintre obiecte VBA și Com.

Se colectează următoarele câmpuri:

  - **ComObjectInstantiatedCount** - numărul de instanțieri obiect COM

  - **HashComObjectInstantiatedClsid** - cod hash al identificatorului de clasă obiect COM

  - **HashProjectName** - cod hash al numelui proiectului VBA

  - **TagId** - etichetă unică

#### <a name="officeextensibilityvbatelemetrydeclare"></a>Office.Extensibility.VBATelemetryDeclare 

Colectează informații despre invocarea Win32 API în soluții VBA. Utilizat pentru a înțelege interacțiunea dintre VBA și utilizare și pentru suplimentarea investigațiilor de securitate.

Se colectează următoarele câmpuri:

  - **DeclareCount** - numărul de declarații

  - **HashDeclare** - codul hash al numelui DLL

  - **HashEntryPoint** - codul hash al numelui API

  - **HashProjectName** - cod hash al numelui proiectului VBA

  - **IsPtrSafe** - dacă mențiunea din declarație este compatibilă pentru o arhitectură diferită

  - **TagId** - etichetă unică

#### <a name="officeoutlookdesktopadd-insadd-inloaded"></a>Office.Outlook.Desktop.Add-ins.Add-inLoaded

Colectează succesul și eșecul încărcării unui program de completare de către Outlook. Aceste date sunt monitorizate activ pentru a garanta că Outlook funcționează corect cu programele de completare ale clientului. Aceste date sunt utilizate pentru a detecta și investiga probleme.

Se colectează următoarele câmpuri:

  - **Activitate HVA standard** fără nicio sarcină particularizată

#### <a name="officeoutlookmacaddinapiusage"></a>Office.Outlook.Mac.AddinAPIUsage

Colectează succese și eșecuri ale execuției programului de completare în Outlook. Aceste date sunt monitorizate activ pentru a garanta că Outlook funcționează corect cu programele de completare. Aceste date sunt utilizate pentru a detecta și investiga probleme.

Se colectează următoarele câmpuri:

- **AccountType** - tipul de cont asociat cu programul de completare 

- **Cookie** - modul cookie utilizat de programul de completare

- **Despid** - identificator de expediere 

- **Endtime** - ora la care s-a încheiat programul de completare 

- **ExecutionTime** - perioada de executare a programului de completare 

- **Result** - rezultatul utilizării programului de completare în Outlook 

- **StartTime** - ora la care a început programul de completare


#### <a name="officeoutlookmacaddineventapisusage"></a>Office.Outlook.Mac.AddinEventAPIsUsage

Colectează succese sau eșecuri ale execuției programului de completare în Outlook. Aceste date sunt monitorizate activ pentru a garanta că Outlook funcționează corect cu programele de completare. Aceste date sunt utilizate pentru a detecta și investiga probleme.

Se colectează următoarele câmpuri:

- **AddinType** - tipul de program de completare 

- **EventAction** - acțiunea efectuată de programul de completare 

- **EventDispid** - identificator de expediere

- **EventResult** - rezultatul acțiunii efectuate de programul de completare 

#### <a name="officeoutlookmacaddininstallationfrominclientstore"></a>Office.Outlook.Mac.AddInInstallationFromInClientStore

Colectează succese sau eșecuri ale instalării programului de completare în Outlook. Aceste date sunt monitorizate activ pentru a garanta că Outlook funcționează corect cu programele de completare. Aceste date sunt utilizate pentru a detecta și investiga probleme.

Se colectează următoarele câmpuri:

- **AccountType** - tipul de cont asociat cu un program de completare 

- **FailureReason** - motivul pentru eșecul la instalarea programului de completare 

- **MarketplaceAssetId** identificator al programului de completare în magazin 

- **Status** - starea instalării programului de completare


#### <a name="officeprogrammabilityadd-insinternalsetconnectenterprise"></a>Office.Programmability.Add-ins.InternalSetConnectEnterprise

Eveniment generat atunci când un program de completare COM este încărcat pe un dispozitiv de întreprindere. 

Se colectează următoarele câmpuri:

  - **Rezultatul activității** - starea de succes a conexiunii

  - **Add-inconnectFlag** - comportamentul curent de încărcare

  - **Add-inId** - ID-ul clasei programului de completare

  - **Add-inTimeDateStamp** - marca de timp a programului de completare din metadatele DLL

  - **IsBootInProgress** - dacă aplicația Office se află în procesul de pornire

#### <a name="officevisiovisioaddonload"></a>Office.Visio.Visio.AddonLoad

Capturează erori atunci când o soluție nu reușește să se încarce. Esențial pentru a depana erorile de încărcare a programului de completare în Visio.

Se colectează următoarele câmpuri:

  - **Data\_Load1Error:integer** - valoarea de eroare în timpul încărcării programului de completare Visio

#### <a name="officevisiovisioaddonusage"></a>Office.Visio.Visio.AddonUsage

Capturează erori atunci când există o eroare în funcționalitatea soluției. Esențial pentru a depana erorile programului de completare în programe de completare.

Se colectează următoarele câmpuri:

  - **Data\_DocumentSessionLogID:string** - identificator sesiune document

  - **Data\_IsEnabled** : **bool** - true, dacă soluția este activată

  - **Data\_TemplateID:string** - GUID al șablonului în care a fost încărcată soluția. Conectat ca 0 pentru soluție particularizată

  - **Data\_AddOnID** : **string** - GUID pentru a identifica programul de completare încărcat

  - **Data\_Error** : **integer** - ID eroare

### <a name="security-subtype"></a>*Subtip de securitate*

Condițiile de eroare ale documentelor, caracteristicilor și programelor de completare care pot compromite securitatea, inclusiv pregătirea pentru actualizarea produselor.

#### <a name="officeappguardcreatecontainer"></a>Office.AppGuard.CreateContainer

Colectăm coduri de eroare și dacă containerul exista deja sau nu. De asemenea, colectăm coduri de eroare pentru un eveniment de resetare, în caz că nu reușim să creăm containerul la prima încercare. Datele vor fi utilizate pentru a identifica procentul de sesiuni prin care am creat cu succes containerul pentru lansarea aplicațiilor Protecție aplicații Office. De asemenea, datele vor permite ca Microsoft să identifice și să abordeze codurile de eroare din crearea containerului.

Se colectează următoarele câmpuri:

- **ErrorCode1** - Tipul codului de eroare din configurarea containerului.  

- **ErrorCode2** - Codul de eroare din executarea creării. 

- **ErrorCode3** - Codul de eroare suplimentar. 

- **ID** - Un identificator unic (GUID) pentru crearea containerului.

- **ResetError** - Codul de eroare de la încercarea de a reseta containerul după o încercare nereușită.

- **ResetErrorCode1** - Tipul codului de eroare din configurarea containerului după comanda de resetare. 

- **ResetErrorCode2** - Codul de eroare din executarea creării după comanda de resetare.

- **ResetErrorCode3** - Codul de eroare suplimentar după comanda de resetare.

- **ResetErrorType** - Tipul de eroare în timpul resetării: Creare, Pregătire fișier sau Lansare.

- **WarmBoot** - Identifică dacă containerul a fost creat deja sau nu.

#### <a name="officeappguardlaunchfile"></a>Office.AppGuard.LaunchFile

Acest eveniment indică rezultatul unei executări de lansare a fișierului din Protecție aplicații. Vom putea defini procentul de sesiuni în care am lansat un fișier Word, Excel sau PowerPoint și codurile de eroare pentru încercările eșuate.

Se colectează următoarele câmpuri:

- **AppId** - Identifică ce aplicație este lansată.

- **DetachedDuration** - Identifică timpul total în care a fost efectuată activitatea îmbinată. 

- **ErrorCode1** - Tipul codului de eroare din configurarea containerului.  

- **ErrorCode2** - Codul de eroare din executarea creării. 

- **ErrorCode3** - Codul de eroare suplimentar. 

- **FileId** - Un Identificator unic (GUID) a fost returnat din Windows API după lansarea unui fișier.

- **ID** - Un Identificator unic (GUID) pentru lansarea și crearea unui fișier. Acest ID este utilizat pentru a corela evenimente din Office și Windows.

- **ResetError** - Codul de eroare de la încercarea de a reseta containerul după o încercare nereușită.

- **ResetErrorCode1** - Tipul codului de eroare din configurarea containerului după comanda de resetare. 

- **ResetErrorCode2** - Codul de eroare din executarea comenzii de creare după resetare.

- **ResetErrorCode3** - Codul de eroare suplimentar după comanda de resetare.  

- **ResetErrorType** - Tipul de eroare: Creare, PrepFile sau Lansare.



#### <a name="officesecurityactivationfilterclsidactivated"></a>Office.Security.ActivationFilter.CLSIDActivated

Urmărește momentul în care un identificator de clasă specific (Flash, Silverlight etc.) este activat în Office. Utilizat pentru a urmări impactul blocării controalelor Flash, Silverlight și Shockwave asupra utilizatorilor finali.

Se colectează următoarele câmpuri:

  - **ActivationType** - tip de activare pentru control

  - **Blocked** - a fost controlul blocat de Office

  - **CLSID** - identificator de clasă al controlului

  - **Count** - de câte ori a fost activat controlul

#### <a name="officesecurityactivationfilterfailedtoregister"></a>Office.Security.ActivationFilter.FailedToRegister

Urmărește o condiție de eroare în atenuarea securității care blochează activarea unor controale periculoase în Office.

Utilizat pentru a diagnostica condițiile de eroare în atenuarea securității care ar putea afecta securitatea utilizatorilor finali.

Se colectează următoarele câmpuri:

  - Fără

#### <a name="officesecuritycomsecurityfileextensionlistfromservice"></a>Office.Security.ComSecurity.FileExtensionListFromService

Urmărește dacă extensiile de blocare ale arhivatorului au fost citite din serviciul de configurare sau am utilizat lista implicită a clientului. Utilizat pentru a garanta eficiența atenuării securității care protejează utilizatorii finali ai Office.

Se colectează următoarele câmpuri:

  - **RetrievedFromServiceStatus** - am reușit să preluăm lista de extensii de fișier pentru blocare; în caz contrar care a fost cauza erorii

#### <a name="officesecuritycomsecurityload"></a>Office.Security.ComSecurity.Load

Urmărește când un obiect OLE este încărcat într-un document. Utilizat pentru a garanta eficiența atenuării securității care protejează utilizatorii finali ai Office.

Se colectează următoarele câmpuri:

  - **Clsid** - identificator de clasă al controlului OLE

  - **Count** - de câte ori s-a încărcat controlul OLE

  - **DocUrlHash** - cod hash care reprezintă în mod unic documentul. (Notă: nicio modalitate de a afla detaliile reale ale documentului din aceasta. Este doar o reprezentare unică a documentului.)

  - **IsCategorized** - a fost controlul OLE clasificat pentru încărcare în Office

  - **IsInsertable** - poate fi controlul OLE inserat sau nu

#### <a name="officesecuritycomsecurityobjdetected"></a>Office.Security.ComSecurity.ObjDetected

Urmărește când un obiect OLE este detectat într-un document. Utilizat pentru a garanta eficiența atenuării securității care protejează utilizatorii finali ai Office.

Se colectează următoarele câmpuri:

  - **Clsid** - identificator de clasă al controlului OLE

  - **Count** - de câte ori a fost detectat acest obiect OLE

  - **DocUrlHash** - cod hash care reprezintă în mod unic documentul. (Notă: nicio modalitate de a afla detaliile reale ale documentului din aceasta. Este doar o reprezentare unică a documentului.)

  - **IsCategorized** - este controlul OLE clasificat pentru încărcare în Office

  - **IsInsertable** - poate fi controlul OLE inserat sau nu

#### <a name="officesecuritycomsecuritypackageractivation"></a>Office.Security.ComSecurity.PackagerActivation

Urmărește rezultatul atenuării securității care blochează extensii periculoase încorporate în documente Office. Utilizat pentru a garanta eficiența atenuării securității care protejează utilizatorii finali ai Office.

Se colectează următoarele câmpuri:

  - **FromInternet** - a fost documentul de pe internet

  - **PackagerSetting** - care a fost setarea arhivatorului curent

  - **TrustedDocument** - a fost documentul un document de încredere

#### <a name="officesecuritycomsecuritypackageractivationerrors"></a>Office.Security.ComSecurity.PackagerActivationErrors

Urmărește condițiile erorii în atenuarea securității care blochează extensii periculoase încorporate în documente Office. Utilizat pentru a garanta eficiența atenuării securității care protejează utilizatorii finali ai Office.

Se colectează următoarele câmpuri:

  - **Error** - cod de eroare

  - **Extension** - care era extensia fișierului

  - **FromInternet** - a fost documentul de pe internet

  - **LinkedDocument** - era un document legat sau nu

  - **PackagerSetting** - care a fost setarea arhivatorului curent

  - **TrustedDocument** - a fost documentul de încredere


#### <a name="officesecuritymacrointernetvbablockenabled"></a>Office.Security.Macro.InternetVBABlockEnabled

Urmărește dacă macrocomanda de blocare din setarea internetului este activată la un client. Evaluați utilizarea atenuării securității pentru a vă proteja împotriva macrocomenzilor rău intenționate.

Se colectează următoarele câmpuri:

  - Fără

#### <a name="officesecuritymacropolicydigsigtrustedpublishers"></a>Office.Security.Macro.PolicyDigSigTrustedPublishers

Urmărește dacă s-a verificat faptul că macrocomanda provine de la un editor de încredere. Utilizat pentru a garanta eficiența atenuării securității care protejează utilizatorii finali ai Office.

Se colectează următoarele câmpuri:

  - **Policy** - este politica setată sau nu sau nu este disponibilă

#### <a name="officesecuritymacroprompted"></a>Office.Security.Macro.Prompted

Urmărește când i se solicită unui utilizator să activeze macrocomenzile VBA. Utilizat pentru a evalua prevalența macrocomenzilor VBA și a antrena atenuări de securitate viitoare care restricționează executarea macrocomenzilor ca răspuns la incidentele de securitate.

Se colectează următoarele câmpuri:

  - **PromptType** -ce tip de solicitare a fost afișată

  - **VBAMacroAntiVirusHash** - cod hash antivirus al macromenzii

  - **VBAMacroAntiVirusHRESULT** - rezultatul evaluării antivirus

#### <a name="officesecuritymacrovbasecureruntimesessionenablestate"></a>Office.Security.Macro.VBASecureRuntimeSessionEnableState

Urmărește fiecare verificare a momentului execuției AMSI efectuată atunci când se execută o macrocomandă. Urmărește eficiența verificării momentului execuției AMSI aferente executării macrocomenzii și identifică erorile care ar putea afecta securitatea utilizatorilor finali.

Se colectează următoarele câmpuri:

  - **IsRegistry** - a setat administratorul o anumită înlocuire în registry

  - **State** - care este starea pentru un moment de execuție sigur

#### <a name="officesecuritymacroxl4prompted"></a>Office.Security.Macro.XL4Prompted

Urmărește când i se solicită unui utilizator să activeze macrocomenzile XL4. Utilizat pentru a evalua prevalența macrocomenzilor XL4 în Excel pentru a antrena atenuări de securitate viitoare care blochează XL4 în mod implicit ca răspuns la incidentele de securitate care implică folosirea abuzivă a macrocomenzilor XL4.

Se colectează următoarele câmpuri:

  - **PromptType** -ce tip de solicitare a fost afișată


#### <a name="officesecurityocxufiprompt"></a>Office.Security.OCX.UFIPrompt

Urmărește când i se afișează utilizatorului o solicitare de securitate la încărcarea unui control ActiveX, care este marcat Nesigur pentru inițializare. Utilizat pentru a urmări prevalența controalelor UFI ActiveX din documentele Office pentru a antrena atenuări (de ex., controalele killbitting) ca răspuns la incidentele de securitate.

Se colectează următoarele câmpuri:

  - **IsFromInternet** - este documentul deschis de pe internet

  - **IsSecureReaderMode** - este documentul deschis într-un cititor sigur

  - **OcxTrustCenterSettings** - care este setarea ActiveX curentă


#### <a name="officesecuritysecurereaderhostopeninosr"></a>Office.Security.SecureReaderHost.OpenInOSR

Urmărește finalizarea unei deschideri în Vizualizarea protejată. Utilizat pentru a diagnostica condiții care conduc la erori când deschiderea fișierelor în Vizualizarea protejată afectează securitatea și productivitatea clienților.

Se colectează următoarele câmpuri:

  - Fără

## <a name="product-and-service-usage-data-events"></a>Evenimente cu date despre utilizarea produselor și a serviciilor

Iată subtipurile de date din această categorie:

- [Succesul caracteristicii aplicației](#application-feature-success-subtype)
- [Starea aplicației și inițializare](#application-status-and-boot-subtype)
- [Configurație accesibilitate Office](#office-accessibility-configuration-subtype)
- [Confidențialitate](#privacy-subtype)


### <a name="application-feature-success-subtype"></a>*Subtip privind succesul caracteristicii aplicației*

Succesul funcționalității aplicației. Limitat la deschiderea și închiderea aplicației și a documentelor, editarea fișierelor și partajarea fișierelor (colaborare).

#### <a name="accountaction"></a>account.action

Necesar pentru a garanta funcționarea cu succes a configurării contului și este utilizat pentru a monitoriza starea creării contului, capacitatea de a adăuga noi conturi de e-mail și de a monitoriza resetări soft de cont 

Se colectează următoarele câmpuri: 

- **account_calendar_count** - câte calendare are contul
 
- **action** - tip de acțiune efectuată, de ex. create_account, delete_account.
 
- **duration_seconds** - durata acțiunii
 
- **entry_point** - punct de intrare al acțiunii, cum a început utilizatorul acțiunea
 
- **has_hx** - dacă dispozitivul are un cont care utilizează noul nostru serviciu de sincronizare a corespondenței, nu neapărat contul în care s-a efectuat acțiunea
 
- **is_hx** - este contul care utilizează noul nostru de sincronizare a corespondenței
 
- **is_shared_mailbox** - dacă acțiunea se referă la o cutie poștală partajată
 
- **number_of_accounts** - numărul total de conturi în care s-a efectuat acțiunea
 
- **result** - rezultatul acțiunii, de ex. succes, eșec.
   
- **server_type** - tipul de server pentru cont, asemănător cu account_type
 
- **shared_type** - tipul de cont partajat (în cazul în care contul este partajat)
 
- **scope** - scopul acțiunii; pentru ștergerea contului, this_device sau all_devices
 
- **total_calendar_accounts** - numărul de conturi de calendar din aplicație în momentul acțiunii
 
- **total_email_accounts** - numărul de conturi de e-mail din aplicație în momentul acțiunii
 
- **total_file_accounts** - numărul de conturi de fișier din aplicație în momentul acțiunii

#### <a name="accountlifecycle"></a>account.lifecycle

Acest eveniment este colectat pentru a garanta funcționarea cu succes a configurării contului și este utilizat pentru a monitoriza starea creării contului, capacitatea de a adăuga noi conturi de e-mail și de a monitoriza resetări soft de cont

Se colectează următoarele câmpuri: 

- **action** - Tipul de acțiune efectuată asupra contului, cum ar fi adăugare, eliminare sau resetare

#### <a name="addnewaccountstep"></a>add.new.account.step

Acest eveniment ne permite să detectăm cât de departe a ajuns utilizatorul în formularul de creare a unui nou cont.  Indică când utilizatorul s-a mutat în alt pas sau dacă s-a retras.  Avem nevoie de aceste informații pentru a detecta dacă orice pași eșuează și pentru a vă asigura că crearea conturilor de utilizator a reușit. 

Următorul câmp este colectat: 

- **OTAddAccountCurrentStep** - care poate avea următoarele valori: profile_form, redirect_mobile_check, mobile_check_success

#### <a name="apperror"></a>app.error

Urmărește erorile critice ale aplicației utilizate astfel încât să putem preveni problemele care ar putea duce la căderea aplicației sau care ar putea să vă împiedice să citiți e-mailurile.

Se colectează următoarele câmpuri: 

- **clientName** - numele clientului pentru fișierul din cloud în care s-a produs eroarea, dacă se aplică.

- **cloudfile_error_type** - tipul de eroare care s-a produs pentru fișierul din cloud, dacă se aplică.

- **cloudfile_response_name** - numele răspunsului pentru eroarea care s-a produs pentru fișierul din cloud, dacă se aplică.

- **component_name** - numele componentei aplicației în care s-a produs eroarea, cum ar fi corespondența sau calendarul.

- **debug_info** - informații despre eroarea care a apărut pentru fișierul din cloud pentru a putea să stabiliți motivul pentru care s-a produs eroarea.

- **error_origin_identifier** - originea erorii care s-a produs în schița în care s-a produs eroarea, dacă se aplică.

- **error_type** - tipul de eroare care s-a produs. Unele exemple includ salvarea schiței, trimiterea schiței și eroarea din fișierul din cloud.

- **exdate** - data extinsă a regulii (se aplică numai erorilor de recurență a rezervării) *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în compilările mai vechi.]*

- **exrule** - valoarea extinsă a regulii (se aplică numai erorilor de recurență a rezervării) *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în compilările mai vechi.]*

- **has_attachments** - arată dacă schița în care s-a produs eroarea are atașări, dacă se aplică.

- **is_IRM_protected** - arată dacă schița în care s-a produs eroarea este protejată de Information Rights Management, dacă se aplică.

- **is_legitimate** - arată dacă eroarea provine dintr-o eroare de programare sau nu. Erorile de programare sunt considerate neligitime.

- **is_local** - arată dacă schița în care s-a produs eroarea s-a sincronizat la server, dacă se aplică.

- **is_recoverable** - arată dacă eroarea poate fi recuperată sau dacă este o eroare fatală.

- **rdate** - data recurenței regulii (se aplică numai erorilor de recurență a rezervării) *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în compilările mai vechi.]*

- **rrule** - regula de recurență însăși (se aplică numai erorilor de recurență a rezervării) *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în compilările mai vechi.]*

- **rrule_error_message** - mesajul de eroare a regulii de recurență (se aplică numai erorilor de recurență a rezervării) *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în compilările mai vechi.]*

- **rrule_error_type** - tipul de eroare a regulii de recurență (se aplică numai erorilor de recurență a rezervării) *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în compilările mai vechi.]*

- **status_code** - codul de stare al erorii care s-a produs. Aceasta ne ajută să înțelegem cauza erorii.

Toate caracterele sunt posibile proprietăți. Aceasta ne ajută să înțelegem caracterele din corpul mesajului de schiță în care s-a produs eroarea. De exemplu, „a”, „b”, „c” sunt posibile proprietăți.

#### <a name="applaunchreport"></a>app.launch.report

Acest eveniment ne permite să detectăm și să remediem probleme în care Outlook pornește lent sau incomplet, îngreunând utilizarea aplicației de către utilizatori. Acesta include informații despre caracteristici specifice care au fost activate și despre durata de pornire al părților.

Se colectează următoarele câmpuri: 

- **is_agenda_widget_active** - ne spune dacă widgetul agendă este activ.

- **is_alert_available** - ne spune dacă aplicația a fost configurată ca să permită alerte în notificări.

- **is_background_refresh_available** - ne spune dacă aplicația a fost configurată ca să poată împrospăta fundalul.

- **is_badge_available** - ne spune dacă aplicația a fost configurată ca să permită ecusoane în notificări.

- **is_intune_managed** - ne spune dacă aplicația este gestionată de Intune.

- **is_registered_for_remote_notifications** - ne spune dacă aplicația a fost înregistrată pentru notificări de la distanță.

- **is_sound_available** - ne spune dacă aplicația a fost configurată ca să permită sunete în notificări.

- **is_watch_app_installed** - ne spune dacă a fost instalată aplicația Outlook pentru telefon.

- **is_watch_paired** - ne spune dacă aplicația Outlook pentru telefon este asociată cu aplicația Outlook principală.

- **launch_to_db_ready_ms** - ne spune timpul petrecut de aplicația Outlook de la lansare la baza de date pentru a fi gata.

- **num_calendar_accounts** - ne spune numărul de conturi de calendar din aplicație.

- **num_cloud_file_accounts** - ne spune numărul de conturi de stocare din aplicație.

- **num_hx_calendar_accounts** - ne spune numărul de conturi de calendar din aplicație care se conectează la noul nostru serviciu de sincronizare a corespondenței.

- **num_hx_mail_accounts** - ne spune numărul de conturi de e-mail din aplicație care se conectează la noul nostru serviciu de sincronizare a corespondenței.

- **num_mail_accounts** - ne spune numărul de conturi de e-mail din aplicație.

#### <a name="calendaraction"></a>calendar.action

Este utilizat cu scopul de a monitoriza orice impact posibil negativ asupra capacității dvs. de a efectua acțiuni de calendar de bază, cum ar fi crearea sau editarea evenimentelor.  Evenimentul ar putea include și o serie de nume de proprietate și dacă s-au modificat sau nu. De exemplu, „title_changed”, „online_meeting_changed” și „description_changed” sunt nume de proprietăți incluse pentru a ne ajuta să înțelegem dacă există probleme la editarea anumitor proprietăți.

Se colectează următoarele câmpuri: 

- **account_sfb_enabled** - ne ajută să ne asigurăm că Skype for Business este configurat corect. 

- **action** - tipul de acțiune efectuat în calendar. Aceasta include lucruri cum ar fi deschiderea, editarea, adăugarea comenzilor rapide, amânarea etc. Ne ajută să ne asigurăm că experiența noastră de calendar funcționează așa cum vă așteptați și că nu s-a întrerupt 

- **action_result** - rezultatul acțiunii întreprinse în cazul componentelor de calendar. Aceasta poate include valori cum ar fi succes, eșec, necunoscut și timp de expirare. Utilizate pentru a urmări rata de succes a acțiunilor și a determina dacă există o problemă răspândită privind acțiunile din calendar. 

- **attendee_busy_status** - starea liber/ocupat a participantului la care este corelată acțiunea. Această valoare poate fi Liber, Ocupat sau Încercare. Ne ajută să înțelegem dacă există o problemă în legătură cu acțiunile asociate unei anumite stări Ocupat. 

- **availability** - valoarea de disponibilitate dacă valoarea liber/ocupat s-a modificat la întâlnire. Ne ajută să înțelegem dacă există probleme privind setarea unei anumite valori de disponibilitate. 

- **calendar_onlinemeeting_default_provider** - conține furnizorul de întâlnire online implicit pentru utilizare cu crearea de întâlniri online acceptate de server. Printre acestea se numără tipurile de Skype, Skype for Business, Hangout și Teams for Business. Ne ajută să diagnosticăm probleme potențiale privind crearea de întâlniri online în cazul anumitor furnizori. 

- **calendar_onlinemeeting_enabled** - adevărat în cazul în care calendarul acceptă crearea de întâlniri online acceptate de server pe baza unui furnizor de întâlnire online implicit. Ne ajută să înțelegem dacă există probleme privind calendarele de întâlnire activate online. 

- **calendar_type** - tipul de calendar în care se află un eveniment după ce utilizatorul a editat întâlnirea. Între valorile posibile se numără principal, secundar, partajat și grup. Ne ajută să înțelegem dacă există probleme privind un anumit tip de calendar. 

- **delete_action_origin** - originea acțiunii de ștergere efectuate. Aici sunt incluse valori, cum ar fi bara de navigare, bara de instrumente și bara de instrumente pentru capsule.  Ne ajută să înțelegem dacă există probleme privind ștergerea unei întâlniri dintr-o anumită locație. 

- **distribution_list_count** - numărul de participanți care se află pe liste de distribuire. Ne ajută să urmărim dacă există probleme privind participanții de pe listele de distribuire. 

- **guest_count** - numărul de persoane din întâlnire.  Ne ajută să ne asigurăm că invitații sunt adăugați corect. 

- **is_all_day** - utilizat împreună cu „meeting_duration” pentru a specifica dacă aceasta este o întâlnire de o zi întreagă. Ne ajută să înțelegem dacă există probleme privind acțiunile efectuate pentru întâlnirile de o zi întreagă. 

- **is_location_permission_granted** - dacă utilizatorul a acordat permisiunea de locație a sistemului la aplicație. Dacă permisiunea pentru locație este acordată, aplicația poate afișa informații despre utilitate suplimentare în interfața cu utilizatorul. Cunoscând dacă permisiunea de locație este acordată ne permite să aflăm cât de des se afișează utilizatorilor informațiile suplimentare despre utilitate.

- **is_organizer** - ne ajută să înțelegem dacă întâlnirile pot fi editate și create corect de către organizator. 

- **is_recurring** - ne ajută să înțelegem dacă există o problemă care influențează în mod specific întâlnirile recurente. 

- **launch_point** - punctul de lansare a acțiunii. Pot fi valori cum ar fi antet widget, subsol widget, widget toată ziua și comandă rapidă pentru calendar. Ne ajută să înțelegem contextul de la care a început acțiunea. 

- **location_count** - numărul de locații setate la crearea și editarea evenimentului. Ne ajută să înțelegem dacă există probleme privind crearea sau editarea evenimentelor cu un anumit număr de locații. 

- **location_selection_source_type** - tipul sursei de selectare a locației. Acesta poate include valori cum ar fi sugestia de locație, particularizat și existent. Ne ajută să diagnosticăm toate problemele întâmpinate la selectarea unei locații de la o anumită sursă. 

- **location_session_id** - ID-ul sesiunii de selectare a locației de întâlnire. Ne ajută să diagnosticăm toate problemele întâmpinate la alegerea unei locații de adăugat la întâlnire. 

- **location_type** - tipul de locație selectat.  Conține tipuri cum ar fi locația particularizată, sală de conferințe și Bing. Ne ajută să înțelegem problemele privind adăugarea anumitor tipuri de locație la întâlnire. 

- **meeting_duration** - durata întâlnirii.  Ne ajută să ne asigurăm că întâlnirile sunt configurate cu orele corecte. 

- **meeting_insights_type** - tipul de detalii despre întâlnire în detaliile evenimentului.  Printre acestea se numără fișierul și mesajul. Ne ajută să înțelegem numărul de detalii de întâlnire care sunt afișate. 

- **meeting_type** - tipul de întâlnire online asociată cu acțiunea.  Printre acestea se numără tipurile de Skype, Skype for Business, Hangout și Teams for Business. Ne ajută să înțelegem dacă întâlnirile online sunt configurate corect. 

- **origin** - originea acțiunii din calendar. Printre acestea se numără tipuri cum ar fi agendă, calendar, agendă widget etc. Ne ajută să ne asigurăm că interacțiunea la nivelul componentelor de calendar funcționează corect 

- **recurrence_scope** - tipul de recurență al întâlnirii, fie recurență, fie serie.  Ne ajută să înțelegem dacă există probleme privind editarea diferitelor tipuri de recurență a întâlnirii. 

- **reminder_time** - ora pentru memento pentru întâlnire, dacă s-a modificat.  Se utilizează pentru a vă asigura că ora de memento pentru întâlnire este salvată corect. 

- **reminders_count** - numărul de mementouri pentru eveniment dacă s-au modificat mementourile. Ne ajută să diagnosticăm toate problemele privind mai multe mementouri pentru un eveniment. 

- **sensitivity** - sensibilitatea întâlnirii. Printre acestea se numără tipurile normal, personal, privat și confidențial. Ne ajută să înțelegem dacă sensibilitatea întâlnirii este configurată corect. 

- **session_duration** - durata sesiunii a fost socotită în milisecunde. Ne ajută să înțelegem dacă există probleme care măresc perioada de timp necesară pentru a efectua acțiunea din calendar. 

- **shared_calendar_result** - rezultatul unei acțiuni efectuate într-un calendar partajat. Între valorile posibile se numără Ok, Fără permisiune, Necunoscut, Proprietar local, iar proprietarul este Grup. Ne ajută să înțelegem fiabilitatea acțiunilor efectuate în calendarele partajate. 

- **time_picker_origin** - originea selectorului de timp pentru o acțiune de salvare. Include valori, cum ar fi mai multe opțiuni și mai puține opțiuni. Ne ajută să înțelegem cum a navigat utilizatorul în flux pentru a salva întâlnirea și a vă asigura că funcționează corect 

- **title** - titlul sugerat automat de valori definite de aplicație. Printre acestea se numără valori, cum ar fi „Apel”, „Prânz” și „Skype”. Ne ajută să înțelegem dacă sugestia automată pentru titlu este configurată corect. 

- **txp** - tipul de rezervare sau de rezervare la eveniment, dacă există. Acest lucru include tipuri cum ar fi rezervarea evenimentului, rezervarea unui zbor, închirierea unei mașini etc. Ne ajută să înțelegem dacă fișele de rezervare funcționează corect. 

- **upcoming_event_count** - numărul de evenimente viitoare afișate în vizualizarea Evenimente viitoare. Ne ajută să înțelegem dacă există probleme privind vizualizarea de evenimente viitoare. 

- **upcoming_event_seconds_until_event** - numărul de secunde până la începerea următorului eveniment. Ne ajută să înțelegem evenimentele tipice, afișate în vizualizarea Evenimente viitoare. 

- **value** - detaliu specific acțiunii, cum ar fi durata întârzierii alertei sau categoria repetare-până la. Ne ajută să înțelegem contextul în care a fost efectuată acțiunea. 

#### <a name="combinedsearchuse"></a>combined.search.use

Este utilizat pentru a monitoriza posibilul impact negativ asupra capacității dvs. de a efectua funcționalități de căutare-cheie, cum ar fi căutarea de e-mailuri, persoane de contact sau evenimente.

Se colectează următoarele câmpuri pentru Android: 

- **account_switcher_action_type** - acest tip de acțiune urmărește dacă utilizatorul a utilizat comutatorul de cont în descoperire sau dacă s-a decis să comute între conturi

- **action_type** - tipul de acțiune efectuat pentru căutare. Acest lucru identifică dacă o căutare a fost începută, este în curs sau s-a încheiat și ce acțiuni au fost întreprinse în timpul căutării, de exemplu, dacă a fost utilizat un microfon. Acest lucru este esențial pentru a asigura căutări precise și utile. 

- **conversation_id** - ID unic pentru fiecare sesiune de căutare (de exemplu, de fiecare dată când utilizatorul intră în caseta de căutare)

- **entrance_type** - acesta determină modul în care utilizatorul a început interogarea de căutare, din fila Căutare, interogare zero, titlu de căutare sau rezultat de căutare. 

- **has_contact_results** - simplu dacă sunt afișate sau nu rezultate de contact în interogarea de căutare

- **include_deleted** - în cazul în care căutarea afișează opțiunile șterse în rezultatele căutării 

- **is_ics_external_data** - capturează dacă un eveniment adăugat este intern (adică adăugat în Outlook la calendarul Outlook) sau extern (adică adăugată din altă aplicație de e-mail, cum ar fi Gmail la calendarul Outlook).

- **is_network_fully_connected** - valoare utilizată pentru a obține un indiciu despre motivul din spatele căutării offline. Dacă rețeaua este conectată și căutarea este offline, motivul poate fi expirarea serverului

- **is_offline_search** - dacă sesiunea de căutare este căutarea offline pe baza rezultatelor de căutare returnate de HX

- **re_enter_search_tab** - valoarea booleană pentru a indica dacă un utilizator a comutat între file înainte de a selecta un rezultat de căutare

- **result_selected_type** - cu ce tip de date care au fost afișate interacționează utilizatorul de ex. vedeți toată persoanele de contact, conversațiile, evenimentul etc. 

- **search_conversation_result_data** - conține date despre conversația selectată dintr-un rezultat de căutare, inclusiv tipul de cont (hx, ac etc.), dacă mesajul este deținut de un serviciu în cloud și dacă deplasarea paginii afișate este aceeași pagină cu primul mesaj. 

- **search_origin** - de unde provine căutarea, de ex. asistentul vocal, Cortana, intrarea de la tastatură etc. 

- **search_scope** - un șir care indică tipul de cont pe care îl căuta utilizatorul (de ex., Exchange, Gmail etc.) sau dacă a fost în Toate conturile. 

- **search_suggestion_type** - indică ce se află în spatele sugestiei de căutare, de ex., este o corecție ortografică? Pe baza istoricului? Completare automată?

- **search_request_reason** - indică motivul pentru care a fost trimisă o solicitare de căutare din aplicație, indicând, de fapt, componenta sau acțiunea utilizatorului care a invocat o căutare.

- **search_result_filter_type** - indică ce tip de filtru a fost aplicat pentru căutare, afișare totală sau doar atașări

Următoarele câmpuri sunt colectate în aplicațiile iOS ale Outlook Mobile: 

- **action** - tipul de acțiune efectuat pentru căutare. Acest lucru identifică dacă o căutare a fost începută, este în curs sau s-a încheiat și ce acțiuni au fost întreprinse în timpul căutării, de exemplu, dacă a fost utilizat un microfon. Acest lucru este esențial pentru a asigura căutări precise și utile.

- **answer_result_selected_count** - urmărește de câte ori căutarea a fost „reușită”, de exemplu dacă utilizatorul a găsit persoana pe care o căuta? Ați compus un mesaj de e-mail? Ați marcat mesajul în document? 

- **contact_result_in_full_list_selected_count** - urmărește de câte ori a cerut utilizatorul „Vedeți toate persoanele de contact” din lista completă în timpul sesiunii de căutare combinate

- **contact_result_selected_count** - urmărește numărul de persoane de contact care au fost selectate în timpul sesiunii de căutare combinate

- **conversation_result_selected_count** - urmărește câte conversații au fost selectate în timpul sesiunilor de căutare combinate

- **mail_paging_gesture_count** - urmărește câte gesturi de paginare pentru căutare de e-mail au fost efectuate în cadrul sesiunii de căutare combinată

- **mail_requests_count** - urmărește câte solicitări de căutare de e-mail au fost trimise în sesiunea de căutare combinată

- **people_filter_selected_contacts_count** - urmărește câte contacte au fost selectate în filtrul utilizatori

- **search_session_ended_type** - indică unde s-a încheiat o căutare, deoarece interogarea a fost anulată sau actualizată

- **search_suggestion_type** - indică ce se află în spatele sugestiei de căutare, de ex., este o corecție ortografică? Pe baza istoricului? Completare automată?

- **see_all_contacts_selected_count** - urmărește de câte ori a fost selectat „Vedeți toate persoanele de contact” în timpul sesiunii de căutare combinate

- **subtab_type** - urmărește unde a selectat utilizatorul rezultatul, din ce filă de rezultate

- **top_mail_result_selected_count** - urmărește de câte ori un utilizator selectează cele mai bune rezultate oferite.

- **ui_reload_result_count** - înregistrează perioadele de reîncărcare UI din cauza actualizării setului de rezultate (în timpul interogării corespunzătoare)

- **ui_reload_result_time** - înregistrează timpul total consumat pentru reîncărcarea interfeței utilizatorului din cauza actualizării setului de rezultate (în timpul interogării corespunzătoare)

- **ui_reload_status_count** - înregistrează perioadele de reîncărcare UI din cauza actualizării de stare (în timpul interogării corespunzătoare)

- **ui_reload_status_time** - înregistrează timpul total petrecut pentru reîncărcarea UI din cauza actualizării de stare (în timpul interogării corespunzătoare)

#### <a name="composemailaccessory"></a>compose.mail.accessory

Acest eveniment ne permite să detectăm și să remediem problemele privind acțiunile principale de compunere a e-mailului, pentru a vă împiedica să întâmpinați probleme la atașarea unui fișier, realizarea unei fotografie ca atașare sau trimiterea disponibilității.

Se colectează următoarele câmpuri: 

- **action** - ne comunică acțiunea încercată atunci când s-a înregistrat acțiunea. Printre exemple se numără atașarea unui fișier și prezentarea mai multor opțiuni.

- **icon_name** - ne spune numele pictogramei afișate atunci când acțiunea este înregistrată.
 
- **origin** – Spuneți-ne sursa acțiunii. Valorile posibile sunt quick_reply și full_screen.

- **toolbar_type** – Spuneți-ne tipul de bară de instrumente care se prezintă pe pagina de alcătuire. Valorile posibile sunt compose_actions și formatare.


#### <a name="conversationviewaction"></a>conversation.view.action

Este utilizat pentru a monitoriza posibilul impact negativ asupra capacității de a vizualiza și a răspunde la mesajele de e-mail

Se colectează următoarele câmpuri:

- **contains_mention** - ne spune dacă conversația a avut o @ menționare aplicată pentru a ne ajuta să detectăm probleme ce vizează mențiuni de e-mail

- **conversation_type** - ne spune ce tip de vizualizare a mesajelor de e-mail a fost redată, cum ar fi o singură vizualizare de mesaj sau mai multe vizualizări de mesaje. Ne ajută să detectăm problemele legate de un anumit tip de mesaj din vizualizarea conversației prin e-mail.

- **reaction_origin** - indică originea de unde a reacționat utilizatorul 

- **reaction_type** - indică tipul de reacție al utilizatorului

- **suggested_reply_char_count** - ne spune câte caractere au răspunsurile sugerate pe care le oferim (dacă sunt disponibile), pentru a ne ajuta la detectarea anomaliilor și a problemelor legate de sugestiile noastre

- **suggested_reply_click_pos** - ne spune în ce poziție este redat răspunsul sugerat (dacă este disponibil), astfel încât să putem detecta problemele privind o anumită sugestie

- **suggested_reply_type** - indică tipul de răspuns sugerat pentru această acțiune. Valorile posibile sunt text, send_avail și create_meeting.

- **use_default_quick_reply_mode** - ne spune dacă s-a utilizat modul implicit de răspuns rapid pentru a ne ajuta să detectăm probleme legate de experiența de răspuns rapid pentru mesajele de e-mail

#### <a name="draftaction"></a>draft.action

Este utilizat pentru a monitoriza posibilul impact negativ asupra capacității de a crea și a salva schițe de e-mail

Se colectează următoarele câmpuri: 

- **action** - tip de acțiune, de ex., salvare, abandonare.
 
- **draft_message_id** - ID-ul de mesaj al schiței

- **is_groups** - dacă schița este trimisă într-un/dintr-un folder de grup
 
- **origin** - unde a fost inițiată schița, de exemplu, detalii despre mesaj, compunere.

- **smart_compose_model_version** - urmărește ce versiune de model de compunere inteligentă este utilizată

- **suggestions_requested** - indică câte sugestii de compunere inteligentă au fost solicitate

- **suggestions_results** - un rezultat al sugestiilor inteligente compuse, adică acceptat, respins

- **suggestions_returned** - indică numărul de sugestii de compunere inteligentă returnate de la server

- **suggestions_shown** - indică câte sugestii de compunere inteligentă sunt afișate utilizatorului
 
- **thread_id** - ID-ul de fir al schiței de conversație este asociat cu

#### <a name="draganddrop"></a>drag.and.drop

Acest eveniment ne permite să detectăm dacă acțiunea de glisare și fixare a reușit sau nu.  Se utilizează pentru a vă asigura că experiențele de glisare și fixare funcționează corect între aplicații, atât ca eveniment de fixare în Outlook, cât și ca eveniment de glisare care iese din Outlook.  Cu aceste date, avem capacitatea de a ne asigura că întreaga experiență cu alte aplicații funcționează așa cum este de așteptat.

Se colectează următoarele câmpuri: 

- **action** - Acțiunea va fi glisare sau fixare

- **location** - în cazul unei acțiuni de glisare, acest lucru ne va spune din ce locație a început utilizatorul glisarea.  În cazul unei acțiuni de fixare, acest lucru ne va spune unde anume a fixat utilizatorul fișierul care a fost glisat. 

- **source** - în cazul unei acțiuni de fixare, acesta ne va spune din ce locație a început utilizatorul glisarea. Aceasta ne ajută să descoperim mai bine problemele cu o anumită sursă, cum ar fi OneDrive sau Fișiere, într-o anumită locație de fixare, cum ar fi un mesaj de e-mail nou.

#### <a name="drawerevent"></a>drawer.event

Este utilizat pentru a monitoriza posibilul impact negativ asupra capacității de a accesa foldere în inbox

Se colectează următoarele câmpuri:

- **add_calendar_option** - indică tipul de calendar adăugat din sertar, de ex. calendar interesant, calendar de corespondență, calendar partajat, pentru a ne ajuta să detectăm probleme legate de anumite tipuri de calendare

- **calendar_accounts_count** - indică numărul de conturi de calendar pentru a ne ajuta să detectăm problemele legate de numărul de conturi pe care le aveți

- **calendar_apps_count** - indică numărul de aplicații de calendar prezente pe dispozitivul utilizatorului, pentru a ne ajuta să detectăm problemele legate de aplicațiile de calendar

- **drawer_type** - indică tipul de sertar: interogare calendar, corespondență sau zero, pentru a ne ajuta să detectăm probleme legate de tipul de sertar

- **from_favorites** - indică dacă acțiunea a fost luată din Preferințe pentru a ne ajuta să detectăm probleme legate de preferințe

- **group_calendar_count** - indică numărul de calendare pentru cont, pentru a ne ajuta să detectăm probleme legate de calendare de grup

- **inbox_unread_count** - indică numărul de mesaje necitite din Inbox, pentru a ne ajuta să detectăm probleme privind afișarea numerelor pentru mesaje necitite din Inbox.

- **interesting_calendar_accounts_count** - indică numărul de conturi eligibile pentru calendare interesante de pe dispozitiv, pentru a ne ajuta să detectăm probleme legate de calendare interesante

- **is_group_calendar** - indică dacă este un calendar de grup pentru a ne ajuta să detectăm probleme legate de calendare de grup

- **mail_folder_type** - indică tipul de folder de corespondență, de ex., Inbox, schițe etc., pentru a ne ajuta să detectăm probleme legate de tipurile de foldere.

- **mail_accounts_count** - indică numărul de conturi de e-mail pentru a ne ajuta să detectăm problemele legate de conturile de corespondență.

- **selected_group_calendar_count** - indică numărul de calendare de grup care sunt selectate și active în interfața cu utilizatorul

- **visibility_toggle** - indică dacă utilizatorul activează sau dezactivează un anumit calendar, pentru a ne ajuta să detectăm probleme privind afișarea sau ascunderea calendarelor

#### <a name="ipccreaterepublishinglicense"></a>IpcCreateRepublishingLicense

Este colectat atunci când un utilizator încearcă să deschidă un document protejat prin IRM sau să aplice protecții IRM. Acesta conține informațiile necesare pentru a investiga și a diagnostica corect problemele care apar atunci când se realizează apelul API IpcCreateRepublishingLicense. 

Se colectează următoarele câmpuri:

- **AppInfo.ClientHierarchy** - ierarhie client care indică faptul că aplicația rulează în mediul de producție sau în mediul de dezvoltator

- **AppInfo.Name** - nume aplicație

- **AppInfo.Version** - versiunea aplicației

- **iKey** - ID al serverului pentru servicii de înregistrare

- **RMS.Duration** - timp total pentru finalizarea apelului API

- **RMS.DurationWithoutExternalOps** - timp total minus operațiuni externe consumate, cum ar fi latența de rețea.

- **RMS.ErrorCode** - codul de eroare returnat de apelul API, dacă există.

- **RMS.HttpCall** - indică dacă există operațiune HTTP

- **RMS.Result** - succes sau eșec al apelului API

- **RMS.ScenarioId** - ID al scenariului definit de API

- **RMS.SDKVersion** - versiunea clientului pentru Serviciul de administrare a drepturilor

- **RMS.StatusCode** - cod de stare al rezultatului returnat

#### <a name="ipcgetlicenseproperty"></a>IpcGetLicenseProperty

Este colectat atunci când un utilizator încearcă să deschidă un document protejat prin IRM sau să aplice protecții IRM. Acesta conține informațiile necesare pentru a investiga și a diagnostica corect problemele care apar atunci când se realizează apelul API IpcGetLicenseProperty. 

Se colectează următoarele câmpuri:

- **AppInfo.ClientHierarchy** - ierarhie client care indică faptul că aplicația rulează în mediul de producție sau în mediul de dezvoltator

- **AppInfo.Name** - nume aplicație.

- **AppInfo.Version** - versiunea aplicației

- **iKey** - ID al serverului pentru servicii de înregistrare

- **RMS.Duration** - timp total pentru finalizarea apelului API

- **RMS.DurationWithoutExternalOps** - timp total minus operațiuni externe consumate, cum ar fi latența de rețea.

- **RMS.ErrorCode** - codul de eroare returnat de apelul API, dacă există.

- **RMS.HttpCall** - indică dacă există o operațiune HTTP

- **RMS.LicensePropertyType** - tip de proprietate licență

- **RMS.Result** - succes sau eșec al apelului API

- **RMS.ScenarioId** - ID al scenariului definit de API

- **RMS.SDKVersion** - versiunea clientului pentru Serviciul de administrare a drepturilor

- **RMS.StatusCode** - cod de stare al rezultatului returnat

#### <a name="ipcgetserializedlicenseproperty"></a>IpcGetSerializedLicenseProperty

Este colectat atunci când un utilizator încearcă să deschidă un document protejat prin IRM sau să aplice protecții IRM. Acesta conține informațiile necesare pentru a investiga și a diagnostica corect problemele care apar atunci când se realizează apelul API IpcGetSerializedLicenseProperty. 

Se colectează următoarele câmpuri:

- **AppInfo.ClientHierarchy** - ierarhie client care indică faptul că aplicația rulează în mediul de producție sau în mediul de dezvoltator

- **AppInfo.Name** - nume aplicație.

- **AppInfo.Version** - versiunea aplicației

- **iKey** - ID al serverului pentru servicii de înregistrare

- **RMS.Duration** - timp total pentru finalizarea apelului API

- **RMS.DurationWithoutExternalOps** - timp total minus operațiuni externe consumate, cum ar fi latența de rețea.

- **RMS.ErrorCode** - codul de eroare returnat de apelul API, dacă există.

- **RMS.HttpCall** - indică dacă există o operațiune HTTP

- **RMS.LicensePropertyType** - tip de proprietate licență

- **RMS.Result** - succes sau eșec al apelului API

- **RMS.ScenarioId** - ID al scenariului definit de API

- **RMS.SDKVersion** - versiunea clientului pentru Serviciul de administrare a drepturilor

- **RMS.StatusCode** - cod de stare al rezultatului returnat

#### <a name="ipcgettemplateissuerlist"></a>IpcGetTemplateIssuerList

Este colectat atunci când un utilizator încearcă să deschidă un document protejat prin IRM sau să aplice protecții IRM. Acesta conține informațiile necesare pentru a investiga și a diagnostica corect problemele care apar atunci când se realizează apelul API IpcGetTemplateIssuerList. 

Se colectează următoarele câmpuri:

- **AppInfo.ClientHierarchy** - ierarhie client care indică faptul că aplicația rulează în mediul de producție sau în mediul de dezvoltator

- **AppInfo.Name** - nume aplicație.

- **AppInfo.Version** - versiunea aplicației

- **iKey** - ID al serverului pentru servicii de înregistrare

- **RMS.AuthCallbackProvided** - indică dacă se furnizează apelare inversă pentru autentificare ca intrare pentru apelul API sau nu

- **RMS.ConnectionInfo.ExtranetUrl** - URL de extranet pentru informațiile de conexiune

- **RMS.ConnectionInfo.IntranetUrl** - URL de intranet pentru informațiile de conexiune

- **RMS.ConnectionMode** - modul de conexiune între clientul Serviciu de administrare a drepturilor și server: online sau offline

- **RMS.Duration** - timp total pentru finalizarea apelului API

- **RMS.DurationWithoutExternalOps** - timp total minus operațiuni externe consumate, cum ar fi latența de rețea.

- **RMS.ErrorCode** - codul de eroare returnat de apelul API, dacă există.

- **RMS.GuestTenant** - ID-ul entității găzduite invitat pentru utilizator

- **RMS.HomeTenant** - ID-ul entității găzduite domiciliu pentru utilizator

- **RMS.HttpCall** - indică dacă există operațiune HTTP

- **RMS.Identity.ExtranetUrl** - URL-ul de extranet pentru serverul Serviciului de administrare a drepturilor pentru utilizator, colectat în timpul obținerii unui nou Certificat de cont de drepturi de la server
 
- **RMS.Identity.IntranetUrl** - URL-ul de intranet pentru serverul Serviciului de administrare a drepturilor pentru utilizator, colectat în timpul obținerii unui nou Certificat de cont de drepturi de la server

- **RMS.Identity.Status** - prima dată când se obține Certificatul de cont de drepturi de la server sau când se reînnoiește Certificatul de cont de drepturi 

- **RMS.Identity.Type** - tipul de cont de utilizator, cum ar fi cont Windows sau cont live

- **RMS.Identity.UserProvided** - indică dacă adresa de e-mail a utilizatorului a fost furnizată sau nu în timpul obținerii unui nou Certificat de cont de drepturi de la server

- **RMS.IssuerId** - ID-ul serverului Serviciului de administrare a drepturilor care emite Certificatul de cont de drepturi 

- **RMS.LicenseFormat** - formatul licenței: Xrml sau Json

- **RMS.RACType** - tipul Certificatului de cont de drepturi

- **RMS.Result** - succes sau eșec al apelului API

- **RMS.ScenarioId** - ID al scenariului definit de API

- **RMS.SDKVersion** - versiunea clientului pentru Serviciul de administrare a drepturilor

- **RMS.ServerType** - tipul de server al Serviciului de administrare a drepturilor

- **RMS.StatusCode** - cod de stare al rezultatului returnat

- **UserInfo.UserObjectId** - ID al obiectului utilizator

#### <a name="ipcgettemplatelist"></a>IpcGetTemplateList

Este colectat atunci când un utilizator încearcă să deschidă un document protejat prin IRM sau să aplice protecții IRM. Acesta conține informațiile necesare pentru a investiga și a diagnostica corect problemele care apar atunci când se realizează apelul API IpcGetTemplateList. 

Se colectează următoarele câmpuri:

- **AppInfo.ClientHierarchy** - ierarhie client care indică faptul că aplicația rulează în mediul de producție sau în mediul de dezvoltator

- **AppInfo.Name** - nume aplicație.

- **AppInfo.Version** - versiunea aplicației

- **iKey** - ID al serverului pentru servicii de înregistrare

- **RMS.AuthCallbackProvided** - indică dacă se furnizează apelare inversă pentru autentificare ca intrare pentru apelul API sau nu

- **RMS.ConnectionInfo.ExtranetUrl** - URL de extranet pentru informațiile de conexiune

- **RMS.ConnectionInfo.IntranetUrl** - URL de intranet pentru informațiile de conexiune

- **RMS.ConnectionMode** - modul de conexiune între clientul Serviciu de administrare a drepturilor și server: online sau offline

- **RMS.Duration** - timp total pentru finalizarea apelului API

- **RMS.DurationWithoutExternalOps** - timp total minus operațiuni externe consumate, cum ar fi latența de rețea.

- **RMS.ErrorCode** - codul de eroare returnat de apelul API, dacă există.

- **RMS.GuestTenant** - ID-ul entității găzduite invitat pentru utilizator

- **RMS.HomeTenant** - ID-ul entității găzduite domiciliu pentru utilizator

- **RMS.HttpCall** - indică dacă există operațiune http

- **RMS.Identity.ExtranetUrl** - URL-ul de extranet pentru serverul Serviciului de administrare a drepturilor pentru utilizator, colectat în timpul obținerii unui nou Certificat de cont de drepturi de la server
 
- **RMS.Identity.IntranetUrl** - URL-ul de intranet pentru serverul Serviciului de administrare a drepturilor pentru utilizator, colectat în timpul obținerii unui nou Certificat de cont de drepturi de la server

- **RMS.Identity.Status** - prima dată când se obține Certificatul de cont de drepturi de la server sau când se reînnoiește Certificatul de cont de drepturi 

- **RMS.Identity.Type** - tipul de cont de utilizator, cum ar fi cont Windows sau cont live

- **RMS.Identity.UserProvided** - indică dacă adresa de e-mail a utilizatorului a fost furnizată sau nu în timpul obținerii unui nou Certificat de cont de drepturi de la server

- **RMS.IssuerId** - ID-ul serverului Serviciului de administrare a drepturilor care emite Certificatul de cont de drepturi 

- **RMS.LicenseFormat** - formatul licenței: Xrml sau Json

- **RMS.RACType** - tipul Certificatului de cont de drepturi

- **RMS.Result** - succes sau eșec al apelului API

- **RMS.ScenarioId** - ID al scenariului definit de API

- **RMS.SDKVersion** - versiunea clientului pentru Serviciul de administrare a drepturilor

- **RMS.ServerType** - tipul de server al Serviciului de administrare a drepturilor

- **RMS.StatusCode** - cod de stare al rezultatului returnat

- **RMS.TemplatesCount** - numărul de șabloane

- **UserInfo.UserObjectId** - ID al obiectului utilizator

#### <a name="ipcpcreatelicensefromscratch"></a>IpcpCreateLicenseFromScratch

Este colectat atunci când un utilizator încearcă să deschidă un document protejat prin IRM sau să aplice protecții IRM. Acesta conține informațiile necesare pentru a investiga și a diagnostica corect problemele care apar atunci când se realizează apelul API IpcpCreateLicenseFromScratch. 

Se colectează următoarele câmpuri:

- **AppInfo.ClientHierarchy** - ierarhie client care indică faptul că aplicația rulează în mediul de producție sau în mediul de dezvoltator

- **AppInfo.Name** - nume aplicație.

- **AppInfo.Version** - versiunea aplicației

- **iKey** - ID al serverului pentru servicii de înregistrare

- **RMS.Duration** - timp total pentru finalizarea apelului API

- **RMS.DurationWithoutExternalOps** - timp total minus operațiuni externe consumate, cum ar fi latența de rețea.

- **RMS.ErrorCode** - codul de eroare returnat de apelul API, dacă există.

- **RMS.GuestTenant** - ID-ul entității găzduite invitat pentru utilizator

- **RMS.HomeTenant** - ID-ul entității găzduite domiciliu pentru utilizator

- **RMS.HttpCall** - indică dacă există operațiune HTTP

- **RMS.Identity.ExtranetUrl** - URL-ul de extranet pentru serverul Serviciului de administrare a drepturilor pentru utilizator, colectat în timpul obținerii unui nou Certificat de cont de drepturi de la server

- **RMS.Identity.IntranetUrl** - URL-ul de intranet pentru serverul Serviciului de administrare a drepturilor pentru utilizator, colectat în timpul obținerii unui nou Certificat de cont de drepturi de la server

- **RMS.Identity.UserProvided** - indică dacă adresa de e-mail a utilizatorului a fost furnizată sau nu în timpul obținerii unui nou Certificat de cont de drepturi de la server

- **RMS.IssuerId** - ID-ul serverului Serviciului de administrare a drepturilor care emite Certificatul de cont de drepturi 

- **RMS.LicenseFormat** - formatul licenței: Xrml sau Json

- **RMS.RACType** - tipul Certificatului de cont de drepturi

- **RMS.Result** - succes sau eșec al apelului API

- **RMS.ScenarioId** - ID al scenariului definit de API

- **RMS.SDKVersion** - versiunea clientului pentru Serviciul de administrare a drepturilor

- **RMS.ServerType** - tipul de server al Serviciului de administrare a drepturilor

- **RMS.StatusCode** - cod de stare al rezultatului returnat

- **RMS.TokenProvided** - indică dacă se furnizează tokenul ca intrare pentru apelul API sau nu 

- **RMS.UserProvided** - indică dacă se furnizează consumatorul ca intrare pentru apelul API sau nu 

- **UserInfo.UserObjectId** - ID al obiectului utilizator 

#### <a name="ipcpcreatelicensefromtemplate"></a>IpcpCreateLicenseFromTemplate

Este colectat atunci când un utilizator încearcă să deschidă un document protejat prin IRM sau să aplice protecții IRM. Acesta conține informațiile necesare pentru a investiga și a diagnostica corect problemele care apar atunci când se realizează apelul API IpcpCreateLicenseFromTemplate.  

Se colectează următoarele câmpuri:

- **AppInfo.ClientHierarchy** - ierarhie client care indică faptul că aplicația rulează în mediul de producție sau în mediul de dezvoltator

- **AppInfo.Name** - nume aplicație.

- **AppInfo.Version** - versiunea aplicației

- **iKey** - ID al serverului pentru servicii de înregistrare

- **RMS.AuthCallbackProvided** - indică dacă se furnizează apelare inversă pentru autentificare ca intrare pentru apelul API sau nu

- **RMS.ConnectionMode** - modul de conexiune între clientul Serviciu de administrare a drepturilor și server: online sau offline

- **RMS.Duration** - timp total pentru finalizarea apelului API

- **RMS.DurationWithoutExternalOps** - timp total minus operațiuni externe consumate, cum ar fi latența de rețea.

- **RMS.ErrorCode** - codul de eroare returnat de apelul API, dacă există.

- **RMS.HttpCall** - indică dacă există operațiune http

- **RMS.Result** - succes sau eșec al apelului API

- **RMS.ScenarioId** - ID al scenariului definit de API

- **RMS.SDKVersion** - versiunea clientului pentru Serviciul de administrare a drepturilor

- **RMS.StatusCode** - cod de stare al rezultatului returnat

- **RMS.TokenProvided** - indică dacă se furnizează tokenul ca intrare pentru apelul API sau nu 

- **RMS.UserProvided** - indică dacă se furnizează consumatorul ca intrare pentru apelul API sau nu 

#### <a name="ipcpgettemplatelistforuser"></a>IpcpGetTemplateListForUser

Este colectat atunci când un utilizator încearcă să deschidă un document protejat prin IRM sau să aplice protecții IRM. Acesta conține informațiile necesare pentru a investiga și a diagnostica corect problemele care apar atunci când se realizează apelul API IpcpGetTemplateListForUser.  

Se colectează următoarele câmpuri:

- **AppInfo.ClientHierarchy** - ierarhie client care indică faptul că aplicația rulează în mediul de producție sau în mediul de dezvoltator

- **AppInfo.Name** - nume aplicație.

- **AppInfo.Version** - versiunea aplicației

- **iKey** - ID al serverului pentru servicii de înregistrare

- **RMS.ApplicationScenarioId** - ID al scenariului furnizat de aplicație

- **RMS.AuthCallbackProvided** - indică dacă se furnizează apelare inversă pentru autentificare ca intrare pentru apelul API sau nu

- **RMS.ConnectionInfo.ExtranetUrl** - URL de extranet pentru informațiile de conexiune

- **RMS.ConnectionInfo.IntranetUrl** - URL de intranet pentru informațiile de conexiune

- **RMS.ConnectionMode** - modul de conexiune între clientul Serviciu de administrare a drepturilor și server: online sau offline

- **RMS.Duration** - timp total pentru finalizarea apelului API

- **RMS.DurationWithoutExternalOps** - timp total minus operațiuni externe consumate, cum ar fi latența de rețea.

- **RMS.ErrorCode** - codul de eroare returnat de apelul API, dacă există.

- **RMS.GuestTenant** - ID-ul entității găzduite invitat pentru utilizator

- **RMS.HomeTenant** - ID-ul entității găzduite domiciliu pentru utilizator

- **RMS.HttpCall** - indică dacă există o operațiune HTTP

- **RMS.Identity.ExtranetUrl** - URL-ul de extranet pentru serverul Serviciului de administrare a drepturilor pentru utilizator, colectat în timpul obținerii unui nou Certificat de cont de drepturi de la server

- **RMS.Identity.IntranetUrl** - URL-ul de intranet pentru serverul Serviciului de administrare a drepturilor pentru utilizator, colectat în timpul obținerii unui nou Certificat de cont de drepturi de la server

- **RMS.Identity.Status** - prima dată când se obține Certificatul de cont de drepturi de la server sau când se reînnoiește Certificatul de cont de drepturi 

- **RMS.Identity.Type** - tipul de cont de utilizator, cum ar fi cont Windows sau cont live

- **RMS.Identity.UserProvided** - indică dacă adresa de e-mail a utilizatorului a fost furnizată sau nu în timpul obținerii unui nou Certificat de cont de drepturi de la server

- **RMS.IssuerId** - ID-ul serverului Serviciului de administrare a drepturilor care emite Certificatul de cont de drepturi 

- **RMS.LicenseFormat** - formatul licenței: Xrml sau Json

- **RMS.RACType** - tipul Certificatului de cont de drepturi

- **RMS.Result** - succes sau eșec al apelului API

- **RMS.ScenarioId** - ID al scenariului definit de API

- **RMS.SDKVersion** - versiunea clientului pentru Serviciul de administrare a drepturilor

- **RMS.ServerType** - tipul de server al Serviciului de administrare a drepturilor

- **RMS.StatusCode** - cod de stare al rezultatului returnat

- **RMS.TemplatesCount** - numărul de șabloane

- **RMS.TokenProvided** - indică dacă se furnizează tokenul ca intrare pentru apelul API sau nu 
    
- **RMS.UserProvided** - indică dacă se furnizează consumatorul ca intrare pentru apelul API sau nu 

- **UserInfo.UserObjectId** - ID al obiectului utilizator 

#### <a name="ipcpserializelicense"></a>IpcpSerializeLicense

Colectat atunci când un user încearcă să aplice protecții IRM la document. Acesta conține informațiile necesare pentru a investiga și a diagnostica corect problemele care apar atunci când se realizează apelul API IpcpSerializeLicense. 

Se colectează următoarele câmpuri:

- **AppInfo.ClientHierarchy** - ierarhie client care indică faptul că aplicația rulează în mediul de producție sau în mediul de dezvoltator

- **AppInfo.Name** - nume aplicație.

- **AppInfo.Version** - versiunea aplicației

- **iKey** - ID al serverului pentru servicii de înregistrare

- **RMS.ApplicationScenarioId** - ID al scenariului furnizat de aplicație

- **RMS.AuthCallbackProvided** - indică dacă se furnizează apelare inversă pentru autentificare ca intrare pentru apelul API sau nu

- **RMS.ConnectionMode** - modul de conexiune între clientul Serviciu de administrare a drepturilor și server: online sau offline

- **RMS.ContentId** - ID-ul de conținut al documentului

- **RMS.Duration** - timp total pentru finalizarea apelului API

- **RMS.DurationWithoutExternalOps** - timp total minus operațiuni externe consumate, cum ar fi latența de rețea.

- **RMS.ErrorCode** - codul de eroare returnat de apelul API, dacă există.

- **RMS.GuestTenant** - ID-ul entității găzduite invitat pentru utilizator

- **RMS.HomeTenant** - ID-ul entității găzduite domiciliu pentru utilizator

- **RMS.HttpCall** - indică dacă există operațiune http

- **RMS.Identity.ExtranetUrl** - URL-ul de extranet pentru serverul Serviciului de administrare a drepturilor pentru utilizator, colectat în timpul obținerii unui nou Certificat de cont de drepturi de la server

- **RMS.Identity.IntranetUrl** - URL-ul de intranet pentru serverul Serviciului de administrare a drepturilor pentru utilizator, colectat în timpul obținerii unui nou Certificat de cont de drepturi de la server

- **RMS.Identity.Status** - prima dată când se obține Certificatul de cont de drepturi de la server sau când se reînnoiește Certificatul de cont de drepturi 

- **RMS.Identity.Type** - tipul de cont de utilizator, cum ar fi cont Windows sau cont live

- **RMS.Identity.UserProvided** - indică dacă adresa de e-mail a utilizatorului a fost furnizată sau nu în timpul obținerii unui nou Certificat de cont de drepturi de la server

- **RMS.IssuerId** - ID-ul serverului Serviciului de administrare a drepturilor care emite Certificatul de cont de drepturi 

- **RMS.KeyHandle** - adresa de memorie pentru handle-ul de cheie

- **RMS.LicenseFormat** - formatul licenței: Xrml sau Json

- **RMS.PL.KeyType** – valori „Single” sau „Double”. Indică dacă PL a fost protejat cu protecție cu o singură cheie sau cu protecție cu cheie dublă.

- **RMS.RACType** - tipul Certificatului de cont de drepturi

- **RMS.Result** - succes sau eșec al apelului API

- **RMS.ScenarioId** - ID al scenariului definit de API

- **RMS.SDKVersion** - versiunea clientului pentru Serviciul de administrare a drepturilor

- **RMS.ServerType** - tipul de server al Serviciului de administrare a drepturilor

- **RMS.StatusCode** - cod de stare al rezultatului returnat

- **RMS.TokenProvided** - indică dacă se furnizează tokenul ca intrare pentru apelul API sau nu 

- **RMS.UserProvided** - indică dacă se furnizează consumatorul ca intrare pentru apelul API sau nu 

- **UserInfo.UserObjectId** - ID al obiectului utilizator 

#### <a name="ipcsetlicenseproperty"></a>IpcSetLicenseProperty

Este colectat atunci când un utilizator încearcă să deschidă un document protejat prin IRM sau să aplice protecții IRM. Acesta conține informațiile necesare pentru a investiga și a diagnostica corect problemele care apar atunci când se realizează apelul API IpcSetLicenseProperty. 

Se colectează următoarele câmpuri:

- **AppInfo.ClientHierarchy** - ierarhie client care indică faptul că aplicația rulează în mediul de producție sau în mediul de dezvoltator

- **AppInfo.Name** - nume aplicație.

- **AppInfo.Version** - versiunea aplicației

- **iKey** - ID al serverului pentru servicii de înregistrare

- **RMS.Duration** - timp total pentru finalizarea apelului API

- **RMS.DurationWithoutExternalOps** - timp total minus operațiuni externe consumate, cum ar fi latența de rețea.

- **RMS.ErrorCode** - codul de eroare returnat de apelul API, dacă există. 

- **RMS.HttpCall** - indică dacă există operațiune http

- **RMS.LicensePropertyType** - tip de proprietate licență

- **RMS.Result** - succes sau eșec al apelului API

- **RMS.ScenarioId** - ID al scenariului definit de API

- **RMS.SDKVersion** - versiunea clientului pentru Serviciul de administrare a drepturilor

- **RMS.StatusCode** - ID al scenariului definit de API


#### <a name="linkclickedaction"></a>link.clicked.action

Evenimentul este utilizat pentru a urmări succesul utilizatorilor în vizualizarea unei adrese URL în vizualizarea web Microsoft Edge și pentru a finaliza scenarii web standard în acea vizualizare web fără a se confrunta cu erori

Se colectează următoarele câmpuri:

- **account_type** - dacă vizualizarea web Microsoft Edge a fost lansată de la un mesaj de e-mail sau de la un eveniment din Outlook, tastați contul de unde provine adresa URL

- **action** - acțiunea efectuată de utilizator în Outlook din momentul în care atinge un URL până la momentul când iese din acel flux (a deschis linkul în vizualizarea web Microsoft Edge, pagina nu a reușit să se încarce în vizualizarea web, a efectuat o căutare în vizualizarea web, a ieși din vizualizarea web Microsoft Edge pentru a deschide linkul într-o aplicație de browser web etc.)

- **duration** - durata sesiunii utilizatorului

- **launch_type** - dacă a fost lansată vizualizarea web Microsoft Edge, a fost din Outlook, dintr-un widget sau dintr-o componentă a sistemului de operare

- **origin** - dacă utilizatorul a efectuat o acțiune în vizualizarea web Microsoft Edge, originea respectivei acțiuni

- **referrer** - locația adresei URL pe care utilizatorul a atins-o (e-mail, eveniment de calendar, card TXP etc.)

- **search_scope** - dacă utilizatorul a efectuat o căutare în vizualizarea web Microsoft Edge, domeniul acelei căutări (Toate, Imagini, Videoclipuri etc.)

- **search_subtype** - dacă utilizatorul a efectuat o căutare în vizualizarea web Microsoft Edge, a fost o căutare inițială sau o căutare rafinată

- **session_summary_page_loaded_count** - numărul de pagini încărcate de utilizator în timpul sesiunii în vizualizarea web Microsoft Edge

- **session_summary_search_count** - numărul de căutări Bing efectuate de utilizator în timpul sesiunii în vizualizarea web Microsoft Edge

- **session_summary_session_id** - identificator pentru sesiunea de utilizatori prezentă din vizualizarea web Microsoft Edge

- **txp** – dacă vizualizarea web Microsoft Edge a fost lansată dintr-un card TXP, tipul de eveniment pentru cardul respectiv (de masă, zbor etc.)

- **txp_component** - dacă vizualizarea web Microsoft Edge a fost lansată dintr-un card TXP, tipul de componentă de interfață utilizator pentru acel card


#### <a name="mailaction"></a>mail.action

Este utilizat pentru a monitoriza posibilul impact negativ asupra capacității dvs. de a efectua acțiuni critice de corespondență (cum ar fi rularea modului filetat de corespondență, asigurarea funcționării acțiunilor de triere a corespondenței) pentru a vă asigura că aplicația funcționează corect pentru e-mail.

Se colectează următoarele câmpuri:

- **account** - contul care e efectuat acțiunea *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

- **action** - urmărește ce tip de acțiune a fost întreprins, de ex., arhivare, ștergere, marcare ca citit etc. 

- **attachment_content_type** - tipul de conținut al atașării descărcate 

- **attachment_content_type_with_count** - urmărește numărul de atașări din e-mail

- **attachment_download_result** - rezultatul (de ex., succes/eșec) pentru o acțiune de descărcare a atașărilor

- **attachment_download_time** - ora unei acțiuni de descărcare a atașărilor

- **attachment_extn** - extensia fișierului din atașarea descărcată

- **attachment_id** - identificatorul sistemului pentru atașarea descărcată 

- **attachment_size** - dimensiunea atașării descărcate

- **domain** - domeniul documentului deschis

- **duration** - urmărește cât timp a durat acțiunea ca șir în limba engleză, ușor de citit de utilizatori (de exemplu, 1s, 4H)

- **error** - mesaj de eroare asociat cu acțiunea 

- **event_mode** - în ce tip de mod de eveniment a fost: grupuri sau altele. 

- **Extension** - extensia de fișier a linkului sau atașării asociate cu această acțiune 

- **internet_message_id** - ID-ul mesajului de urmărire

- **is_group_escalation** - indică dacă mesajul în care fost întreprinsă acțiunea a fost trimis la cutia poștală a utilizatorului din cauza unei escaladări (abonat la grup)

- **is_rule** - indică dacă acțiunea de corespondență efectuată resetează o clasificare prioritară/o altă clasificare

- **is_threaded_mode** - indică dacă mesajul a fost în modul filetat sau nu, de ex. cum sunt grupate mesajele

- **is_unread** - indică dacă mesajul este necitit că acțiunea a fost efectuată

- **left_swipe_setting** - indică ce acțiune a fost setată pentru a fi glisarea din stânga

- **message_id** - ID mesaj server direcționat spre acțiune sau listă separată prin virgulă dacă au fost în acțiune mai multe elemente.

- **message_type** - indică tipul de mesaj tip de acțiune pentru care s-a efectuat acțiunea în** - grup sau altele

- **number_selected** - numărul de elemente selectate de utilizator în lista de mesaje și acțiunile efectuate în timpul mai multor moduri de selecție.

- **origin** - sursă de acțiune, de ex., trageți cu degetul prin celule, interogare zero, link direct, vizualizare e-mail, listă de e-mail etc.

- **reported_to_msft** - după ce trimiteți un e-mail la E-mailuri nedorite (spam) sau Coș de gunoi (phishing), se poate alege ca acțiunea să fie raportată către Microsoft.

- **retry** - dacă acțiunea a fost reîncercată

- **right_swipe_setting** - indică ce acțiune a fost setată pentru a fi glisarea din stânga 

- **shortcut** - indică dacă s-a utilizat o comandă rapidă și ce comandă rapidă a fost utilizată pentru planificarea unui mesaj, de ex. mai târziu, mâine, alegeți ora etc.

- **size** - extensia linkului sau a atașării asociate cu această acțiune

- **source_folder** - urmărește tipul de folder sursă atunci când acțiunea indică trecerea de la un folder la altul, de exemplu, în Inbox, Coșul de gunoi etc. 

- **source_inbox** - indică în ce inbox are loc acțiunea de corespondență (de ex. Mesaje prioritare, Alte mesaje etc.) - starea acțiunii, de exemplu, succesul sau punctul de eroare

- **target_folder** - indică tipul de folder țintă atunci când mutați e-mailurile dintr-un folder în altul

- **thread_id** - ID de fir al conversației direcționate spre acțiune sau al listei separate prin virgulă dacă au fost vizate mai multe elemente

- **time_taken_to_fetch_access_token** - timp necesar pentru a prelua un simbol de acces la sistem pentru utilizare la deschiderea unui link

- **time_taken_to_fetch_drive_item** - timp necesar pentru a prelua o resursă OneDrive când faceți clic

- **time_taken_to_fetch_embed_viewer_resource** - timp necesar pentru a inițializa Vizualizatorul încorporat la deschiderea linkurilor

- **time_taken_to_load_embed_viewer** - timp necesar pentru a inițializa Vizualizatorul încorporat la deschiderea linkurilor

- **time_taken_to_load_link** - timp necesar pentru ca o acțiune de încărcare a linkului să se finalizeze

- **time_taken_to_tap_attachment** - timpul dintre deschiderea mesajului și clicul pe atașare

- **time_taken_to_tap_link** - timpul necesar utilizatorului între vizualizarea mesajului și clicul pe un link

- **Txp** - indică dacă există un tip de element txp asociat cu e-mailul la care s-a efectuat acțiunea, de ex., rezervarea evenimentului, rezervarea zborului etc. 

- **type** - tip de document deschis prin intermediul linkului

#### <a name="mailcompose"></a>mail.compose

Este utilizat pentru a monitoriza posibilul impact negativ asupra capacității de a compune și a răspunde la mesaje de e-mail, cum ar fi să întâmpinați probleme privind răspunsul, să vă formatați e-mailul sau să trimiteți mesaje de e-mail.

Se colectează următoarele câmpuri: 

- **draft_message_id** - ID-ul schiței conversației create ca schiță pentru a ne ajuta să detectăm probleme legate de e-mailuri schiță

- **message_id** - ID-ul mesajului conversației la care s-a răspuns sau de la care s-a redirecționat pentru a ne ajuta să detectăm probleme legate de un anumit mesaj

- **origin** - ne spune de unde provine compunerea, de ex., de la dintr-un răspuns tuturor, un nou răspuns compus sau răspuns rapid. Ne ajută să detectăm problemele asociate cu un tip de origine răspuns specific.

- **is_group_escalation** - dacă mesajul este un mesaj de grup escaladat, pentru ca noi să putem detecta problemele de compunere legate de grupuri.

- **is_link** - ne spune dacă schița nouă care a fost creată a fost efectuată de la un link. Ne ajută să detectăm problemele asociate cu schițele create din linkuri.

- **is_force_touch** - ne spune dacă schița nouă care a fost creată a fost efectuată de la o acțiune de atingere forțată. Ne ajută să detectăm problemele asociate cu schițele create din această acțiune.

- **is_group** - dacă evenimentul a început într-un spațiu al grupurilor pentru ca noi să putem detecta problemele de compunere legate de grupuri.

- **source_inbox** - ne spune inboxul sursă, de exemplu, dacă au fost Mesajele prioritare sau Alte mesaje

- **thread_id** - ID-ul firului conversației la care s-a răspuns sau de la care s-a redirecționat pentru a ne ajuta să detectăm probleme legate de un anumit mesaj

#### <a name="meetingcalltoaction"></a>meeting.call.to.action

Este utilizat cu scopul de a monitoriza posibilul impact negativ asupra capacității dvs. de a efectua acțiuni de întâlnire foarte importante, cum ar fi crearea și editarea evenimentelor, precum și oferirea de răspuns la ele.

Se colectează următoarele câmpuri:

- **event_mode** - indică dacă acest eveniment a fost de la un grup sau nu pentru a ne ajuta să detectăm probleme legate de evenimentele din grup

- **meeting_id** - un ID de întâlnire care ne ajută să urmărim problemele de-a lungul vieții unei întâlniri, pentru a ne ajuta să detectăm probleme privind anumite întâlniri

- **meeting_provider** - indică furnizorul pentru o întâlnire online, de exemplu, Teams, Skype for Business, pentru a ne ajuta să detectăm probleme privind anumiți furnizori de întâlnire online

- **notify_type** - indică tipul de răspuns pentru alte tipuri de conturi, pentru a ne ajuta să detectăm probleme legate de tipuri de conturi diferite

- **recurrence** - indică frecvența cu care se întâmplă această întâlnire, de exemplu, recurență sau serie, pentru a ne ajuta să detectăm probleme privind seria de întâlniri recurente

- **response** - indică tipul de răspuns, cum ar fi acceptare sau refuz pentru anumite tipuri de conturi, pentru a ne ajuta să detectăm probleme privind răspunsul la evenimente

- **response_message_length** - indică lungimea mesajului pentru a ne ajuta să detectăm probleme legate de răspunsurile la întâlnire

- **review_time_proposal_action_type** - indică o nouă propunere de oră pentru răspunsul utilizatorului, pentru a ne ajuta să detectăm probleme legate de propunerea unei noi ore

- **send_response** - indică dacă s-a trimis un răspuns pentru a ne ajuta să detectăm probleme la trimiterea răspunsurilor de invitație la întâlnire

- **txp** - indică ce tip de întâlnire a fost generată din rezervări de zbor și livrări, pentru a ne ajuta să detectăm probleme legate de acest tip de întâlnire

- **with_message_enabled** - indică dacă un utilizator poate răspunde cu un mesaj pentru a ne ajuta să detectăm probleme privind răspunsul la invitații la întâlnire

#### <a name="officeandroiddocsuifileoperationsopendocumentmeasurements"></a>Office.Android.DocsUI.FileOperations.OpenDocumentMeasurements

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforma Android și înregistrările atunci când are loc o operațiune de deschidere a fișierelor. Evenimentul vă ajută să păstrați operațiunea de deschidere a fișierelor în siguranță, actualizată și corect funcțională. Scopul colectării acestor date este de a îmbunătăți în permanență performanța de deschidere a fișierelor. 

Se colectează următoarele câmpuri:

- **Data_AppDocsOperationDuration** - durata petrecută în substrat în timpul unei operațiuni de deschidere a fișierelor.

- **Data_AppDuration** - durata petrecută în procesarea aplicațiilor în timpul unei operațiuni de deschidere a fișierelor. 

- **Data_AppWarmUpGain** - câștigul în durata de încărcare a aplicației pe care-l obținem prin preîncărcarea în prealabil a unei părți a aplicației.

- **Data_BootDuration** - durata pornirii aplicației în procesul de deschidere a fișierului.

- **Data_ClosePreviouslyOpenedMarkers** - în unele scenarii de deschidere a fișierelor, închiderea unui document deschis anterior are loc înainte de deschiderea documentului curent. Această durată dintre unele operațiuni care au loc în acest caz este capturată într-o valoare șir care are formatul \<functionId>\<functionValue>\<functionId>\<functionValue>...

- **Data_Doc_AccessMode** - o enumerare indicând modul de acces al fișierului, de exemplu, doar în citire, citiți scrierea.

- **Data_Doc_AsyncOpenKind** - o enumerare indicând tipul de flux asincron utilizat pentru deschiderea fișierului.

- **Data_Doc_ChunkingType** - o enumerare indicând tipul de algoritm de segmentare a unui fișier.

- **Data_Doc_EdpState** - o enumerare indicând starea de protecție a datelor de întreprindere a unui fișier.

- **Data_Doc_Ext** - extensia fișierului

- **Data_Doc_Fqdn** - nume gazdă server al fișierului.

- **Data_Doc_FqdnHash** - un identificator unic global (GUID) care identifică în mod unic un nume gazdă server.

- **Data_Doc_IdentityTelemetryId** - un GUID care identifică în mod unic identitatea utilizată pentru a deschide un fișier. 

- **Data_Doc_InitializationScenario** - o enumerare indicând tipul de scenariu detaliat al unei operațiuni deschise de fișier.

- **Data_Doc_IOFlags** - o enumerare indicând semnalizările IO ale unei operațiuni deschise de fișier, de exemplu, dacă fișierul este în cache sau nu.

- **Data_Doc_IsCloudCollabEnabled** - dacă colaborarea în cloud este activată sau nu pentru fișier.

- **Data_Doc_IsIncrementalOpen** - dacă fișierul a fost sau nu deschis prin deschidere treptată.

- **Data_Doc_IsOcsSupported** - dacă un fișier acceptă sau nu serviciul de colaborare Office.

- **Data_Doc_IsOpeningOfflineCopy** - dacă se deschide sau nu un fișier dintr-o copie memorată în cache offline.

- **Data_Doc_IsPrefetched** - dacă a fost sau nu preluat fișierul înainte de a se deschide operațiunea.

- **Data_Doc_IsSyncBacked** - dacă un fișier în cloud există sau nu local și dacă este sincronizat cu serverul.

- **Data_Doc_Location** - o enumerare indicând unde se află fișierul, de exemplu, local sau în cloud.

- **Data_Doc_ReadOnlyReasons** - o enumerare indicând doar motivul de citire a unui fișier.

- **Data_Doc_ResourceIdHash** - un GUID care identifică în mod unic ID-ul de resursă server al fișierului.

- **Data_Doc_RtcType** - o enumerare indicând tipul de canal în timp real (RTC) utilizat de fișier.

- **Data_Doc_ServerDocId** - un GUID care identifică în mod unic ID-ul documentului server.

- **Data_Doc_ServerProtocol** - o enumerare indicând protocolul de server al unui fișier în cloud.

- **Data_Doc_ServerType** - o enumerare indicând tipul de server al unui fișier în cloud.

- **Data_Doc_ServerVersion** - o enumerare indicând versiunea serverului unui fișier în cloud.

- **Data_Doc_SessionId** - un număr întreg, incrementat de 1 pentru fiecare operațiune de deschidere a fișierului într-o sesiune.

- **Data_Doc_SharePointServiceContext** - un șir utilizat la corelarea jurnalelor din partea client și pe partea de server, de obicei, este un fel de ID.

- **Data_Doc_SizeInBytes** - dimensiunea documentului în octeți

- **Data_Doc_SpecialChars** - o enumerare indicând ce tip de caracter special are adresa URL a fișierului.

- **Data_Doc_UrlHash** - un GUID care identifică în mod unic URL-ul fișierului.

- **Data_Doc_UsedWrsDataOnOpen** - dacă fișierul a fost deschis incremental folosind datele WRS memorate pre-cache.

- **Data_Doc_WopiServiceId** - un șir indicând ce serviciu este un fișier aplicație de interfață deschisă pentru aplicația web (WOPI).

- **Data_ErrorId_Code** - un cod de eroare care indică o eroare în operațiunea de colectare a datelor

- **Data_ErrorId_Tag** - o etichetă din cod pentru a vă ajuta să găsiți punctul de eroare

- **Data_FileOpenFlowMarkers** - înainte de a începe procesul de deschidere a fișierului, există unele preprocesări implicate. Acest timp necesar pentru preprocesare este capturată într-o valoare șir care are formatul \<functionId>\<functionValue>\<functionId>\<functionValue>...

- **Data_FirstPartyProviderApp** - dacă un fișier deschis în Word, Excel sau PowerPoint, sau în aplicațiile Office este invocată de la o altă aplicație Microsoft, atunci numele aplicației furnizorul respectiv este capturat aici.

- **Data_InclusiveMeasurements** - o valoare șir de logare durata de timp petrecută în anumite apeluri de funcție, într-un format cu eticheta funcției și durata, care include durata apelurilor subfuncții. 

- **Data_InitializationReason** - o enumerare indicând modul în care se deschide fișierul, de ex. element UI, declanșat de altă aplicație etc.

- **Data_Measurements** - o valoare șir care conectează timpul petrecut în anumite apeluri de funcție într-un format cu eticheta funcției și durata care include durata apelurilor subfuncție.

- **Data_OfficeMobileInitReason** - o enumerare care indică punctul de intrare al fișierului deschis. 

- **Data_RenderToInSpaceDuration** - durata dintre sfârșitul de randare și animația conturului/pânzei.

- **Data_SilhouetteDuration** - durata de randare a fișierului deschis.

- **Data_TimeSplitMeasurements** - o valoare șir de logare durata de timp petrecută în anumite apeluri de funcție, într-un format cu eticheta funcției și ora de început și durata. 

#### <a name="officeandroiddocsuipaywallcontrolskuchoosertoggled"></a>Office.Android.DocsUI.PaywallControl.SkuChooserToggled

Telemetrie de utilizare pentru a vedea de câte ori comută utilizatorul între SKU-uri diferite înainte de a încerca o achiziție. Utilizat pentru a înțelege utilizarea selectorului SKU și pentru optimizarea experienței de achiziționare în cadrul aplicației în versiunile viitoare.

Se colectează următoarele câmpuri:

- **EventDate** – marca de timp pentru când a avut loc evenimentul 

- **SessionID** – GUID pentru conectarea evenimentelor după sesiune

#### <a name="officeandroidearlytelemetryexpansionfilesavailability"></a>Office.Android.EarlyTelemetry.ExpansionFilesAvailability

Activăm fișierele de extindere Pachet kit Android (APK) pentru aplicația Office pentru dispozitive mobile. Fișierele de extindere APK sunt fișiere de resurse suplimentare pe care dezvoltatorii de aplicații Android le pot publica împreună cu aplicația. Pentru a înțelege fiabilitatea fișierelor de extindere, vom înregistra în jurnal o semnalizare care indică dacă fișierele de extindere sunt disponibile sau nu, la fiecare boot.

Se colectează următoarele câmpuri:

- **Data_ExpansionFilesAvailable** - un semnalizator boolean care indică dacă fișierele de extindere APK sunt disponibile pe dispozitiv la momentul bootării aplicației.

#### <a name="officeandroidearlytelemetryexpansionfilesdownloader"></a>Office.Android.EarlyTelemetry.ExpansionFilesDownloader

Activăm fișierele de extindere Pachet kit Android (APK) pentru aplicația Office pentru dispozitive mobile. Fișierele de extindere APK sunt fișiere de resurse suplimentare, pe care dezvoltatorii de aplicații Android le pot publica împreună cu aplicația lor.  Pentru a înțelege fiabilitatea mecanismului de descărcare a fișierului nostru de extindere, înregistrăm o semnalizare care indică dacă reușim să descărcăm cu succes fișiere de extindere.

Se colectează următoarele câmpuri: 

- **Data_DownloadSuccess** - Un semnalizator Boolean care indică dacă descărcarea fișierelor de extindere APK este reușită, de fiecare dată când încercăm o descărcare în timpul bootării aplicației.


#### <a name="officeandroidintuneintunecompliancerequest"></a>Office.Android.Intune.IntuneComplianceRequest

Acest eveniment este colectat pentru aplicații Office care rulează pe Android, inclusiv Office Mobile, Word, Excel, PowerPoint și OneNote. Evenimentul indică o încercare de conectare la un cont de organizație licențiat Intune, unde administratorul organizației a configurat politica pentru a impune accesul condiționat la aplicație. Acesta este utilizat pentru a înțelege numărul de utilizatori finali care încearcă să utilizeze aplicațiile sub această configurare a politicii și este combinat cu un alt eveniment, Office.Android.Intune.IntuneComplianceStatus, pentru a garanta impunerea politicii configurate. 

Nu se colectează câmpuri de date.

#### <a name="officeandroidintuneintunecompliancestatus"></a>Office.Android.Intune.IntuneComplianceStatus

Acest eveniment este colectat pentru aplicații Office care rulează pe Android, inclusiv Office Mobile, Word, Excel, PowerPoint și OneNote. Evenimentul indică o încercare de conectare la un cont de organizație licențiat Intune, unde administratorul organizației a configurat politica pentru a impune accesul condiționat la aplicație. Acest eveniment indică starea de conformitate a aplicației la care utilizatorul s-a conectat și este utilizat pentru a investiga erorile. Acesta este combinat cu un alt eveniment, Office.Android.Intune.IntuneComplianceRequest, pentru a garanta impunerea politicii configurate.
  
Se colectează următoarele câmpuri:

- **Data_ComplianceStatus** - indică starea de conformitate a aplicației în timpul conectării cu un cod de eroare succes sau eșec.
  - -1 – Eroare necunoscută
  -    0 – Aplicația respectă politicile organizației
  - 1 – Aplicația nu respectă politicile organizației
  - 2 – Erori legate de servicii
  - 3 – Erori legate de rețea
  - 4 – Aplicația nu a reușit să regăsească simbolul de autentificare 
  - 5 – Răspunsul din partea serviciului nu a fost încă primit
  - 6 – Aplicația portalul firmei trebuie să fie instalată

#### <a name="officeandroidodwxpssotelemetry"></a>Office.Android.ODWXPSSO.Telemetry

Acest eveniment vă ajută să înțelegeți compatibilitatea cu altă aplicație Microsoft de pe dispozitiv, aplicația noastră are o conectare unică neasistată, de la ce punct de intrare și așa mai departe. De asemenea, vă ajută să înțelegeți motivul erorii în procesul de conectare unică neasistată.  Vom obține detalii mai bune, precum sursa aplicației Microsoft de pe dispozitiv, vom oferi o conectare unică. Acționați asupra erorilor, atunci când conectarea unică nu funcționează așa cum vă așteptați.

Se colectează următoarele câmpuri:

- **AccountType** - Indică tipul de cont cu care se face conectarea unică, cum ar fi cont Microsoft personal sau de la locul de muncă.

- **EntryPoint** - Indică punctul de intrare din aplicație, de unde a fost inițiată tentativa de conectare unică.

- **ErrorCode** - Indică codul de eroare al tentativei de conectare unică.

- **ErrorDescription** - Indică codul de eroare al tentativei de conectare unică.

- **HResult** - Indică codul de stare al rezultatului tentativei de conectare unică.

- **ProviderPackageId** - Altă aplicație Microsoft de pe dispozitiv, de la care se face conectarea unică.

#### <a name="officeandroidphonenumbersignins"></a>Office.Android.PhoneNumberSignIns

Acest eveniment vă ajută să înțelegeți dacă utilizatorul s-a conectat sau s-a înregistrat cu un cont Microsoft cu număr de telefon sau prin e-mail personal.  Acest eveniment vă ajută să cunoașteți numărul de utilizatori care se pot conecta sau să se înregistreze cu un cont Microsoft cu număr de telefon personal.

Se colectează următoarele câmpuri:

- **EntryPoint** - indică punctul de intrare din aplicație, de unde a fost inițiată tentativa de conectare unică.

- **IsEmailMissing** - lipsește e-mailul din informațiile de profil cont?

- **IsPhoneNumberMissing** - lipsește numărul de telefon din informațiile de profil cont?

- **UserDecision** -indică alegerea făcută de către utilizator, cum ar fi de conectare sau de înregistrare sau de conectare ulterioară.

#### <a name="officeandroidusersignindecision"></a>Office. Android. UserSignInDecision

Acest eveniment vă ajută să înțelegeți în ce stadiu de utilizator este retras un flux de conectare, de ce nu reușiți să vă conectați, numărul de utilizatori conectați cu succes din ce punct de intrare din aplicație etc.  Acest eveniment vă ajută să vă conectați la datele din pâlnie, vă ajută să înțelegeți în ce stadiu utilizatorii primesc mai mult etc.

Se colectează următoarele câmpuri:

- **AccountType** - indică tipul de cont cu care se face conectarea unică, cum ar fi contul Microsoft personal sau contul de la locul de muncă.

- **AfterLicensingState** - indică starea de licențiere a aplicațiilor după ce s-a finalizat conectarea.

- **AllowedEditsWithoutSignIn** - indică câte editări libere s-au scurs înainte de a încerca să se conecteze.

- **BeforeLicensingState** - indică starea de licențiere a aplicațiilor după ce s-a finalizat conectarea.

- **CompletionState** - indică etapa finalizării conectării.

- **EntryPoint** - indică punctul de intrare din aplicație, de unde a fost inițiată tentativa de conectare unică.

- **HRDAutoAcceleratedSignUpAttemptCount** - indică numărul de înscrieri accelerate încercate.

- **HRDAutoAcceleratedSignUpQuitCount** - indică numărul de înscrieri accelerate care au fost anulate.

- **HResult** - indică codul de stare al rezultatului operațiunii de conectare.

- **IsPhoneOnlyAuthFeatureEnabled** - este permis sau nu conectarea bazată pe numărul de telefon?

- **LicenseActivationHResult** - indică codul de stare al tentativei de activare a licenței.

- **LicenseActivationMessageCode** - indică codul de mesaj din serviciul de licențiere.

- **NoFreeEditsTreatmentValue** - editările gratuite sunt permise sau nu?

- **SignUpAttemptCount** - indică faptul că numărul de înscrieri a fost încercat.

- **StartMode** - indică modul în care a fost lansată încercarea de conectare.

- **UserDecision** -indică alegerea făcută de către utilizator, cum ar fi de conectare sau de înregistrare sau de conectare ulterioară.

#### <a name="officeappcompatappcompatagentupload"></a>Office.AppCompat.AppCompat.AgentUpload

Generat la pornirea clientului atunci când utilizatorul final a activat Tabloul de bord de telemetrie Office.  Colectează informații despre momentul în care Agentul de telemetrie Office a încărcat date în folderul partajat. Utilizarea principală a acestui eveniment este pentru monitorizarea stării Agentului de telemetrie Office, iar utilizarea secundară a evenimentului este pentru estimarea utilizării Tabloului de bord de telemetrie Office.

Se colectează următoarele câmpuri:

- **UploadTime** - marca de timp a ultimei încărcări reușite efectuate de Agentul de telemetrie.


#### <a name="officeappcompatappcompatagentscanandupload"></a>Office.AppCompat.AppCompat.AgentScanAndUpload

Colectat doar atunci când utilizatorul final a activat Tabloul de bord de telemetrie Office. Colectează informații privind momentul în care se execută Agentul de telemetrie Office.    Acest lucru se colectează doar atunci când Tabloul de bord de telemetrie Office este activat și este utilizat pentru a determina starea de funcționare a agentului de telemetrie Office.

Se colectează următoarele câmpuri:

  - **Data.AgentExit** - marcă de timp privind momentul în care ieșirea agentului de telemetrie se efectuează cu succes

  - **Data.AgentScan** - marcă de timp privind momentul în care agentul de telemetrie a finalizat cu succes o scanare

  - **Data.AgentUpload** - marcă de timp privind momentul în care agentul de telemetrie finalizează cu succes încărcarea

#### <a name="officeappcompatappcompattelemetrydashboardresiliencycrashlog"></a>Office.AppCompat.AppCompat.TelemetryDashboardResiliencyCrashLog

Colectat doar atunci când Tabloul de bord de telemetrie Office a fost activat de utilizatorul final (cel mai probabil un administrator). Colectează apariția unor căderi de documente și programe de completare Office.  Se colectează doar atunci când utilizatorul a activat Tabloul de bord de telemetrie Office și este utilizat pentru a stabili dacă au loc mai multe căderi de programe de completare sau documente.

Se colectează următoarele câmpuri:

  - **Data.CollectionTime** - marcă de timp privind momentul în care a fost înregistrat în jurnal un eveniment de cădere

#### <a name="officeappdocsappdocsdocumentoperation"></a>Office.AppDocs.AppDocs.DocumentOperation

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platformele Android, iOS, Universal și Windows. Evenimentul înregistrează momentul când are loc o operațiune de fișier (creare/deschidere/salvare/export/etc/) și este utilizat pentru a înțelege experiențele de utilizator, pe baza informațiilor de operațiune a fișierelor.

Se colectează următoarele câmpuri:

- **Data_AppIdForReportEndBeforeAppKnown** - ID-ul de aplicație, atunci când nu este cunoscut înainte de a fi solicitat sfârșitul raportului în operațiune.

- **Data_CanContinueFromOnBeforeOperationBegins** - starea CanContinue, înainte de a invoca inițierea rutinei de tratare.

- **Data_DetachedDuration** – durata procesului de detașare a unui eveniment. 

- **Data_Doc_AccessMode** – o enumerare care indică modul de acces al fișierului, de exemplu, doar în citire, citire-scriere.

- **Data_Doc_AsyncOpenKind** – o enumerare care indică tipul de flux asincron utilizat pentru deschiderea fișierului.

- **Data_Doc_ChunkingType** – o enumerare care indică tipul de algoritm de segmentare al unui fișier.

- **Data_Doc_EdpState** – o enumerare care indică starea de protecție datelor la nivel de întreprindere ale unui fișier.

- **Data_Doc_Ext** - primele 4 caractere din extensia fișierului.

- **Data_Doc_Fqdn** – nume gazdă server al fișierului.

- **Data_Doc_FqdnHash** – un GUID care identifică în mod unic numele de gazdă server.

- **Data_Doc_IdentityTelemetryId** - codul hash unidirecțional al identității utilizatorului folosită pentru efectuarea deschiderii.

- **Data_Doc_InitializationScenario** – o enumerare care indică tipul de scenariu detaliat al unei operațiuni de deschidere a fișierelor.

- **Data_Doc_IOFlags** – o enumerare care indică semnalizările IO ale unei operațiuni de deschidere a fișierelor, de exemplu, dacă fișierul este în cache sau nu.

- **Data_Doc_IsCloudCollabEnabled** – dacă colaborarea în cloud este activată sau nu pentru fișier.

- **Data_Doc_IsIncrementalOpen** – dacă fișierul a fost sau nu deschis prin deschidere treptată.

- **Data_Doc_IsOcsSupported** – dacă un fișier acceptă sau nu serviciul de colaborare Office.

- **Data_Doc_IsOpeningOfflineCopy** – dacă un fișier dintr-o copie memorată în cache offline se deschide sau nu.

- **Data_Doc_IsPrefetched** – dacă fișierul înainte de operațiunea de deschidere a fost sau nu preluat.

- **Data_Doc_IsSyncBacked** – dacă un fișier în cloud există sau nu local și dacă este sincronizat cu serverul.

- **Data_Doc_Location** – o enumerare care indică unde se află fișierul, de exemplu, local sau în cloud.

- **Data_Doc_ReadOnlyReasons** – o enumerare care indică motivul doar în citire al unui fișier.

- **Data_Doc_ResourceIdHash** – un GUID care identifică în mod unic ID-ul de resursă server al fișierului.

- **Data_Doc_RtcType** – o enumerare care indică tipul de canal în timp real (RTC) utilizat de fișier.

- **Data_Doc_ServerDocId** – un GUID care identifică în mod unic ID-ul de document server.

- **Data_Doc_ServerProtocol** – o enumerare care indică protocolul de server al unui fișier în cloud.

- **Data_Doc_ServerType** – o enumerare care indică tipul de server al unui fișier în cloud.

- **Data_Doc_ServerVersion** – o enumerare care indică versiunea de server al unui fișier în cloud.

- **Data_Doc_SessionId** – un număr întreg, crescut cu 1 pentru fiecare operațiune de deschidere a fișierului într-o sesiune.

- **Data_Doc_SharePointServiceContext** – un șir utilizat pentru corelarea jurnalelor din partea client și de partea server, de obicei, este un fel de ID.

- **Data_Doc_SizeInBytes** – dimensiunea documentului în octeți.

- **Data_Doc_SpecialChars** – o enumerare indicând ce tip de caracter special are adresa URL a fișierului.

- **Data_Doc_UrlHash** – un GUID care identifică în mod unic URL-ul fișierului.

- **Data_Doc_UsedWrsDataOnOpen** – dacă fișierul a fost sau nu deschis incremental folosind datele WRS memorate pre-cache.

- **Data_Doc_WopiServiceId** – un șir care indică de la ce serviciu provine un fișier WOPI (aplicație de interfață deschisă pentru aplicația web).

- **Data_DocumentInputCurrency** – tipul de intrare a documentului utilizat de operațiune.

- **Data_DocumentOperation_AppId** – valoarea de enumerare reprezentând ID-ul unei aplicații.

- **Data_DocumentOperation_EndEventId** – eticheta care reprezintă locul în care operațiunea s-a încheiat.

- **Data_DocumentOperation_EndReason** – valoarea de enumerare reprezentând motivul final.

- **Data_DocumentOperation_IsReinitialized** – reinițializează un document deja deschis.

- **Data_DocumentOperation_isTargetECBeginEC** - dacă contextul de execuție a țintei este identică cu contextul din care a fost deschis.

- **Data_DocumentOperation_ParamsFlags** – semnalizările de enumerare utilizate pentru a porni operațiunea.

- **Data_DocumentOperation_TelemetryReason** – reprezentarea de enumerare a punctului de intrare pentru evenimentul deschis. De exemplu, deschideți din MRU sau navigați, activare fișier etc.

- **Data_FileOInclusiveMeasurements** – o valoare șir care înregistrează durata de timp petrecută în anumite apeluri de funcții, într-un format cu eticheta funcției și durata care include durata apelurilor de sub-funcții.

- **Data_FileOMeasurements** – o valoare șir care înregistrează timpul petrecut în anumite apeluri de funcții, într-un format cu eticheta funcției și durata care exclude durata apelurilor de sub-funcții.

- **Data_InitializationReason** - reprezentarea enumerării a motivului specific al operațiunii. Ex - deschideți de la o adresă URL sau dintr-o cale de fișier locală, creați cu selectorul de fișiere, copiați la calea fișierului, exportați la URL etc.

- **Data_IsDisambiguateCsiNetworkConnectivityErrorEnabled** .

- **Data_IsNameMissingInUrl** – indică dacă numele nu a fost analizat din URL.

- **Data_IsPathMissingForLocalFile** – indică dacă acesta este un fișier local fără cale.

- **Data_IsUnpackedLinkSupportedForOpen** – indică dacă linkurile neambalate sunt acceptate pentru deschidere.

- **Data_LinksOpenRightScenario** – valoare de enumerare pentru linkurile din scenariul de deschidere din dreapta.

- **Data_OpEndEventId** - eticheta care reprezintă locul în care operațiunea s-a încheiat.

- **Data_OperationType** - reprezentarea enumerării tipului generic de operațiune. Ex -creare, deschidere, copiere, salvare etc.

- **Data_RelatedPrevOpTelemetryReason** – este operațiunea corelată cu operațiunea anterioară.

- **Data_StopwatchDuration** – timpul total pentru eveniment.

- **Data_UnpackLinkHint** – enumerarea reprezentând acțiunea potențială a utilizatorului, pe baza unui link de dezarhivare.

- **Data_UnpackLinkPromptResult** – enumerarea reprezentând răspunsul solicitării de dezarhivare a linkului.

#### <a name="officedocsappdocsoperationopenfrommrubypath"></a>Office.Docs.AppDocs.OperationOpenFromMruByPath

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platformele Android, iOS, Universal și Windows. Acest eveniment înregistrează atunci când are loc o operațiune de deschidere a fișierelor din calea furnizată de lista utilizată cel mai recent și este folosit pentru a înțelege și pentru a acorda prioritate experienței utilizatorului pe baza informațiilor operațiunii de deschidere a fișierelor.

Se colectează următoarele câmpuri:

- **Data_AppIdForReportEndBeforeAppKnown** - ID-ul de aplicație, atunci când nu este cunoscut înainte de a fi solicitat sfârșitul raportului în operațiune.

- **Data_CanContinueFromOnBeforeOperationBegins** - starea CanContinue, înainte de a invoca inițierea rutinei de tratare.

- **Data_DetachedDuration** – durata procesului de detașare a unui eveniment. 

- **Data_Doc_AccessMode** – o enumerare care indică modul de acces al fișierului, de exemplu, doar în citire, citire-scriere.

- **Data_Doc_AsyncOpenKind** – o enumerare care indică tipul de flux asincron utilizat pentru deschiderea fișierului.

- **Data_Doc_ChunkingType** – o enumerare care indică tipul de algoritm de segmentare al unui fișier.

- **Data_Doc_EdpState** – o enumerare care indică starea de protecție datelor la nivel de întreprindere ale unui fișier.

- **Data_Doc_Ext** – primele patru caractere din extensia fișierului.

- **Data_Doc_Fqdn** – nume gazdă server al fișierului.

- **Data_Doc_FqdnHash** – un GUID care identifică în mod unic numele de gazdă server.

- **Data_Doc_IdentityTelemetryId** – codul hash unidirecțional al identității de utilizator folosit pentru a efectua deschiderea.

- **Data_Doc_InitializationScenario** – o enumerare care indică tipul de scenariu detaliat al unei operațiuni de deschidere a fișierelor.

- **Data_Doc_IOFlags** – o enumerare care indică semnalizările IO ale unei operațiuni de deschidere a fișierelor, de exemplu, dacă fișierul este în cache sau nu.

- **Data_Doc_IsCloudCollabEnabled** – dacă colaborarea în cloud este activată sau nu pentru fișier.

- **Data_Doc_IsIncrementalOpen** – dacă fișierul a fost sau nu deschis prin deschidere treptată.

- **Data_Doc_IsOcsSupported** – dacă un fișier acceptă sau nu serviciul de colaborare Office.

- **Data_Doc_IsOpeningOfflineCopy** – dacă un fișier dintr-o copie memorată în cache offline se deschide sau nu.

- **Data_Doc_IsPrefetched** – dacă fișierul înainte de operațiunea de deschidere a fost sau nu preluat.

- **Data_Doc_IsSyncBacked** – dacă un fișier în cloud există sau nu local și dacă este sincronizat cu serverul.

- **Data_Doc_Location** – o enumerare care indică unde se află fișierul, de exemplu, local sau în cloud.

- **Data_Doc_ReadOnlyReasons** – o enumerare care indică motivul doar în citire al unui fișier.

- **Data_Doc_ResourceIdHash** – un GUID care identifică în mod unic ID-ul de resursă server al fișierului.

- **Data_Doc_RtcType** – o enumerare care indică tipul de canal în timp real (RTC) utilizat de fișier.

- **Data_Doc_ServerDocId** – un GUID care identifică în mod unic ID-ul de document server.

- **Data_Doc_ServerProtocol** – o enumerare care indică protocolul de server al unui fișier în cloud.

- **Data_Doc_ServerType** – o enumerare care indică tipul de server al unui fișier în cloud.

- **Data_Doc_ServerVersion** – o enumerare care indică versiunea de server al unui fișier în cloud.

- **Data_Doc_SessionId** – un număr întreg, crescut cu 1 pentru fiecare operațiune de deschidere a fișierului într-o sesiune.

- **Data_Doc_SharePointServiceContext** – un șir utilizat pentru corelarea jurnalelor din partea client și de partea server, de obicei, este un fel de ID.

- **Data_Doc_SizeInBytes** – dimensiunea documentului în octeți.

- **Data_Doc_SpecialChars** – o enumerare indicând ce tip de caracter special are adresa URL a fișierului.

- **Data_Doc_UrlHash** – un GUID care identifică în mod unic URL-ul fișierului.

- **Data_Doc_UsedWrsDataOnOpen** – dacă fișierul a fost sau nu deschis incremental folosind datele WRS memorate pre-cache.

- **Data_Doc_WopiServiceId** – un șir care indică de la ce serviciu provine un fișier WOPI (aplicație de interfață deschisă pentru aplicația web).

- **Data_DocumentInputCurrency** – tipul de intrare a documentului utilizat de operațiune.

- **Data_DocumentOperation_AppId** – valoarea de enumerare reprezentând ID-ul unei aplicații.

- **Data_DocumentOperation_EndEventId** – eticheta care reprezintă locul în care operațiunea s-a încheiat.

- **Data_DocumentOperation_EndReason** – valoarea de enumerare reprezentând motivul final.

- **Data_DocumentOperation_IsReinitialized** – reinițializează un document deja deschis.

- **Data_DocumentOperation_ParamsFlags** – semnalizările de enumerare utilizate pentru a porni operațiunea.

- **Data_DocumentOperation_TelemetryReason** – reprezentarea de enumerare a punctului de intrare pentru evenimentul deschis. De exemplu, deschideți din MRU sau navigați, activare fișier etc.

- **Data_DocumentOperation_isTargetECBeginEC** – dacă contextul de execuție a țintei este același ca și contextul din care a fost deschis.

- **Data_FileOInclusiveMeasurements** – o valoare șir care înregistrează durata de timp petrecută în anumite apeluri de funcții, într-un format cu eticheta funcției și durata care include durata apelurilor de sub-funcții.

- **Data_FileOMeasurements** – o valoare șir care înregistrează timpul petrecut în anumite apeluri de funcții, într-un format cu eticheta funcției și durata care exclude durata apelurilor de sub-funcții.

- **Data_IsNameMissingInUrl** – indică dacă numele nu a fost analizat din URL.

- **Data_IsPathMissingForLocalFile** – indică dacă acesta este un fișier local fără cale.

- **Data_IsUnpackedLinkSupportedForOpen** – indică dacă linkurile neambalate sunt acceptate pentru deschidere.

- **Data_LinksOpenRightScenario** – valoare de enumerare pentru linkurile din scenariul de deschidere din dreapta.

- **Data_OpEndEventId** - eticheta care reprezintă locul în care operațiunea s-a încheiat.

- **Data_RelatedPrevOpTelemetryReason** – este operațiunea corelată cu operațiunea anterioară.

- **Data_StopwatchDuration** – timpul total pentru eveniment.

- **Data_UnpackLinkHint** – enumerarea reprezentând acțiunea potențială a utilizatorului, pe baza unui link de dezarhivare.

- **Data_UnpackLinkPromptResult** – enumerarea reprezentând răspunsul solicitării de dezarhivare a linkului.

#### <a name="officedocsappdocsoperationopenfrommrubyurl"></a>Office.Docs.AppDocs.OperationOpenFromMruByUrl

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platformele Android, iOS, Universal și Windows. Evenimentul înregistrează atunci când are loc o operațiune de deschidere a fișierelor din URL-ul furnizat în lista utilizată cel mai recent și este folosit pentru a înțelege și pentru a acorda prioritare experienței utilizatorului, pe baza informațiilor despre operațiune de deschidere a fișierului. 

Se colectează următoarele câmpuri:

- **Data_AppIdForReportEndBeforeAppKnown** - ID-ul de aplicație, atunci când nu este cunoscut înainte de a fi solicitat sfârșitul raportului în operațiune.

- **Data_CanContinueFromOnBeforeOperationBegins** - starea CanContinue, înainte de a invoca inițierea rutinei de tratare.

- **Data_DetachedDuration** – durata procesului de detașare a unui eveniment. 

- **Data_Doc_AccessMode** – o enumerare care indică modul de acces al fișierului, de exemplu, doar în citire, citire-scriere.

- **Data_Doc_AsyncOpenKind** – o enumerare care indică tipul de flux asincron utilizat pentru deschiderea fișierului.

- **Data_Doc_ChunkingType** – o enumerare care indică tipul de algoritm de segmentare al unui fișier.

- **Data_Doc_EdpState** – o enumerare care indică starea de protecție datelor la nivel de întreprindere ale unui fișier.

- **Data_Doc_Ext** – primele patru caractere din extensia fișierului.

- **Data_Doc_Fqdn** – nume gazdă server al fișierului.

- **Data_Doc_FqdnHash** – un GUID care identifică în mod unic numele de gazdă server.

- **Data_Doc_IdentityTelemetryId** – codul hash unidirecțional al identității de utilizator folosit pentru a efectua deschiderea.

- **Data_Doc_InitializationScenario** – o enumerare care indică tipul de scenariu detaliat al unei operațiuni de deschidere a fișierelor.

- **Data_Doc_IOFlags** – o enumerare care indică semnalizările IO ale unei operațiuni de deschidere a fișierelor, de exemplu, dacă fișierul este în cache sau nu.

- **Data_Doc_IsCloudCollabEnabled** – dacă colaborarea în cloud este activată sau nu pentru fișier.

- **Data_Doc_IsIncrementalOpen** – dacă fișierul a fost sau nu deschis prin deschidere treptată.

- **Data_Doc_IsOcsSupported** – dacă un fișier acceptă sau nu serviciul de colaborare Office.

- **Data_Doc_IsOpeningOfflineCopy** – dacă un fișier dintr-o copie memorată în cache offline se deschide sau nu.

- **Data_Doc_IsPrefetched** – dacă fișierul înainte de operațiunea de deschidere a fost sau nu preluat.

- **Data_Doc_IsSyncBacked** – dacă un fișier în cloud există sau nu local și dacă este sincronizat cu serverul.

- **Data_Doc_Location** – o enumerare care indică unde se află fișierul, de exemplu, local sau în cloud.

- **Data_Doc_ReadOnlyReasons** – o enumerare care indică motivul doar în citire al unui fișier.

- **Data_Doc_ResourceIdHash** – un GUID care identifică în mod unic ID-ul de resursă server al fișierului.

- **Data_Doc_RtcType** – o enumerare care indică tipul de canal în timp real (RTC) utilizat de fișier.

- **Data_Doc_ServerDocId** – un GUID care identifică în mod unic ID-ul de document server.

- **Data_Doc_ServerProtocol** – o enumerare care indică protocolul de server al unui fișier în cloud.

- **Data_Doc_ServerType** – o enumerare care indică tipul de server al unui fișier în cloud.

- **Data_Doc_ServerVersion** – o enumerare care indică versiunea de server al unui fișier în cloud.

- **Data_Doc_SessionId** – un număr întreg, crescut cu 1 pentru fiecare operațiune de deschidere a fișierului într-o sesiune.

- **Data_Doc_SharePointServiceContext** – un șir utilizat pentru corelarea jurnalelor din partea client și de partea server, de obicei, este un fel de ID.

- **Data_Doc_SizeInBytes** – dimensiunea documentului în octeți.

- **Data_Doc_SpecialChars** – o enumerare indicând ce tip de caracter special are adresa URL a fișierului.

- **Data_Doc_UrlHash** – un GUID care identifică în mod unic URL-ul fișierului.

- **Data_Doc_UsedWrsDataOnOpen** – dacă fișierul a fost sau nu deschis incremental folosind datele WRS memorate pre-cache.

- **Data_Doc_WopiServiceId** – un șir care indică de la ce serviciu provine un fișier WOPI (aplicație de interfață deschisă pentru aplicația web).

- **Data_DocumentInputCurrency** – tipul de intrare a documentului utilizat de operațiune.

- **Data_DocumentOperation_AppId** – valoarea de enumerare reprezentând ID-ul unei aplicații.

- **Data_DocumentOperation_EndEventId** – eticheta care reprezintă locul în care operațiunea s-a încheiat.

- **Data_DocumentOperation_EndReason** – valoarea de enumerare reprezentând motivul final.

- **Data_DocumentOperation_IsReinitialized** – reinițializează un document deja deschis.

- **Data_DocumentOperation_ParamsFlags** – semnalizările de enumerare utilizate pentru a porni operațiunea.

- **Data_DocumentOperation_TelemetryReason** – reprezentarea de enumerare a punctului de intrare pentru evenimentul deschis. De exemplu, deschideți din MRU sau navigați, activare fișier etc.

- **Data_DocumentOperation_isTargetECBeginEC** – dacă contextul de execuție a țintei este același ca și contextul din care a fost deschis.

- **Data_FileOInclusiveMeasurements** – o valoare șir care înregistrează durata de timp petrecută în anumite apeluri de funcții, într-un format cu eticheta funcției și durata care include durata apelurilor de sub-funcții.

- **Data_FileOMeasurements** – o valoare șir care înregistrează timpul petrecut în anumite apeluri de funcții, într-un format cu eticheta funcției și durata care exclude durata apelurilor de sub-funcții.

- **Data_IsNameMissingInUrl** – indică dacă numele nu a fost analizat din URL.

- **Data_IsPathMissingForLocalFile** – indică dacă acesta este un fișier local fără cale.

- **Data_IsUnpackedLinkSupportedForOpen** – indică dacă linkurile neambalate sunt acceptate pentru deschidere.

- **Data_LinksOpenRightScenario** – valoare de enumerare pentru linkurile din scenariul de deschidere din dreapta.

- **Data_OpEndEventId** - eticheta care reprezintă locul în care operațiunea s-a încheiat.

- **Data_RelatedPrevOpTelemetryReason** – este operațiunea corelată cu operațiunea anterioară.

- **Data_StopwatchDuration** – timpul total pentru eveniment.

- **Data_UnpackLinkHint** – enumerarea reprezentând acțiunea potențială a utilizatorului, pe baza unui link de dezarhivare.

- **Data_UnpackLinkPromptResult** – enumerarea reprezentând răspunsul solicitării de dezarhivare a linkului.


#### <a name="officedocsappdocsoperationopenfrompath"></a>Office.Docs.AppDocs.OperationOpenFromPath

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platformele Android, iOS, Universal și Windows. Evenimentul înregistrează atunci când are loc o operațiune de deschidere a fișierului de pe o cale și este folosit pentru a înțelege și pentru a acorda prioritare experiențelor utilizatorului, pe baza informațiilor despre operațiunea de deschidere a fișierelor.

Se colectează următoarele câmpuri:

- **Data_AppIdForReportEndBeforeAppKnown** - ID-ul de aplicație, atunci când nu este cunoscut înainte de a fi solicitat sfârșitul raportului în operațiune.

- **Data_CanContinueFromOnBeforeOperationBegins** - starea CanContinue, înainte de a invoca inițierea rutinei de tratare.

- **Data_DetachedDuration** – durata procesului de detașare a unui eveniment. 

- **Data_Doc_AccessMode** – o enumerare care indică modul de acces al fișierului, de exemplu, doar în citire, citire-scriere.

- **Data_Doc_AsyncOpenKind** – o enumerare care indică tipul de flux asincron utilizat pentru deschiderea fișierului.

- **Data_Doc_ChunkingType** – o enumerare care indică tipul de algoritm de segmentare al unui fișier.

- **Data_Doc_EdpState** – o enumerare care indică starea de protecție datelor la nivel de întreprindere ale unui fișier.

- **Data_Doc_Ext** – primele patru caractere din extensia fișierului.

- **Data_Doc_Fqdn** – nume gazdă server al fișierului.

- **Data_Doc_FqdnHash** – un GUID care identifică în mod unic numele de gazdă server.

- **Data_Doc_IdentityTelemetryId** – codul hash unidirecțional al identității de utilizator folosit pentru a efectua deschiderea.

- **Data_Doc_InitializationScenario** – o enumerare care indică tipul de scenariu detaliat al unei operațiuni de deschidere a fișierelor.

- **Data_Doc_IOFlags** – o enumerare care indică semnalizările IO ale unei operațiuni de deschidere a fișierelor, de exemplu, dacă fișierul este în cache sau nu.

- **Data_Doc_IsCloudCollabEnabled** – dacă colaborarea în cloud este activată sau nu pentru fișier.

- **Data_Doc_IsIncrementalOpen** – dacă fișierul a fost sau nu deschis prin deschidere treptată.

- **Data_Doc_IsOcsSupported** – dacă un fișier acceptă sau nu serviciul de colaborare Office.

- **Data_Doc_IsOpeningOfflineCopy** – dacă un fișier dintr-o copie memorată în cache offline se deschide sau nu.

- **Data_Doc_IsPrefetched** – dacă fișierul înainte de operațiunea de deschidere a fost sau nu preluat.

- **Data_Doc_IsSyncBacked** – dacă un fișier în cloud există sau nu local și dacă este sincronizat cu serverul.

- **Data_Doc_Location** – o enumerare care indică unde se află fișierul, de exemplu, local sau în cloud.

- **Data_Doc_ReadOnlyReasons** – o enumerare care indică motivul doar în citire al unui fișier.

- **Data_Doc_ResourceIdHash** – un GUID care identifică în mod unic ID-ul de resursă server al fișierului.

- **Data_Doc_RtcType** – o enumerare care indică tipul de canal în timp real (RTC) utilizat de fișier.

- **Data_Doc_ServerDocId** – un GUID care identifică în mod unic ID-ul de document server.

- **Data_Doc_ServerProtocol** – o enumerare care indică protocolul de server al unui fișier în cloud.

- **Data_Doc_ServerType** – o enumerare care indică tipul de server al unui fișier în cloud.

- **Data_Doc_ServerVersion** – o enumerare care indică versiunea de server al unui fișier în cloud.

- **Data_Doc_SessionId** – un număr întreg, crescut cu 1 pentru fiecare operațiune de deschidere a fișierului într-o sesiune.

- **Data_Doc_SharePointServiceContext** – un șir utilizat pentru corelarea jurnalelor din partea client și de partea server, de obicei, este un fel de ID.

- **Data_Doc_SizeInBytes** – dimensiunea documentului în octeți.

- **Data_Doc_SpecialChars** – o enumerare indicând ce tip de caracter special are adresa URL a fișierului.

- **Data_Doc_UrlHash** – un GUID care identifică în mod unic URL-ul fișierului.

- **Data_Doc_UsedWrsDataOnOpen** – dacă fișierul a fost sau nu deschis incremental folosind datele WRS memorate pre-cache.

- **Data_Doc_WopiServiceId** – un șir care indică de la ce serviciu provine un fișier WOPI (aplicație de interfață deschisă pentru aplicația web).

- **Data_DocumentInputCurrency** – tipul de intrare a documentului utilizat de operațiune.

- **Data_DocumentOperation_AppId** – valoarea de enumerare reprezentând ID-ul unei aplicații.

- **Data_DocumentOperation_EndEventId** – eticheta care reprezintă locul în care operațiunea s-a încheiat.

- **Data_DocumentOperation_EndReason** – valoarea de enumerare reprezentând motivul final.

- **Data_DocumentOperation_IsReinitialized** – reinițializează un document deja deschis.

- **Data_DocumentOperation_ParamsFlags** – semnalizările de enumerare utilizate pentru a porni operațiunea.

- **Data_DocumentOperation_TelemetryReason** – reprezentarea de enumerare a punctului de intrare pentru evenimentul deschis. De exemplu, deschideți din MRU sau navigați, activare fișier etc.

- **Data_DocumentOperation_isTargetECBeginEC** – dacă contextul de execuție a țintei este același ca și contextul din care a fost deschis.

- **Data_FileOInclusiveMeasurements** – o valoare șir care înregistrează durata de timp petrecută în anumite apeluri de funcții, într-un format cu eticheta funcției și durata care include durata apelurilor de sub-funcții.

- **Data_FileOMeasurements** – o valoare șir care înregistrează timpul petrecut în anumite apeluri de funcții, într-un format cu eticheta funcției și durata care exclude durata apelurilor de sub-funcții.

- **Data_IsNameMissingInUrl** – indică dacă numele nu a fost analizat din URL.

- **Data_IsPathMissingForLocalFile** – indică dacă acesta este un fișier local fără cale.

- **Data_IsUnpackedLinkSupportedForOpen** – indică dacă linkurile neambalate sunt acceptate pentru deschidere.

- **Data_LinksOpenRightScenario** – valoare de enumerare pentru linkurile din scenariul de deschidere din dreapta.

- **Data_OpEndEventId** - eticheta care reprezintă locul în care operațiunea s-a încheiat.

- **Data_RelatedPrevOpTelemetryReason** – este operațiunea corelată cu operațiunea anterioară.

- **Data_StopwatchDuration** – timpul total pentru eveniment.

- **Data_UnpackLinkHint** – enumerarea reprezentând acțiunea potențială a utilizatorului, pe baza unui link de dezarhivare.

- **Data_UnpackLinkPromptResult** – enumerarea reprezentând răspunsul solicitării de dezarhivare a linkului.

#### <a name="officedocsappdocsoperationopenfromprotocolhandler"></a>Office.Docs.AppDocs.OperationOpenFromProtocolHandler

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platformele Android, iOS, Universal și Windows. Evenimentul înregistrează atunci când are loc o operațiune de deschidere a fișierului dintr-o altă aplicație folosind interfața rutinei de tratare al protocolului și este folosit pentru a înțelege și pentru a acorda prioritare experiențelor utilizatorului, pe baza informațiilor despre operațiune de deschidere a fișierelor.

Se colectează următoarele câmpuri:

- **Data_AppIdForReportEndBeforeAppKnown** - ID-ul de aplicație, atunci când nu este cunoscut înainte de a fi solicitat sfârșitul raportului în operațiune.

- **Data_CanContinueFromOnBeforeOperationBegins** - starea CanContinue, înainte de a invoca inițierea rutinei de tratare.

- **Data_DetachedDuration** – durata procesului de detașare a unui eveniment. 

- **Data_Doc_AccessMode** – o enumerare care indică modul de acces al fișierului, de exemplu, doar în citire, citire-scriere.

- **Data_Doc_AsyncOpenKind** – o enumerare care indică tipul de flux asincron utilizat pentru deschiderea fișierului.

- **Data_Doc_ChunkingType** – o enumerare care indică tipul de algoritm de segmentare al unui fișier.

- **Data_Doc_EdpState** – o enumerare care indică starea de protecție datelor la nivel de întreprindere ale unui fișier.

- **Data_Doc_Ext** – primele patru caractere din extensia fișierului.

- **Data_Doc_Fqdn** – nume gazdă server al fișierului.

- **Data_Doc_FqdnHash** – un GUID care identifică în mod unic numele de gazdă server.

- **Data_Doc_IdentityTelemetryId** – codul hash unidirecțional al identității de utilizator folosit pentru a efectua deschiderea.

- **Data_Doc_InitializationScenario** – o enumerare care indică tipul de scenariu detaliat al unei operațiuni de deschidere a fișierelor.

- **Data_Doc_IOFlags** – o enumerare care indică semnalizările IO ale unei operațiuni de deschidere a fișierelor, de exemplu, dacă fișierul este în cache sau nu.

- **Data_Doc_IsCloudCollabEnabled** – dacă colaborarea în cloud este activată sau nu pentru fișier.

- **Data_Doc_IsIncrementalOpen** – dacă fișierul a fost sau nu deschis prin deschidere treptată.

- **Data_Doc_IsOcsSupported** – dacă un fișier acceptă sau nu serviciul de colaborare Office.

- **Data_Doc_IsOpeningOfflineCopy** – dacă un fișier dintr-o copie memorată în cache offline se deschide sau nu.

- **Data_Doc_IsPrefetched** – dacă fișierul înainte de operațiunea de deschidere a fost sau nu preluat.

- **Data_Doc_IsSyncBacked** – dacă un fișier în cloud există sau nu local și dacă este sincronizat cu serverul.

- **Data_Doc_Location** – o enumerare care indică unde se află fișierul, de exemplu, local sau în cloud.

- **Data_Doc_ReadOnlyReasons** – o enumerare care indică motivul doar în citire al unui fișier.

- **Data_Doc_ResourceIdHash** – un GUID care identifică în mod unic ID-ul de resursă server al fișierului.

- **Data_Doc_RtcType** – o enumerare care indică tipul de canal în timp real (RTC) utilizat de fișier.

- **Data_Doc_ServerDocId** – un GUID care identifică în mod unic ID-ul de document server.

- **Data_Doc_ServerProtocol** – o enumerare care indică protocolul de server al unui fișier în cloud.

- **Data_Doc_ServerType** – o enumerare care indică tipul de server al unui fișier în cloud.

- **Data_Doc_ServerVersion** – o enumerare care indică versiunea de server al unui fișier în cloud.

- **Data_Doc_SessionId** – un număr întreg, crescut cu 1 pentru fiecare operațiune de deschidere a fișierului într-o sesiune.

- **Data_Doc_SharePointServiceContext** – un șir utilizat pentru corelarea jurnalelor din partea client și de partea server, de obicei, este un fel de ID.

- **Data_Doc_SizeInBytes** – dimensiunea documentului în octeți.

- **Data_Doc_SpecialChars** – o enumerare indicând ce tip de caracter special are adresa URL a fișierului.

- **Data_Doc_UrlHash** – un GUID care identifică în mod unic URL-ul fișierului.

- **Data_Doc_UsedWrsDataOnOpen** – dacă fișierul a fost sau nu deschis incremental folosind datele WRS memorate pre-cache.

- **Data_Doc_WopiServiceId** – un șir care indică de la ce serviciu provine un fișier WOPI (aplicație de interfață deschisă pentru aplicația web).

- **Data_DocumentInputCurrency** – tipul de intrare a documentului utilizat de operațiune.

- **Data_DocumentOperation_AppId** – valoarea de enumerare reprezentând ID-ul unei aplicații.

- **Data_DocumentOperation_EndEventId** – eticheta care reprezintă locul în care operațiunea s-a încheiat.

- **Data_DocumentOperation_EndReason** – valoarea de enumerare reprezentând motivul final.

- **Data_DocumentOperation_IsReinitialized** – reinițializează un document deja deschis.

- **Data_DocumentOperation_ParamsFlags** – semnalizările de enumerare utilizate pentru a porni operațiunea.

- **Data_DocumentOperation_TelemetryReason** – reprezentarea de enumerare a punctului de intrare pentru evenimentul deschis. De exemplu, deschideți din MRU sau navigați, activare fișier etc.

- **Data_DocumentOperation_isTargetECBeginEC** – dacă contextul de execuție a țintei este același ca și contextul din care a fost deschis.

- **Data_FileOInclusiveMeasurements** – o valoare șir care înregistrează durata de timp petrecută în anumite apeluri de funcții, într-un format cu eticheta funcției și durata care include durata apelurilor de sub-funcții.

- **Data_FileOMeasurements** – o valoare șir care înregistrează timpul petrecut în anumite apeluri de funcții, într-un format cu eticheta funcției și durata care exclude durata apelurilor de sub-funcții.

- **Data_IsNameMissingInUrl** – indică dacă numele nu a fost analizat din URL.

- **Data_IsPathMissingForLocalFile** – indică dacă acesta este un fișier local fără cale.

- **Data_IsUnpackedLinkSupportedForOpen** – indică dacă linkurile neambalate sunt acceptate pentru deschidere.

- **Data_LinksOpenRightScenario** – valoare de enumerare pentru linkurile din scenariul de deschidere din dreapta.

- **Data_OpEndEventId** - eticheta care reprezintă locul în care operațiunea s-a încheiat.

- **Data_RelatedPrevOpTelemetryReason** – este operațiunea corelată cu operațiunea anterioară.

- **Data_StopwatchDuration** – timpul total pentru eveniment.

- **Data_UnpackLinkHint** – enumerarea reprezentând acțiunea potențială a utilizatorului, pe baza unui link de dezarhivare.

- **Data_UnpackLinkPromptResult** – enumerarea reprezentând răspunsul solicitării de dezarhivare a linkului.

#### <a name="officedocsappdocsoperationopenfromshell"></a>Office.Docs.AppDocs.OperationOpenFromShell

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platformele Android, iOS, Universal și Windows. Evenimentul înregistrează atunci când are loc o operațiune de deschidere a fișierelor din adresa URL furnizat în lista utilizată cel mai recent și este folosit pentru a înțelege și pentru a acorda prioritare experiențelor de utilizator, pe baza informațiilor despre operațiune de deschidere a fișierelor.

Se colectează următoarele câmpuri:

- **Data_AppIdForReportEndBeforeAppKnown** - ID-ul de aplicație, atunci când nu este cunoscut înainte de a fi solicitat sfârșitul raportului în operațiune.

- **Data_CanContinueFromOnBeforeOperationBegins** - starea CanContinue, înainte de a invoca inițierea rutinei de tratare.

- **Data_DetachedDuration** – durata procesului de detașare a unui eveniment. 

- **Data_Doc_AccessMode** – o enumerare care indică modul de acces al fișierului, de exemplu, doar în citire, citire-scriere.

- **Data_Doc_AsyncOpenKind** – o enumerare care indică tipul de flux asincron utilizat pentru deschiderea fișierului.

- **Data_Doc_ChunkingType** – o enumerare care indică tipul de algoritm de segmentare al unui fișier.

- **Data_Doc_EdpState** – o enumerare care indică starea de protecție datelor la nivel de întreprindere ale unui fișier.

- **Data_Doc_Ext** – primele patru caractere din extensia fișierului.

- **Data_Doc_Fqdn** – nume gazdă server al fișierului.

- **Data_Doc_FqdnHash** – un GUID care identifică în mod unic numele de gazdă server.

- **Data_Doc_IdentityTelemetryId** – codul hash unidirecțional al identității de utilizator folosit pentru a efectua deschiderea.

- **Data_Doc_InitializationScenario** – o enumerare care indică tipul de scenariu detaliat al unei operațiuni de deschidere a fișierelor.

- **Data_Doc_IOFlags** – o enumerare care indică semnalizările IO ale unei operațiuni de deschidere a fișierelor, de exemplu, dacă fișierul este în cache sau nu.

- **Data_Doc_IsCloudCollabEnabled** – dacă colaborarea în cloud este activată sau nu pentru fișier.

- **Data_Doc_IsIncrementalOpen** – dacă fișierul a fost sau nu deschis prin deschidere treptată.

- **Data_Doc_IsOcsSupported** – dacă un fișier acceptă sau nu serviciul de colaborare Office.

- **Data_Doc_IsOpeningOfflineCopy** – dacă un fișier dintr-o copie memorată în cache offline se deschide sau nu.

- **Data_Doc_IsPrefetched** – dacă fișierul înainte de operațiunea de deschidere a fost sau nu preluat.

- **Data_Doc_IsSyncBacked** – dacă un fișier în cloud există sau nu local și dacă este sincronizat cu serverul.

- **Data_Doc_Location** – o enumerare care indică unde se află fișierul, de exemplu, local sau în cloud.

- **Data_Doc_ReadOnlyReasons** – o enumerare care indică motivul doar în citire al unui fișier.

- **Data_Doc_ResourceIdHash** – un GUID care identifică în mod unic ID-ul de resursă server al fișierului.

- **Data_Doc_RtcType** – o enumerare care indică tipul de canal în timp real (RTC) utilizat de fișier.

- **Data_Doc_ServerDocId** – un GUID care identifică în mod unic ID-ul de document server.

- **Data_Doc_ServerProtocol** – o enumerare care indică protocolul de server al unui fișier în cloud.

- **Data_Doc_ServerType** – o enumerare care indică tipul de server al unui fișier în cloud.

- **Data_Doc_ServerVersion** – o enumerare care indică versiunea de server al unui fișier în cloud.

- **Data_Doc_SessionId** – un număr întreg, crescut cu 1 pentru fiecare operațiune de deschidere a fișierului într-o sesiune.

- **Data_Doc_SharePointServiceContext** – un șir utilizat pentru corelarea jurnalelor din partea client și de partea server, de obicei, este un fel de ID.

- **Data_Doc_SizeInBytes** – dimensiunea documentului în octeți.

- **Data_Doc_SpecialChars** – o enumerare indicând ce tip de caracter special are adresa URL a fișierului.

- **Data_Doc_UrlHash** – un GUID care identifică în mod unic URL-ul fișierului.

- **Data_Doc_UsedWrsDataOnOpen** – dacă fișierul a fost sau nu deschis incremental folosind datele WRS memorate pre-cache.

- **Data_Doc_WopiServiceId** – un șir care indică de la ce serviciu provine un fișier WOPI (aplicație de interfață deschisă pentru aplicația web).

- **Data_DocumentInputCurrency** – tipul de intrare a documentului utilizat de operațiune.

- **Data_DocumentOperation_AppId** – valoarea de enumerare reprezentând ID-ul unei aplicații.

- **Data_DocumentOperation_EndEventId** – eticheta care reprezintă locul în care operațiunea s-a încheiat.

- **Data_DocumentOperation_EndReason** – valoarea de enumerare reprezentând motivul final.

- **Data_DocumentOperation_IsReinitialized** – reinițializează un document deja deschis.

- **Data_DocumentOperation_ParamsFlags** – semnalizările de enumerare utilizate pentru a porni operațiunea.

- **Data_DocumentOperation_TelemetryReason** – reprezentarea de enumerare a punctului de intrare pentru evenimentul deschis. De exemplu, deschideți din MRU sau navigați, activare fișier etc.

- **Data_DocumentOperation_isTargetECBeginEC** – dacă contextul de execuție a țintei este același ca și contextul din care a fost deschis.

- **Data_FileOInclusiveMeasurements** – o valoare șir care înregistrează durata de timp petrecută în anumite apeluri de funcții, într-un format cu eticheta funcției și durata care include durata apelurilor de sub-funcții.

- **Data_FileOMeasurements** – o valoare șir care înregistrează timpul petrecut în anumite apeluri de funcții, într-un format cu eticheta funcției și durata care exclude durata apelurilor de sub-funcții.

- **Data_IsNameMissingInUrl** – indică dacă numele nu a fost analizat din URL.

- **Data_IsPathMissingForLocalFile** – indică dacă acesta este un fișier local fără cale.

- **Data_IsUnpackedLinkSupportedForOpen** – indică dacă linkurile neambalate sunt acceptate pentru deschidere.

- **Data_LinksOpenRightScenario** – valoare de enumerare pentru linkurile din scenariul de deschidere din dreapta.

- **Data_OpEndEventId** - eticheta care reprezintă locul în care operațiunea s-a încheiat.

- **Data_RelatedPrevOpTelemetryReason** – este operațiunea corelată cu operațiunea anterioară.

- **Data_StopwatchDuration** – timpul total pentru eveniment.

- **Data_UnpackLinkHint** – enumerarea reprezentând acțiunea potențială a utilizatorului, pe baza unui link de dezarhivare.

- **Data_UnpackLinkPromptResult** – enumerarea reprezentând răspunsul solicitării de dezarhivare a linkului.


#### <a name="officedocsappdocsoperationopenfromurl"></a>Office.Docs.AppDocs.OperationOpenFromUrl

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platformele Android, iOS, Universal și Windows. Evenimentul înregistrează atunci când are loc o operațiune de deschidere a fișierelor din URL-ul și pentru a acorda prioritare experiențelor de utilizator, pe baza informațiilor despre operațiune de deschidere a fișierelor.

Se colectează următoarele câmpuri:

- **Data_AppIdForReportEndBeforeAppKnown** - ID-ul de aplicație, atunci când nu este cunoscut înainte de a fi solicitat sfârșitul raportului în operațiune.

- **Data_CanContinueFromOnBeforeOperationBegins** - starea CanContinue, înainte de a invoca inițierea rutinei de tratare.

- **Data_DetachedDuration** – durata procesului de detașare a unui eveniment. 

- **Data_Doc_AccessMode** – o enumerare care indică modul de acces al fișierului, de exemplu, doar în citire, citire-scriere.

- **Data_Doc_AsyncOpenKind** – o enumerare care indică tipul de flux asincron utilizat pentru deschiderea fișierului.

- **Data_Doc_ChunkingType** – o enumerare care indică tipul de algoritm de segmentare al unui fișier.

- **Data_Doc_EdpState** – o enumerare care indică starea de protecție datelor la nivel de întreprindere ale unui fișier.

- **Data_Doc_Ext** – primele patru caractere din extensia fișierului.

- **Data_Doc_Fqdn** – nume gazdă server al fișierului.

- **Data_Doc_FqdnHash** – un GUID care identifică în mod unic numele de gazdă server.

- **Data_Doc_IdentityTelemetryId** – codul hash unidirecțional al identității de utilizator folosit pentru a efectua deschiderea.

- **Data_Doc_InitializationScenario** – o enumerare care indică tipul de scenariu detaliat al unei operațiuni de deschidere a fișierelor.

- **Data_Doc_IOFlags** – o enumerare care indică semnalizările IO ale unei operațiuni de deschidere a fișierelor, de exemplu, dacă fișierul este în cache sau nu.

- **Data_Doc_IsCloudCollabEnabled** – dacă colaborarea în cloud este activată sau nu pentru fișier.

- **Data_Doc_IsIncrementalOpen** – dacă fișierul a fost sau nu deschis prin deschidere treptată.

- **Data_Doc_IsOcsSupported** – dacă un fișier acceptă sau nu serviciul de colaborare Office.

- **Data_Doc_IsOpeningOfflineCopy** – dacă un fișier dintr-o copie memorată în cache offline se deschide sau nu.

- **Data_Doc_IsPrefetched** – dacă fișierul înainte de operațiunea de deschidere a fost sau nu preluat.

- **Data_Doc_IsSyncBacked** – dacă un fișier în cloud există sau nu local și dacă este sincronizat cu serverul.

- **Data_Doc_Location** – o enumerare care indică unde se află fișierul, de exemplu, local sau în cloud.

- **Data_Doc_ReadOnlyReasons** – o enumerare care indică motivul doar în citire al unui fișier.

- **Data_Doc_ResourceIdHash** – un GUID care identifică în mod unic ID-ul de resursă server al fișierului.

- **Data_Doc_RtcType** – o enumerare care indică tipul de canal în timp real (RTC) utilizat de fișier.

- **Data_Doc_ServerDocId** – un GUID care identifică în mod unic ID-ul de document server.

- **Data_Doc_ServerProtocol** – o enumerare care indică protocolul de server al unui fișier în cloud.

- **Data_Doc_ServerType** – o enumerare care indică tipul de server al unui fișier în cloud.

- **Data_Doc_ServerVersion** – o enumerare care indică versiunea de server al unui fișier în cloud.

- **Data_Doc_SessionId** – un număr întreg, crescut cu 1 pentru fiecare operațiune de deschidere a fișierului într-o sesiune.

- **Data_Doc_SharePointServiceContext** – un șir utilizat pentru corelarea jurnalelor din partea client și de partea server, de obicei, este un fel de ID.

- **Data_Doc_SizeInBytes** – dimensiunea documentului în octeți.

- **Data_Doc_SpecialChars** – o enumerare indicând ce tip de caracter special are adresa URL a fișierului.

- **Data_Doc_UrlHash** – un GUID care identifică în mod unic URL-ul fișierului.

- **Data_Doc_UsedWrsDataOnOpen** – dacă fișierul a fost sau nu deschis incremental folosind datele WRS memorate pre-cache.

- **Data_Doc_WopiServiceId** – un șir care indică de la ce serviciu provine un fișier WOPI (aplicație de interfață deschisă pentru aplicația web).

- **Data_DocumentInputCurrency** – tipul de intrare a documentului utilizat de operațiune.

- **Data_DocumentOperation_AppId** – valoarea de enumerare reprezentând ID-ul unei aplicații.

- **Data_DocumentOperation_EndEventId** – eticheta care reprezintă locul în care operațiunea s-a încheiat.

- **Data_DocumentOperation_EndReason** – valoarea de enumerare reprezentând motivul final.

- **Data_DocumentOperation_IsReinitialized** – reinițializează un document deja deschis.

- **Data_DocumentOperation_ParamsFlags** – semnalizările de enumerare utilizate pentru a porni operațiunea.

- **Data_DocumentOperation_TelemetryReason** – reprezentarea de enumerare a punctului de intrare pentru evenimentul deschis. De exemplu, deschideți din MRU sau navigați, activare fișier etc.

- **Data_DocumentOperation_isTargetECBeginEC** – dacă contextul de execuție a țintei este același ca și contextul din care a fost deschis.

- **Data_FileOInclusiveMeasurements** – o valoare șir care înregistrează durata de timp petrecută în anumite apeluri de funcții, într-un format cu eticheta funcției și durata care include durata apelurilor de sub-funcții.

- **Data_FileOMeasurements** – o valoare șir care înregistrează timpul petrecut în anumite apeluri de funcții, într-un format cu eticheta funcției și durata care exclude durata apelurilor de sub-funcții.

- **Data_IsNameMissingInUrl** – indică dacă numele nu a fost analizat din URL.

- **Data_IsPathMissingForLocalFile** – indică dacă acesta este un fișier local fără cale.

- **Data_IsUnpackedLinkSupportedForOpen** – indică dacă linkurile neambalate sunt acceptate pentru deschidere.

- **Data_LinksOpenRightScenario** – valoare de enumerare pentru linkurile din scenariul de deschidere din dreapta.

- **Data_OpEndEventId** - eticheta care reprezintă locul în care operațiunea s-a încheiat.

- **Data_RelatedPrevOpTelemetryReason** – este operațiunea corelată cu operațiunea anterioară.

- **Data_StopwatchDuration** – timpul total pentru eveniment.

- **Data_UnpackLinkHint** – enumerarea reprezentând acțiunea potențială a utilizatorului, pe baza unui link de dezarhivare.

- **Data_UnpackLinkPromptResult** – enumerarea reprezentând răspunsul solicitării de dezarhivare a linkului.


#### <a name="officeappleactivateperpetual"></a>Office.Apple.ActivatePerpetual

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Evenimentul este utilizat pentru a monitoriza starea fluxului de activare perpetuă, precum și a investiga cauzele erorilor, prin revizuirea valorilor FailedAt.

Se colectează următoarele câmpuri:

- **Data_FailedAt** - colectăm un șir reprezentând locul erorii în fluxul de activare a licenței permanente.

#### <a name="officeappleactivatesubscription"></a>Office.Apple.ActivateSubscription

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Colectăm informații despre migrarea de la stiva de cod de licențiere moștenită la piuneza codului de licențiere vNext. Acest lucru este utilizat pentru a monitoriza starea fluxului de activare a abonamentului, precum și pentru a urmări dacă aceasta este o migrare de licențiere către vNext și dacă s-a utilizat identitatea primară.

Se colectează următoarele câmpuri:

- **Data_ActivatingPrimaryIdentity** -o valoare adevărat/fals care denotă dacă a fost utilizată identitatea primară. 

- **Data_NULSubscriptionLicensed** - o valoare adevărat/fals care denotă starea abonamentului

#### <a name="officeapplecisauthticketwithidentity"></a>Office.Apple.CISAuthTicketWithIdentity

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Evenimentul este utilizat pentru capturarea erorilor de generare a tokenurilor de autentificare în timpul InAppPurchase pe Mac (evenimentul înregistrează codul de eroare primit).  Acest eveniment este utilizat pentru detectarea și pentru a ajuta la depanarea erorilor de generare a tokenurilor de autentificare.

Se colectează următoarele câmpuri:

- **Data_EmptyAuthToken** - colectăm un șir reprezentând locul erorii în fluxul activare a licenței permanente.

- **Data_TicketAuthError** - cod de eroare care indică cauza erorii

- **Data_ValidIdentity** - dacă clientul are o identitate validă

#### <a name="officeappleinappassociationactivity"></a>Office.Apple.InAppAssociationActivity

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Colectăm informații legate de asocierea produselor după o achiziție în cadrul aplicației. Înregistrăm ce SKU de abonament asociem.  Acest lucru este utilizat pentru a monitoriza starea asociațiilor de produs achiziționare din aplicație.

Se colectează următoarele câmpuri:

- **Data_ProductID** -SKU-ul de abonament pe care încercăm să-l asociem produsului.

#### <a name="officeappleinapppurchaseactivity"></a>Office.Apple.InAppPurchaseActivity

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. 

Colectăm informații legate de achizițiile de produse din AppStore. Urmărim rezultatul achiziției (eșec, succes, problemă de plată etc.), tipul de solicitare de achiziție (recuperare, achiziționare) și SKU-ul/produsul achiziționat (Microsoft 365 Family etc.)  Aceste date se utilizează pentru a monitoriza starea fluxurilor de achiziție din cadrul aplicației.

Se colectează următoarele câmpuri:

- **Data_ Data_PurchaseResult** - rezultatul operațiunii de achiziție

- **Data_ProductID** - produsul achiziționat

- **Data_PurchaseRequestType** - tipul de solicitare de achiziție

#### <a name="officeappleintune"></a>Office.Apple.InTune

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Vom colecta dacă sesiunea curentă este gestionată de Intune. Acest lucru este utilizat pentru a pivota/filtra în sesiunile gestionate Intune și ne permite să investigăm eventualele probleme legate de executarea Office ca aplicație gestionată de Intune.

Se colectează următoarele câmpuri:

- **Data_EventID** - colectăm un șir reprezentând un cod care indică dacă sesiunea este gestionată de Intune.

#### <a name="officeapplelicensingmaclicensingstate"></a>Office.Apple.Licensing.Mac.LicensingState

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Evenimentul captează starea curentă a licenței pentru o sesiune dintr-un computer (ID-ul de licență OLS, SKU-ul utilizat, existența sau absența perioadei de grație, RFM etc.). Datele colectate sunt utilizate pentru detectarea erorilor și pentru investigarea cauzelor erorilor. 

Se colectează următoarele câmpuri:

- **Data_DidRunPreview** - un șir care indică dacă această sesiune este rulată sub previzualizare

- **Data_LicensingACID** - un șir reprezentând un identificator intern al sistemului de licențiere

- **Data_LicensingType** - un șir reprezentând tipul de licență

- **Data_OLSLicenseId** - un șir reprezentând un identificator de licență

- **Data_State** - un șir reprezentând starea actuală a licenței

#### <a name="officeconnectdeviceactivitystart"></a>Office.ConnectDevice.Activity.Start

Ne permite să știm dacă o conexiune la un dispozitiv sau aplicație a reușit.  Utilizat pentru starea și monitorizarea caracteristicilor. Evenimentul este generat de Microsoft Data Streamer pentru programul de completare Excel.

Se colectează următoarele câmpuri:

- **Datasource_Type** - dispozitiv serial sau informații Serviciu pentru aplicații

- **DataSource_Name** - numele sursei de date conectate

- **Activity_Name** = numele activității „ConnectDevice”

- **Activity_CV** = ID pentru corelarea evenimentelor în sesiunea de conectare

- **Activity_StartStopType** = Start

- **Activity_DateTimeTicks** = Oră Dată pentru activitate
 
#### <a name="officeconnectdeviceactivitystop"></a>Office.ConnectDevice.Activity.Stop

Ne permite să știm dacă o conexiune la un dispozitiv sau aplicație a reușit. Utilizat pentru starea și monitorizarea caracteristicilor Evenimentul este generat de Microsoft Data Streamer pentru programul de completare Excel.

Se colectează următoarele câmpuri:

- **Datasource_Type** - dispozitiv serial sau informații Serviciu pentru aplicații

- **DataSource_Name** - numele sursei de date conectate

- **Activity_Name** - numele activității „ConnectDevice”

- **Activity_CV** - ID pentru corelarea evenimentelor în sesiunea de conectare

- **Activity_StartStopType** - Stop

- **Activity_DateTimeTicks** - Oră Dată pentru activitate

#### <a name="officedocsappledocsuxiossaveasthroughfilemenu"></a>Office.Docs.Apple.DocsUXiOSSaveAsThroughFileMenu 

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Acest eveniment înregistrează atunci când are loc o operațiune „Salvare ca“ și este utilizată pentru a înțelege și a acorda prioritate experienței utilizatorului, pe baza informațiilor de operațiune de fișier, cum ar fi categoriile de locație.  O operațiune „salvare ca“ are loc de fiecare dată când un utilizator creează un fișier nou și îl salvează pentru prima dată sau salvează o copie a unui fișier existent într-o locație nouă.

Se colectează următoarele câmpuri:

- **Data_OriginServiceType** - clasificarea abstractă a locației originale a unui fișier, cum ar fi „SharePoint“, „OneDrive“, „locală“, „WOPI“ etc. și în mod explicit nu este locația reală a fișierului.

- **Data_ServiceType** - clasificarea abstractă a locației originale a unui fișier după finalizarea salvării, cum ar fi „SharePoint“, „OneDrive“, „locală“, „WOPI“ etc. și în mod explicit nu este locația reală a fișierului.

#### <a name="officedocsappledocsuxmacatmentioninsertedatmention"></a>Office.Docs.Apple.DocsUXMacAtMentionInsertedAtMention 

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Acest eveniment înregistrează atunci când un utilizator menționează cu „@“ un alt utilizator și este utilizat pentru a înțelege și a acorda prioritate experienței utilizatorilor, în funcție de modul în care utilizatorii colaborează cu alți utilizatori.

Se colectează următoarele câmpuri:

- **Data_CharactersTyped** - o valoare numerică care indică numărul total de caractere tastate în textul de menționare cu „@“.

#### <a name="officedocsappledocsuxmacodspsharingwebviewsharingcompleted"></a>Office.Docs.Apple.DocsUXMacODSPSharingWebViewSharingCompleted 

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Acest eveniment înregistrează atunci când un utilizator alege să partajeze un document în cloud utilizând experiența de partajare OneDrive și este utilizat pentru a înțelege mai bine și a acorda prioritate experienței utilizatorilor pe baza partajării documentelor.

Se colectează următoarele câmpuri:

- **Data_ShareType** - un șir specificat în cod care indică tipul de operațiune de partajare care a fost finalizată, inclusiv, dar fără a se limita la „Copiere link“, „mai multe aplicații“, „Teams“.

- **Data_ShareWebViewMode** - un șir specificat în cod care indică ce tip de mod de partajare era activ când s-a finalizat partajarea, inclusiv, dar fără a se limita la „ManageAccess“, „AtMentions“, „Partajare“.

#### <a name="officedocsuicollaborationcoauthorgalleryrowtapped"></a>Office.DocsUI.Collaboration.CoauthorGalleryRowTapped 

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Acest eveniment înregistrează atunci când un utilizator selectează să vizualizeze lista de co-autori actuali.  Aceste date se utilizează pentru a înțelege mai bine și a acorda prioritate experiențelor de utilizator legate de elaborarea în comun a unui document în același timp.

Se colectează următoarele câmpuri:

- **Data_CoauthorCount** - o valoare numerică care reprezintă numărul total de persoane care editează în prezent același document ca al utilizatorului.

#### <a name="officedocsuicollaborationcollabcornerpeoplegallerycoauthorsupdated"></a>Office.DocsUI.Collaboration.CollabCornerPeopleGalleryCoauthorsUpdated 

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Evenimentul înregistrează atunci când se modifică numărul de co-autori activi într-un document din cloud.  Aceste date se utilizează pentru a înțelege mai bine și a acorda prioritate experiențelor de utilizator legate de elaborarea în comun a unui document în același timp.

Se colectează următoarele câmpuri:

- **Data_CoauthorsJoined** - numărul de co-autori care s-au alăturat documentului.

- **Data_CoauthorsLeft** - numărul de co-autori care au părăsit documentul.

- **Data_NewCoauthorCount** - noul contor de co-autori activi din document. 

- **Data_OldCoauthorCount** - numărul anterior de co-autori activi înaintea actualizării.

- **Data_ServiceType** - o clasificare abstractă a locației unui fișier, cum ar fi „SharePoint“, „OneDrive“, „locală“, „WOPI“ etc. și în mod explicit nu este locația reală a fișierului.

#### <a name="officedocsuidocstagedocstagecreatenewfromtemplate"></a>Office.DocsUI.DocStage.DocStageCreateNewFromTemplate 

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Evenimentul înregistrează atunci când se creează un nou fișier din experiența „Nou din șablon“ și este utilizat pentru a înțelege mai bine și a acorda prioritate experienței utilizatorului, pe baza informațiilor de creare a documentelor.

Se colectează următoarele câmpuri:

- **Data_InHomeTab** - o valoare booleană care indică dacă s-a creat noul fișier din șablon din fila Pornire din noua experiență a fișierului.

- **Data_InSearch** - un boolean care indică dacă fișierul a fost creat atunci când utilizatorul căuta un șablon.

- **Data_IsHomeTabEnabled** - o valoare booleană care indică dacă fila Pornire este disponibilă în prezent pentru utilizator.

- **Data_IsRecommendedEnabled** - o valoare booleană care indică dacă experiența „Recomandare“ este disponibilă în prezent pentru utilizator.

- **Data_TemplateIndex** - indexul numeric al fișierului șablon, așa cum este afișat vizual utilizatorului.

- **Data_TemplateType** - o clasificare ajutătoare pentru a distinge tipul de șablon, cum ar fi, dar fără limitare, șabloane „online“, șabloane „căutare online“, șabloane „locale“.

#### <a name="officedocsuidocstagerecommendedopen"></a>Office.DocsUI.DocStage.RecommendedOpen

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Acest eveniment înregistrează atunci când are loc o operațiune din secțiunea fișierelor recomandate a galeriei de documente și este utilizată pentru a înțelege și a acorda prioritate experienței utilizatorului, pe baza informațiilor de operațiune de fișier.

Se colectează următoarele câmpuri:

- **Data_Success** - o valoare booleană pentru a indica dacă operațiunea a reușit.

#### <a name="officedocsuifileoperationsdocsuifileopenmacrequired"></a>Office.DocsUI.FileOperations.DocsUIFileOpenMacRequired

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Acest eveniment înregistrează atunci când are loc o operațiune de deschidere de fișier și este utilizată pentru a înțelege și a acorda prioritate experienței utilizatorului, pe baza informațiilor operațiunii de deschidere de fișier, cum ar fi categoriile de locație „ServiceType“ și primele patru caractere ale extensiei.

Se colectează următoarele câmpuri:

- **Data_Ext** - extensia de fișier limitată la primele patru caractere ale extensiei sau mai puțin.

- **Data_ServiceType** - clasificarea abstractă a locației unui fișier, cum ar fi „SharePoint“, „OneDrive“, „locală“, „WOPI“ etc.

#### <a name="officedocsuifileoperationsopendocumentmeasurements"></a>Office.DocsUI.FileOperations.OpenDocumentMeasurements

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme iOS. Acest eveniment înregistrează atunci când are loc o operațiune de deschidere a fișierului și este utilizată pentru a înțelege și a acorda prioritate experienței utilizatorului, pe baza informațiilor de operațiune a deschiderii fișierului, în mod special informații legate de funcționalitate.

Se colectează următoarele câmpuri:

- **Data_AppDuration** - durata petrecută în procesarea aplicațiilor în timpul unei operațiuni de deschidere a fișierelor.

- **Data_BootDuration** - durata procesului de încărcare a fișierului deschis.

- **Data_ClickOrigin** - un șir care indică partea din care a fost linkul atunci când utilizatorul a făcut clic pe un link în iOS Outlook pentru a deschide un fișier în aplicația Office.

- **Data_ClickTime** - vremea epocii Unix când utilizatorul a făcut clic pe un link în iOS Outlook pentru a deschide fișierul în aplicația Office.

- **Data_ClosePreviouslyOpenedMarkers** - o valoare șir de caractere ce înregistrează în jurnal durata de timp între unele apeluri de funcții, într-un format cu ID de funcție și durată.

- **Data_DetachedDuration** - durata procesului de detașare a unui eveniment. 

- **Data_Doc_AccessMode** - o enumerare indicând modul de acces al fișierului, de exemplu, doar în citire, citiți scrierea.

- **Data_Doc_AsyncOpenKind** - o enumerare indicând tipul de flux asincron utilizat pentru deschiderea fișierului.

- **Data_Doc_ChunkingType** - o enumerare indicând tipul de algoritm de segmentare a unui fișier.

- **Data_Doc_EdpState** - o enumerare indicând starea de protecție a datelor de întreprindere a unui fișier.

- **Data_Doc_Ext** - extensia fișierului

- **Data_Doc_Fqdn** - nume gazdă server al fișierului.

- **Data_Doc_FqdnHash** - un GUID care identifică în mod unic nume gazdă server.

- **Data_Doc_IdentityTelemetryId** - un GUID care identifică în mod unic identitatea utilizată pentru a deschide un fișier.

- **Data_Doc_InitializationScenario** - o enumerare indicând tipul de scenariu detaliat al unei operațiuni deschise de fișier.

- **Data_Doc_IOFlags** - o enumerare indicând semnalizările IO ale unei operațiuni deschise de fișier, de exemplu, dacă fișierul este în cache sau nu.

- **Data_Doc_IsCloudCollabEnabled** - dacă colaborarea în cloud este activată sau nu pentru fișier.

- **Data_Doc_IsIncrementalOpen** - dacă fișierul a fost sau nu deschis prin deschidere treptată.

- **Data_Doc_IsOcsSupported** - dacă un fișier acceptă sau nu serviciul de colaborare Office.

- **Data_Doc_IsOpeningOfflineCopy** - dacă se deschide sau nu un fișier dintr-o copie memorată în cache offline.

- **Data_Doc_IsPrefetched** - dacă a fost sau nu preluat fișierul înainte de a se deschide operațiunea.

- **Data_Doc_IsSyncBacked** - dacă un fișier în cloud există sau nu local și dacă este sincronizat cu serverul.

- **Data_Doc_Location** - o enumerare indicând unde se află fișierul, de exemplu, local sau în cloud.

- **Data_Doc_ReadOnlyReasons** - o enumerare indicând doar motivul de citire a unui fișier.

- **Data_Doc_ResourceIdHash** - un GUID care identifică în mod unic ID-ul de resursă server al fișierului.

- **Data_Doc_RtcType** - o enumerare indicând tipul de canal în timp real (RTC) utilizat de fișier.

- **Data_Doc_ServerDocId** - un GUID care identifică în mod unic ID-ul documentului server.

- **Data_Doc_ServerProtocol** - o enumerare indicând protocolul de server al unui fișier în cloud.

- **Data_Doc_ServerType** - o enumerare indicând tipul de server al unui fișier în cloud.

- **Data_Doc_ServerVersion** - o enumerare indicând versiunea serverului unui fișier în cloud.

- **Data_Doc_SessionId** - un număr întreg, incrementat de 1 pentru fiecare operațiune de deschidere a fișierului într-o sesiune.

- **Data_Doc_SharePointServiceContext** - un șir utilizat pentru corelarea jurnalelor din partea client și pe partea de server, de obicei, este un fel de ID.

- **Data_Doc_SizeInBytes** - dimensiunea documentului în octeți

- **Data_Doc_SpecialChars** - o enumerare indicând ce tip de caracter special are adresa URL a fișierului.

- **Data_Doc_UrlHash** - un GUID care identifică în mod unic URL-ul fișierului.

- **Data_Doc_UsedWrsDataOnOpen** - dacă fișierul a fost deschis incremental folosind datele WRS memorate pre-cache.

- **Data_Doc_WopiServiceId** - un șir indicând ce serviciu este un fișier WOPI (aplicație de interfață deschisă pentru aplicația web).

- **Data_HWModel** - o valoare șir de înregistrare a modelului de dispozitiv iPhone sau iPad.

- **Data_InclusiveMeasurements** - o valoare șir de logare durata de timp petrecută în anumite apeluri de funcție, într-un format cu eticheta funcției și durata, care include durata apelurilor sub-funcții.

- **Data_InitializationReason** - o enumerare indicând modul în care se deschide fișierul, de exemplu, de la ce element UI sau declanșat de altă aplicație.

- **Data_IsDocumentAlreadyOpen** - fie că fișierul este sau nu deschis deja.

- **Data_IsInterrupted** - dacă operațiunea de deschidere a fișierului a fost întreruptă sau nu de trecerea aplicațiilor în fundal.

- **Data_Measurements** - o valoare șir de logare durata de timp petrecută în anumite apeluri de funcție, într-un format cu eticheta funcției și durata care include durata apelurilor sub-funcții.

- **Data_OpenInPlace** - dacă un fișier trebuie sau nu să fie copiat în containerul sandbox din Office înainte ca utilizatorul să-l poată deschide.

- **Data_OpenStartTime** - vremea epocii Unix când s-a deschis fișierul.

- **Data_SilhouetteDuration** - durata de randare a fișierului deschis.

- **Data_SourceApplication** - un șir indicând ID-ul pachetelor din aplicația sursă atunci când s-a declanșat un fișier deschis de altă aplicație.

- **Data_StopwatchDuration** - durata de la începutul și până la sfârșitul evenimentului.

- **Data_TimeSplitMeasurements** - o valoare șir de logare durata de timp petrecută în anumite apeluri de funcție, într-un format cu eticheta funcției și ora de început și durata.

#### <a name="officedocsuifileoperationsopenfilewithreason"></a>Office.DocsUI.FileOperations.OpenFileWithReason 

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Acest eveniment înregistrează atunci când are loc o operațiune de deschidere de fișier și este utilizată pentru a înțelege și a acorda prioritate experienței utilizatorului, pe baza informațiilor operațiunii de deschidere de fișier, cum ar fi categoriile de locație „ServiceType“ și locul din cadrul aplicației de unde utilizatorul a solicitat deschiderea unui fișier.

Se colectează următoarele câmpuri:

- **Data_IsCandidateDropboxFile** - aceasta este o valoare booleană care este conectată dacă inspectând calea fișierului, credem că ar putea fi dintr-un folder sincronizat cu Dropbox.

- **Data_IsSignedIn** - dacă un utilizator este sau nu conectat atunci când fișierul este salvat.

- **Data_OpenReason** - motivul deschis reprezintă o valoare numerică care indică de unde din aplicație un utilizator a deschis un fișier.

- **Data_ServiceType** - clasificarea numerică abstractă a locației unui fișier, cum ar fi „SharePoint“, „OneDrive“, „locală“, „WOPI“ etc. și în mod explicit nu este locația reală a fișierului.

#### <a name="officedocsuifileoperationssavetourl"></a>Office.DocsUI.FileOperations.SaveToURL

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Evenimentul înregistrează atunci când apare o operațiune de „salvare ca“ și este utilizată pentru a înțelege și a acorda prioritate experienței utilizatorului, pe baza informațiilor operațiunii de deschidere de fișier, cum ar fi categoriile de locație și primele patru caractere ale extensiei.  O operațiune „salvare ca“ are loc de fiecare dată când un utilizator creează un fișier nou și îl salvează pentru prima dată sau salvează o copie a unui fișier existent într-o locație nouă.

Se colectează următoarele câmpuri:

- **Data_FileExtension** - primele patru caractere din extensia fișierului nou.

- **Data_IsNewFileCreation** - indică dacă operațiunea de salvare este pentru un fișier nou sau o copie a unui fișier existent.

- **Data_IsSignedIn** - dacă un utilizator este sau nu conectat atunci când fișierul este salvat.

- **Data_SaveErrorCode** - o valoare numerică setată dacă există o eroare care vă ajută să identificați tipul acesteia.

- **Data_SaveErrorDomain** - specifică domeniul SaveErrorCode, așa cum este definit de către Apple SaveErrorDomains „sunt șiruri arbitrare utilizate pentru a diferenția grupurile de coduri“.

- **Data_SaveLocation** - o clasificare abstractă a locației unui fișier, cum ar fi „SharePoint“, „OneDrive“, „locală“, „WOPI“ etc. și în mod explicit nu este locația reală a fișierului.

- **Data_SaveOperationType** - o valoare numerică definită de grupul de valori NSSaveOperationType al Apple.

#### <a name="officedocsuisharinguicloudupsellshown"></a>Office.DocsUI.SharingUI.CloudUpsellShown 

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Acest eveniment înregistrează atunci când un utilizator trece prin documentul de vânzări la flux în cloud.  Aceste date se utilizează pentru a înțelege mai bine și a acorda prioritate experiențelor de utilizator legate de mutarea documentelor in locații din cloud.

Se colectează următoarele câmpuri:

- **Data_FileStyle** - o valoare numerică care indică din ce scenariu a fost afișată experiența din vânzări, cum ar fi de la un comutator salvare automată sau un buton partajare.

- **Data_FileType** - primele patru caractere din extensia fișierului actual.

- **Data_InDocStage** - o valoare Booleană care indică dacă experiența de upsell este afișată din galeria de documente sau dintr-o fereastră de document.

- **Data_IsDocumentOpened** - un Boolean care indică dacă documentul curent pentru care se afișează experiența din vânzări este, de asemenea, deschis.

- **Data_IsDraft** - un Boolean care indică dacă fișierul curent a fost salvat vreodată.

- **Data_IsSheetModal** - un Boolean care indică dacă experiența de vânzări a fost prezentată modal sau nu.

#### <a name="officedocsuisharinguicloudupsellupload"></a>Office.DocsUI.SharingUI.CloudUpsellUpload 

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Acest eveniment înregistrează atunci când un utilizator alege să încarce un fișier nou sau local în cloud, precum și rezultatul operațiunii respective.  Aceste date se utilizează pentru a înțelege mai bine și a acorda prioritate experiențelor de utilizator legate de mutarea documentelor in locații din cloud.

Se colectează următoarele câmpuri:

- **Data_FileStyle** - o valoare numerică care indică din ce scenariu a fost afișată experiența din vânzări, cum ar fi de la un comutator salvare automată sau un buton partajare.

- **Data_FileType** - primele patru caractere din extensia fișierului actual.

- **Data_InDocStage** - un Boolean care indică dacă experiența din vânzări este afișată din galeria de documente sau dintr-o fereastră de document.

- **Data_IsDefaultServiceLocation** - o valoare booleană care indică dacă locația selectată pentru a încărca documentul în este locația implicită.

- **Data_IsDocumentOpened** - un Boolean care indică dacă documentul curent pentru care se afișează experiența din vânzări este, de asemenea, deschis.

- **Data_IsDraft** - un Boolean care indică dacă fișierul curent a fost salvat vreodată.

- **Data_IsSheetModal** - un Boolean care indică dacă experiența de vânzări a fost prezentată modal sau nu.

- **Data_LocationServiceType** - o clasificare abstractă a locației unui fișier, cum ar fi „SharePoint“, „OneDrive“, „locală“, „WOPI“ etc. și în mod explicit nu este locația reală a fișierului.

- **Data_UploadAction** - un șir specificat în cod care indică dacă încărcarea a fost o operațiune de mutare sau de copiere.

- **Data_UploadResult** - un șir specificat în cod, care indică rezultatul tentativei de încărcare, inclusiv, dar fără a se limita la „Success“, „UserCancelledUpload“ și „PreAuthFailed“.

#### <a name="officedocsuisharinguicopylinkoperation"></a>Office.DocsUI.SharingUI.CopyLinkOperation

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Acest eveniment se înregistrează atunci când un utilizator alege să partajeze un document prin generarea unui link la un document din cloud și este utilizat pentru a înțelege mai bine și a acorda prioritate experienței utilizatorilor pe baza partajării documentelor.

Se colectează următoarele câmpuri:

- **Data_ServiceType** - o clasificare abstractă a locației unui fișier, cum ar fi „SharePoint“, „OneDrive“, „locală“, „WOPI“ etc. și în mod explicit nu este locația reală a fișierului.

- **Data_LinkType** - un șir specificat în cod care descrie tipul de operațiune de invitație efectuată, cum ar fi „ViewOnly“ și „ViewAndEdit“.

- **Data_ShareScenario** - o descriere de șir specificat în cod în care, în interfața de utilizator a aplicației fișierul este partajat din, inclusiv, dar fără a se limita la, „FileMenu“, „OpenTabShareActionMenu“, „RecentTabShareActionMenu“.

#### <a name="officedocsuisharinguidocsuionedriveshare"></a>Office.DocsUI.SharingUI.DocsUIOneDriveShare 

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Acest eveniment înregistrează atunci când un utilizator alege să partajeze un document în cloud utilizând experiența de partajare OneDrive și este utilizat pentru a înțelege mai bine și a acorda prioritate experienței utilizatorilor pe baza partajării documentelor.

Se colectează următoarele câmpuri:

- **Data_ODSPShareWebviewShareError** - dacă experiența de partajare întâmpină o eroare, aceasta este o valoare numerică, pentru a vă ajuta să identificați motivul acesteia.

- **Data_ODSPShareWebviewShareGrantAccessResult** - o valoare booleană care atunci când este adevărată, indică faptul că o operațiune de partajare ușoară s-a finalizat cu succes.

- **Data_ODSPShareWebviewShareSuccessType** - când o operațiune de partajare termină cu succes aceasta este o valoare numerică utilizată pentru a determina ce tip de operațiune de partajare a fost finalizată.

- **Data_WebViewInfoResult** - dacă interfața de utilizator nu reușește să se încarce, aceasta este o valoare numerică pentru a vă ajuta să identificați motivul erorii. 

- **Data_WebViewLoadTimeInMs** - o valoare numerică care înregistrează perioada de timp necesară pentru ca interfața de utilizator Web să se încarce.

#### <a name="officedocsuisharinguiinvitepeople"></a>Office.DocsUI.SharingUI.InvitePeople 

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Acest eveniment înregistrează atunci când un utilizator alege să invite persoane la un document din cloud și este utilizat pentru a înțelege mai bine și a acorda prioritate experienței utilizatorilor pe baza partajării documentelor.

Se colectează următoarele câmpuri:

- **Data_ServiceType** - o clasificare abstractă a locației unui fișier, cum ar fi „SharePoint“, „OneDrive“, „locală“, „WOPI“ etc. și în mod explicit nu este locația reală a fișierului.

- **Data_InviteeCount** - numărul total de persoane invitate la un document într-o singură acțiune de invitație.

- **Data_LinkType** - un șir specificat în cod care descrie tipul de operațiune de invitație efectuată, cum ar fi „ViewOnly“ și „ViewAndEdit“.

- **Data_MessageLength** - un contor numeric al numărului total de caractere trimise în mesajul de invitație.

- **Data_ShareScenario** - o descriere de șir specificat în cod în care, în interfața de utilizator a aplicației fișierul este partajat din, inclusiv, dar fără a se limita la, „FileMenu“, „OpenTabShareActionMenu“, „RecentTabShareActionMenu“.

#### <a name="officedocsuisharinguisendacopyoperation"></a>Office.DocsUI.SharingUI.SendACopyOperation

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Evenimentul înregistrează atunci când un utilizator alege să trimită o copie a unui document și este utilizat pentru a înțelege mai bine și a acorda prioritate experienței utilizatorilor pe baza partajării documentelor.

Se colectează următoarele câmpuri:

- **Data_IsHomeTabEnabled** - o valoare booleană care indică dacă fila Pornire este disponibilă în prezent pentru utilizator.

- **Data_IsRecommendedEnabled** - o valoare booleană care indică dacă experiența „Recomandare“ este disponibilă în prezent pentru utilizator.

- **Data_OperationType** - o valoare numerică pentru a indica ce tip de operațiune de trimitere a unei copii are loc, cum ar fi trimiterea unei copii într-un mesaj de e-mail sau trimiterea unei copii prin controlul partajare Apple.

- **Data_ServiceType** - o clasificare abstractă a locației unui fișier, cum ar fi „SharePoint“, „OneDrive“, „locală“, „WOPI“ etc. și în mod explicit nu este locația reală a fișierului.

- **Data_ShareFileType** - o descriere de șir specificată în cod pentru ce tip de obiect este partajat, inclusiv, dar fără a se limita la, „document“, „PDF“, „imagine“.

- **Data_ShareScenario** - o descriere de șir specificat în cod în care, în interfața de utilizator a aplicației fișierul este partajat din, inclusiv, dar fără a se limita la, „FileMenu“, „OpenTabShareActionMenu“, „RecentTabShareActionMenu“.

- **Data_SharingService** - un boolean care indică dacă fișierul a fost creat atunci când utilizatorul căuta un șablon.

#### <a name="officedocsuisharinguiupsellshare"></a>Office.DocsUI.SharingUI.UpsellShare 

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Acest eveniment înregistrează atunci când un utilizator trece prin documentul de vânzări la flux în cloud pentru a încerca să partajeze un document.   Aceste date se utilizează pentru a înțelege mai bine și a acorda prioritate experiențelor de utilizator legate de mutarea documentelor in locații din cloud.

Se colectează următoarele câmpuri:

- **Data_FileOperationResult** - o valoare numerică pentru a indica dacă operațiunea a reușit.

- **Data_HostedFromDocStage** - un Boolean pentru a indica dacă un utilizator trece prin vânzare în flux în cloud din experiența DocStage sau dintr-un document deschis.

- **Data_isLocalCopyOn** - un Boolean pentru a indica dacă utilizatorul a ales să păstreze o copie locală a documentului încărcat într-o locație din cloud sau să mute documentul existent într-o locație din cloud.

- **Data_NewFileType** - o clasificare abstractă a noii locații a unui fișier, cum ar fi „SharePoint“, „OneDrive“, „locală“, „WOPI“ etc. și în mod explicit nu este locația reală a fișierului.

- **Data_OriginalFileType** - o clasificare abstractă a locației unui fișier, cum ar fi „SharePoint“, „OneDrive“, „locală“, „WOPI“ etc. și în mod explicit nu este locația reală a fișierului.

- **Data_UploadButtonPressed** - un Boolean pentru a indica dacă utilizatorul a ales să încarce documentul curent într-o locație din cloud.

- **Data_UploadError** - o valoare numerică care indică tipul de eroare care a survenit dacă o operațiune de încărcare nu reușește.

- **Data_UpsellAppearsFromDelegate** - o valoare booleană care indică dacă vizualizarea a fost afișată din meniul partajare.

#### <a name="officeextensibilitycatalogexchangeprocessentitlement"></a>Office.Extensibility.Catalog.ExchangeProcessEntitlement

Date privind procesarea unui drept individual și program de completare atribuit unui administrator de entitate găzduită Office 365.

Utilizat la crearea de diagrame (solicitat de conducerea echipei) privind succesul clienților și analiza problemelor clienților.

Se colectează următoarele câmpuri:

  - **AppVersion** - versiunea aplicației gazdă a programului de completare

  - **SolutionId** - GUID care reprezintă un program de completare unic

  - **TelemetryId** - GUID care reprezintă un utilizator unic

#### <a name="officeextensibilitycatalogexchangeprocessmanifest"></a>Office.Extensibility.Catalog.ExchangeProcessManifest

Date privind procesarea unui manifest individual pentru un program de completare atribuit unui administrator de entități găzduite Office 365. Utilizate la analiza problemelor clienților și la diagramele cu succesele clienților.
 
Se colectează următoarele câmpuri:

- **AppVersion** - versiunea aplicației

- **IsAllReturnedManifestsParsed** - bool indicând că am analizat toate manifestele returnate

- **IsAppCommand** - bool indicând dacă este o aplicație cu comenzi de aplicație 

- **ReturnedManifestsParsed** - contorizează manifestele analizate

- **SolutionId** - ID-ul soluției

- **TelemetryId** - identificator de telemetrie bazat pe identitatea autentificată

#### <a name="officeextensibilityodpappcommandsribbonclick"></a>Office.Extensibility.ODPAppCommandsRibbonClick

Colectează dacă a avut sau nu succes clicul pe controlul programului de completare particularizat. Se utilizează pentru a detecta probleme la interacțiunea utilizatorului cu controalele programului de completare.
 
Se colectează următoarele câmpuri:

- **CommandActionType** - tip de comandă program de completare

- **CommandLabel** - eticheta comenzii pe care s-a făcut clic

- **SolutionId** - ID-ul soluției

#### <a name="officefeedeventsinitializing"></a>Office.Feed.Events.Initializing

Acest eveniment este colectat când începe inițializarea fluxului. Acest eveniment este utilizat pentru a indica faptul că fluxul începe și pentru a diagnostica problemele de fiabilitate la lansarea fluxului.

- **AppInfo.Language** - limba aplicației în format de etichetă de limbă IETF.

- **AppInfo.Name** - numele componentei utilizate (Flux Office).

- **AppInfo.Version** - versiunea aplicației.

- **clientCorrelationId** - identificatorul unic global pentru sesiunea aplicației.

- **clientType** - aplicația pe care rulează componenta.

- **DeviceInfo.Make** - producătorul dispozitivului sau numele OEM al dispozitivului.

- **DeviceInfo.NetworkProvider** - rețeaua sau operatorul mobil, cum ar fi „AT&T”.

- **DeviceInfo.NetworkType** - tipul de conectivitate al rețelei dispozitivului utilizat, cum ar fi „Cu fir”, „Wifi” sau „WWAN” (date/celular).

- **DeviceInfo.OsName** - numele dispozitivului OS.

- **DeviceInfo_SDKUid** - identifică în mod unic dispozitivul din perspectiva SDK-ului de telemetrie

- **eventId** - identificator de nume al evenimentului. 

- **EventInfo.SdkVersion** - versiunea SDK a telemetriei utilizate de client pentru a genera evenimentul.

- **eventpriority** - valoare de enumerare pentru prioritatea de trimitere a evenimentului.

- **feature** - utilizat pentru a grupa diverse evenimente cu aceeași caracteristică.

- **hostAppRing** - populația utilizatorilor cărora le-a fost distribuită aplicația.

- **properties** - conține proprietăți metadate suplimentare, colectate pentru fiecare eveniment.
        
    - **ClientTimeStamp** - marcă de timp privind momentul în care a fost înregistrat de când evenimentul a fost înregistrat de client.

- **publicEventName** - nume eveniment orientat spre public.  

- **region** - regiunea geografică a serviciului de flux la care este conectat utilizatorul. 

- **tenantAadObjectId** - identificator unic global pentru entitatea găzduită a utilizatorului.

- **type** - tipul evenimentului înregistrat, de exemplu, urmărire, eroare, eveniment, QoS.

- **userAadObjectId** - identificatorul de utilizator unic global pentru un cont Microsoft Enterprise.

- **UserInfo.Id** - identificatorul de utilizator unic global pentru un cont Microsoft Enterprise.

- **UserInfo.IdType** - specifică tipul de ID utilizator. 

- **UserInfo.Language** - limba utilizatorului în format de etichetă de limbă IETF.

- **UserInfo.MsaId** - identificatorul de utilizator unic global pentru un cont Microsoft consumator.

- **UserInfo.OMSTenantId** - entitatea găzduită la care este asociat abonamentul unui utilizator. Ne permite să clasificăm problemele și să identificăm dacă este o problemă pe scară largă sau una izolată la un set de utilizatori sau la o anumită entitate găzduită.

- **UserInfo.TimeZone** - fusul orar al utilizatorului față de UTC.

- **userPuid** - identificatorul de utilizator unic global pentru un cont Microsoft consumator.

- **version** - versiunea clientului de flux.

#### <a name="officefeedeventsofficefeeddidappear"></a>Office.Feed.Events.OfficeFeedDidAppear

Evenimentul este colectat când fluxul este prezentat utilizatorului. Evenimentul este utilizat pentru a verifica dacă fluxul a finalizat etapa de inițializare și pentru a diagnostica problemele de fiabilitate la lansarea fluxului.

- **AppInfo.Language** - limba aplicației în format de etichetă de limbă IETF.

- **AppInfo.Name** - numele componentei utilizate (Flux Office).

- **AppInfo.Version** - versiunea aplicației.

- **bridgeWaitingTime** - măsurătoare pentru diagnosticarea performanței în redarea fluxului.

- **clientCorrelationId** - identificatorul unic global pentru sesiunea aplicației.

- **clientScenario** - scenariu discriminator pentru diverse variante de flux.

- **ClientTimeStamp** - marca de timp a momentului în care evenimentul a fost înregistrat în jurnal de către client.

- **clientType** - aplicația pe care rulează componenta.

- **DeviceInfo.Make** - producătorul dispozitivului sau numele OEM al dispozitivului.

- **DeviceInfo.NetworkProvider** - rețeaua sau operatorul mobil, cum ar fi „AT&T”.

- **DeviceInfo.NetworkType** - tipul de conectivitate al rețelei dispozitivului utilizat, cum ar fi „Cu fir”, „Wifi” sau „WWAN” (date/celular).

- **DeviceInfo.OsName** - numele dispozitivului OS.

- **DeviceInfo_SDKUid** - identifică în mod unic dispozitivul din perspectiva SDK-ului de telemetrie

- **eventId** - identificator de nume al evenimentului.

- **EventInfo.SdkVersion** - versiunea SDK a telemetriei utilizate de client pentru a genera evenimentul.

- **eventpriority** - valoare de enumerare pentru prioritatea de trimitere a evenimentului.

- **feature** - utilizat pentru a grupa diverse evenimente cu aceeași caracteristică.

- **hostAppRing** - populația utilizatorilor cărora le-a fost distribuită aplicația.

- **properties** - conține proprietăți metadate suplimentare, colectate pentru fiecare eveniment. *[Acest eveniment a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

- **publicEventName** - nume eveniment orientat spre public.  

- **region** - regiunea geografică a serviciului de flux la care este conectat utilizatorul. 

- **renderTime** - măsurătoare pentru diagnosticarea performanței în redarea fluxului.

- **tenantAadObjectId** - identificator unic global pentru entitatea găzduită a utilizatorului.

- **type** - tipul evenimentului înregistrat, de exemplu, urmărire, eroare, eveniment, QoS.

- **userAadObjectId** - identificatorul de utilizator unic global pentru un cont Microsoft Enterprise.

- **UserInfo.Id** - identificatorul de utilizator unic global pentru un cont Microsoft Enterprise.

- **UserInfo.IdType** - specifică tipul de ID utilizator. 

- **UserInfo.Language** - limba utilizatorului în format de etichetă de limbă IETF.

- **UserInfo.MsaId** - identificatorul de utilizator unic global pentru un cont Microsoft consumator.

- **UserInfo.OMSTenantId** - entitatea găzduită la care este asociat abonamentul unui utilizator. Ne permite să clasificăm problemele și să identificăm dacă este o problemă pe scară largă sau una izolată la un set de utilizatori sau la o anumită entitate găzduită.

- **UserInfo.TimeZone** - fusul orar al utilizatorului față de UTC.

- **userPuid** - identificatorul de utilizator unic global pentru un cont Microsoft consumator.

- **version** - versiunea clientului de flux.


#### <a name="officefeedbacksurveyfloodgateclientsurveytracked"></a>Office.Feedback.Survey.FloodgateClient.SurveyTracked

Monitorizează atunci când un dispozitiv eligibil pentru o anchetă pornește o aplicație. Se utilizează pentru a evalua experiența sondajului, precum și pentru a vă asigura de funcționarea corectă a semnalului utilizat pentru a analiza problemele și stările clienților.

Se colectează următoarele câmpuri:

- **ExpirationTimeUTC** – data/ora la care ancheta va expira

- **SurveyName** – numele anchetei afișate

- **SurveyId** – instanța unică a unei campanii

- **UniqueId** – ID pentru a identifica fragmentul individual de telemetrie

#### <a name="officefeedbacksurveyfloodgateclienttriggermet"></a>Office.Feedback.Survey.FloodgateClient.TriggerMet

Monitorizează atunci când un dispozitiv a îndeplinit criteriile pentru a afișa o anchetă. Se utilizează pentru a evalua procesul de declanșare a sondajului, precum și pentru a vă asigura de funcționarea corectă a semnalului utilizat pentru a analiza problemele și stările clienților

Se colectează următoarele câmpuri:

- **ExpirationTimeUTC** – data/ora la care ancheta va expira

- **SurveyName** – numele anchetei afișate

- **SurveyId** – instanța unică a unei campanii

- **UniqueId** – ID pentru a identifica fragmentul individual de telemetrie

#### <a name="officefeedbacksurveyfloodgateclientuserselected"></a>Office.Feedback.Survey.FloodgateClient.UserSelected

Monitorizează atunci când un dispozitiv a fost selectat pentru o anchetă. Se utilizează pentru a evalua experiența sondajului, precum și pentru a vă asigura de funcționarea corectă a semnalului utilizat pentru a analiza problemele și stările clienților.

Se colectează următoarele câmpuri:

- **ExpirationTimeUTC** – data/ora la care ancheta va expira

- **SurveyName** – numele anchetei afișate

- **SurveyId** – instanța unică a unei campanii

- **UniqueId** – ID pentru a identifica fragmentul individual de telemetrie

#### <a name="officefeedbacksurveyuiandroid"></a>Office.Feedback.Survey.UI.Android

Pe un dispozitiv Android, monitorizează atunci când un utilizator pe un dispozitiv interacționează cu promptul și interfața de utilizator a anchetei. Se utilizează pentru a evalua experiența integrală a sondajului, precum și pentru a vă asigura de funcționarea corectă a semnalului utilizat pentru a analiza problemele și stările clienților.

Se colectează următoarele câmpuri:

- **ExpirationTimeUTC** – data/ora la care ancheta va expira

- **SurveyName** – numele anchetei afișate

- **SurveyId** – instanța unică a unei campanii

- **UniqueId** – ID pentru a identifica fragmentul individual de telemetrie

#### <a name="officefeedbacksurveyuiios"></a>Office.Feedback.Survey.UI.IOS

Pe un dispozitiv iOS, monitorizează atunci când un utilizator pe un dispozitiv interacționează cu promptul și interfața de utilizator a anchetei. Se utilizează pentru a evalua experiența integrală a sondajului, precum și pentru a vă asigura de funcționarea corectă a semnalului utilizat pentru a analiza problemele și stările clienților.

Se colectează următoarele câmpuri:

- **ExpirationTimeUTC** – data/ora la care ancheta va expira

- **SurveyName** – numele anchetei afișate

- **SurveyId** – instanța unică a unei campanii

- **UniqueId** – ID pentru a identifica fragmentul individual de telemetrie

#### <a name="officefeedbacksurveyuimac"></a>Office.Feedback.Survey.UI.Mac

Pe un dispozitiv Mac, monitorizează atunci când un utilizator pe un dispozitiv interacționează cu promptul și interfața de utilizator a anchetei. Se utilizează pentru a evalua experiența integrală a sondajului, precum și pentru a vă asigura de funcționarea corectă a semnalului utilizat pentru a analiza problemele și stările clienților.

Se colectează următoarele câmpuri:

- **ExpirationTimeUTC** – data/ora la care ancheta va expira

- **SurveyName** – numele anchetei afișate

- **SurveyId** – instanța unică a unei campanii

- **UniqueId** – ID pentru a identifica fragmentul individual de telemetrie

#### <a name="officefeedbacksurveyuiwin32"></a>Office.Feedback.Survey.UI.Win32

Pe un dispozitiv Win32, monitorizează interacțiunea utilizatorului pe un dispozitiv cu mesajul transmis de către sistemul de operare al sondajului si interfața cu utilizatorul a sondajului. Se utilizează pentru a evalua experiența integrală a sondajului, precum și pentru a vă asigura de funcționarea corectă a semnalului utilizat pentru a analiza problemele și stările clienților.

Se colectează următoarele câmpuri:

- **ExpirationTimeUTC** – data/ora la care ancheta va expira

- **SurveyName** – numele anchetei afișate

- **SurveyId** – instanța unică a unei campanii

- **UniqueId** – ID pentru a identifica fragmentul individual de telemetrie

#### <a name="officefeedbacksurveyuiwin32toast"></a>Office.Feedback.Survey.UI.Win32.Toast

Monitorizează când se afișează solicitarea pentru prompt de anchetă. Se utilizează pentru a evalua starea procesului de solicitare a anchetei, precum și pentru a vă asigura funcționarea corectă a semnalului utilizat pentru a analiza problemele și stările clienților.

Se colectează următoarele câmpuri:

- **ExpirationTimeUTC** – data/ora la care ancheta va expira

- **SurveyName** – numele anchetei afișate

- **SurveyId** – instanța unică a unei campanii

- **UniqueId** – ID pentru a identifica fragmentul individual de telemetrie

#### <a name="officefileiocsiccachedfilecsiloadfilebasic"></a>Office.FileIO.CSI.CCachedFileCsiLoadFileBasic

Ne permite să știm dacă un fișier s-a deschis cu succes din nivelul FIO. Utilizat pentru starea și monitorizarea caracteristicilor.

Se colectează următoarele câmpuri:

  - **Activity.Group -** etichetă care permite gruparea unui set de evenimente de monitorizare pentru a gestiona succesul general

  - **Activity.IsHVA -** semnalizare care indică faptul că evenimentul este de importanță critică pentru succesul utilizatorului

  - **Data.AsyncOpen -** semnalizare care indică faptul că deschiderea prezenta conținut care a sosit după ce corpul principal a fost deschis

  - **Data.CacheFileId -** se conectează la telemetrie Cache pentru documente Office pentru a activa analize de impact ale problemelor cu memoria cache asupra experienței utilizatorului
 
  - **Data.CFREnabled** - indică faptul că CacheFileRuntime este activat pentru sesiune.

  - **Data.CFRFailure** - a indicat că CacheFileRuntime a avut eroare.
  
  - **Data.CoauthStatus -** raportează starea de colaborare a documentului la deschidere

  - **Data.CountOfMultiRoundTripsDownload -** numărul de transferuri la serverul utilizat pentru a depana problemele privind performanța și rețeaua

  - **Data.CountOfMultiRoundTripsUpload -** numărul de transferuri la serverul utilizat pentru a depana problemele privind performanța și rețeaua

  - **Data.DialogId -** setați dacă o casetă de dialog UI a fost afișată în timpul deschiderii, ceea ce indică faptul că i s-a afișat un mesaj de avertizare utilizatorului

  - **Data.DidFallbackToDAV -** setați dacă documentul a fost deschis utilizându-se un protocol de transfer de fișiere mai vechi

  - **Data.Doc.AccessMode -** documentul este numai în citire/editabil

  - **Data.Doc.AssistedReadingReasons -** setați dacă documentul are implementată o protecție a datelor electronice

  - **Data.Doc.AsyncOpenKind –** indică dacă s-a deschis o versiune memorată în cache a documentului cloud și ce logică de reîmprospătare asincronă s-a folosit.

  - **Data.Doc.ChunkingType -** unități utilizate pentru deschiderea incrementală a documentelor

  - **Data.Doc.EdpState -** setare de protecție a datelor electronice pentru document

  - **Data.Doc.Ext -** extensia documentului (docx/xlsb/pptx etc.)

  - **Data.Doc.Extension -** depășit

  - **Data.Doc.FileFormat -** versiunea de protocol pentru formatul fișierului

  - **Data.Doc.Fqdn -** numele de domeniu OneDrive sau SharePoint Online

  - **Data.Doc.FqdnHash -** codul hash unidirecțional pentru numele de domeniu identificabil al clientului

  - **Data.Doc.IdentityTelemetryId -** codul hash unidirecțional pentru identitatea de utilizator folosită pentru deschidere

  - **Data.Doc.IdentityUniqueId -** depășit

  - **Data.Doc.InitializationScenario -** înregistrează cum a fost deschis documentul

  - **Data.Doc.IOFlags -** rapoarte privind semnalizările memorate în cache folosite pentru a seta opțiuni de solicitare

  - **Data.Doc.IrmRights -** acțiunile permise de politica de protejare a datelor electronice aplicată pentru document/utilizator

  - **Data.Doc.IsCloudCollabEnabled -** semnalizare care indică faptul că serviciul acceptă colaborarea în cloud

  - **Data.Doc.IsIncrementalOpen -** semnalizare care indică faptul că documentul a fost deschis incremental

  - **Data.Doc.IsOcsSupported -** semnalizare care indică faptul că documentul este acceptat în serviciul de colaborare

  - **Data.Doc.IsOpeningOfflineCopy -** semnalizare care indică faptul că s-a deschis copia offline a unui document

  - **Data.Doc.IsSyncBacked -** semnalizare care indică faptul că pe computer există o copie sincronizată automat a documentului

  - **Data.Doc.Location -** indică ce serviciu a furnizat documentul (OneDrive, File Server, SharePoint etc.)

  - **Data.Doc.LocationDetails -** indică ce Folder cunoscut a furnizat un document stocat local

  - **Data.Doc.NumberCoAuthors -** numărul de alți utilizatori dintr-o sesiune de editare în colaborare

  - **Data.Doc.PasswordFlags -** arată semnalizările de parole pentru citire sau citire/scriere setate

  - **Data.Doc.ReadOnlyReasons -** motivele pentru care documentul a fost deschis doar în citire

  - **Data.Doc.ResourceIdHash -** identificator de document anonimizat, folosit în diagnosticarea problemelor

  - **Data.Doc.ServerDocId -** identificator de document anonimizat și invariabil, folosit în diagnosticarea problemelor

  - **Data.Doc.ServerProtocol -** versiunea de protocol folosită în comunicarea cu serviciul

  - **Data.Doc.ServerType -** tipul de server care oferă serviciul (SharePoint, OneDrive, WOPI etc.)

  - **Data.Doc.ServerVersion -** versiunea serverului care oferă serviciul

  - **Data.Doc.SessionId -** identifică o anumită sesiune de editare a documentului din sesiunea completă

  - **Data.Doc.SharePointServiceContext -** informații de diagnosticare din solicitările SharePoint Online

  - **Data.Doc.SizeInBytes -** indicator privind dimensiunea documentului

  - **Data.Doc.SpecialChars -** indicator privind caracterele speciale din calea sau adresa URL a documentului

  - **Data.Doc.StorageProviderId -** depășit

  - **Data.Doc.StreamAvailability -** indicator care arată dacă șirul documentului este disponibil/dezactivat

  - **Data.Doc.SyncBackedType -** indicator privind tipul documentului (local sau bazat pe servicii)

  - **Data.Doc.UrlHash -** cod hash unidirecțional, pentru crearea unui identificator naiv de document

  - **Data.Doc.UsedWrsDataOnOpen -** indicator de diagnosticare pentru deschiderea incrementală a documentului

  - **Data.Doc.WopiServiceId -** conține identificatorul unic al furnizorului de servicii WOPI

  - **Data.DocumentLoadEndpoint -** dublură depășită/redundantă a (Data.Doc.Location și Data.Doc.IsSyncbacked)

  - **Data.DocumentSizeInBytes -** depășit/redundant înlocuit de Data.Doc. SizeInBytes

  - **Data.DocumentSizeOnDisk -** depășit

  - **Data.DoesBaseHaveContentOnOpen -** modificați diagnosticarea de urmărire asigurându-vă că avem cea mai recentă versiune a unui fișier partajat

  - **Data.DoesWorkingBranchHaveExcludedDataOnOpen -** modificați diagnosticarea de urmărire asigurându-vă că avem cea mai recentă versiune a unui fișier partajat

  - **Data.DownloadFragmentSize -** dimensiunea datelor trimise într-o subsolicitare pentru diagnosticarea problemelor privind rețeaua

  - **Data.DsmcStartedTooEarly -** indică o eroare care începe o sesiune de editare în colaborare

  - **Data.EditorsCount -** numărul altor colaboratori care editează documentul

  - **Data.ExcludedDataThresholdInBytes -** dimensiune de fișier obligatorie pentru deschiderea Asynch pentru în vederea utilizării

  - **Data.FileIOResult.Code -** cache de la ultimul cod de retur deschis din nivelul de protocol

  - **Data.FileIOResult.Success -** cache de la ultimul indicator de succes deschis din nivelul de protocol

  - **Data.FileIOResult.Tag -** cache de la ultima etichetă de eroare deschisă din nivelul de protocol

  - **Data.FileIOResult.Type -** cache de la ultimul tip de eroare deschisă din nivelul de protocol

  - **Data.FqdnHash -** Depășit, înlocuit de Data\_Doc\_FqdnHash

  - **Data.FullIError -** cache de la toate codurile de eroare deschise din nivelul de protocol

  - **Data.FullyQualifiedDomainName -** depășit, înlocuit de Data\_Doc\_Fqdn

  - **Data.Input.FileOpenState -** starea solicitată de aplicație (Read/ReadWrite etc.)

  - **Data.Input.OpenAsync -** deschidere Async solicitată de aplicație

  - **Data.Input.OpenOfflineCopy -** deschidere din copia offline solicitată de adăugare

  - **Data.IOFlags -** depășit

  - **Data.IsBaseBranchEmptyOnOpen -** modificați diagnosticarea de urmărire asigurându-vă că avem cea mai recentă versiune a unui fișier partajat

  - **Data.IsCachedHistoricalVersion -** cache-ul conține o versiune mai veche a documentului

  - **Data.IsDocEnterpriseProtected -** documentul a fost protejat prin criptare (Protecția documentelor electronice/EDP)

  - **Data.IsDocInODC -** documentul a fost deschis înainte și este deja în cache

  - **Data.IsMapUnMapCase -** parte din starea fișierului memorat în cache

  - **Data.IsMapUnMapCase.End -** parte din starea fișierului memorat în cache

  - **Data.IsOfficeHydrationInProgress -** documentul este restaurat din spațiul de stocare offline de Windows

  - **Data.isOfficeHydrationRequired -** documentul se află momentan în spațiul de stocare offline

  - **Data.isOpenFromCollab -** cea mai recentă copie a documentului a fost preluată din serviciul de colaborare partajat

  - **Data.isPendingNameExist -** redenumirea documentului este în curs

  - **Data.IsStubFile -** documentul nu a fost salvat încă în serviciul în cloud

  - **Data.IsSyncBackedStateDifferentThanOnLastOpen -** starea documentului s-a modificat, este posibil ca modificările să se fi produs în timp ce documentul nu era deschis

  - **Data.isTaskCanceledAfterOpenComplete -** depășit

  - **Data.IsWorkingBranchAvailableOnOpen -** modificați diagnosticarea de urmărire asigurându-vă că avem cea mai recentă versiune a unui fișier partajat

  - **Data.LicenseStatus** - starea licenței produsului de diagnosticare, utilizată pentru a valida faptul că sunt activate caracteristicile corespunzătoare ale produsului pentru tipul de licență al utilizatorului 

  - **Data.LicenseType -** indică starea licenței (gratuită/plătită/de încercare etc.)

  - **Data.Location -** indică tipul suportului de stocare/locația (USB, Cloud etc.)

  - **Data.LockRequestDocMode -** indică dacă documentul este disponibil pentru alte persoane

  - **Data.MyDeferredValue -** depășit

  - **Data.Network.BytesReceived -** depășit

  - **Data.Network.BytesSent -** depășit

  - **Data.Network.ConnectionsCreated -** depășit

  - **Data.Network.ConnectionsEnded -** depășit

  - **Data.OcsDisableReasons -** motivul pentru care serviciul de colaborare partajată nu a fost disponibil pentru document

  - **Data.OcsHostOnOpen -** semnalizare care indică faptul că controlul va comuta la serviciul de colaborare partajată în timpul Deschiderii

  - **Data.OpeningOfflineCopy -** semnalizare care indică faptul că copia locală a documentului va fi deschisă

  - **Data.Partition -** depășit

  - **Data.RequestTime -** depășit

  - **Data.ResourceIdHash -** depășit

  - **Data.ResumedIncrementalOpen -** depășit

  - **Data.RTCEnabled -** protocolul de distribuire de modificare rapidă a început

  - **Data.SaveOnOpen -** modificările nesalvate din documentul local au fost salvate în serviciu în timpul deschiderii

  - **Data.ServerProtocol -** depășit, înlocuit de Data\_Doc\_ServerProtocol

  - **Data.ServerType -** depășit, înlocuit de Data\_Doc\_ServerType

  - **Data.ServerVersion -** depășit, înlocuit de Data\_Doc\_ServerVersion

  - **Data.ServiceId -** depășit, înlocuit de Data\_Doc\_WopiServiceId

  - **Data.SessionId -** depășit

  - **Data.ShouldSwitchToServerOnly -** copia locală a documentului nu poate fi utilizată și trebuie utilizată versiunea server

  - **Data.SpecialChars -** depășit

  - **Data.StopwatchDuration -** depășit

  - **Data.SyncBackedFileTelemetrySessionId -** depășit

  - **Data.SyncElapsedTime -** depășit

  - **Data.SyncRequestId -** depășit

  - **Data.TestProperty -** depășit

  - **Data.TransitionToHostOnOpen -** semnalizare care indică faptul că sesiunea se va conecta la serviciul de găzduire a documentului

  - **Data.TransitionToHostOnOpenResult -** starea tranziției la serviciul de găzduire

  - **Data.UseCachedNetworkConnection -** semnalizare care indică dacă o conexiune a fost reutilizată sau dacă a fost creată o conexiune nouă

  - **Data.UseClientIdAsSchemaLockId -** semnalizare pentru a controla modul în care documentele sunt blocate în cadrul serviciului

  - **Data.VersionType** - indică ce tip de versiune este operațiunea deschisă curentă.

  - **Data.WopiServiceId -** depășit, înlocuit de Data\_Doc\_WopiServiceId

#### <a name="officefileiocsiccachedfilecsisavefilebasic"></a>Office.FileIO.CSI.CCachedFileCsiSaveFileBasic

Ne permite să știm dacă un fișier a fost salvat cu succes din nivelul FIO. Utilizat pentru starea și monitorizarea caracteristicilor.

Se colectează următoarele câmpuri:

  - **Activity.Group -** etichetă care permite gruparea unui set de evenimente de monitorizare pentru a gestiona succesul general

  - **Activity.IsHVA -** semnalizare care indică faptul că evenimentul este de importanță critică pentru succesul utilizatorului

  - **Data.AsyncOpen -** semnalizare care indică faptul că documentul a fost deschis cu conținutul care a sosit după ce corpul principal a fost deschis

  - **Data.BaseDownloadTriggered -** modificați diagnosticarea de urmărire care indică faptul că a fost solicitată versiunea de bază a documentului

  - **Data.BlockAutoUploadReasons -** motivul codurilor pentru starea de încărcare blocată (de ex., exemplu Salvarea automată este dezactivată, documentul este în tranziție)

  - **Data.BlockUploadDueToFailedSaveAsOverExisting -** încărcarea este blocată întrucât ar putea să eșueze dacă se reîncearcă

  - **Data.CacheFileId -** se conectează la telemetrie Cache pentru documente Office pentru a activa analize de impact ale problemelor cu memoria cache asupra experienței utilizatorului

  - **Data.ChartType -** depășit

  - **Data.CoAuthStatus -** raportează starea de colaborare a documentului la salvare

  - **Data.CoauthUpdatesContext -** raportează context (îmbinare/deschidere incrementală)

  - **Data.CountOfMultiRoundTripsDownload -** numărul de transferuri la serverul utilizat pentru a depana problemele privind performanța și rețeaua

  - **Data.CountOfMultiRoundTripsUpload -** numărul de transferuri la serverul utilizat pentru a depana problemele privind performanța și rețeaua
  
  - **Data.CFREnabled** - indică faptul că CacheFileRuntime este activat pentru sesiune.

  - **Data.CFRFailure** - a indicat că CacheFileRuntime a avut eroare.

  - **Data.DialogChoice -** înregistrează alegerea efectuată în toate casetele de dialog de eroare

  - **Data.DialogId -** înregistrează DialogId ale tuturor casetelor de dialog de eroare care se afișează în timpul salvării

  - **Data.Dmc.IsOcsSupported -** depășit

  - **Data.Doc.AccessMode -** documentul este numai în citire

  - **Data.Doc.AssistedReadingReasons -** setați dacă documentul are implementată o protecție a datelor electronice

  - **Data.Doc.AsyncOpenKind –** indică dacă s-a deschis o versiune memorată în cache a documentului cloud și ce logică de reîmprospătare asincronă s-a folosit.

  - **Data.Doc.ChunkingType -** unități utilizate pentru deschiderea incrementală a documentelor

  - **Data.Doc.EdpState -** setare de protecție a datelor electronice pentru document

  - **Data.Doc.Ext -** extensia documentului (docx/xlsm/pptx etc.)

  - **Data.Doc.Extension -** depășit

  - **Data.Doc.FileFormat -** versiunea de protocol pentru formatul fișierului

  - **Data.Doc.Fqdn -** numele de domeniu OneDrive sau SharePoint Online

  - **Data.Doc.FqdnHash -** codul hash unidirecțional pentru numele de domeniu identificabil al clientului

  - **Data.Doc.FqdnHasi -** depășit

  - **Data.Doc.IdentityTelemetryId -** codul hash unidirecțional pentru identitatea de utilizator folosită pentru salvare

  - **Data.Doc.IdentityUniqueId -** depășit

  - **Data.Doc.IKFlags -** depășit

  - **Data.Doc.InitializationScenario -** înregistrează cum a fost deschis documentul

  - **Data.Doc.IOFlags -** rapoarte privind semnalizările memorate în cache folosite pentru a seta opțiuni de solicitare

  - **Data.Doc.IrmRights -** acțiunile permise de politica de protejare a datelor electronice aplicată pentru document/utilizator

  - **Data.Doc.IsCloudCollabEnabled -** semnalizare care indică faptul că aplicația acceptă colaborarea în cloud

  - **Data.Doc.IsIncrementalOpen -** semnalizare care arată că documentul a fost deschis incremental

  - **Data.Doc.IsOcsSupported -** semnalizare care indică faptul că documentul acceptă colaborarea în cloud

  - **Data.Doc.IsOpeningOfflineCopy -** semnalizare care indică faptul că s-a deschis copia offline a unui document

  - **Data.Doc.IsSyncBacked -** semnalizare care indică faptul că pe computer există o copie sincronizată automat a documentului

  - **Data.Doc.Location -** indică ce serviciu a furnizat documentul (OneDrive, File Server, SharePoint etc.)

  - **Data.Doc.LocationDetails -** indică ce Folder cunoscut a furnizat un document stocat local

  - **Data.Doc.NumberCoAuthors -** numărul de alți utilizatori dintr-o sesiune de editare în colaborare

  - **Data.Doc.PasswordFlags -** arată semnalizările de parole pentru citire sau citire/scriere setate

  - **Data.Doc.ReadOnlyReasons -** motivele pentru care documentul a fost deschis doar în citire

  - **Data.Doc.ResourceIdHash -** identificator de document anonimizat, folosit în diagnosticarea problemelor

  - **Data.Doc.ServerDocId -** identificator de document anonimizat și invariabil, folosit în diagnosticarea problemelor

  - **Data.Doc.ServerProtocol -** versiunea de protocol folosită în comunicarea cu serviciul

  - **Data.Doc.ServerType -** tipul de server care oferă serviciul (SharePoint, OneDrive, WOPI etc.)

  - **Data.Doc.ServerVersion -** versiunea serverului care oferă serviciul

  - **Data.Doc.SessionId -** identifică o anumită sesiune de editare a documentului din sesiunea completă

  - **Data.Doc.SharePointServiceContext -** informații de diagnosticare din solicitările SharePoint Online

  - **Data.Doc.SizeInBytes -** indicator privind dimensiunea documentului

  - **Data.Doc.SpecialChars -** indicator privind caracterele speciale din calea sau adresa URL a documentului

  - **Data.Doc.StorageProviderId -** depășit

  - **Data.Doc.StreamAvailability -** indicator care arată dacă șirul documentului este disponibil/dezactivat

  - **Data.Doc.SussionId -** depășit

  - **Data.Doc.SyncBackedType -** indicator privind tipul documentului (local sau bazat pe servicii)

  - **Data.Doc.UrlHash -** cod hash unidirecțional, pentru crearea unui identificator naiv de document

  - **Data.Doc.UsedWrsDataOnOpen -** indicator de diagnosticare pentru deschiderea incrementală a documentului

  - **Data.Doc.WopiServiceId -** conține identificatorul unic al furnizorului de servicii WOPI

  - **Data.DocnReadOnlyReasons -** depășit

  - **Data.DocumentSaveEndpoint -** depășit, înlocuit de Data\_Doc\_Location

  - **Data.DocumentSaveType -** tip de salvare (Normal, Creare, Salvare ca)

  - **Data.DocumentSizeOnDisk -** depășit, înlocuit de Data\_Doc\_SizeInBytes

  - **Data.DoesBaseHaveContentOnOpen -** modificați diagnosticarea de urmărire asigurându-vă că avem cea mai recentă versiune a unui fișier partajat

  - **Data.DoesWorkingBranchHaveExcludedDataOnOpen -** modificați diagnosticarea de urmărire asigurându-vă că avem cea mai recentă versiune a unui fișier partajat

  - **Data.DstDoc.AccessMode -** documentul nou este numai în citire/editabil

  - **Data.DstDoc.EdpState -** setare de protecție a datelor electronice pentru document nou

  - **Data.DstDoc.Extension -** extensia documentului nou (docx/xlsm/pptx etc.)

  - **Data.DstDoc.FileFormat -** protocolul formatului de fișier al documentului nou

  - **Data.DstDoc.Fqdn -** numele de domeniu OneDrive sau SharePoint Online al documentului nou

  - **Data.DstDoc.FqdnHash -** codul hash unidirecțional pentru numele de domeniu identificabil al clientului pentru documentul nou

  - **Data.DstDoc.IdentityUniqueId -** depășit

  - **Data.DstDoc.IOFlags -** semnalizările de opțiuni memorate în cache ale documentului nou utilizate la deschidere

  - **Data.DstDoc.IsOpeningOfflineCopy -** semnalizare care arată că s-a deschis o copie offline a unui document nou

  - **Data.DstDoc.IsSyncBacked -** semnalizare care arată că pe computer există o copie sincronizată automat a documentului

  - **Data.DstDoc.Location -** arată ce serviciu a furnizat documentul nou (OneDrive, File Server, SharePoint etc.)

  - **Data.DstDoc.NumberCoAuthors -** numărul de alți utilizatori dintr-o sesiune de editare în colaborare în documentul nou

  - **Data.DstDoc.ReadOnlyReasons -** motivele pentru care documentul nou a fost deschis doar în citire

  - **Data.DstDoc.ResourceIdHash -** identificator de document anonimizat, folosit în diagnosticarea problemelor cu documentul nou

  - **Data.DstDoc.ServerDocId -** identificator de document anonimizat invariabil, folosit în diagnosticarea problemelor cu documentul nou

  - **Data.DstDoc.ServerProtocol -** versiunea de protocol folosită în comunicarea cu serviciul la crearea documentului nou

  - **Data.DstDoc.ServerType -** tipul de server care oferă serviciul (SharePoint, OneDrive, WOPI etc.) pentru documentul nou

  - **Data.DstDoc.ServerVersion -** versiunea serverului care oferă serviciul pentru documentul nou

  - **Data.DstDoc.SessionId -** identifică o anumită sesiune de editare a documentului din sesiunea completă pentru documentul nou

  - **Data.DstDoc.SharePointServiceContext -** informații de diagnosticare din solicitările SharePoint Online pentru documentul nou

  - **Data.DstDoc.SizeInBytes -** indicator privind dimensiunea documentului ale documentului nou

  - **Data.DstDoc.UrlHash -** cod hash unidirecțional pentru crearea unui identificator naiv pentru documentul pentru documentul nou

  - **Data.EditorsCount -** numărul altor colaboratori care editează documentul

  - **Data.FullIError -** cache de la toate codurile de eroare din nivelul de protocol

  - **Data.HasFilteredCategories -** depășit

  - **Data.HasFilteredCategoryNames -** depășit

  - **Data.HasFilteredSeries -** depășit

  - **Data.HasFilteredSeriesNames -** depășit

  - **Data.HasPendingSaveAs -** indică faptul că o solicitare Salvare ca/Salvare copie este în curs

  - **Data.Input.FileOpenState -** starea solicitată de aplicație (Read/ReadWrite etc.)

  - **Data.Input.FileSaveState -** State starea solicitată de aplicație (Salvare în timpul deschiderii, Salvare ca etc.)

  - **Data.Input.NetworkCost -** indică cost/tip de rețea (contorizată, contorizată peste limită etc.)

  - **Data.Input.OpenAsync -** semnalizarea indică faptul că aplicația a solicitat o deschidere asincronă

  - **Data.Input.OpenOfflineCopy -** semnalizarea indică faptul că aplicația a solicitat o deschidere offline

  - **Data.IsCachedHistoricalVersion -** indică faptul că acest fișier memorat în cache nu este cea mai recentă versiune

  - **Data.IsHtml -** indică faptul că formatul textului HTML a fost lipit

  - **Data.IsLegacyCode -** indică faptul că formatul textului cu cod moștenit a fost lipit

  - **Data.IsLocalOnlyFile -** indică faptul că fișierul a fost deschis doar din spațiul de stocare local

  - **Data.IsLocalOrSyncBackedFile -** indică faptul că fișierul a fost deschis local și mapat prin serviciu

  - **Data.IsMapUnMapCase -** parte din starea fișierului memorat în cache

  - **Data.isOpenFromCollab -** indică faptul că fișierul a fost deschis din serviciul de colaborare partajată

  - **Data.IsStubFile -** documentul nu a fost partajat încă în serviciul în cloud

  - **Data.IsSyncBackedFile -** documentul este într-un folder care este actualizat prin sincronizare automată

  - **Data.IsSyncBackedStateDifferentThanOnLastOpen -** starea documentului s-a modificat, este posibil ca modificările să se fi produs în timp ce documentul nu era deschis

  - **Data.IsWorkingBranchAvailableOnOpen -** modificați diagnosticarea de urmărire asigurându-vă că avem cea mai recentă versiune a unui fișier partajat

  - **Data.Location -** indică tipul suportului de stocare/locația (USB, Cloud etc.)

  - **Data.LockRequestDocMode -** indică dacă documentul este disponibil pentru alte persoane

  - **Data.MruRequestResult -** depășit

  - **Data.NewDataNotAvailableReason -** depășit

  - **Data.OcsDisableReasons -** nu este utilizat de Salvare

  - **Data.OcsHostOnOpen -** nu este utilizat de Salvare

  - **Data.Output.FileSaveState -** starea la finalizarea salvării

  - **Data.PivotChart -** depășit

  - **Data.resolveConflictState -** coduri pentru motiv pentru ca o solicitare să rezolve conflicte de îmbinare

  - **Data.RTCEnabled -** protocolul de distribuire de modificare rapidă a început

  - **Data.SaveAsToCurrent -** indică faptul că documentul activ va suprascrie fișierul stocat

  - **Data.ServiceId -** depășit, înlocuit de Data\_Doc\_WopiServiceId

  - **Data.SessionId -** depășit

  - **Data.SizeInBytes -** depășit, înlocuit de Data\_Doc\_SizeInBytes

  - **Data.StopwatchDuration -** depășit

  - **Data.SyncBackedFileRequiresOnlineTransition -** semnalizare care indică faptul că acțiunea de salvare este blocată temporar de tranziția online

  - **Data.SyncBackedFileSaveOnOpen -** semnalizare care indică faptul că modificările efectuate de sincronizarea automată necesită salvare la deschidere

  - **Data.TelemetryId -** depășit

  - **Data.TriggerSaveAfterBaseDownload -** modificați diagnosticarea de urmărire asigurându-vă că avem cea mai recentă versiune a unui fișier partajat

  - **Data.UploadBlockedDueToCoherencyFailure -** salvarea în serviciu a blocat rezoluția utilizatorului în așteptare privind modificările aflate în conflict

  - **Data.UploadBlockedDueToFailedSaveAsOverExisting -** salvare în serviciu blocată din cauza unei încercări nereușite de a suprascrie un fișier existent

  - **Data.UploadPreemptedForCoherency -** salvare în serviciu abandonată întrucât sunt efectuate mai multe modificări de către utilizator

  - **Data.UploadPreemptedForSaveAsOverExistingFailure -** salvare în serviciu abandonată din cauza erorii SaveAsOverExisting anterioare

  - **Data.UploadScheduled -** fișierul este gata să fie încărcat asincron în serviciu

  - **Data.UseClientIdAsSchemaLockId -** semnalizare pentru a controla modul în care documentele sunt blocate în cadrul serviciului

  - **Data.WorkingCopySaved -** modificați diagnosticarea de urmărire asigurându-vă că avem cea mai recentă versiune a unui fișier partajat

  - **Data.ZrtSaveAsforSyncBackedBusinessEnabled -** semnalizare care indică salvarea rapidă activată pentru SharePoint Online

  - **Data.ZrtSaveAsforSyncBackedConsumerEnabled -** semnalizare care indică salvarea rapidă activată pentru OneDrive Consumer

  - **Data.ZrtSaveAsforSyncBackedCTBusinessEnabled -** semnalizare care indică salvarea rapidă a tipurilor de conținut activată pentru SharePoint Online

  - **Data.ZrtSaveAsforSyncBackedCTConsumerEnabled -** semnalizare care indică salvarea rapidă a tipurilor de conținut activată pentru OneDrive Consumer

  - **Data.ZrtSaveAsforSyncBackedMetaDataBusinessEnabled -** semnalizare care indică salvarea rapidă a metadatelor de fișiere activată pentru SharePoint Online

  - **Data.ZrtSaveAsforSyncBackedMetaDataConsumerEnabled -** semnalizare care indică salvarea rapidă a metadatelor de fișiere activată pentru OneDrive Consumer-

#### <a name="officefindtimeappfailedtostart"></a>Office.FindTime.AppFailedToStart

Colectat atunci când aplicația nu reușește să pornească din cauza unei erori în timpul pornirii. Utilizat pentru a urmări excepții și căderi. Ajută la monitorizarea și depanarea stării aplicației.

Se colectează următoarele câmpuri:
- **DateTime** - marcă de timp privind momentul în care evenimentul este înregistrat în jurnal

- **EventName** - numele evenimentului conectat

#### <a name="officefirstrunappleactivationresult"></a>Office.FirstRun.Apple.ActivationResult

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Evenimentul este utilizat pentru a monitoriza starea fluxului nostru de activare a aplicațiilor. Colectăm date pentru a afla rezultatul activității de activare a abonamentului Office 365, împreună cu fluxul utilizat pentru activare (prima experiență de rulare, fluxul în aplicație, achiziționare etc.).

Se colectează următoarele câmpuri:

- **Data_ActivationStatusCollectionTime** - un marcaj temporal

- **Data_ActivationStatusError** - un cod de eroare de activare.

- **Data_ActivationStatusFlowType** - o valoare numerică indicând tipul de flux de activare

#### <a name="officefirstrunappleactivationstatus"></a>Office.FirstRun.Apple.ActivationStatus

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Acest eveniment este utilizat pentru a afla rezultatul activității de activare a abonamentului Office 365, împreună cu fluxul utilizat pentru activare (FRE, în aplicație, achiziționare etc.). Colectăm date care conțin tipul de activare, tipul de flux (FRE/DocStage/Purchase) și ID-ul serviciului de licențiere Office.

Se colectează următoarele câmpuri:

- **Data_ActivationTypeCollectionTime** - un marcaj temporal

- **Data_ActivationTypeFlowType** - o valoare numerică indicând tipul de flux de activare

- **Data_ActivationTypeOLSLicense** - un identificator al licenței

- **Data_ActivationTypeStatus** - un cod de stare de activare.

#### <a name="officefirstrunapplefirstruncomplete"></a>Office.FirstRun.Apple.FirstRunComplete

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Evenimentul ne anunță dacă utilizatorul rulează în freemium, tipul de flux în execuție (FRE/DocStage/Purchase) și tipul de identitate (MSA/OrgID). Utilizăm acest eveniment pentru a ne da seama dacă s-a finalizat prima experiență de rulare (FRE) și tipul de identitate utilizat pentru conectare (MSA/OrgID).

Se colectează următoarele câmpuri:

- **Data_FirstRunCompletedCollectionTime** - o marcă de timp care înregistrează ora la care s-a finalizat fluxul

- **Data_FirstRunCompletedFlowType** - un cod care denotă tipul de flux de utilizator care a fost finalizat 

- **Data_FirstRunCompletedFreemiumStatus** - un cod reprezentând starea finalizării pentru un flux de utilizator freemium

- **Data_FirstRunCompletedIdentityType** - tipul de identitate al utilizatorului care a terminat fluxul

#### <a name="officefirstrunapplefirstrunstart"></a>Office.FirstRun.Apple.FirstRunStart

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Evenimentul ne anunță că un utilizator a introdus prima experiență de rulare și tipul de flux care rulează (FRE/DocStage/Purchase). Utilizăm acest eveniment pentru a ne da seama dacă prima experiență de rulare (FRE) a fost începută cu succes.

Se colectează următoarele câmpuri:

- **Data_FirstRunStartedCollectionTime** - o marcă de timp care înregistrează ora la care s-a finalizat fluxul

- **Data_FirstRunStartedFlowType** - un cod care denotă tipul de flux de utilizator care a fost finalizat 

#### <a name="officefirstrunapplefirstrunstartedandcompleted"></a>Office.FirstRun.Apple.FirstRunStartedAndCompleted

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Evenimentul ne anunță dacă utilizatorul rulează în freemium, tipul de flux în execuție (FRE/DocStage/Purchase) și tipul de identitate (MSA/OrgID). Vom utiliza acest eveniment pentru a ne da seama care este starea de funcționare a fluxului nostru de experiență de prima rulare (FRE).

Se colectează următoarele câmpuri:

- **Data_FirstRunCompletedCollectionTime** - o marcă de timp care înregistrează ora la care s-a finalizat fluxul

- **Data_FirstRunCompletedFlowType** - un cod care denotă tipul de flux de utilizator care a fost finalizat  

- **Data_FirstRunCompletedFreemiumStatus** - un cod reprezentând starea finalizării pentru un flux de utilizator freemium

- **Data_FirstRunCompletedIdentityType** - tipul de identitate al utilizatorului care a terminat fluxul

- **Data_FirstRunStartedCollectionTime** - o marcă de timp care înregistrează ora la care s-a început fluxul

- **Data_FirstRunStartedFlowType** - un cod care denotă tipul de flux de utilizator care a fost început

#### <a name="officefirstrunappleinapppurchaseactivationfail"></a>Office.FirstRun.Apple.InAppPurchaseActivationFail

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Evenimentul este utilizat pentru a monitoriza starea fluxului nostru de activare a aplicațiilor. Colectăm date pentru a afla rezultatul activității de activare a achiziției în cadrul aplicației, împreună cu fluxul utilizat pentru activare (prima experiență de rulare, achiziționarea în aplicația Flow etc.). 

Se colectează următoarele câmpuri:

- **Data_ActivationFailCollectionTime** - un marcaj temporal care înregistrează ora la care s-a produs eroarea de activare 

- **Data_ActivationFailFlowType** - un cod care denotă tipul de flux de utilizator care a fost exercitat

- **Data_AssociatedSuccessfullyCollectionTime** - un marcaj temporal care înregistrează ora la care s-a produs asocierea 

- **Data_AssoicatedSuccessfullyFlowType** - un cod care denotă tipul de flux de utilizator care a fost exercitat

#### <a name="officefirstrunappleinapppurchaseactivationsuccess"></a>Office.FirstRun.Apple.InAppPurchaseActivationSuccess

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Evenimentul este utilizat pentru a monitoriza starea fluxului nostru de activare a aplicațiilor. Colectăm date pentru a afla rezultatul activității de activare a achiziției în cadrul aplicației, împreună cu fluxul utilizat pentru activare (prima experiență de rulare, achiziționarea în aplicația Flow etc.). 

Se colectează următoarele câmpuri:

- **Data_ActivatedSuccessfullyCollectionTime** - un marcaj temporal care înregistrează ora la care s-a produs activarea 

- **Data_ActivatedSuccessfullyFlowType** - un cod care denotă tipul de flux de utilizator care a fost exercitat

- **Data_AssociatedSuccessfullyCollectionTime** - un marcaj temporal care înregistrează ora la care s-a produs asocierea 

- **Data_AssoicatedSuccessfullyFlowType** - un cod care denotă tipul de flux de utilizator care a fost exercitat

#### <a name="officefirstrunappleinapppurchaseassociationfailed"></a>Office.FirstRun.Apple.InAppPurchaseAssociationFailed

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Evenimentul este utilizat pentru a monitoriza starea fluxului nostru de activare a aplicațiilor. Colectăm date pentru a afla rezultatul activității de activare a achiziției în cadrul aplicației, împreună cu fluxul utilizat pentru activare (prima experiență de rulare, achiziționarea în aplicația Flow etc.). 

Se colectează următoarele câmpuri:

- **Data_AppChargedSuccessfullyCollectionTime** - un marcaj temporal care înregistrează ora la care a fost încărcată achiziția

- **Data_AppChargedSuccessfullyFlowType** - un cod care denotă tipul de flux de utilizator care a fost exercitat

- **Data_AssociationFailedCollectionTime** - un marcaj temporal care înregistrează ora la care nu s-a reușit asocierea de aplicații

- **Data_AssociationFailedFlowType** - un cod care denotă tipul de flux de utilizator care a fost exercitat

- **Data_AssociationFailedResult** - un cod care denotă tipul de eroare observată

#### <a name="officefirstrunappleinapppurchaseassociationsuccess"></a>Office.FirstRun.Apple.InAppPurchaseAssociationSuccess

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Evenimentul este utilizat pentru a monitoriza starea fluxului nostru de activare a aplicațiilor. Colectăm date pentru a afla rezultatul activității de activare a achiziției în cadrul aplicației, împreună cu fluxul utilizat pentru activare (prima experiență de rulare, achiziționarea în aplicația Flow etc.). 

Se colectează următoarele câmpuri:

- **Data_AppChargedSuccessfullyCollectionTime** - un marcaj temporal care înregistrează ora la care a fost încărcată achiziția

- **Data_AppChargedSuccessfullyFlowType** - un cod care denotă tipul de flux de utilizator care a fost exercitat

- **Data_AssociatedSuccessfullyCollectionTime** - un marcaj temporal care înregistrează ora la care nu s-a reușit asocierea de aplicații

- **Data_AssoicatedSuccessfullyFlowType** - un cod care denotă tipul de flux de utilizator care a fost exercitat

#### <a name="officefirstrunappleinapppurchasefailures"></a>Office.FirstRun.Apple.InAppPurchaseFailures

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Evenimentul este utilizat pentru a monitoriza starea fluxului nostru de activare a aplicațiilor. Colectăm date despre rezultatul fluxului de achiziții în cadrul aplicației.

Se colectează următoarele câmpuri:

- **Data_AppStoreFailureFlowType** - un cod care denotă tipul de flux de utilizator care a fost exercitat

- **Data_AppStoreFailureResult** - rezultatul erorii observat

- **Data_CancelRequestFlowType** - un cod care denotă tipul de flux de utilizator care a fost exercitat

- **Data_EventId** - un cod care denotă tipul de eroare observată

#### <a name="officefirstrunappleinapppurchasesattempted"></a>Office.FirstRun.Apple.InAppPurchasesAttempted

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Evenimentul este utilizat pentru a monitoriza starea fluxului nostru de achiziție în cadrul aplicațiilor. Colectăm date pentru a urmări încercările de achiziție din cadrul aplicației și tipul lor de SKU achiziționat (lunar/anual/Home/personal).

Se colectează următoarele câmpuri:

- **Data_EventId** - un cod care denotă tipul de rezultat observat

- **Data_PurchasedClickedOfferType** - tipul de SKU încercat la achiziționare

- **Data_PurchaseSuccessfulFlowType** - un cod care denotă tipul de flux de utilizator care a fost exercitat

#### <a name="officefirstrunappleinapprestoreattempted"></a>Office.FirstRun.Apple.InAppRestoreAttempted

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Evenimentul este utilizat pentru a monitoriza starea fluxului nostru de achiziție în cadrul aplicațiilor. Colectăm date pentru a urmări restaurările încercate în cadrul aplicațiilor

Se colectează următoarele câmpuri:

- **Data_EventId** - un cod care denotă tipul de rezultat al tentativei

- **Data_RestoreAttemptFlowType** - un cod care denotă tipul de flux de utilizator care a fost exercitat

#### <a name="officefirstrunappleinapprestoreattemptfailed"></a>Office.FirstRun.Apple.InAppRestoreAttemptFailed

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Evenimentul este utilizat pentru a monitoriza starea fluxului nostru de achiziție în cadrul aplicațiilor. Colectăm date pentru a urmări restaurările încercate în cadrul aplicațiilor precum și fluxurile și erorile lor asociate.

Se colectează următoarele câmpuri:

- **Data_RestoreButtonFlowType** - un cod care denotă tipul de flux de utilizator care a fost exercitat

- **Data_RestoredFailedPaymentCancelledFlowType** - un cod care denotă tipul de flux de anulare a plăților care a fost exercitat

- **Data_RestoredFailedUnKnownFlowType** - dacă încercarea nu a reușit din cauza exercițiului unui flux de utilizator neașteptat

- **Data_RestoredFailedUnKnownResult** - dacă încercarea nu a reușit din motive necunoscute

#### <a name="officefirstrunapplemacfirstruncompleted"></a>Office.FirstRun.Apple.MacFirstRunCompleted

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Evenimentul ne anunță că un utilizator a trecut prin prima experiență de rulare. Utilizăm acest eveniment pentru a ne da seama dacă prima experiență de rulare (FRE) a fost finalizată cu succes.

Se colectează următoarele câmpuri:

- **Data_FirstRunCollectionTime** - un marcaj de timp care înregistrează ora la care s-a finalizat fluxul.

#### <a name="officefirstrunapplemacwxpfirstrunstarted"></a>Office.FirstRun.Apple.MacWXPFirstRunStarted

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Evenimentul ne anunță că un utilizator a intrat în prima experiență de rulare. Utilizăm acest eveniment pentru a ne da seama dacă prima experiență de rulare (FRE) a fost începută cu succes.

Se colectează următoarele câmpuri:

- **Data_FirstRunPanelName** - numele panoului din care a început experiența

#### <a name="officeiospaywallpaywallpresented"></a>Office.iOS.Paywall.Paywall.Presented

Această telemetrie de utilizare critică este colectată atunci când se afișează controlul Paywall utilizatorului și este utilizat pentru înțelegerea experienței de achiziție în cadrul aplicației pentru utilizator și pentru optimizarea acesteia pentru versiunile viitoare.

Se colectează următoarele câmpuri:

- **entryPoint** - Șir – butonul/fluxul din care a fost afișat Paywall. Cum ar fi „Buton upgrade premium” sau „Primul flux de rulare”

- **isFRE** - Boolean – Afișăm prima experiență de rulare sau interfața utilizator obișnuită?

#### <a name="officeiospaywallpaywallstats"></a>Office.iOS.Paywall.Paywall.Stats

Această metadată pe baza sesiunii este colectată atunci când este afișat utilizatorului interfața de utilizator Paywall, durata interacțiunii și dacă o achiziție a fost încercată cu sau fără succes.    Datele sunt utilizate pentru a înțelege utilizarea și starea de funcționare a întregii experiențe de plată și depanare, pentru a optimiza și a depana experiența de achiziție în cadrul aplicației în versiunile viitoare.

Se colectează următoarele câmpuri:

- **entryPoint** - Șir – butonul/fluxul din care a fost afișat Paywall. Cum ar fi „Buton upgrade premium” sau „Primul flux de rulare”.

- **isFRE** - Boolean – Afișăm prima experiență de rulare sau interfața utilizator obișnuită?

- **status** - Șir – Stare de ieșire Paywall. Cum ar fi „inițiat”, „paymentDone”, „provisionFailed”

- **userDuration** - Dublu – Durata în milisecunde a timpului petrecut de utilizator în Paywall

#### <a name="officeiospaywallskuchoosermorebenefitsstats"></a>Office.iOS.Paywall.SKUChooser.MoreBenefits.Stats

Acest eveniment colectează caracteristicile și aplicațiile pe care le extinde utilizatorul din „Vedeți mai multe beneficii”, precum și durata și timpul consumat.  Datele sunt utilizate pentru înțelegerea caracteristicii „Vedeți mai multe beneficii” și pentru optimizarea ulterioară a experienței în versiunile viitoare.

Se colectează următoarele câmpuri:

- **appsExpanded** - Șir - lista separată prin virgulă de servicii/aplicații pentru care au fost extinse beneficiile.

- **productId** - Șir - ID-ul produsului din App Store pentru care utilizatorul vizualizează mai multe beneficii oferite

- **userDuration** - Dublu – Durata în milisecunde a timpului petrecut de utilizator pe ecranul beneficii.

#### <a name="officeiospaywallskuchooserstats"></a>Office.iOS.Paywall.SKUChooser.Stats

Această telemetrie de utilizare este colectată pentru a vedea cum a accesat utilizatorul selectorul SKU, cât timp a petrecut pe ecranul selectorului SKU și de ce a ieșit din selectorul SKU.  Datele sunt utilizate pentru înțelegerea utilizării selectorului SKU și pentru optimizarea experienței de achiziție în cadrul aplicației în versiunile viitoare.

Se colectează următoarele câmpuri:

- **entryPoint** - Șir – butonul/fluxul din care a fost afișat Paywall. Cum ar fi „Buton upgrade premium” sau „Primul flux de rulare”.

- **exitReason** - Șir – motivul ieșirii din selectorul SKU. Cum ar fi „Buybutton”, „CloseButton”

- **isFRE** - Boolean – Afișăm prima experiență de rulare sau interfața utilizator obișnuită?

- **userDuration** - Dublu – Durata în milisecunde a timpului petrecut de utilizator în selectorul SKU.


#### <a name="officelivepersonacardconfigurationsetaction"></a>Office.LivePersonaCard.ConfigurationSetAction

Ne conectăm când utilizatorul se află într-o aplicație care încarcă un card de persoană în anticiparea utilizatorului care deschide Cardul de persoană live.  Datele sunt utilizate pentru a determina dacă respectivul card este încărcat corect. 

Se colectează următoarele câmpuri: 

- **Data.accountType** - dacă utilizatorul aparține unei organizații sau unui consumator

- **Data.appContextId** - ID generat aleatoriu utilizat pentru a identifica conturi diferite în aceeași aplicație

- **Data.AppInfo.Name** - numele serviciului utilizat (fișă de profil)

- **Data. AppInfo_Id** - numele aplicației gazdă

- **Data.AppInfo_Version** - versiunea aplicației gazdă

- **Data.cardCorrelationId** - identificatorul unic global pentru un card de persoană

- **Data.cardPersonaCorrelationId** - identificatorul unic global pentru o anumită persoană afișată într-un card

- **Data.clientCorrelationId** - identificatorul unic global pentru sesiunea aplicației

- **Data.clientType** - tipul de dispozitiv pe care rulează aplicația

- **Data.contextType** - din ce context (aplicație) a fost lansată fișa

- **Data.ecsConfigIds** - identificatori de versiune pentru caracteristicile activate în fișă

- **Data.ecsTagId** - ID etichetă pentru caracteristici

- **Data.eventId** - identificator de nume al evenimentului, de exemplu, „LivePersonaCardRenderedAction”

- **Data. eventpriority** - valoare de enumerare pentru prioritatea de trimitere a evenimentului.

- **Data.feature** - utilizat pentru a grupa diverse evenimente cu aceeași caracteristică (fișă de profil)

- **Data.flights** - caracteristici activate în fișă

- **Data.fromCache** - dacă datele au fost preluate din memorie

- **Data.hasFinePointer** - dacă dispozitivul are capacitatea indicatorului mouse-ului

- **hasHoverEvents** - dacă dispozitivul are capacitate de trecere cu mouse-ul

- **Data.immersiveProfileCorrelationId** - un identificator unic global pentru sesiunea de vizualizare profil extinsă

- **Data.offlineResolved** - dacă s-au preluat date în timp ce erați offline

- **Data.OTelJS.Version** - versiune de OTel logger

- **Data.personaCorrelationId** - un Identificator unic global pentru personaje unice într-o sesiune

- **Date.propreties** - metadate suplimentare colectate pentru fiecare eveniment, după cum urmează: *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

  - **cardCorrelationId** - dublură a Data.appContextId de mai sus
  - **cardPersonaCorrelationId** - dublură a Data.cardCorrelationId de mai sus
  - **ClientTimeStamp** - ora în aplicație la care s-a înregistrat evenimentul
  - **consumerCorrelationId** - dublură a Data.clientCorrelationId de mai sus

  - **externalAppSessionCorrelationId** - un identificator unic global pentru aplicație, pentru a identifica toate cardurile de persoane deschise în aceeași sub-sesiune

- **Data.region** - regiunea geografică a serviciului de back-end a fișei de profil la care este conectat utilizatorul

- **Data.tenantAadObjectId** - entitatea găzduită la care este legat abonamentul unui utilizator. Ne permite să clasificăm problemele și să identificăm dacă este o problemă pe scară largă sau una izolată la un set de utilizatori sau la o anumită entitate găzduită

- **Data.type** - tipul evenimentului înregistrat, de exemplu, urmărire, eroare, eveniment

- **Data.userAadObjectId** - identificatorul de utilizator unic global pentru un cont Microsoft Enterprise (dublură a Data.UserInfo.Id)

- **Data.UserInfo.Id** - identificatorul de utilizator unic global pentru un cont Microsoft Enterprise

- **Data.UserInfo.MsaId** - identificatorul de utilizator unic global pentru un cont Microsoft consumator

- **Data.UserInfo.OMSTenantId** - entitatea găzduită la care este asociat abonamentul unui utilizator. Ne permite să clasificăm problemele și să identificăm dacă este o problemă pe scară largă sau una izolată la un set de utilizatori sau la o anumită entitate găzduită

- **Data.userPuid** - identificatorul de utilizator unic global pentru un cont Microsoft consumator (duplicat pentru Data.UserInfo.MsaId) 

- **Data.version** - versiunea serviciului (fișă de profil)

- **Data. workloadCulture** - set de culturi din aplicația gazdă

- **DeviceInfo_Id** - identificatorul de dispozitiv unic global pentru un dispozitiv

- **DeviceInfo_Make** - marca sistemului de operare

- **DeviceInfo_Model** - modelul dispozitivului

- **DeviceInfo_OsName** - numele dispozitivului OS

- **DeviceInfo_OsVersion** - versiunea sistemului de operare

- **DeviceInfo_SDKUid** - identifică în mod unic dispozitivul din perspectiva SDK-ului de telemetrie

#### <a name="officelivepersonacarduseractionsclosedexpandedpersonacard"></a>Office.LivePersonaCard.UserActions.ClosedExpandedPersonaCard

Conectat atunci când utilizatorul închide un Card de persoană extins. Se utilizează pentru a observa anomalii critice în ratele de eroare la închiderea Cardului de persoană live.

Se colectează următoarele câmpuri:

- **AppInfo_Id** - numele aplicației gazdă

- **AppInfo_Version** - versiunea aplicației gazdă

- **Data.appContextId** - un ID generat aleatoriu utilizat pentru a identifica conturi diferite în aceeași aplicație

- **Data.AppInfo.Name** - numele serviciului utilizat (fișă de profil)

- **Data.cardCorrelationId** - identificatorul unic global pentru un card de persoană

- **Data.cardPersonaCorrelationId** - identificatorul unic global pentru o anumită persoană afișată într-un card

- **Data.clientCorrelationId** - identificatorul unic global pentru sesiunea aplicației

- **Data.clientType** - tipul de dispozitiv pe care rulează aplicația, de exemplu, „Outlook_Win32”

- **Data.eventId** - identificator de nume al evenimentului, de exemplu, „LivePersonaCardRenderedAction”

- **Data.exportName** - nume uman lizibil al evenimentului de acțiune pentru utilizatori, de exemplu, „ClosedExpandedPersonaCard”

- **Data.exportType** - categoria evenimentului pentru solicitarea de export GDPR

- **Data.externalAppSessionCorrelationId** - un Identificator unic global pentru ca aplicația să identifice toate fișele personale deschise în aceeași sub-sesiune

- **Data.feature** - utilizat pentru a grupa diverse evenimente cu aceeași caracteristică (fișă de profil)

- **Data.immersiveProfileCorrelationId** - un identificator unic global pentru sesiunea de vizualizare profil extinsă

- **Data.OTelJS.Version** - versiune de OTel logger

- **Data.personaCorrelationId** - un Identificator unic global pentru personaje unice într-o sesiune

- **Date.propreties** - metadate suplimentare colectate pentru fiecare eveniment, după cum urmează: *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

   - **cardCorrelationId** - dublură a Data.appContextId de mai sus 
   - **cardPersonaCorrelationId** - dublură a Data.cardCorrelationId de mai sus
   - **ClientTimeStamp** - ora la care a avut loc evenimentul în timpul epocii Unix
   - **consumerCorrelationId** - dublură a Data.clientCorrelationId de mai sus 

- **Data.region** - regiunea geografică a serviciului de back-end a fișei de profil la care este conectat utilizatorul

- **Data.tenantAadObjectId** - entitatea găzduită la care este legat abonamentul unui utilizator. Ne permite să clasificăm problemele și să identificăm dacă este o problemă pe scară largă sau una izolată la un set de utilizatori sau la o anumită entitate găzduită

- **Data.type** - tipul evenimentului înregistrat, de exemplu, urmărire, eroare, eveniment

- **Data.userAadObjectId** - identificatorul de utilizator unic global pentru un cont Microsoft Enterprise (dublură a Data.UserInfo.Id)

- **Data.UserInfo.Id** - identificatorul de utilizator unic global pentru un cont Microsoft Enterprise 

- **Data.UserInfo.MsaId** - identificatorul de utilizator unic global pentru un cont Microsoft consumator

- **Data.UserInfo.OMSTenantId** - entitatea găzduită la care este asociat abonamentul unui utilizator. Ne permite să clasificăm problemele și să identificăm dacă este o problemă pe scară largă sau una izolată la un set de utilizatori sau la o anumită entitate găzduită.

- **Data.userPuid** - identificatorul de utilizator unic global pentru un cont Microsoft consumator (duplicat pentru Data.UserInfo.MsaId) 

- **Data.version** - versiunea serviciului (fișă de profil)

- **DeviceInfo_Id** - identificatorul de dispozitiv unic global pentru un dispozitiv

- **DeviceInfo_Make** - marca sistemului de operare

- **DeviceInfo_Model** - modelul dispozitivului

- **Data.Input.NetworkCost** - indică costul/tipul de rețea (contorizată, contorizată peste limită etc.)

- **DeviceInfo_OsName** - numele dispozitivului OS

- **DeviceInfo_OsVersion** - versiunea sistemului de operare

- **PipelineInfo.ClientCountry** - Codul de țară a expeditorului, bazat pe adresa IP a clientului neanulată


#### <a name="officelivepersonacarduseractionsclosedpersonacard"></a>Office.LivePersonaCard.UserActions.ClosedPersonaCard

Ne înregistrăm atunci când utilizatorul închide un Card de persoană.  Datele sunt utilizate pentru a determina dacă respectivul card este încărcat corect. 

Se colectează următoarele câmpuri: 

- **BatchId** - identificator unic global, dacă s-a efectuat un set de solicitări

- **Data.appContextId** - un ID generat aleatoriu utilizat pentru a identifica conturi diferite în aceeași aplicație

- **Data.AppInfo.Name** - numele serviciului utilizat (fișă de profil)

- **Data. AppInfo_Id** - numele aplicației gazdă

- **Data.AppInfo_Version** - versiunea aplicației gazdă

- **Data.cardCorrelationId** - identificatorul unic global pentru un card de persoană

- **Data.cardPersonaCorrelationId** - identificatorul unic global pentru o anumită persoană afișată într-un card

- **Data.clientCorrelationId** - identificatorul unic global pentru sesiunea aplicației

- **Data.clientType** - tipul de dispozitiv pe care rulează aplicația

- **Data.eventId** - identificator de nume al evenimentului, de exemplu, „LivePersonaCardRenderedAction”

- **Data.externalAppSessionCorrelationId** - un identificator unic global pentru ca aplicația să identifice toate fișele personale deschise în aceeași sub-sesiune.

- **Data.feature** - utilizat pentru a grupa diverse evenimente cu aceeași caracteristică (fișă de profil)

- **Data.immersiveProfileCorrelationId** - un identificator unic global pentru sesiunea de vizualizare profil extinsă

- **Data.OTelJS.Version** - versiune de OTel logger

- **Data.personaCorrelationId** - un Identificator unic global pentru personaje unice într-o sesiune

- **Date.propreties** - metadate suplimentare colectate pentru fiecare eveniment, după cum urmează: *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

  - **ClientTimeStamp** - ora în aplicație la care s-a înregistrat evenimentul
  - **cardCorrelationId** - dublură a Data.appContextId de mai sus
  - **cardPersonaCorrelationId** - dublură a Data.cardCorrelationId de mai sus
  - **consumerCorrelationId** - dublură a Data.clientCorrelationId de mai sus

- **Data.region** - regiunea geografică a serviciului de back-end a fișei de profil la care este conectat utilizatorul

- **Data.tenantAadObjectId** - entitatea găzduită la care este legat abonamentul unui utilizator. Ne permite să clasificăm problemele și să identificăm dacă este o problemă pe scară largă sau una izolată la un set de utilizatori sau la o anumită entitate găzduită

- **Data.type** - tipul evenimentului înregistrat, de exemplu, urmărire, eroare, eveniment

- **Data.userAadObjectId** - identificatorul de utilizator unic global pentru un cont Microsoft Enterprise (dublură a Data.UserInfo.Id)

- **Data.UserInfo.Id** - identificatorul de utilizator unic global pentru un cont Microsoft Enterprise

- **Data.UserInfo.MsaId** - identificatorul de utilizator unic global pentru un cont Microsoft consumator

- **Data.UserInfo.OMSTenantId** - entitatea găzduită la care este asociat abonamentul unui utilizator. Ne permite să clasificăm problemele și să identificăm dacă este o problemă pe scară largă sau una izolată la un set de utilizatori sau la o anumită entitate găzduită

- **Data.userPuid** - identificatorul de utilizator unic global pentru un cont Microsoft consumator (duplicat pentru Data.UserInfo.MsaId) 

- **Data.version** - versiunea serviciului (fișă de profil)

- **Data_hostAppRing** - inelul de implementare pentru cardul de persoană

- **Event_ReceivedTime** - ora la care s-a înregistrat evenimentul în serviciu

#### <a name="officelivepersonacarduseractionsopenedexpandedpersonacard"></a>Office.LivePersonaCard.UserActions.OpenedExpandedPersonaCard

Înregistrat atunci când utilizatorul deschide un Card de persoană extins. Se utilizează pentru a observa anomalii critice în ratele de eroare la lansarea Cardului de persoană live.

Se colectează următoarele câmpuri:

- **AppInfo_Id** - numele aplicației gazdă

- **AppInfo_Version** - versiunea aplicației gazdă

- **Data.appContextId** - un ID generat aleatoriu utilizat pentru a identifica conturi diferite în aceeași aplicație

- **Data.AppInfo.Name** - numele serviciului utilizat (fișă de profil)

- **Data.cardCorrelationId** - identificatorul unic global pentru un card de persoană

- **Data.cardPersonaCorrelationId** - identificatorul unic global pentru o anumită persoană afișată într-un card

- **Data.clientCorrelationId** - identificatorul unic global pentru sesiunea aplicației

- **Data.clientScenario** - pentru a identifica caracteristica din aplicație de unde a fost deschisă fișa de personaj

- **Data.clientType** - tipul de dispozitiv pe care rulează aplicația

- **Data.eventId** - identificator de nume al evenimentului, de exemplu, „LivePersonaCardRenderedAction”

- **Data.externalAppSessionCorrelationId** - un identificator unic global pentru ca aplicația să identifice toate fișele personale deschise în aceeași sub-sesiune.

- **Data.exportName** - nume ușor de citit pentru oameni al evenimentului acțiune a utilizatorului, de exemplu,„OpenedPersonaCard”

- **Data.exportType** - categoria evenimentului pentru solicitarea de export GDPR

- **Data.feature** - utilizat pentru a grupa diverse evenimente cu aceeași caracteristică (fișă de profil)

- **Data.hasPersonalInsightRing** - detalii din Office sau LinkedIn pot fi disponibile pentru utilizator

- **Data.hostAppRing** - inelul prin care a fost distribuită aplicația

- **Data.immersiveProfileCorrelationId** - un identificator unic global pentru sesiunea de vizualizare profil extinsă

- **Data.OTelJS.Version** - versiune de OTel logger

- **Data.personaCorrelationId** - un Identificator unic global pentru personaje unice într-o sesiune

- **Date.propreties** - metadate suplimentare colectate pentru fiecare eveniment, după cum urmează: *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

  - **cardCorrelationId** - dublură a Data.appContextId de mai sus 
  - **cardPersonaCorrelationId** - dublură a Data.cardCorrelationId de mai sus
  - **consumerCorrelationId** - dublură a Data.clientCorrelationId de mai sus 

- **Data.region** - regiunea geografică a serviciului de back-end a fișei de profil la care este conectat utilizatorul

- **Data.section** – secțiunea activă din fișa extinsă

- **Data.tenantAadObjectId** - entitatea găzduită la care este legat abonamentul unui utilizator. Ne permite să clasificăm problemele și să identificăm dacă este o problemă pe scară largă sau una izolată la un set de utilizatori sau la o anumită entitate găzduită

- **Data.type** - tipul evenimentului înregistrat, de exemplu, urmărire, eroare, eveniment

- **Data.userAadObjectId** - identificatorul de utilizator unic global pentru un cont Microsoft Enterprise (dublură a Data.UserInfo.Id)

- **Data.UserInfo.Id** - identificatorul de utilizator unic global pentru un cont Microsoft Enterprise 

- **Data.UserInfo.MsaId** - identificatorul de utilizator unic global pentru un cont Microsoft consumator

- **Data.UserInfo.OMSTenantId** - entitatea găzduită la care este asociat abonamentul unui utilizator. Ne permite să clasificăm problemele și să identificăm dacă este o problemă pe scară largă sau una izolată la un set de utilizatori sau la o anumită entitate găzduită

- **Data.userPuid** - identificatorul de utilizator unic global pentru un cont Microsoft consumator (duplicat pentru Data.UserInfo.MsaId) 

- **Data.version** - versiunea serviciului (fișă de profil)

- **DeviceInfo_Id** - identificatorul de dispozitiv unic global pentru un dispozitiv

- **DeviceInfo_Make** - marca sistemului de operare

- **DeviceInfo_Model** - modelul dispozitivului

- **DeviceInfo_OsName** - numele dispozitivului OS

- **DeviceInfo_OsVersion** - versiunea sistemului de operare

- **DeviceInfo_SDKUid** – identifică în mod unic dispozitivul din perspectiva SDK-ului de telemetrie

- **NetworkCost** - indică costul/tipul rețelei (contorizată, contorizată peste limită etc.)

- **NetworkCountry** - codul de țară al expeditorului, pe baza adresei IP necurățată a clientului


#### <a name="officelivepersonacarduseractionsopenedpersonacard"></a>Office.LivePersonaCard.UserActions.OpenedPersonaCard

Înregistrat atunci când utilizatorul deschide un Card de persoană. Se utilizează pentru a observa anomalii critice în ratele de eroare la lansarea Cardului de persoană live.

Se colectează următoarele câmpuri:

- **Data.appContextId** - un ID generat aleatoriu utilizat pentru a identifica conturi diferite în aceeași aplicație

- **Data.AppInfo.Name** - numele serviciului utilizat (fișă de profil)

- **Data.bandwidthEstimateMbps** - estimarea efectivă a lățimii de bandă în Mbps

- **Data.cardCorrelationId** - identificatorul unic global pentru un card de persoană

- **Data.cardPersonaCorrelationId** - identificatorul unic global pentru o anumită persoană afișată într-un card

- **Data.clientCorrelationId** - identificatorul unic global pentru sesiunea aplicației

- **Data.clientType** - tipul de dispozitiv pe care rulează aplicația.

- **Data.eventId** - identificator de nume al evenimentului, de exemplu, „LivePersonaCardRenderedAction”

- **Data.exportName** - nume ușor de citit pentru oameni al evenimentului acțiune a utilizatorului, de exemplu,„OpenedPersonaCard”

- **Data.exportType** - categoria evenimentului pentru solicitarea de export GDPR

- **Data.externalAppSessionCorrelationId** - un Identificator unic global pentru ca aplicația să identifice toate fișele personale deschise în aceeași sub-sesiune

- **Data.feature** - utilizat pentru a grupa diverse evenimente cu aceeași caracteristică (fișă de profil)

- **Data.hasPersonalInsightRing** - detalii din Office sau LinkedIn pot fi disponibile pentru utilizator

- **Data.hostAppRing** - inelul prin care a fost distribuită aplicația

- **Data.immersiveProfileCorrelationId** - un identificator unic global pentru sesiunea de vizualizare profil extinsă

- **Data.OTelJS.Version** - versiune de OTel logger

- **Data.personaCorrelationId** - un Identificator unic global pentru personaje unice într-o sesiune

- **Data.properties** - metadate suplimentare colectate pentru fiecare eveniment, după cum urmează. *[Acest eveniment a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

    - **cardCorrelationId** - dublură a Data.appContextId de mai sus 
    - **cardPersonaCorrelationId** - dublură a Data.cardCorrelationId de mai sus
    - **consumerCorrelationId** - dublură a Data.clientCorrelationId de mai sus 
    - **networkEffectiveType** - tipul efectiv de conexiune de rețea, de exemplu, „slow-2g Online” pentru a identifica dacă utilizatorul este conectat la internet în timpul afișării cardului de persoană
    - **networkType** - tipul de conectivitate de rețea a dispozitivului utilizat
    - **roundTripEstimateMs** - timp de revenire efectiv estimat al conexiunii curente în milisecunde

- **Data.region** - regiunea geografică a serviciului de back-end a fișei de profil la care este conectat utilizatorul

- **Data.tenantAadObjectId** - entitatea găzduită la care este legat abonamentul unui utilizator. Ne permite să clasificăm problemele și să identificăm dacă este o problemă pe scară largă sau una izolată la un set de utilizatori sau la o anumită entitate găzduită

- **Data.type** - tipul evenimentului înregistrat, de exemplu, urmărire, eroare, eveniment

- **Data.userAadObjectId** - identificatorul de utilizator unic global pentru un cont Microsoft Enterprise (dublură a Data.UserInfo.Id)

- **Data.UserInfo.Id** - identificatorul de utilizator unic global pentru un cont Microsoft Enterprise 

- **Data.UserInfo.MsaId** - identificatorul de utilizator unic global pentru un cont Microsoft consumator

- **Data.UserInfo.OMSTenantId** - entitatea găzduită la care este asociat abonamentul unui utilizator. Ne permite să clasificăm problemele și să identificăm dacă este o problemă pe scară largă sau una izolată la un set de utilizatori sau la o anumită entitate găzduită

- **Data.userPuid** - identificatorul de utilizator unic global pentru un cont Microsoft consumator (duplicat pentru Data.UserInfo.MsaId) 

- **Data.version** - versiunea serviciului (fișă de profil)

- **Data.viewType** - definește tipul de fișă de profil afișată

- **Data.wasOpenedAsCompactCard** - utilizat pentru a identifica dacă fișa a fost deschisă ca vizualizare compactă inițial

- **NetworkCost** - indică costul/tipul rețelei (contorizată, contorizată peste limită etc.)

- **NetworkCountry** - codul de țară al expeditorului, pe baza adresei IP necurățată a clientului.

#### <a name="officemanageabilityclient-fetchpolicyprechecks"></a>Office.Manageability.Client Fetch.PolicyPreChecks

Telemetria critică pentru a urmări erorile\\succes pentru validarea pre-verificare a preluării politicii în cloud. ExitReason conține o hartă a enumeratorului pentru condiția de pre-verificare care a nu a reușit.

Se colectează următoarele câmpuri:

  - **Data.ExitReason** - valoarea enumeratorului care spune motivul ieșirii, dacă pre-verificarea nu a reușit

  - **Data.Log** - mesaj de jurnal particularizat care indică succesul sau eșecul pre-verificării

#### <a name="officemanageabilityclientfetchandapplypolicy"></a>Office.Manageability.Client.Fetch.AndApplyPolicy

Telemetrie critică pentru urmărirea erorilor\\succes pentru inițiere preluării politicii în cloud din aplicație. Motivul ieșirii conține o hartă a enumeratorului la motivul eșecului.

Se colectează următoarele câmpuri:

  - **Data.ExitReason** - valoarea enumeratorului care spune motivul ieșirii, dacă pre-verificarea nu a reușit

  - **Data.Log** - mesaj de jurnal particularizat care indică succesul sau eșecul pre-verificării

#### <a name="officeofficemobilepdfviewerpdffileopenmeasurements"></a>Office.OfficeMobile.PdfViewer.PdfFileOpenMeasurements

Acest eveniment este colectat pentru aplicația Office pentru iOS și înregistrează atunci când are loc o operațiune de deschidere de fișier. Colectăm aceste date pentru a asigura o performanță bună pentru deschiderea tuturor fișierelor din aplicație. 

Se colectează următoarele câmpuri:

- **Data_Doc_ActivationFQDN** - nume de domeniu al aplicației furnizor pentru un scenariu de activare a fișierelor (se înregistrează doar informațiile din aplicația primă parte).

- **Data_Doc_CreateTelemetryReason** - motivul de telemetrie pentru crearea PDF-ului. (Ex: Creare din scanare, utilizarea acțiunii „imagine la PDF”, utilizarea acțiunii „document la PDF” etc.)

- **Data_Doc_DownloadDurationms** - timp pentru a descărca un fișier PDF în cloud.

- **Data_Doc_DownloadEndTime** - marcă de timp pentru sfârșitul descărcării unui fișier în cloud.

- **Data_Doc_DownloadStartTime** - marcă de timp pentru începutul descărcării unui fișier în cloud.

- **Data_Doc_FileOpSessionID** - ID unic pentru o sesiune de document

- **Data_Doc_Location** - locația în care se află fișierul (local, ODSP, iCloud, aplicație de fișiere de la terți, wopi

- **Data_Doc_OpenCompletionTime** - marcă de timp pentru încheierea operațiunii de deschiderea a unui fișier PDF.

- **Data_Doc_OpenDurationms** - timp pentru a deschide un fișier PDF în milisecunde.

- **Data_Doc_OpenStartTime** - marcă de timp pentru începerea operațiunii de deschidere a unui fișier PDF.

- **Data_Doc_TelemetryReason** - motivul telemetriei pentru evenimentul deschis (de exemplu: deschidere din MRU sau navigare, activarea fișierelor, activarea protocolului etc.)

- **Doc_RenderDurationms** - timp de redare a unui fișier pdf


#### <a name="officeofficemobilepdfviewerpdffileoperations"></a>Office.OfficeMobile.PdfViewer.PdfFileOperations

Evenimentul este colectat pentru aplicația Office pentru Android. Acesta înregistrează când are loc o operațiune de deschidere, închidere sau salvare de .pdf și este utilizată pentru a înțelege și a acorda prioritate experienței de utilizator bazată pe informațiile despre operațiunea cu fișierul .pdf. Evenimentul ne permite să menținem operațiunile funcționale de deschidere, închidere și salvare a fișierului .pdf așa cum este de așteptat și să îmbunătățim performanța operațiunilor cu fișierele .pdf.

Se colectează următoarele câmpuri:

- **Data_Doc_FileOpSessionID** - ID unic pentru o sesiune de document

- **Data_ErrorCode** - eroare în caz de erori de deschidere a fișierelor/descărcare nereușită/descărcare anulată

- **Data_ErrorMessage** - cod relevant message-to-error

- **Data_FailureReason** - în cazul unei erori de deschidere, aceste enumerări definesc motivul erorii.

- **Data_FileGUID** - identificator global pentru fișierul care este generat aleatoriu

- **Data_FileLocation** - locația în care se află fișierul, de exemplu: local, ODSP, iCloud etc.

- **Data_FileOpenEntryPoint** - punct de intrare pentru deschiderea fișierului

- **Data_FileSize** - dimensiunea fișierului pe care are loc operațiunea

- **Data_NetworkRequestErrorResponse** - răspuns de eroare de rețea corespunzător codului de eroare.

- **Data_NetworkRequestStage** - etapa erorii în cazul descărcării fișierelor PDF din cloud.

- **Data_OpenMode** - modul în care a fost deschis fișierul PDF, de exemplu: 0: modul de vizualizare, 2: modul de semnare

- **Data_PageCount** - numărul de pagini din fișierul PDF.

- **Data_PasswordProtected** - marcaj care spune dacă fișierul este protejat prin parolă sau nu.

- **Data_ProviderApp** - deocamdată precizează aplicația furnizor, în cazul activării fișierului 

- **Data_ReadOnly** - marcaj care spune dacă fișierul este doar în citire sau nu.

- **Data_Result** - starea operațiunii efectuate, de exemplu: true: succes, false: eșec

- **Data_Type** - tipul de operațiune de fișier (deschidere, închidere sau salvare) 

#### <a name="officeofficemobilepdfviewerpdffileoperations"></a>Office.OfficeMobile.PdfViewer.PdfFileOperations

Evenimentul este colectat pentru aplicația Office pentru iOS. Acesta înregistrează când are loc o operațiune de deschidere, închidere sau salvare de .pdf și este utilizată pentru a înțelege și a acorda prioritate experienței de utilizator bazată pe informațiile despre operațiunea cu fișierul .pdf. Evenimentul ne permite să menținem operațiunile funcționale de deschidere, închidere și salvare a fișierului .pdf așa cum este de așteptat și să îmbunătățim performanța operațiunilor cu fișierele .pdf. 

- **Data_Doc_FileOpSessionID** - ID unic pentru o sesiune de document 

- **Data_ErrorCode** - eroare în caz de erori de deschidere a fișierelor/descărcare nereușită/descărcare anulată 

- **Data_ErrorMessage** - mesaj relevant la codul de eroare 

- **Data_FailureReason** - în cazul unei erori de deschidere, aceste enumerări definesc motivul eșecului. 

- **Data_FileGUID** - identificator global pentru fișierul care este generat aleatoriu

- **Data_FileLocation** - locația în care se află fișierul, de exemplu: local, ODSP, iCloud etc. 

- **Data_FileOpenEntryPoint** - punct de intrare pentru deschiderea fișierului 

- **Data_FileSize** - dimensiunea fișierului pe care are loc operațiunea 

- **Data_OpenMode** - modul în care a fost deschis fișierul PDF ( 0: modul de vizualizare 2: modul de semnare) 

- **Data_PageCount** - numărul de pagini din fișierul PDF.

- **Data_PasswordProtected** - marcaj care spune dacă fișierul este protejat prin parolă sau nu. 

- **Data_ProviderApp** - deocamdată precizează aplicația furnizor, în cazul activării fișierului 

- **Data_ReadOnly** - marcaj care precizează dacă fișierul este sau nu doar în citire.

- **Data_Result** - starea operațiunii efectuate ( de exemplu: true: succes, false: eșec) 

- **Data_Type** - tipul de operațiune de fișier (deschidere, închidere sau salvare)


#### <a name="officeonenoteandroidappnavigationnavigationuistatechanged-onenoteappnavigationnavigationuistatechanged-previous-name"></a>Office.OneNote.Android.App.Navigation.NavigationUIStateChanged, OneNote.App.Navigation.NavigationUIStateChanged *(nume anterior)*

Acest eveniment colectează semnalul critic utilizat pentru a asigura că utilizatorii OneNote pot naviga cu succes prin aplicație.  Telemetria se folosește pentru a asigura detectarea regresiei critice pentru aplicația OneNote și starea serviciilor. 

Se colectează următoarele câmpuri: 

- **IS_SPANNED** - indică dacă aplicația este într-un mod extins. Acest lucru este înregistrat în jurnal specific pentru dispozitive pliabile.

- **NEW_STATE** - indică starea aplicațiilor imediat după navigare

- **OLD_STATE** - indică starea aplicațiilor imediat înainte de navigare

#### <a name="officeonenoteandroidlenssdkofficelenslaunched-onenotelenssdkofficelenslaunched-previous-name"></a>Office.OneNote.Android.LensSDK.OfficeLensLaunched, OneNote.LensSDK.OfficeLensLaunched *(nume anterior)*

Acest eveniment colectează semnalul critic utilizat pentru a vă asigura că OfficeLens este lansat corect.  Telemetria se folosește pentru a asigura detectarea regresiei critice pentru aplicația OneNote și starea serviciilor. 

Se colectează următoarele câmpuri: 

- **CAPTURE_MODE** - indică modul în care a fost lansat OfficeLens.  Poate fi implicit, editare, Inserare rapidă sau import video.

- **ERROR_CODE** - indică codul de eroare de lansare în cazul în care a avut loc o eroare în timpul lansării.

- **IMAGE_COUNT** - indică numărul de imagini efectuate

- **LAUNCH_REASON** - indică fluxul în care a fost lansat OfficeLens. Poate fi peste ecranul de blocare sau prin intermediul opțiunilor Cameră sau Galerie din Note adezive sau prin OneNote Canvas etc.


#### <a name="officeonenoteandroidstickynotesnotecreated"></a>Office.OneNote.Android.StickyNotes.NoteCreated
 
Semnal critic utilizat pentru a monitoriza capacitatea utilizatorilor de Note adezive de a crea note în aplicație.   Telemetria se folosește pentru a asigura detectarea regresiei critice pentru aplicația OneNote și starea serviciilor. Dacă utilizatorii nu pot crea o notă, acest lucru va declanșa un incident de mare severitate.

Se colectează următoarele câmpuri:

- **IsExportable** - o semnalizare care indică dacă acest eveniment a fost rezultatul unei acțiuni a utilizatorului sau nu. Ar trebui setată la True, deoarece NoteCreated este o acțiune declanșată de utilizator.

- **NoteLocalId** - Identificator unic distinctiv atribuit unei note în momentul în care un utilizator creează nota în cadrul aplicației.

- **StickyNotes-SDKVersion** - număr de versiune care indică versiunea de Note Adezive folosită de utilizator. Ne permite să identificăm ce versiuni de produs afișează o problemă, astfel încât să o putem stabili corect ca prioritate.


#### <a name="officeonenoteandroidstickynotesnoteviewed"></a>Office.OneNote.Android.StickyNotes.NoteViewed

Semnal critic utilizat pentru a monitoriza capacitatea utilizatorilor de Note adezive de a vizualiza note în aplicație.  Telemetria se folosește pentru a asigura detectarea regresiei critice pentru aplicația OneNote și starea serviciilor. Dacă utilizatorii nu-și pot vizualiza notele, acest lucru va declanșa un incident cu severitate ridicată.

Se colectează următoarele câmpuri:

- **HasImages** - o semnalizare care indică dacă nota vizualizată conține imagini stocate.

- **IsExportable** - o semnalizare care indică dacă acest eveniment a fost rezultatul unei acțiuni a utilizatorului sau nu. Ar trebui setată la True, deoarece NoteViewed este o acțiune declanșată de utilizator.

- **NoteLocalId** - Identificator unic distinctiv atribuit unei note în momentul în care un utilizator creează nota în cadrul aplicației.

- **StickyNotes-SDKVersion** - număr de versiune care indică versiunea de Note Adezive folosită de utilizator. Ne permite să identificăm ce versiuni de produs afișează o problemă, astfel încât să o putem stabili corect ca prioritate.


#### <a name="officeonenotecanvasinkinkstrokelogger"></a>Office.OneNote.Canvas.Ink.InkStrokeLogger 

Acest eveniment este utilizat pentru a detecta și a diagnostica un bug de înaltă frecvență pe care îl întâlnește un utilizator în timp ce folosește caracteristica cerneală.  Acest lucru va fi utilizat pentru a determina modul cel mai potrivit pentru remedierea acestei probleme. 

Se colectează următoarele câmpuri:

- **CurrentCanvasZoomFactor** - factorul de zoom curent al pânzei.

- **CurrentNotebook** - identificator al blocnotesului activ curent.

- **CurrentPage** - identificator al paginii active curente.

- **CurrentSection** - identificator al secțiunii active curente.

- **DefaultCanvasZoomFactor** - factorul de zoom inclus al pânzei.

- **InkStrokeCount** - numărul total de lovituri cu cerneală de la ultimul jurnal.

- **InkStrokeWithLayerInkEffect** - număr urme de cerneală cu efect de cerneală strat de la ultimul jurnal.

- **InkStrokeWithoutPressureCount** - număr de lovituri cu cerneală fără presiune de la ultimul jurnal.

- **InkStrokeWithPencilInkEffect** - număr urme de cerneală cu efect de cerneală obișnuită de la ultimul jurnal.

- **InkStrokeWithTilt** - număr de lovituri cu cerneală cu înclinare de la ultimul jurnal.

#### <a name="officeonenotenavigationcreatepage"></a>Office.OneNote.Navigation.CreatePage

Semnal critic utilizat pentru a monitoriza capacitatea utilizatorilor OneNote de a crea pagini în OneNote.  Telemetria utilizată pentru a asigura detectarea regresiei critice pentru aplicația OneNote și starea serviciilor. Dacă utilizatorii nu pot crea o pagină, acest lucru va declanșa un incident de severitate înaltă.

Se colectează următoarele câmpuri:

- **IsAtSectionEnd** - indică dacă s-a creat sau nu o pagină nouă la sfârșitul secțiunii.

- **IsBlank** - indică dacă pagina nouă este necompletată sau creată cu un șablon.

- **IsRecentsView** - indică dacă o pagină este creată din recente sau nu.

- **NavView** - indică dacă o pagină este creată dintr-o vizualizare de navigare sau nu.

- **NoteType** - indică tipul unei pagini (notă rapidă, listă sau fotografie).

- **QuickNoteType** - indică tipul unei pagini (notă rapidă, listă sau fotografie).

- **RailState** - indică starea șinei de navigare OneNote atunci când se creează o pagină.

- **Trigger** - indică un punct de intrare acolo unde începe acțiunea de creare a paginii.

- **TriggerInfo** - indică informații suplimentare despre trigger.


#### <a name="officeonenotenavigationcreatesection"></a>Office.OneNote.Navigation.CreateSection

Semnal critic utilizat pentru a monitoriza capacitatea utilizatorilor OneNote de a crea secțiuni în OneNote.  Telemetria utilizată pentru a asigura detectarea regresiei critice pentru aplicația OneNote și starea serviciilor. Dacă utilizatorii nu pot crea o pagină, acest lucru va declanșa un incident de severitate înaltă.

Se colectează următoarele câmpuri

- **NotebookID** - identificator unic al unui blocnotes.

- **SectionID** - identificator unic al unei secțiuni create.

- **Trigger** - indică un punct de intrare acolo unde începe acțiunea de creare a secțiunii.

- **TriggerInfo** - indică informații suplimentare despre trigger.


#### <a name="officeonenotenavigationnavigate"></a>Office.OneNote.Navigation.Navigate

Semnal critic utilizat pentru a monitoriza capacitatea utilizatorilor OneNote de a naviga prin pagini în OneNote.  Telemetria utilizată pentru a asigura detectarea regresiei critice pentru aplicația OneNote și starea serviciilor. Dacă utilizatorii nu pot naviga, acest lucru va declanșa un incident de severitate înaltă.

Se colectează următoarele câmpuri:

- **FromNotebook** - identificator unic al unui blocnotes.

- **FromPage** - identificator unic al unei pagini.

- **FromSection** - identificator unic al unei secțiuni.

- **FromSectionGroup** - identificator unic al unui grup de secțiuni.

- **IsCurrentUserEduStudent** - indică dacă utilizatorul curent are rol de student într-un blocnotes de educație sau nu.

- **IsEduNotebook** - indică dacă pagina curentă este într-un blocnotes de educație sau nu.

- **IsEduNotebookReadOnlyPage** - indică dacă pagina curentă este o pagină doar în citire într-un blocnotes de educație sau nu.

- **ToNotebook** - identificator unic al unui blocnotes.

- **ToPage** - identificator unic al unei pagini.

- **ToSection** - identificator unic al unei secțiuni.

- **ToSectionGroup** - identificator unic al unui grup de secțiuni.


#### <a name="officeonenotenotebookmanagementcreatenotebook"></a>Office.OneNote.NotebookManagement.CreateNotebook

Semnal critic utilizat pentru a monitoriza capacitatea utilizatorilor OneNote de a crea blocnotesuri în OneNote.  Telemetria utilizată pentru a asigura detectarea regresiei critice pentru aplicația OneNote și starea serviciilor. Dacă utilizatorii nu pot crea blocnotesuri, acest lucru va declanșa un incident de severitate înaltă.

Se colectează următoarele câmpuri:
    
- **NotebookID** - identificator unic al unui blocnotes.


#### <a name="officeonenotenotebookmanagementopennotebook"></a>Office.OneNote.NotebookManagement.OpenNotebook

Semnal critic utilizat pentru a monitoriza capacitatea utilizatorilor OneNote de a deschide blocnotesuri în OneNote.  Telemetria utilizată pentru a asigura detectarea regresiei critice pentru aplicația OneNote și starea serviciilor. Dacă utilizatorii nu pot deschide blocnotesuri, acest lucru va declanșa un incident de severitate înaltă.

Se colectează următoarele câmpuri:

-  **NotebookID** - identificator unic al unui blocnotes.

    
#### <a name="officeonenotesearchsearch"></a>Office.OneNote.Search.Search

ID al semnalului critic utilizat pentru a monitoriza capacitatea utilizatorilor OneNote de a găsi informații în mii de pagini și blocnotesuri.   Telemetria utilizată pentru a asigura detectarea regresiei critice pentru aplicația OneNote și starea serviciilor. Dacă utilizatorii nu pot găsi informații în blocnotesuri, acest lucru va declanșa un incident de severitate înaltă.

Se colectează următoarele câmpuri:

- **PageSearchResultCount** - indică numărul de rezultate ale căutării găsite într-un mod de căutare a paginilor.

-  **PageTimeToFirstResultInMs** - indică intervalul de timp necesar pentru OneNote pentru a găsi prima potrivire într-un mod de căutare a paginilor.
    
-  **PageTimeToLastResultInMs** - indică intervalul de timp necesar pentru OneNote pentru a găsi ultima potrivire într-un mod de căutare a paginilor.

-  **PageTimeToMedianResultInMs** - indică mediana intervalului de timp necesar pentru ca OneNote să găsească toate potrivirile într-un mod de căutare a paginilor.

-  **SearchResultCount** - indică numărul de rezultate ale căutării.

-  **TagSearchResultCount** - indică numărul de rezultate ale căutării găsite într-un mod de căutare de etichete.

-  **TagTimeToFirstResultInMs** - indică intervalul de timp necesar pentru OneNote pentru a găsi prima potrivire într-un mod de căutare de etichete.

-  **TagTimeToLastResultInMs** - indică intervalul de timp necesar pentru ca OneNote să găsească prima potrivire într-un mod de căutare de etichete.

-  **TagTimeToMedianResultInMs** - indică mediana intervalului de timp necesar pentru ca OneNote să găsească toate potrivirile într-un mod de căutare de etichete.

-  **TimeToFirstResultInMs** - indică intervalul de timp necesar pentru OneNote pentru a găsi prima potrivire.

-  **TimeToLastResultInMs** - indică intervalul de timp necesar pentru OneNote pentru a găsi ultima potrivire.

-  **TimeToMedianResultInMs** - indică mediana intervalului de timp necesar pentru ca OneNote să găsească toate potrivirile.

### <a name="officeonenotesigscriticalerrorencountered"></a>Office.OneNote.SIGS.CriticalErrorEncountered

Acest eveniment capturează un semnal critic utilizat pentru a monitoriza starea de bună funcționare a Serviciului de integrare a semnalului (SIGS), conectându-se de fiecare dată când se întâlnește o eroare critică. Erorile critice pot bloca întregul SIGS, iar acesta ne va ajuta să găsim toate aceste probleme imediat ce sunt întâmpinate de utilizatori. 

Fără acesta, vom fi dependenți de utilizatori pentru a raporta problemele cu care se confruntă. Absența unei astfel de telemetrii ar cauza ca durata de procesare pentru astfel de probleme să fie mult mai lungă.

Se colectează următoarele câmpuri: 

- **ErrorCode** - codul problemei care a fost atins de utilizator.


#### <a name="officeonenotestickynotesnotecreated-on-ios-onenotestickynotesnotecreated-on-android"></a>Office.OneNote.StickyNotes.NoteCreated (pe iOS), OneNote.StickyNotes.NoteCreated (pe Android)

Acesta este un semnal critic utilizat pentru a monitoriza capacitatea utilizatorilor de Note adezive de a crea note în aplicație.  Telemetria se folosește pentru a asigura detectarea regresiei critice pentru aplicația OneNote și starea serviciilor. Dacă utilizatorii nu pot crea o notă, acest lucru va declanșa un incident de severitate înaltă.

Se colectează următoarele câmpuri:

- **NoteLocalId** - Identificator unic distinctiv atribuit unei note în momentul în care un utilizator creează nota în cadrul aplicației.

- **IsExportable** - o semnalizare care indică dacă acest eveniment a fost rezultatul unei acțiuni a utilizatorului sau nu. Ar trebui setată la True, deoarece NoteCreated este o acțiune declanșată de utilizator.

- **StickyNotes-SDKVersion** - număr de versiune care indică versiunea de Note Adezive folosită de utilizator. Ne permite să identificăm ce versiuni de produs afișează o problemă, astfel încât să o putem stabili corect ca prioritate.


#### <a name="officeonenotestickynotesnoteviewed-on-ios-onenotestickynotesnoteviewed-on-android"></a>Office.OneNote.StickyNotes.NoteViewed (pe iOS), OneNote.StickyNotes.NoteViewed (pe Android)

Acesta este un semnal critic utilizat pentru a monitoriza capacitatea utilizatorilor de Note adezive de a crea note în aplicație.  Telemetria se folosește pentru a asigura detectarea regresiei critice pentru aplicația OneNote și starea serviciilor. Dacă utilizatorii nu pot crea o notă, acest lucru va declanșa un incident de severitate înaltă.

Se colectează următoarele câmpuri:

- **HasImages** - o semnalizare care indică dacă nota vizualizată conține imagini stocate.

- **IsExportable** - o semnalizare care indică dacă acest eveniment a fost rezultatul unei acțiuni a utilizatorului sau nu. Ar trebui setată la True, deoarece NoteViewed este o acțiune declanșată de utilizator.

- **NoteLocalId** - Identificator unic distinctiv atribuit unei note în momentul în care un utilizator creează nota în cadrul aplicației.

- **StickyNotes-SDKVersion** - număr de versiune care indică versiunea de Note Adezive folosită de utilizator. Ne permite să identificăm ce versiuni de produs afișează o problemă, astfel încât să o putem stabili corect ca prioritate.


#### <a name="officeonenotestoragenotebooksyncresult"></a>Office.OneNote.Storage.NotebookSyncResult
 
Acest eveniment înregistrează rezultatul sincronizării blocnotesului. Este utilizat pentru a afla câte ținte de sincronizare unice există atunci când se calculează scorul de sincronizare OneNote.
 
Se colectează următoarele câmpuri

- **CachedError_Code** - un cod numerotat sau alfanumeric utilizat pentru a determina natura erorii memorate în cache și/sau motivul pentru care aceasta s-a produs
    
- **CachedError_Description** - o descriere a erorii memorate în cache

- **CachedError_Tag** - indică unde în cod se generează eroarea memorată în cache

- **CachedError_Type** - tipul erorii memorate în cache, de exemplu Win32Error etc.

- **ExecutionTime** - timp în milisecunde necesare pentru a reproduce blocnotesul

- **Gosid** - ID al spațiului de obiecte global

- **IdentityType** - tip de identitate, de exemplu Windows Live, Org ID etc.

- **InitialReplicationInSession** - dacă această reproducere este sau nu prima reproducere a blocnotesului după deschidere

- **IsBackgroundSync** - este o sincronizare de fundal sau nu

- **IsCachedErrorSuppressed** - este eroarea memorată în cache suprimată sau nu

- **IsCachedErrorUnexpected** - este eroarea memorată în cache neașteptată sau nu

- **IsNotebookErrorSuppressed** - este eroarea de sincronizare la nivel de blocnotes suprimată sau nu

- **IsNotebookErrorSuppressed** - este eroarea de sincronizare la nivel de blocnotes neașteptată sau nu

- **IsSectionErrorSuppressed** - este eroarea de sincronizare a secțiunii suprimată sau nu

- **IsSectionErrorUnexpected** - este eroarea de sincronizare a secțiunii neașteptată sau nu

- **IsUsingRealtimeSync** - sincronizarea blocnotesului utilizează sincronizarea modernă a conținutului paginilor sau nu

- **LastAttemptedSync** - marca de timp când a încercat să fie sincronizat blocnotesul ultima dată

- **LastBackgroundSync** - marca de timp când s-a încercat cea mai recentă sincronizare de fundal

- **LastNotebookViewedDate** - data când a fost vizualizat ultima dată blocnotesul

- **LastSuccessfulSync** - marca de timp când s-a sincronizat cu succes blocnotesul înainte

- **NeedToRestartBecauseOfInconsistencies** - trebuie să reporniți sincronizarea din cauza inconsecvențelor sau nu

- **NotebookErrorCode** - cod de eroare sincronizare la nivel de blocnotes salvat în spațiul grafic din blocnotes

- **NotebookId** - ID blocnotes

- **NotebookType** - tip blocnotes

- **ReplicatingAgainBecauseOfInconsistencies** - sincronizarea repornește din cauza inconsecvențelor sau nu

- **SectionError_Code** - un cod numerotat sau alfanumeric utilizat pentru a determina natura erorii de sincronizare a secțiunii și/sau motivul pentru care aceasta s-a produs

- **SectionError_Description** - o descriere a erorii de sincronizare a secțiunii

- **SectionError_Tag** - indică unde în cod se generează eroarea de sincronizare a secțiunii

- **SectionError_Type** - tipul erorii de sincronizare a secțiunii, de exemplu Win32Error etc.

- **Success** - s-a sincronizat blocnotesul cu succes sau nu

- **SyncDestinationType** - tipul destinației de sincronizare, adică OneDrive sau SharePoint Online

- **SyncId** - un număr unic pentru fiecare sincronizare de blocnotes

- **SyncWasFirstInSession** - este acestă sincronizare prima sincronizare din sesiunea curentă

- **SyncWasUserInitiated** - este această sincronizare inițiată de utilizator sau nu

- **TenantId** - ID-ul entității găzduite SharePoint

- **TimeSinceLastAttemptedSync** - perioada de la ultima încercare de sincronizare a blocnotesului

- **TimeSinceLastSuccessfulSync** - perioada de la ultima sincronizare de blocnotes reușită


#### <a name="officeonenotesystemapplifecycleapplaunch"></a>Office.OneNote.System.AppLifeCycle.AppLaunch

Semnal critic utilizat pentru a ne asigura că utilizatorii OneNote pot lansa cu succes aplicația. Telemetria se folosește pentru a asigura detectarea regresiei critice pentru aplicația OneNote și starea serviciilor. Dacă utilizatorii nu pot lansa aplicația în fereastra noastră de performanță, acest lucru va declanșa un incident de severitate înaltă.

Se colectează următoarele câmpuri: Niciunul

#### <a name="officeoutlookdesktopaccountconfigurationcreateaccountresult"></a>Office.Outlook.Desktop.AccountConfiguration.CreateAccountResult

Rezultatul adăugării unui cont la Outlook într-un profil nou, din Office Backstage sau din caseta de dialog Setări cont. Datele sunt monitorizate în mod activ pentru a garanta că nu vedem valori maxime în erori. De asemenea, vom analiza datele pentru a găsi zone care necesită îmbunătățiri. Dorim să îmbunătățim această rata de succes cu ocazia fiecărei versiuni.

Se colectează următoarele câmpuri:

  - **AccountCreationResult** - rezultatul (succes, eroare, anulare etc.) adăugării contului în Outlook.

  - **AccountCreationTime** - timpul necesar pentru a încerca crearea unui cont

  - **AccountInfoSource** - sursă setări cont (de ex. AutoDiscover, GuessSmart, AutoDetect etc.)

  - **AccountType** - tipul de cont configurat.

  - **HashedEmailAddress** - adresa de e-mail cu cod hash

  - **ShowPasswordPageFlightEnabled** - indicatorul care arată dacă este activată ediția flight ShowPopImapPasswordPage

#### <a name="officeoutlookdesktopaccountconfigurationrepairaccountresult"></a>Office.Outlook.Desktop.AccountConfiguration.RepairAccountResult

Rezultatul reparării unui cont sau al modificării setărilor complexe de cont. Datele sunt monitorizate în mod activ pentru a garanta că nu vedem valori maxime în erori. De asemenea, vom analiza datele pentru a găsi zone care necesită îmbunătățiri. Întrucât aceasta este o experiență nouă (refactorizată), dorim să ne asigurăm că am înțeles corect.

Se colectează următoarele câmpuri:

  - **AccountInfoSource** - sursă de informații cont pentru contul utilizat pentru a încerca repararea

  - **AccountType** - tipul de cont pentru care s-a încercat repararea contului

  - **HashedEmailAddress** - adresa de e-mail cu cod hash

  - **ManualRepairRequested** - indicatorul care arată dacă a fost solicitată repararea manuală

  - **Result** - rezultatul încercării de a repara contul. De exemplu: „Success” sau „Fail\_SaveChangesToAccount”

#### <a name="officeoutlookdesktopaccountconfigurationupdatepasswordresult"></a>Office.Outlook.Desktop.AccountConfiguration.UpdatePasswordResult

Rezultatul actualizării parolei unui cont din lista verticală de Setări cont. Datele sunt monitorizate în mod activ pentru a garanta că nu vedem valori maxime în erori. De asemenea, vom analiza datele pentru a găsi zone care necesită îmbunătățiri. Întrucât aceasta este o experiență nouă (refactorizată), dorim să ne asigurăm că am înțeles corect.

Se colectează următoarele câmpuri:

  - **AccountType** - tipul de cont pentru care s-a încercat actualizarea parolei

  - **HashedEmailAddress** - adresa de e-mail cu cod hash

  - **Result** - rezultatul încercării de a actualiza parola. De exemplu:: „Success” sau „Fail\_AllowLessSecureAppsDisabled”


#### <a name="officeoutlookdesktopstorescreatenewstore"></a>Office.Outlook.Desktop.Stores.CreateNewStore

Colectează rezultatul de creare a unui magazin nou (cu tip și versiune), precum și codul rezultat. Monitorizăm în mod activ acest eveniment pentru a urmări capacitatea în bună stare a unui utilizator de a sincroniza și stoca e-mailuri local, de a arhiva e-mailuri (într-un fișier PST) sau a utiliza Grupuri.

Se colectează următoarele câmpuri:

  - **Activitate HVA standard** cu nicio sarcină particularizată

  - **StoreType** - tipul de magazin creat OST/PST/NST

  - **StoreVersion** - versiunea de magazin creată Small/Large/Tardis

#### <a name="officeoutlookmacaccountaddworkflow"></a>Office.Outlook.Mac.AccountAddWorkflow

Rezultatul adăugării unui cont în Outlook. Datele sunt monitorizate pentru a garanta că nu vedem valori maxime în erori. De asemenea analizăm datele pentru a găsi zone care necesită îmbunătățiri. Dorim să îmbunătățim această rata de succes cu ocazia fiecărei versiuni. 

Se colectează următoarele câmpuri:

- **AccountConfigMethod** - metoda de configurare a contului

- **AccountType** - tipul de cont configurat.

- **AccountWorkflowSession** - sesiunea în care se încearcă fluxul de lucru pentru cont

- **SessionDuration** - durata sesiunii 

- **ThreadID** - identificator pentru fir


#### <a name="officeoutlookmacaccountonboardingflow"></a>Office.Outlook.Mac.AccountOnboardingFlow

Rezultatul adăugării unui cont în Outlook utilizând noua experiență de configurare a conturilor. Datele sunt monitorizate pentru a garanta că nu vedem valori maxime în erori. De asemenea analizăm datele pentru a găsi zone care necesită îmbunătățiri. Dorim să îmbunătățim această rata de succes cu ocazia fiecărei versiuni. 

Se colectează următoarele câmpuri:

- **AccountConfigAutoSignIn** - configurarea automată a contului setată de administrator

- **AccountConfigDomain** - domeniu specificat în timpul configurării contului 

- **AccountConfigEntryPoint** - punct de intrare în care utilizatorul a introdus configurația contului 

- **AccountConfigErrorCode** - cod de eroare întâlnit în timpul configurării contului 

- **AccountConfigErrorString** - eroare întâlnită în timpul configurării contului

- **AccountConfigMethod** - metodă de configurare a contului

- **AccountConfigPhase** - etapa curentă a fluxului de lucru pentru configurarea contului

- **AccountConfigPhaseFrom** - etapa inițială a fluxului de lucru pentru configurarea contului 

- **AccountConfigPhaseTo** - ultima etapă a fluxului de lucru pentru configurarea contului 

- **AccountType** - tip de cont configurat

- **AccountWorkflowSession** - sesiunea în care se încearcă fluxul de lucru pentru cont

- **SessionDuration** - durata sesiunii


#### <a name="officeoutlookmacdeleteaccountusage"></a>Office.Outlook.Mac.DeleteAccountUsage

Rezultatul ștergerii unui cont în Outlook. Datele sunt monitorizate pentru a garanta că nu vedem valori maxime în erori. De asemenea analizăm datele pentru a găsi zone care necesită îmbunătățiri. Dorim să îmbunătățim această rata de succes cu ocazia fiecărei versiuni. 

Se colectează următoarele câmpuri:

- **AccountType** - tip de cont configurat

- **AccountID** - identificator cont

- **DeprovisionAccount** - indică dacă este eliminat contul din server

- **IsFastDelete** - indică dacă contul este șters pe firul de fundal

#### <a name="officepowerpointdocoperationclose"></a>Office.PowerPoint.DocOperation.Close

Colectat când prezentările PowerPoint sunt oprite. Acesta conține informațiile necesare pentru a investiga și a diagnostica corect problemele care au loc prin procesul de închidere care implică persistența și sincronizarea datelor utilizatorului. Microsoft utilizează aceste date pentru a garanta faptul că închiderea funcționează conform așteptărilor, iar conținutul utilizatorilor a persistat cu succes.

Se colectează următoarele câmpuri:

  - **Data\_AddDocTelemetryResult:long -** această intrare în jurnal are toate datele de telemetrie necesare pentru documente (câmpurile Data\_Doc\_\*)? Dacă nu, de ce?

  - **Data\_AutoSaveDisabledReasons:string -** set de valori predefinite privind motivul pentru care salvarea automată a fost dezactivată de la acest document? (Eroare de îmbinare, Salvare eroare, Politică de grup etc.)

  - **Data\_CloseReason:long -** cum s-a efectuat închiderea? Închideți documentul? Închideți aplicația?

  - **Data\_CppUncaughtExceptionCount:long -** număr de excepții netratate

  - **Data\_DetachedDuration:long -** timpul cât activitatea a fost detașată/nu a rulat

  - **Data\_Doc\_AccessMode:long -** cum a fost deschis acest document (doar în citire | citire-scriere)

  - **Data\_Doc\_AssistedReadingReasons:long -** set predefinit de valori pentru care documentul a fost deschis în modul de citire asistată

  - **Data_Doc_AsyncOpenKind:long –** indică dacă s-a deschis o versiune memorată în cache a documentului cloud și ce logică de reîmprospătare asincronă s-a folosit.

  - **Data\_Doc\_ChunkingType:long -** cum este stocat documentul în SharePoint

  - **Data\_Doc\_EdpState:long -** starea Enterprise Data Protection a documentului

  - **Data\_Doc\_Ext:string -** extensia documentului

  - **Data\_Doc\_Extension:string -** extensia documentului

  - **Data\_Doc\_FileFormat:long -** set predefinit de valori pentru formatul fișierului (mai granular decât extensia)

  - **Data\_Doc\_Fqdn:string -** unde este stocat documentul (SharePoint.com, live.net), disponibil numai pentru domeniile Office 365

  - **Data\_Doc\_FqdnHash:string -** codul hash al locului unde este stocat documentul

  - **Data\_Doc\_IdentityTelemetryId:string -** GUID unic al utilizatorului

  - **Data\_Doc\_IdentityUniqueId:string -** identificator unic al identității folosite pentru acțiunea Documente partajate

  - **Data\_Doc\_IOFlags:long -** bitmask pentru diferite semnalizări legate de IO pentru un anumit document

  - **Data\_Doc\_IrmRights:long -** set predefinit de valori pentru tipul de Information Rights Management aplicat pentru acest document (Redirecționare, Răspuns, SecureReader, Editare etc.)

  - **Data\_Doc\_IsCloudCollabEnabled:bool -** true dacă antetul „IsCloudCollabEnabled” a fost deja primit dintr-o solicitare OPTIONS.

  - **Data\_Doc\_IsIncrementalOpen:bool -** documentul a fost deschis incremental (caracteristică nouă care deschide documentul fără să-l descarce în totalitate)

  - **Data\_Doc\_IsOcsSupported:bool -** dacă documentul acceptă elaborarea în comun folosind noul serviciu OCS

  - **Data\_Doc\_IsOpeningOfflineCopy:bool -** verifică dacă documentul este deschis din memoria cache locală

  - **Data\_Doc\_IsSyncBacked:bool -** verifică dacă documentul este deschis din folderul care folosește aplicația de sincronizare inversă OneDrive

  - **Data\_Doc\_Location:long -** set predefinit de valori privind locul de stocare a documentului (Local, SharePoint, WOPI, Rețea etc.)

  - **Data\_Doc\_LocationDetails:long -** set predefinit de valori privind locația mai detaliată (folderul Temp, folderul de descărcări, Documente OneDrive, Imagini OneDrive etc.)

  - **Data\_Doc\_NumberCoAuthors:long -** numărul de coautori la momentul deschiderii unui document

  - **Data\_Doc\_PasswordFlags:long -** set predefinit de valori privind modul în care documentul este criptat cu o parolă (Fără, parolă pentru citire, parolă pentru editare)-

  - **Data\_Doc\_ReadOnlyReasons:long -** set predefinit de valori privind motivul pentru care acest document a fost marcat doar în citire (blocat pe server, document final, protejat prin parolă pentru editare etc.)

  - **Data\_Doc\_ResourceIdHash:string -** codul hash al identificatorului de resurse pentru documentele stocate în cloud

  - **Data_Doc_RtcType -**  indică modul în care a fost configurat canalul în timp real (RTC) pentru fișierul curent (dezactivat, neacceptat, la cerere, activat permanent etc.).

  - **Data\_Doc\_ServerDocId:string –** identificatorul imutabil pentru documentele stocate în cloud

  - **Data\_Doc\_ServerProtocol:long -** set predefinit de valori privind protocolul folosit în comunicarea cu serverul (Http, Cobalt, WOPI etc.)

  - **Data\_Doc\_ServerType:long -** set predefinit de valori privind tipul serverului (SharePoint, DropBox, WOPI)

  - **Data\_Doc\_ServerVersion:long -** dacă serverul se bazează pe Office14, Office15, Office 16

  - **Data\_Doc\_SessionId:long -** GUID generat care identifică instanța documentului din aceeași sesiune de proces

  - **Data\_Doc\_SharePointServiceContext:string -** un șir opac, de obicei GridManagerID.FarmID. Util pentru corelarea jurnalului de la client și de pe server

  - **Data\_Doc\_SizeInBytes:long -** dimensiunea documentului în octeți

  - **Data\_Doc\_SpecialChars:long -** Bitmask ce arată caracterele speciale din adresa URL sau calea documentului

  - **Data\_Doc\_StorageProviderId:string -** șir care identifică furnizorul de stocare al documentului, precum „DropBox”

  - **Data\_Doc\_StreamAvailability:long -** set predefinit de valori privind starea șirului de document (disponibil, dezactivat definitiv, indisponibil)

  - **Data\_Doc\_UrlHash:string -** codul hash pentru adresa URL completă a documentelor stocate în cloud

  - **Data\_Doc\_UsedWrsDataOnOpen:bool -** true dacă fișierul a fost deschis incremental folosind datele WRS prememorate în cache pentru gazdă

  - **Data\_Doc\_WopiServiceId:string -** identificatorul serviciului WOPI, de ex. „Dropbox”

  - **Data\_DocHasStorage:bool -** are acest document spațiu de stocare local?

  - **Data\_fLifeguarded:bool –** documentul a fost vreodată protejat (caracteristică pentru a remedia automat erorile din documente, fără intervenția utilizatorului)?

  - **Data\_IsDocAutoSaveable:bool -** poate fi prezentarea salvată automat?

  - **Data\_IsDocDirty:bool -** are prezentarea modificări care nu sunt încă salvate?

  - **Data\_IsNewDoc:bool -** este un document nou sau existent

  - **Data\_IsRecoveredDoc:bool -** este documentul recuperat? (Dacă sesiunea anterioară a căzut, afișăm panoul de recuperare a documentului la următoarea sesiune)

  - **Data\_NewDocDiscarded:bool -** a fost eliminată noua prezentare fără a fi salvată

  - **Data\_OCSClosingDlgCanceled:bool -** dacă încărcarea este în așteptare pe OCS în timp ce utilizatorul închide documentul, apare o casetă de dialog care îndeamnă utilizatorul să aștepte. Ce opțiune a ales utilizatorul?

  - **Data\_OCSClosingDlgExpired:bool -** a expirat caseta de dialog (după 1 minut) singură?

  - **Data\_OCSClosingStatus:long -** care este starea finală a OCS (În CSI, Poate fi închis, În tranziție OCS, În tranziție CSI etc.)

  - **Data\_OCSClosingWaitDurationMS:long -** cât timp a trebuit să aștepte utilizatorul ca să se încarce OCS

  - **Data\_OCSHandleTransitionResult:long -** set de valori predefinite al rezultatului tranziției efectuate la închidere (S-a încercat deja, Continuați pentru a închide etc.)

  - **Data\_ServerDocId:string -** GUID pentru a identifica în mod unic un document

  - **Data\_StopwatchDuration:long –** timpul total al activității

  - **Data\_UserContinuedZRTClose:bool -** după afișarea casetei de dialog la închidere, a selectat utilizatorul „Continuare” pentru a închide?

#### <a name="officepowerpointdocoperationnewdocument"></a>Office.PowerPoint.DocOperation.NewDocument

Colectat când PowerPoint creează o prezentare nouă.  Include măsurători de eroare și succes și performanță.

Aceste informații sunt utilizate pentru a garanta că putem crea cu succes fișiere fără degradarea performanței.

Se colectează următoarele câmpuri:

  - **NewDocumentType** - dacă noul document este creat pornind de la un șablon sau este creat de la zero?

  - **FLifeguarded** - este documentul protejat (caracteristică ce restabilește starea unui document deteriorat fără a adresa solicitări utilizatorului)

#### <a name="officepowerpointdocoperationopencompleteprotocol"></a>Office.PowerPoint.DocOperation.OpenCompleteProtocol

Colectat când PowerPoint deschide prezentări. Acesta conține informațiile necesare pentru a investiga și a diagnostica corect problemele care au loc până la etapele finale ale procesului de deschidere.

Microsoft utilizează aceste date pentru a garanta că această caracteristică funcționează conform așteptărilor și că nu există nicio degradare în ceea ce privește deschiderea prezentărilor.

Se colectează următoarele câmpuri:

  - **Data\_AntiVirusScanMethod:long -** setul predefinit de valori de tipul antivirusului scanat (IOAV, AMSI, Fără etc.)

  - **Data\_AntiVirusScanStatus:long -** setul predefinit de valori pentru scanarea antivirus care apare pentru fiecare document deschis (NoThreatsDetected, Failed, MalwareDetected etc.)

  - **Data\_CloseAndReopen:bool -** a fost acest document închis și redeschis?

  - **Data\_DetachedDuration:long -** timpul cât activitatea a fost detașată/nu a rulat

  - **Data\_Doc\_AccessMode:long -** cum a fost deschis acest document (doar în citire | citire-scriere)

  - **Data\_Doc\_AssistedReadingReasons:long -** set predefinit de valori pentru care documentul a fost deschis în modul de citire asistată

  - **Data_Doc_AsyncOpenKind:long –** indică dacă s-a deschis o versiune memorată în cache a documentului cloud și ce logică de reîmprospătare asincronă s-a folosit.

  - **Data\_Doc\_ChunkingType:long -** cum este stocat documentul în SharePoint

  - **Data\_Doc\_EdpState:long -** starea Enterprise Data Protection a documentului

  - **Data\_Doc\_Ext:string -** extensia documentului

  - **Data\_Doc\_Extension:string -** extensia documentului

  - **Data\_Doc\_FileFormat:long -** set predefinit de valori pentru formatul fișierului (mai granular decât extensia)

  - **Data\_Doc\_Fqdn:string -** unde este stocat documentul (SharePoint.com, live.net), disponibil numai pentru domeniile Office 365

  - **Data\_Doc\_FqdnHash:string -** codul hash al locului unde este stocat documentul

  - **Data\_Doc\_IdentityTelemetryId:string -** GUID unic al utilizatorului

  - **Data\_Doc\_IdentityUniqueId:string -** identificator unic al identității folosite pentru acțiunea Documente partajate

  - **Data\_Doc\_IOFlags:long -** bitmask pentru diferite semnalizări legate de IO pentru un anumit document

  - **Data\_Doc\_IrmRights:long -** set predefinit de valori pentru tipul de Information Rights Management aplicat pentru acest document (Redirecționare, Răspuns, SecureReader, Editare etc.)

  - **Data\_Doc\_IsCloudCollabEnabled:bool -** true dacă antetul „IsCloudCollabEnabled” a fost deja primit dintr-o solicitare OPTIONS.

  - **Data\_Doc\_IsIncrementalOpen:bool -** documentul a fost deschis incremental (caracteristică nouă care deschide documentul fără să-l descarce în totalitate)

  - **Data\_Doc\_IsOcsSupported:bool -** dacă documentul acceptă elaborarea în comun folosind noul serviciu OCS

  - **Data\_Doc\_IsOpeningOfflineCopy:bool -** documentul este deschis din memoria cache locală?

  - **Data\_Doc\_IsSyncBacked:bool -** dacă documentul este deschis din folderul care folosește aplicația de sincronizare inversă OneDrive

  - **Data\_Doc\_Location:long -** set predefinit de valori privind locul de stocare a documentului (Local, SharePoint, WOPI, Rețea etc.)

  - **Data\_Doc\_LocationDetails:long -** set predefinit de valori privind locația mai detaliată (folderul Temp, folderul de descărcări, Documente OneDrive, Imagini OneDrive etc.)

  - **Data\_Doc\_NumberCoAuthors:long -** numărul de coautori la momentul deschiderii unui document

  - **Data\_Doc\_PasswordFlags:long -** set predefinit de valori privind modul în care documentul este criptat cu o parolă (Fără, parolă pentru citire, parolă pentru editare)-

  - **Data\_Doc\_ReadOnlyReasons:long -** set predefinit de valori privind motivul pentru care acest document a fost marcat doar în citire (blocat pe server, document final, protejat prin parolă pentru editare etc.)

  - **Data\_Doc\_ResourceIdHash:string -** codul hash al identificatorului de resurse pentru documentele stocate în cloud

  - **Data_Doc_RtcType -**  indică modul în care a fost configurat canalul în timp real (RTC) pentru fișierul curent (dezactivat, neacceptat, la cerere, activat permanent etc.).

  - **Data\_Doc\_ServerDocId:string –** identificatorul imutabil pentru documentele stocate în cloud

  - **Data\_Doc\_ServerProtocol:long -** set predefinit de valori privind protocolul folosit în comunicarea cu serverul (Http, Cobalt, WOPI etc.)

  - **Data\_Doc\_ServerType:long -** set predefinit de valori privind tipul serverului (SharePoint, DropBox, WOPI)

  - **Data\_Doc\_ServerVersion:long -** dacă serverul se bazează pe Office14, Office15, Office 16

  - **Data\_Doc\_SessionId:long -** GUID generat care identifică instanța documentului din aceeași sesiune de proces

  - **Data\_Doc\_SharePointServiceContext:string -** un șir opac, de obicei GridManagerID.FarmID. Util pentru corelarea jurnalelor de la client și de pe server

  - **Data\_Doc\_SizeInBytes:long -** dimensiunea documentului în octeți

  - **Data\_Doc\_SpecialChars:long -** Bitmask ce arată caracterele speciale din adresa URL sau calea documentului

  - **Data\_Doc\_StorageProviderId:string -** șir care identifică furnizorul de stocare al documentului, precum „DropBox”

  - **Data\_Doc\_StreamAvailability:long -** set predefinit de valori privind starea șirului de document (disponibil, dezactivat definitiv, indisponibil)

  - **Data\_Doc\_UrlHash:string -** codul hash pentru adresa URL completă a documentelor stocate în cloud

  - **Data\_Doc\_UsedWrsDataOnOpen:bool -** true dacă fișierul a fost deschis incremental folosind datele WRS prememorate în cache pentru gazdă

  - **Data\_Doc\_WopiServiceId:string -** identificatorul serviciului WOPI, de ex. „Dropbox”

  - **Data\_ExecutionCount:long -** de câte ori am executat protocolul IncOpen înainte de a executa acest protocol (OpenComplete)

  - **Data\_FailureComponent:long -** set predefinit de valori privind componenta care a cauzat nereușita protocolului (Conflict, CSI, Internă etc.)

  - **Data\_FailureReason:long –** set predefinit de valori privind motivul nereușitei (FileIsCorrupt, BlockedByAntivirus etc.)

  - **Data_FullDownloadRoundTripCount:long -** numărul de trasee dus-întors la server care au fost necesare pentru a descărca întregul document.
  
  - **Data_IsProtocolRunInIncOpenMode:bool -** dacă protocolul a fost executat pentru o descărcare incrementală, care este o descărcare în care s-au descărcat părți ale documentului după o afișare inițială către utilizator.

  - **Data\_MethodId:long -** în plan intern, ce linie de cod a fost executată ultima

  - **Data\_StopwatchDuration:long –** timpul total al activității

  - **Data\_TimeToEdit:long -** timpul necesar pentru ca documentul să devină editabil

  - **Data\_TimeToView:long -** timpul necesar pentru ca primul diapozitiv al documentului să fie redat

  - **Data\_UnhandledException:bool -** orice excepție nativă netratată?

#### <a name="officepowerpointdocoperationsave"></a>Office.PowerPoint.DocOperation.Save

Colectată ori de câte ori PowerPoint efectuează o salvare utilizând calea de cod modernă. Include tipul de rezultat, succes sau eșec, al măsurătorilor performanței de salvare și metadatele relevante ale documentului.  Erorile de salvare pot duce la pierderea unor date. Microsoft utilizează aceste date pentru a garanta faptul că această caracteristică funcționează conform așteptărilor, iar conținutul utilizatorilor a persistat cu succes.

Se colectează următoarele câmpuri:

  - **Data\_AddDocTelemetryResult:long -** această intrare în jurnal are toate datele de telemetrie necesare pentru documente (câmpurile Data\_Doc\_\*)? Dacă nu, de ce?

  - **Data\_BeforeSaveEvent:long -** timpul necesar pentru a ridica evenimentul Document înainte de salvare

  - **Data\_CheckDownRevSaveTimeMS:long -** timpul necesar pentru a verifica revizuirea

  - **Data\_CheckMacroSaveTimeMS:long -** timpul necesar pentru a salva macrocomenzi

  - **Data\_ClearAutoSaveTimeMS:long -** timpul necesar pentru a elimina semnalizarea Salvare automată

  - **Data\_ClearDirtyFlagTimeMS:long -** timpul necesar pentru a elimina semnalizarea cu erori a documentului

  - **Data\_CloneDocumentTimeMS:long -** timpul necesar pentru clona documentul înainte de a începe salvarea

  - **Data\_CommitTransactionTimeMS:long -** timpul necesar pentru a valida tranzacția de salvare

  - **Data\_CppUncaughtExceptionCount:long -** excepții native neprinse în timp ce rula activitatea

  - **Data\_DetachedDuration:long -** timpul cât activitatea a fost detașată/nu a rulat

  - **Data\_Doc\_AccessMode:long -** cum a fost deschis acest document (doar în citire | citire-scriere)

  - **Data\_Doc\_AssistedReadingReasons:long -** set predefinit de valori pentru care documentul a fost deschis în modul de citire asistată

  - **Data_Doc_AsyncOpenKind:long –** indică dacă s-a deschis o versiune memorată în cache a documentului cloud și ce logică de reîmprospătare asincronă s-a folosit.

  - **Data\_Doc\_ChunkingType:long -** cum este stocat documentul în SharePoint

  - **Data\_Doc\_EdpState:long -** starea Enterprise Data Protection a documentului

  - **Data\_Doc\_Ext:string -** extensia documentului

  - **Data\_Doc\_Extension:string -** extensia documentului

  - **Data\_Doc\_FileFormat:long -** set predefinit de valori pentru formatul fișierului (mai granular decât extensia)

  - **Data\_Doc\_Fqdn:string -** unde este stocat documentul (SharePoint.com, live.net), disponibil numai pentru domeniile Office 365

  - **Data\_Doc\_FqdnHash:string -** codul hash al locului unde este stocat documentul

  - **Data\_Doc\_IdentityTelemetryId:string -** GUID unic al utilizatorului

  - **Data\_Doc\_IdentityUniqueId:string -** identificator unic al identității folosite pentru acțiunea Documente partajate

  - **Data\_Doc\_IOFlags:long -** bitmask pentru diferite semnalizări legate de IO pentru un anumit document

  - **Data\_Doc\_IrmRights:long -** set predefinit de valori pentru tipul de Information Rights Management aplicat pentru acest document (Redirecționare, Răspuns, SecureReader, Editare etc.)

  - **Data\_Doc\_IsCloudCollabEnabled:bool -** true dacă antetul „IsCloudCollabEnabled” a fost deja primit dintr-o solicitare OPTIONS.

  - **Data\_Doc\_IsIncrementalOpen:bool -** documentul a fost deschis incremental (caracteristică nouă care deschide documentul fără să-l descarce în totalitate)

  - **Data\_Doc\_IsOcsSupported:bool -** dacă documentul acceptă elaborarea în comun folosind noul serviciu OCS

  - **Data\_Doc\_IsOpeningOfflineCopy:bool -** verifică dacă documentul este deschis din memoria cache locală

  - **Data\_Doc\_IsSyncBacked:bool -** dacă documentul este deschis din folderul care folosește aplicația de sincronizare inversă OneDrive

  - **Data\_Doc\_Location:long -** set predefinit de valori privind locul de stocare a documentului (Local, SharePoint, WOPI, Rețea etc.)

  - **Data\_Doc\_LocationDetails:long -** set predefinit de valori privind locația mai detaliată (folderul Temp, folderul de descărcări, Documente OneDrive, Imagini OneDrive etc.)

  - **Data\_Doc\_NumberCoAuthors:long -** numărul de coautori la momentul deschiderii unui document

  - **Data\_Doc\_PasswordFlags:long -** set predefinit de valori privind modul în care documentul este criptat cu o parolă (Fără, parolă pentru citire, parolă pentru editare)

  - **Data\_Doc\_ReadOnlyReasons:long -** set predefinit de valori privind motivul pentru care acest document a fost marcat doar în citire (blocat pe server, document final, protejat prin parolă pentru editare etc.)

  - **Data\_Doc\_ResourceIdHash:string -** codul hash al identificatorului de resurse pentru documentele stocate în cloud

  - **Data_Doc_RtcType -**  indică modul în care a fost configurat canalul în timp real (RTC) pentru fișierul curent (dezactivat, neacceptat, la cerere, activat permanent etc.).

  - **Data\_Doc\_ServerDocId:string –** identificatorul imutabil pentru documentele stocate în cloud

  - **Data\_Doc\_ServerProtocol:long -** set predefinit de valori privind protocolul folosit în comunicarea cu serverul (Http, Cobalt, WOPI etc.)

  - **Data\_Doc\_ServerType:long -** set predefinit de valori privind tipul serverului (SharePoint, DropBox, WOPI)

  - **Data\_Doc\_ServerVersion:long -** dacă serverul se bazează pe Office14, Office15, Office 16

  - **Data\_Doc\_SessionId:long -** GUID generat care identifică instanța documentului din aceeași sesiune de proces

  - **Data\_Doc\_SharePointServiceContext:string -** un șir opac, de obicei GridManagerID.FarmID. Util pentru corelarea jurnalelor de la client și de pe server

  - **Data\_Doc\_SizeInBytes:long -** dimensiunea documentului în octeți

  - **Data\_Doc\_SpecialChars:long -** Bitmask ce arată caracterele speciale din adresa URL sau calea documentului

  - **Data\_Doc\_StorageProviderId:string -** șir care identifică furnizorul de stocare al documentului, precum „DropBox”

  - **Data\_Doc\_StreamAvailability:long -** set predefinit de valori privind starea șirului de document (disponibil, dezactivat definitiv, indisponibil)

  - **Data\_Doc\_UrlHash:string -** codul hash pentru adresa URL completă a documentelor stocate în cloud

  - **Data\_Doc\_UsedWrsDataOnOpen:bool -** true dacă fișierul a fost deschis incremental folosind datele WRS prememorate în cache pentru gazdă

  - **Data\_Doc\_WopiServiceId:string -** identificatorul serviciului WOPI, de ex. „Dropbox”

  - **Data\_DurationUAEOnSaveStartedMs:long -** timpul necesar pentru Ieșire aplicație necunoscută în timpul salvării

  - **Data\_EnsureSaveTransactionTimeMS:long -** timpul necesar pentru a garanta crearea tranzacției de salvare, dacă nu există deja

  - **Data\_FailureComponent:long-** set predefinit de valori privind componenta care a cauzat nereușita protocolului (Conflict, CSI, Internă etc.)

  - **Data\_FailureReason:long –** set predefinit de valori privind motivul nereușitei (FileIsCorrupt, BlockedByAntivirus etc.)

  - **Data\_fLifeguarded:bool –** documentul a fost vreodată protejat (caracteristică pentru a remedia automat erorile din documente, fără intervenția utilizatorului)?

  - **Data\_HandleEnsureContentType:long -** timpul necesar pentru a garanta că toate tipurile de conținut sunt corecte

  - **Data\_HandleEnsureContentTypeTimeMS:long -** timpul necesar pentru a garanta că toate tipurile de conținut sunt corecte

  - **Data\_HasEmbeddedFont:bool -** are acest document fonturi încorporate?

  - **Data\_InitializeSaveTimeMS:long -** timpul necesar de a inițializa conținutul documentului pentru a începe salvarea

  - **Data\_InOCSTransition:bool -** este această salvare efectuată pentru a realiza tranziția la OCS

  - **Data\_IsSavingWithEmbeddedFont:bool -** are acest document fonturi încorporate?

  - **Data\_MethodId:long -** în plan intern, ce linie de cod a fost executată ultima

  - **Data\_PerformEmbedFontsTimeMS:long -** timpul necesar pentru serializarea fonturilor încorporate

  - **Data\_PerformModernSaveTimeMS:long -** timpul necesar pentru a efectua o salvare modernă (cod nou)

  - **Data\_PerformPostSaveTimeMS:long -** timpul necesar pentru a executa funcții post salvare (notificări, anulare intrări)

  - **Data\_PrepareForSaveTimeMS:long -** timpul necesar pentru a începe salvarea

  - **Data\_RaiseDocumentBeforeSaveEventTimeMS:long -** timpul necesar pentru a ridica evenimentul BeforeSave

  - **Data\_ReflectDocumentChangeTimeMS:long -** timpul necesar pentru a reflecta modificările salvate în interfața cu utilizatorul (repopulare miniaturi etc.)

  - **Data\_ReportStartTimeMS:long -** timpul necesar pentru a finaliza inițializarea telemetriei pentru salvare

  - **Data\_ReportSuccessTimeMS:long -** timpul necesar pentru a finaliza raportarea salvării reușite

  - **Data\_ResetDirtyFlagOnErrorTimeMS:long -** timpul necesar pentru a reseta semnalizarea cu erori a documentului la eroare

  - **Data\_SaveReason:long -** set predefinit de valori privind motivul pentru care s-a efectuat această salvare (AutoSave, ToOCSTransitionSave, ToCSITransitionSave etc.)

  - **Data\_SaveType:long -** set predefinit de valori privind tipul de salvare (Salvare ca, Publicare, Manual, Salvare OM etc.)

  - **Data\_SavingWithFont:bool-** salvăm documentul cu noi fonturi încorporate?

  - **Data\_ScrubClonedDocumentTimeMS:long -** timp necesar pentru a elimina informațiile personale privind copia clonată a documentului

  - **Data\_StopwatchDuration:long -** timpul total al activității

  - **Data\_TransactionType:long -** este o tranzacție de Salvare sau Îmbinare și salvare?

#### <a name="officepowerpointdocoperationsaveas"></a>Office.PowerPoint.DocOperation.SaveAs

Colectat ori de câte ori PowerPoint efectuează o Salvare ca. Include tipul de rezultat, succes sau eșec, al măsurătorilor performanței de salvare și metadatele relevante ale documentului. Erorile de salvare pot duce la pierderea unor date.  Microsoft utilizează aceste date pentru a garanta faptul că această caracteristică funcționează conform așteptărilor, iar conținutul utilizatorilor a persistat cu succes.

Se colectează următoarele câmpuri:

- **Data_AddDocTelemetryResult:long** - această intrare în jurnal are toate datele de telemetrie necesare pentru documente (câmpurile Data_Doc_*)? Dacă nu, de ce?

- **Data_CppUncaughtExceptionCount:long** - excepții native neprinse în timp ce rula activitatea

- **Data_DetachedDuration:long** - timpul cât activitatea a fost detașată/nu a rulat

- **Data_DstDoc_AccessMode:long** - cum a fost deschis acest document (doar în citire | citire-scriere)

- **Data_DstDoc_AssistedReadingReasons:long** - set predefinit de valori pentru care documentul a fost deschis în modul de citire asistată

- **Data_DstDoc_AsyncOpenKind:long –** indică dacă s-a deschis o versiune memorată în cache a noului document cloud și ce logică de reîmprospătare asincronă s-a folosit.

- **Data_DstDoc_ChunkingType:long** - cum este stocat documentul în SharePoint

- **Data_DstDoc_EdpState:long** - starea Enterprise Data Protection a documentului

- **Data_DstDoc_Ext:string** - extensia documentului

- **Data_DstDoc_Extension:string** - extensia documentului

- **Data_DstDoc_FileFormat:long** - set predefinit de valori pentru formatul fișierului (mai granular decât extensia)

- **Data_DstDoc_Fqdn:string** - unde este stocat documentul (SharePoint.com, live.net), disponibil numai pentru domeniile Office 365
    
- **Data_DstDoc_FqdnHash:string** - codul hash al locului unde este stocat documentul

- **Data_DstDoc_IdentityTelemetryId:string** - GUID unic al utilizatorului

- **Data_DstDoc_IdentityUniqueId:string** - identificator unic al identității folosite pentru acțiunea Documente partajate

- **Data_DstDoc_IOFlags:long** - bitmask pentru diferite semnalizări legate de IO pentru un anumit document

- **Data_DstDoc_IrmRights:long** - set predefinit de valori pentru tipul de Information Rights Management aplicat pentru acest document (Redirecționare, Răspuns, SecureReader, Editare etc.)
    
- **Data_DstDoc_IsCloudCollabEnabled:bool** - true dacă antetul „IsCloudCollabEnabled” a fost deja primit dintr-o solicitare OPTIONS.

- **Data_DstDoc_IsIncrementalOpen:bool** - documentul a fost deschis incremental (caracteristică nouă care deschide documentul fără să-l descarce în totalitate)

- **Data_DstDoc_IsOcsSupported:bool** - dacă documentul acceptă elaborarea în comun folosind noul serviciu OCS

- **Data_DstDoc_IsOpeningOfflineCopy:bool** - verifică dacă documentul este deschis din memoria cache locală

- **Data_DstDoc_IsSyncBacked:bool** - dacă documentul este deschis din folderul care folosește aplicația de sincronizare inversă OneDrive
    
- **Data_DstDoc_Location:long** - set predefinit de valori privind locul de stocare a documentului (Local, SharePoint, WOPI, Rețea etc.)

- **Data_DstDoc_LocationDetails:long** - set predefinit de valori privind locația mai detaliată (folderul Temp, folderul de descărcări, Documente OneDrive, Imagini OneDrive etc.)

- **Data_DstDoc_NumberCoAuthors:long** - numărul de coautori la momentul deschiderii unui document

- **Data_DstDoc_PasswordFlags:long** - set predefinit de valori privind modul în care documentul este criptat cu o parolă (Fără, parolă pentru citire, parolă pentru editare)

- **Data_DstDoc_ReadOnlyReasons:long** - set predefinit de valori privind motivul pentru care acest document a fost marcat doar în citire (blocat pe server, document final, protejat prin parolă pentru editare etc.)

- **Data_DstDoc_ResourceIdHash:string** - codul hash al identificatorului de resurse pentru documentele stocate în cloud

- **Data_DstDoc_ServerDocId:string** - identificatorul invariabil pentru documentele stocate în cloud

- **Data_DstDoc_ServerProtocol:long** - set predefinit de valori privind protocolul folosit în comunicarea cu serverul (Http, Cobalt, WOPI etc.)

- **Data_DstDoc_ServerType:long** - set predefinit de valori privind tipul serverului (SharePoint, DropBox, WOPI)

- **Data_DstDoc_ServerVersion:long** - dacă serverul se bazează pe Office14, Office15, Office 16

- **Data_DstDoc_SessionId:long** - GUID generat care identifică instanța documentului din aceeași sesiune de proces

- **Data_DstDoc_SharePointServiceContext:string** - un șir opac, de obicei GridManagerID.FarmID. Util pentru corelarea jurnalelor de la client și de pe server

- **Data_DstDoc_SizeInBytes:long** - dimensiunea documentului în octeți

- **Data_DstDoc_SpecialChars:long** - Bitmask ce arată caracterele speciale din adresa URL sau din calea documentului

- **Data_DstDoc_StorageProviderId:string** - șir care identifică furnizorul de stocare al documentului, precum „DropBox”

- **Data_DstDoc_StreamAvailability:long** - set predefinit de valori privind starea șirului de document (disponibil, dezactivat definitiv, indisponibil)

- **Data_DstDoc_UrlHash:string** - codul hash pentru adresa URL completă a documentelor stocate în cloud

- **Data_DstDoc_UsedWrsDataOnOpen:bool** - true dacă fișierul a fost deschis incremental folosind datele WRS prememorate în cache pentru gazdă

- **Data_DstDoc_WopiServiceId:string** - identificatorul serviciului WOPI, de ex. „Dropbox”

- **Data_FileType:long** - set predefinit de valori al tipului de fișier intern

- **Data_fLifeguarded:bool** - documentul a fost vreodată protejat (caracteristică pentru a remedia automat erorile din documente, fără intervenția utilizatorului)?

- **Data_FWebCreated:bool** - are acest document o semnalizare WebCreator?

- **Data_SaveReason:long** - set predefinit de valori privind motivul pentru care s-a efectuat această salvare (AutoSave, ToOCSTransitionSave, ToCSITransitionSave etc.)

- **Data_SaveType:long** - set predefinit de valori privind tipul de salvare (Salvare ca, Publicare, Manual, Salvare OM etc.) 

- **Data_SrcDoc_AccessMode:long** - cum a fost deschis acest document (doar în citire | citire-scriere)

- **Data_SrcDoc_AssistedReadingReasons:long** - set predefinit de valori pentru care documentul a fost deschis în modul de citire asistată

- **Data_SrcDoc_AsyncOpenKind:long –** indică dacă s-a deschis o versiune memorată în cache a documentului cloud original și ce logică de reîmprospătare asincronă s-a folosit.

- **Data_SrcDoc_ChunkingType:long** - cum este stocat documentul în SharePoint 

- **Data_SrcDoc_EdpState:long** - starea Enterprise Data Protection a documentului

- **Data_SrcDoc_Ext:string** - extensia documentului

- **Data_SrcDoc_Extension:string** - extensia documentului

- **Data_SrcDoc_FileFormat:long** - set predefinit de valori pentru formatul fișierului (mai granular decât extensia)

- **Data_SrcDoc_Fqdn:string** - unde este stocat documentul (SharePoint.com, live.net), disponibil numai pentru domeniile Office 365

- **Data_SrcDoc_FqdnHash:string** - codul hash al locului unde este stocat documentul

- **Data_SrcDoc_IdentityTelemetryId:string** - GUID unic al utilizatorului

- **Data_SrcDoc_IdentityUniqueId:string** - identificator unic al identității folosite pentru acțiunea Documente partajate

- **Data_SrcDoc_IOFlags:long** - bitmask pentru diferite semnalizări legate de IO pentru un anumit document

- **Data_SrcDoc_IrmRights:long** - set predefinit de valori pentru tipul de Information Rights Management aplicat pentru acest document (Redirecționare, Răspuns, SecureReader, Editare etc.)

- **Data_SrcDoc_IsCloudCollabEnabled:bool** - true dacă antetul „IsCloudCollabEnabled” a fost deja primit dintr-o solicitare OPTIONS.

- **Data_SrcDoc_IsIncrementalOpen:bool** - documentul a fost deschis incremental (caracteristică nouă care deschide documentul fără să-l descarce în totalitate)

- **Data_SrcDoc_IsOcsSupported:bool** - dacă documentul acceptă elaborarea în comun folosind noul serviciu OCS

- **Data_SrcDoc_IsOpeningOfflineCopy:bool** - verifică dacă documentul este deschis din memoria cache locală

- **Data_SrcDoc_IsSyncBacked:bool** - dacă documentul este deschis din folderul care folosește aplicația de sincronizare inversă OneDrive

- **Data_SrcDoc_Location:long** - set predefinit de valori privind locul de stocare a documentului (Local, SharePoint, WOPI, Rețea etc.)

- **Data_SrcDoc_LocationDetails:long** - set predefinit de valori privind locația mai detaliată (folderul Temp, folderul de descărcări, Documente OneDrive, Imagini OneDrive etc.)

- **Data_SrcDoc_NumberCoAuthors:long** - numărul de coautori la momentul deschiderii unui document

- **Data_SrcDoc_PasswordFlags:long** - set predefinit de valori privind modul în care documentul este criptat cu o parolă (Fără, parolă pentru citire, parolă pentru editare)

- **Data_SrcDoc_ReadOnlyReasons:long** - set predefinit de valori privind motivul pentru care acest document a fost marcat doar în citire (blocat pe server, document final, protejat prin parolă pentru editare etc.)

- **Data_SrcDoc_ResourceIdHash:string** - codul hash al identificatorului de resurse pentru documentele stocate în cloud

- **Data_SrcDoc_ServerDocId:string** - identificatorul invariabil pentru documentele stocate în cloud

- **Data_SrcDoc_ServerProtocol:long** - set predefinit de valori privind protocolul folosit în comunicarea cu serverul (Http, Cobalt, WOPI etc.)

- **Data_SrcDoc_ServerType:long** - set predefinit de valori privind tipul serverului (SharePoint, DropBox, WOPI)

- **Data_SrcDoc_ServerVersion:long** - verfică dacă serverul se bazează pe Office14, Office15 sau Office 16

- **Data_SrcDoc_SessionId:long** - GUID generat ce identifică instanța documentului din aceeași sesiune de proces

- **Data_SrcDoc_SharePointServiceContext:string** - un șir opac, de obicei GridManagerID.FarmID. Util pentru corelarea jurnalelor de la client și de pe server

- **Data_SrcDoc_SizeInBytes:long** - dimensiunea documentului în octeți

- **Data_SrcDoc_SpecialChars:long** - Bitmask ce arată caracterele speciale din adresa URL sau calea documentului

- **Data_SrcDoc_StorageProviderId:string** - șir care identifică furnizorul de stocare al documentului, precum „DropBox”

- **Data_SrcDoc_StreamAvailability:long** - set predefinit de valori privind starea șirului de document (disponibil, dezactivat definitiv, indisponibil)

- **Data_SrcDoc_UrlHash:string** - codul hash pentru adresa URL completă a documentelor stocate în cloud

- **Data_SrcDoc_UsedWrsDataOnOpen:bool** - true dacă fișierul a fost deschis incremental folosind datele WRS prememorate în cache pentru gazdă

- **Data_SrcDoc_WopiServiceId:string** - identificatorul serviciului WOPI, de ex. „Dropbox”

- **Data_StopwatchDuration:long** - timpul total al activității

- **Data_TypeOfSaveDialog:long** - set predefinit de valori de dialog (RUN_SAVEAS_DLG,RUN_SAVEMEDIA_DLG, RUN_SAVEAS_VIDEO_DLG etc.)

- **Data_WaitForSaveOrMergeSuccess:bool** - SaveAs a reușit să aștepte salvarea sau îmbinarea fundalului.
 
- **Data_WaitForSaveOrMergeTimeout:long** - SaveAs a expirat la așteptarea salvării sau a îmbinării fundalului.

- **DstDoc** - noua locație a documentului 

- **SrcDoc** - locația inițială a documentului


#### <a name="officepowerpointdocoperationsavelegacy"></a>Office.PowerPoint.DocOperation.SaveLegacy

Colectat ori de câte ori PowerPoint efectuează o salvare utilizând calea de cod moștenită. Include tipul de rezultat, succes sau eșec, al măsurătorilor performanței de salvare și metadatele relevante ale documentului.  Erorile de salvare pot duce la pierderea unor date.  Microsoft utilizează aceste date pentru a garanta faptul că această caracteristică funcționează conform așteptărilor, iar conținutul utilizatorilor a persistat cu succes.

Se colectează următoarele câmpuri:

- **Data_AddDocTelemetryResult:long** - această intrare în jurnal are toate datele de telemetrie necesare pentru documente (câmpurile Data_Doc_*)? Dacă nu, de ce?

- **Data_CppUncaughtExceptionCount:long** - excepții native neprinse în timp ce rula activitatea

- **Data_DetachedDuration:long** - timpul cât activitatea a fost detașată/nu a rulat

- **Data_Doc_AccessMode:long** - cum a fost deschis acest document (doar în citire / citire-scriere)

- **Data_Doc_AssistedReadingReasons:long** - set predefinit de valori pentru care documentul a fost deschis în modul de citire asistată

- **Data_Doc_AsyncOpenKind:long –** indică dacă s-a deschis o versiune memorată în cache a documentului cloud și ce logică de reîmprospătare asincronă s-a folosit.

- **Data_Doc_ChunkingType:long** - cum este stocat documentul în SharePoint

- **Data_Doc_EdpState:long** - starea Enterprise Data Protection a documentului

- **Data_Doc_Ext:string** - extensia documentului

- **Data_Doc_Extension:string** - extensia documentului

- **Data_Doc_FileFormat:long** - set predefinit de valori pentru formatul fișierului (mai granular decât extensia)

- **Data_Doc_Fqdn:string** - unde este stocat documentul (SharePoint.com, live.net), disponibil numai pentru domeniile Office 365

- **Data_Doc_FqdnHash:string** - codul hash al locului unde este stocat documentul

- **Data_Doc_IdentityTelemetryId:string** - GUID unic al utilizatorului

- **Data_Doc_IdentityUniqueId:string** - identificator unic al identității folosite pentru acțiunea Documente partajate

- **Data_Doc_IOFlags:long** - bitmask pentru diferite semnalizări legate de IO pentru un anumit document

- **Data_Doc_IrmRights:long** - set predefinit de valori pentru tipul de Information Rights Management aplicat pentru acest document (Redirecționare, Răspuns, SecureReader, Editare etc.)

- **Data_Doc_IsCloudCollabEnabled:bool** - true dacă antetul „IsCloudCollabEnabled” a fost deja primit dintr-o solicitare OPTIONS.

- **Data_Doc_IsIncrementalOpen:bool** - documentul a fost deschis incremental (caracteristică nouă care deschide documentul fără să-l descarce în totalitate)

- **Data_Doc_IsOcsSupported:bool** - dacă documentul acceptă elaborarea în comun folosind noul serviciu OCS

- **Data_Doc_IsOpeningOfflineCopy:bool** - verifică dacă documentul este deschis din memoria cache locală

- **Data_Doc_IsSyncBacked:bool** - dacă documentul este deschis din folderul care folosește aplicația de sincronizare inversă OneDrive

- **Data_Doc_Location:long** - set predefinit de valori privind locul de stocare a documentului (Local, SharePoint, WOPI, Rețea etc.)

- **Data_Doc_LocationDetails:long** - set predefinit de valori privind locația mai detaliată (folderul Temp, folderul de descărcări, Documente OneDrive, Imagini OneDrive etc.)

- **Data_Doc_NumberCoAuthors:long** - numărul de coautori la momentul deschiderii unui document

- **Data_Doc_PasswordFlags:long** - set predefinit de valori privind modul în care documentul este criptat cu o parolă (Niciunul, parolă pentru citire, parolă pentru editare)

- **Data_Doc_ReadOnlyReasons:long** - set predefinit de valori privind motivul pentru care acest document a fost marcat doar în citire (blocat pe server, document final, protejat prin parolă pentru editare etc.)

- **Data_Doc_ResourceIdHash:string** - codul hash al identificatorului de resurse pentru documentele stocate în cloud

- **Data_Doc_RtcType** - indică modul în care a fost configurat canalul în timp real (RTC) pentru fișierul curent (dezactivat, neacceptat, la cerere, activat permanent etc.).

- **Data_Doc_ServerDocId:string** - identificator imutabil pentru documentele stocate în cloud

- **Data_Doc_ServerProtocol:long** - set predefinit de valori privind protocolul folosit în comunicarea cu serverul (Http, Cobalt, WOPI etc.)

- **Data_Doc_ServerType:long** - set predefinit de valori privind tipul serverului (SharePoint, DropBox, WOPI) 

- **Data_Doc_ServerVersion:long** - dacă serverul se bazează pe Office14, Office15, Office 16

- **Data_Doc_SessionId:long** - GUID generat care identifică instanța documentului din aceeași sesiune de proces

- **Data_Doc_SharePointServiceContext:string** - un șir opac, de obicei GridManagerID.FarmID. Util pentru corelarea jurnalelor de la client și de pe server

- **Data_Doc_SizeInBytes:long** - dimensiunea documentului în octeți

- **Data_Doc_SpecialChars:long** - Bitmask ce arată caracterele speciale din adresa URL sau calea documentului

- **Data_Doc_StorageProviderId:string** - șir care identifică furnizorul de stocare a documentului, precum „DropBox”

- **Data_Doc_StreamAvailability:long** - set predefinit de valori privind starea șirului de document (disponibil, dezactivat definitiv, indisponibil)

- **Data_Doc_UrlHash:string** - codul hash pentru adresa URL completă a documentelor stocate în cloud

- **Data_Doc_UsedWrsDataOnOpen:bool** - true dacă fișierul a fost deschis incremental folosind datele WRS prememorate în cache pentru gazdă

- **Data_Doc_WopiServiceId:string** - identificatorul serviciului WOPI, de ex. „Dropbox”

- **Data_DstDoc_AccessMode:long** - cum a fost deschis acest document (doar în citire | citire-scriere)

- **Data_DstDoc_AssistedReadingReasons:long** - set predefinit de valori pentru care documentul a fost deschis în modul de citire asistată

- **Data_DstDoc_AsyncOpenKind:long –** indică dacă s-a deschis o versiune memorată în cache a noului document cloud și ce logică de reîmprospătare asincronă s-a folosit.

- **Data_DstDoc_ChunkingType:long** - cum este stocat documentul în SharePoint

- **Data_DstDoc_EdpState:long** - starea Enterprise Data Protection a documentului

- **Data_DstDoc_Ext:string** - extensia documentului

- **Data_DstDoc_Extension:string** - extensia documentului

- **Data_DstDoc_FileFormat:long** - set predefinit de valori pentru formatul fișierului (mai granular decât extensia)

- **Data_DstDoc_Fqdn:string** - unde este stocat documentul (SharePoint.com, live.net), disponibil numai pentru domeniile Office 365
    
- **Data_DstDoc_FqdnHash:string** - codul hash al locului unde este stocat documentul

- **Data_DstDoc_IdentityTelemetryId:string** - GUID unic al utilizatorului

- **Data_DstDoc_IdentityUniqueId:string** - identificator unic al identității folosite pentru acțiunea Documente partajate

- **Data_DstDoc_IOFlags:long** - bitmask pentru diferite semnalizări legate de IO pentru un anumit document

- **Data_DstDoc_IrmRights:long** - set predefinit de valori pentru tipul de Information Rights Management aplicat pentru acest document (Redirecționare, Răspuns, SecureReader, Editare etc.)

- **Data_DstDoc_IsCloudCollabEnabled:bool** - true dacă antetul „IsCloudCollabEnabled” a fost deja primit dintr-o solicitare OPTIONS.

- **Data_DstDoc_IsIncrementalOpen:bool** - documentul a fost deschis incremental (caracteristică nouă care deschide documentul fără să-l descarce în totalitate)

- **Data_DstDoc_IsOcsSupported:bool** - dacă documentul acceptă elaborarea în comun folosind noul serviciu OCS

- **Data_DstDoc_IsOpeningOfflineCopy:bool** - verifică dacă documentul este deschis din memoria cache locală

- **Data_DstDoc_IsSyncBacked:bool** - dacă documentul este deschis din folderul care folosește aplicația de sincronizare inversă OneDrive

- **Data_DstDoc_Location:long** - set predefinit de valori privind locul de stocare a documentului (Local, SharePoint, WOPI, Rețea etc.)

- **Data_DstDoc_LocationDetails:long** - set predefinit de valori privind locația mai detaliată (folderul Temp, folderul de descărcări, Documente OneDrive, Imagini OneDrive etc.)

- **Data_DstDoc_NumberCoAuthors:long** - numărul de coautori la momentul deschiderii unui document

- **Data_DstDoc_PasswordFlags:long** - set predefinit de valori privind modul în care documentul este criptat cu o parolă (Fără, parolă pentru citire, parolă pentru editare)

- **Data_DstDoc_ReadOnlyReasons:long** - set predefinit de valori privind motivul pentru care acest document a fost marcat doar în citire (blocat pe server, document final, protejat prin parolă pentru editare etc.)

- **Data_DstDoc_ResourceIdHash:string** - codul hash al identificatorului de resurse pentru documentele stocate în cloud

- **Data_DstDoc_ServerDocId:string** - identificatorul invariabil pentru documentele stocate în cloud

- **Data_DstDoc_ServerProtocol:long** - set predefinit de valori privind protocolul folosit în comunicarea cu serverul (Http, Cobalt, WOPI etc.)

- **Data_DstDoc_ServerType:long** - set predefinit de valori privind tipul serverului (SharePoint, DropBox, WOPI)

- **Data_DstDoc_ServerVersion:long** - dacă serverul se bazează pe Office14, Office15, Office 16

- **Data_DstDoc_SessionId:long** - GUID generat care identifică instanța documentului din aceeași sesiune de proces

- **Data_DstDoc_SharePointServiceContext:string** - un șir opac, de obicei GridManagerID.FarmID. Util pentru corelarea jurnalelor de la client și de pe server

- **Data_DstDoc_SizeInBytes:long** - dimensiunea documentului în octeți

- **Data_DstDoc_SpecialChars:long** - Bitmask ce arată caracterele speciale din adresa URL sau din calea documentului

- **Data_DstDoc_StorageProviderId:string** - șir care identifică furnizorul de stocare al documentului, precum „DropBox”

- **Data_DstDoc_StreamAvailability:long** - set predefinit de valori privind starea șirului de document (disponibil, dezactivat definitiv, indisponibil)

- **Data_DstDoc_UrlHash:string** - codul hash pentru adresa URL completă a documentelor stocate în cloud

- **Data_DstDoc_UsedWrsDataOnOpen:bool** - true dacă fișierul a fost deschis incremental folosind datele WRS prememorate în cache pentru gazdă

- **Data_DstDoc_WopiServiceId:string** - identificatorul serviciului WOPI, de ex. „Dropbox”

- **Data_FileType:long** - set predefinit de valori al tipului de fișier intern

- **Data_fLifeguarded:bool** - documentul a fost vreodată protejat (caracteristică pentru a remedia automat erorile din documente, fără intervenția utilizatorului)?

- **Data_SaveReason:long** - set predefinit de valori privind motivul pentru care s-a efectuat această salvare (AutoSave, ToOCSTransitionSave, ToCSITransitionSave etc.)

- **Data_SaveType:long** - set predefinit de valori privind tipul de salvare (Salvare ca, Publicare, Manual, Salvare OM etc.)

- **Data_SrcDoc_AccessMode:long** - cum a fost deschis acest document (doar în citire | citire-scriere)

- **Data_SrcDoc_AssistedReadingReasons:long** - set predefinit de valori pentru care documentul a fost deschis în modul de citire asistată

- **Data_SrcDoc_AsyncOpenKind:long –** indică dacă s-a deschis o versiune memorată în cache a documentului cloud original și ce logică de reîmprospătare asincronă s-a folosit.

- **Data_SrcDoc_ChunkingType:long** - cum este stocat documentul în SharePoint

- **Data_SrcDoc_EdpState:long** - starea Enterprise Data Protection a documentului

- **Data_SrcDoc_Ext:string** - extensia documentului

- **Data_SrcDoc_Extension:string** - extensia documentului

- **Data_SrcDoc_FileFormat:long** - set predefinit de valori pentru formatul fișierului (mai granular decât extensia)

- **Data_SrcDoc_Fqdn:string** - unde este stocat documentul (SharePoint.com, live.net), disponibil numai pentru domeniile Office 365

- **Data_SrcDoc_FqdnHash:string** - codul hash al locului unde este stocat documentul 

- **Data_SrcDoc_IdentityTelemetryId:string** - GUID unic al utilizatorului

- **Data_SrcDoc_IdentityUniqueId:string** - identificator unic al identității folosite pentru acțiunea Documente partajate

- **Data_SrcDoc_IOFlags:long** - bitmask pentru diferite semnalizări legate de IO pentru un anumit document

- **Data_SrcDoc_IrmRights:long** - set predefinit de valori pentru tipul de Information Rights Management aplicat pentru acest document (Redirecționare, Răspuns, SecureReader, Editare etc.)
    
- **Data_SrcDoc_IsCloudCollabEnabled:bool** - true dacă antetul „IsCloudCollabEnabled” a fost deja primit dintr-o solicitare OPTIONS.

- **Data_SrcDoc_IsIncrementalOpen:bool** - documentul a fost deschis incremental (caracteristică nouă care deschide documentul fără să-l descarce în totalitate)

- **Data_SrcDoc_IsOcsSupported:bool** - dacă documentul acceptă elaborarea în comun folosind noul serviciu OCS

- **Data_SrcDoc_IsOpeningOfflineCopy:bool** - verifică dacă documentul este deschis din memoria cache locală

- **Data_SrcDoc_IsSyncBacked:bool** - dacă documentul este deschis din folderul care folosește aplicația de sincronizare inversă OneDrive

- **Data_SrcDoc_Location:long** - set predefinit de valori privind locul de stocare a documentului (Local, SharePoint, WOPI, Rețea etc.)

- **Data_SrcDoc_LocationDetails:long** - set predefinit de valori privind locația mai detaliată (folderul Temp, folderul de descărcări, Documente OneDrive, Imagini OneDrive etc.)

- **Data_SrcDoc_NumberCoAuthors:long** - numărul de coautori la momentul deschiderii unui document

- **Data_SrcDoc_PasswordFlags:long** - set predefinit de valori privind modul în care documentul este criptat cu o parolă (Fără, parolă pentru citire, parolă pentru editare)

- **Data_SrcDoc_ReadOnlyReasons:long** - set predefinit de valori privind motivul pentru care acest document a fost marcat doar în citire (blocat pe server, document final, protejat prin parolă pentru editare etc.)

- **Data_SrcDoc_ResourceIdHash:string** - codul hash al identificatorului de resurse pentru documentele stocate în cloud

- **Data_SrcDoc_ServerDocId:string** - identificatorul invariabil pentru documentele stocate în cloud

- **Data_SrcDoc_ServerProtocol:long** - set predefinit de valori privind protocolul folosit în comunicarea cu serverul (Http, Cobalt, WOPI etc.)

- **Data_SrcDoc_ServerType:long** - set predefinit de valori privind tipul serverului (SharePoint, DropBox, WOPI)

- **Data_SrcDoc_ServerVersion:long** - verfică dacă serverul se bazează pe Office14, Office15 sau Office 16

- **Data_SrcDoc_SessionId:long** - GUID generat care identifică instanța documentului din aceeași sesiune de proces

- **Data_SrcDoc_SharePointServiceContext:string** - un șir opac, de obicei GridManagerID.FarmID. Util pentru corelarea jurnalelor de la client și de pe server

- **Data_SrcDoc_SizeInBytes:long** - dimensiunea documentului în octeți

- **Data_SrcDoc_SpecialChars:long** - Bitmask ce arată caracterele speciale din adresa URL sau calea documentului

- **Data_SrcDoc_StorageProviderId:string** - șir care identifică furnizorul de stocare al documentului, precum „DropBox”

- **Data_SrcDoc_StreamAvailability:long** - set predefinit de valori privind starea șirului de document (disponibil, dezactivat definitiv, indisponibil)

- **Data_SrcDoc_UrlHash:string** - codul hash pentru adresa URL completă a documentelor stocate în cloud

- **Data_SrcDoc_UsedWrsDataOnOpen:bool** - true dacă fișierul a fost deschis incremental folosind datele WRS prememorate în cache pentru gazdă

- **Data_SrcDoc_WopiServiceId:string** - identificatorul serviciului WOPI, de ex. „Dropbox”

- **Data_StopwatchDuration:long** - timpul total al activității

- **Data_TypeOfSaveDialog:long** - set predefinit de valori de dialog (RUN_SAVEAS_DLG, RUN_SAVEMEDIA_DLG, RUN_SAVEAS_VIDEO_DLG etc.)

- **Doc** - document curent pentru Salvare

- **DstDoc** - noua locație a documentului (în cazul Salvare ca)

- **SrcDoc** - locația inițială a documentului (în cazul Salvare ca)

#### <a name="officepowerpointpptmacshellprintinfo"></a>Office.PowerPoint.PPT.Mac.Shell.PrintInfo

Colectată de fiecare dată când o operațiune de export PDF s-a finalizat și conține informații despre succesul operațiunii. Aceste informații sunt esențiale pentru a identifica succesul operațiunilor de export PDF pentru aplicația noastră.

Se colectează următoarele câmpuri:

- **Data_ExportAsPDFSucceed** - Boolean care indică dacă exportul ca PDF a fost un succes.


#### <a name="officepowerpointpptsharedslideshowfailure"></a>Office.PowerPoint.PPT.Shared.SlideShow.Failure

Colectarea erorilor în timpul expunerii de diapozitive ca o caracteristică esențială pentru PowerPoint. Microsoft colectează informații despre momentul când apare o eroare în timpul expunerii de diapozitive pentru a îmbunătăți experiența utilizatorului privind expunerea de diapozitive. Microsoft utilizează aceste date pentru a obține informații de diagnosticare privind locul unde apare eroarea în timp ce utilizatorul folosește expunerea de diapozitive.

Se colectează următoarele câmpuri:

- **CountOArtErrors** - numărul total de erori OArt

- **CountOtherErrors** - numărul total de alte erori

- **CountPPTErrors** - numărul total de erori PPT

- **CountSlideShowErrors** - numărul total de erori aferente expunerii de diapozitive

- **FirstOArtError** - prima eroare care a apărut în OArt

- **FirstOtherError** - prima eroare care a apărut în altă zonă

- **FirstPPTError** - prima eroare care a apărut în PPT

- **FirstSlideShowError** - prima eroare care a apărut în expunerea de diapozitive

    
#### <a name="officepowerpointrunprintoperation"></a>Office.PowerPoint.RunPrintOperation

Colectată de fiecare dată când o operațiune de imprimare PDF sau de export PDF s-a finalizat și conține informații despre tipul de aspect, utilizarea numerelor de diapozitiv precum și despre succesul operațiunii. Aceste informații sunt esențiale pentru a identifica succesul operațiunilor de imprimare PDF pentru aplicația noastră.

Se colectează următoarele câmpuri:

- **Data_PrintWithSlideNumbers** - Boolean care indică dacă utilizatorul imprimă cu numere de diapozitiv.

- **Data_SavePrintLayoutType** - tipul de aspect pagină imprimată la momentul începerii operațiunii de imprimare sau de export.

- **Data_Success** - Boolean care indică dacă imprimarea a fost un succes.


#### <a name="officeprojectprojectfilesave"></a>Office.Project.ProjectFileSave

Project salvează un fișier. Acest eveniment indică o salvare Project. Aceasta permite Microsoft să măsoare succesul salvării unui fișier de către Project, ceea ce este important pentru a se evita pierderea de date din document.

Se colectează următoarele câmpuri:

  - **Data\_TriggerTime** - ora salvării

  - **Data\_FileType** - tipul de fișier cu care este salvat proiectul
 
#### <a name="officesessionactivitystart"></a>Office.Session.Activity.Start

Ne permite să știm când a început o sesiune Data Streamer.  Utilizat pentru starea și monitorizarea caracteristicilor. Evenimentul este generat de Microsoft Data Streamer pentru programul de completare Excel.

Se colectează următoarele câmpuri:

- **Activity_Name** - numele activității „Session”

- **Activity_CV** - ID pentru corelarea evenimentelor în sesiunea de conectare

- **Activity_StartStopType** - Start

- **Activity_DateTimeTicks** - Oră Dată pentru activitate

#### <a name="officesessionactivitystop"></a>Office.Session.Activity.Stop

Ne permite să știm când s-a oprit o sesiune Data Streamer Utilizat pentru starea și monitorizarea caracteristicilor. Evenimentul este generat de Microsoft Data Streamer pentru programul de completare Excel.

Se colectează următoarele câmpuri:

- **Activity_Name** - numele activității „Session”

- **Activity_CV** - ID pentru corelarea evenimentelor în sesiunea de conectare

- **Activity_StartStopType** - Stop

- **Activity_DateTimeTicks** - Oră Dată pentru activitate

#### <a name="officestreamdeviceactivitystart"></a>Office.StreamDevice.Activity.Start

Ne permite să știm dacă pornirea sursei de date cu redare în flux a reușit.   Utilizat pentru starea și monitorizarea caracteristicilor. Evenimentul este generat de Microsoft Data Streamer pentru programul de completare Excel.

Se colectează următoarele câmpuri:

- **Datasource_Type** - dispozitiv serial sau informații Serviciu pentru aplicații

- **DataSource_Name** - numele sursei de date conectate

- **Activity_Name** - numele activității „StreamDeviceData” sau „StreamFileData”

- **Activity_CV** - ID pentru corelarea evenimentelor în sesiunea de conectare

- **Activity_StartStopType** - Start

- **Activity_DateTimeTicks** - Oră Dată pentru activitate

#### <a name="officestreamdeviceactivitystop"></a>Office.StreamDevice.Activity.Stop

Ne permite să știm dacă oprirea sursei de date cu redare în flux a reușit.   Utilizat pentru starea și monitorizarea caracteristicilor. Evenimentul este generat de Microsoft Data Streamer pentru programul de completare Excel.

Se colectează următoarele câmpuri:

- **Datasource_Type** - dispozitiv serial sau informații Serviciu pentru aplicații

- **DataSource_Name** - numele sursei de date conectate

- **Activity_Name** - numele activității „StreamDeviceData” sau „StreamFileData”

- **Activity_CV** - ID pentru corelarea evenimentelor în sesiunea de conectare

- **Activity_StartStopType** - Stop

- **Activity_DateTimeTicks** - Oră Dată pentru activitate

#### <a name="officetargetedmessagingabexperimentmessagetrigger"></a>Office.TargetedMessaging.ABExperimentMessageTrigger

Urmărește numărul de utilizatori care primesc mesaje BizBar și Pânză dinamică de la TargetedMessagingService (TMS). Aceste date sunt de importanță critică pentru a înțelege ce mesaje primesc utilizatorii și pe ce suprafață, astfel încât să ne asigurăm că nu le lipsește niciun mesaj care ar putea fi esențial pentru ca aceștia să continue să utilizeze produsul. De asemenea, este necesar să măsurați cu precizie succesul experimentelor și campaniilor noastre desfășurate prin TMS.

Se colectează următoarele câmpuri:

  - **Data\_Surface** - numele suprafeței la care se referă acest mesaj livrat de serviciu

  - **Data\_Flight** - identificator ediție flight ECS/CT care a fost utilizat pentru a livra acest mesaj

  - **Data\_CampaignId** - identificator al campaniei din care face parte acest mesaj

  - **Data\_MessageId** - identificator al acestui mesaj livrat de serviciu

  - **Data\_TransactionId** - identificator al acestei tranzacții cu serviciul

  - **Data\_TriggerPoint** - etapă în care a fost înregistrat în jurnal acest eveniment (mesaj primit versus mesaj afișat)

#### <a name="officetextfontpickerfontselectedwin32"></a>Office.Text.FontPickerFontSelected.Win32

Acest eveniment indică dacă fontul descărcat a fost redat corect. Utilizat pentru a indica succesul sau eșecul descărcării fontului.

Se colectează următoarele câmpuri:

  - **Font name (Data\_Font)** - numele fontului ales în selectorul de font

  - **User click (Data\_FClick)** - dacă utilizatorul a folosit mouse-ul pentru a selecta elementul

#### <a name="officetextresourceclientrequestresourceinternal"></a>Office.Text.ResourceClient.RequestResourceInternal

Acest eveniment indică dacă fontul a fost descărcat corect. Utilizat pentru a indica succesul sau eșecul redării fontului descărcat.

Se colectează următoarele câmpuri:

  - **Data\_FontToken** - numele cu care va fi salvat fișierul de resurse

  - **Data\_HTTPResult** - rezultatul solicitării HTTP

  - **Data\_HTTPStatusCode** - codul HTTP returnat în urma solicitării HTTP

  - **Data\_isInternetOn** - dacă am avut conexiune atunci când am încercat să regăsim resursa

  - **Data\_RequestUrl** - URL-ul resursei CDN pe care încercăm să îl regăsim



#### <a name="officetranslatordocumenttranslated"></a>Office.Translator.DocumentTranslated

Colectează succesul sau nereușita traducerii unui întreg document pe care un utilizator o declanșează în Translator SDX. Acest lucru este de importanță critică pentru a evalua starea caracteristicii de traducere și a reacționa la eventuale întreruperi. Monitorizați starea de funcționare a scenariului „Traducere document” în Word.

Se colectează următoarele câmpuri:

- **Data.actionSource** - cum a fost declanșată traducerea selecției

- **Data.bodyBackgroundColor** - culoare de fundal container temă Office

- **Data.bodyForegroundColor** - culoare de prim-plan container temă Office

- **Data.browserLang** - limbă curentă afișaj browser

- **Data.browserOnline** - depășit

- **Data.browserPlatform** - platformă browser

- **Data.browserUserAgent** - agent utilizator browser

- **Data.colorDepth** - adâncime culoare sistem

- **Data.contentLanguage** - limbă detectată a conținutului de tradus

- **Data.controlBackgroundColor** - culoare de fundal control temă Office

- **Data.controlForegroundColor** - culoare de prim-plan container temă Office

- **Data.correlationId** - identificator unic al solicitării trimise la serviciu

- **Data.crossSessionId** - identificator unic al utilizatorului

- **Data.crossSessionStartTime** - marcă de timp UTC privind momentul în care a început sesiunea de traducere

- **Data.currentTime** - marcă de timp UTC privind momentul în care a fost trimis acest mesaj de telemetrie

- **Data.displayLanguage** - limbă afișaj Office

- **Data.documentSourceLang** - limbă conținut document-

- **Data.documentTargetLang** - documentul Limbă va fi tradus în-

- **Data.environment** - mediul de serviciu la care este trimisă solicitarea

- **Data.errorMessage** - mesaj de eroare raportat de serviciu

- **Data.eventActionType** - tip de eveniment de telemetrie

- **Data.eventTagId** - identificator unic al liniei de cod care a produs acest mesaj de telemetrie

- **Data.flights** - ediții flight activate

- **Data.fileSize** - dimensiunea fișierului Word de tradus

- **Data.fileSource** - unde este găzduit fișierul Word (offline, online)

- **Data.fileType** - extensia fișierului Word

- **Data.innerHeight"** - înălțime container panou lateral

- **Data.innerWidth"** - lățime container panou lateral

- **Data.lookupSourceLang** - neutilizat pentru traducerea documentului

- **Data.lookupTargetLang** - neutilizat pentru traducerea documentului

- **Data.officeHost** - aplicație Office care găzduiește panoul lateral

- **Data.officeLocale** - limbă utilizatorului Office

- **Data.officeMachineId** - identificator unic al dispozitivului

- **Data.officePlatform** - platforma dispozitivului

- **Data.officeSessionId** - identificator al sesiunii Office

- **Data.officeUserId** - identificator unic utilizator Office

- **Data.officeVersion** - versiune de Office

- **Data.pageXOffset** - poziție de defilare orizontală panoul lateral din partea stângă a panoului

- **Data.pageYOffset** - poziție de defilare verticală panoul lateral din partea stângă a panoului

- **Data.pixelDepth** - rezoluția de culori a ecranului

- **Data.responseCode** - cod de răspuns solicitare de la serviciu

- **Data.responseTime** - timp scurs solicitare 

- **Data.resultType** - rezultat solicitare

- **Data.screenHeight** - înălțime ecran în pixeli

- **Data.screenLeft** - coordonata orizontală a ferestrei față de ecran

- **Data.screenTop** - coordonata verticală a ferestrei față de ecran

- **Data.screenWidth** - lățime ecran în pixeli

- **Data.selectedTab** - care filă este selectată selecție sau document

- **Data.serverUrl** - URL serviciu de traducere

- **Data.sessionId** - identificator sesiune panoul lateral

- **Data.sessionStartTime** - marcă de timp UTC privind momentul în care a început sesiunea de traducere

- **Data.sourceTextHash** - codul hash al textului de tradus

- **Data.sourceTextLength** - lungime text de tradus

- **Data.sourceTextWords** - număr de cuvinte în textul de tradus

- **Data.warningMessage** - mesaj de avertisment raportat de serviciu


#### <a name="officetranslatortexttranslated"></a>Office.Translator.TextTranslated

Colectează succesul sau nereușita traducerii unei selecții pe care acțiunea unui utilizator o declanșează în Translator SDX. Acest lucru este de importanță critică pentru a evalua starea caracteristicii de traducere și a reacționa la eventuale întreruperi. Utilizat pentru a monitoriza starea de funcționare a scenariului „Traducere selecție” în Excel, PowerPoint, Word.

Se colectează următoarele câmpuri:

- **Data.actionSource** - cum a fost declanșată traducerea selecției

- **Data.bodyBackgroundColor** - culoare de fundal container temă Office

- **Data.bodyForegroundColor** - culoare de prim-plan container temă Office

- **Data.browserLang** - limbă curentă afișaj browser

- **Data.browserOnline** - depășit

- **Data.browserPlatform** - platformă browser

- **Data.browserUserAgent** - agent utilizator browser

- **Data.colorDepth** - adâncime culoare sistem

- **Data.contentLanguage** - limbă detectată a conținutului de tradus

- **Data.controlBackgroundColor** - culoare de fundal control temă Office

- **Data.controlForegroundColor** - culoare de prim-plan container temă Office

- **Data.correlationId** - identificator unic al solicitării trimise la serviciu

- **Data.crossSessionId** - identificator unic al utilizatorului

- **Data.crossSessionStartTime** - marcă de timp UTC privind momentul în care a început sesiunea de traducere

- **Data.currentTime** - marcă de timp UTC privind momentul în care a fost trimis acest mesaj de telemetrie

- **Data.displayLanguage** - limbă afișaj Office

- **Data.documentSourceLang** - nu se utilizează pentru selecție

- **Data.documentTargetLang** - nu se utilizează pentru selecție traducere

- **Data.environment** - mediul de serviciu la care este trimisă solicitarea

- **Data.errorMessage** - mesaj de eroare raportat de serviciu

- **Data.eventActionType** - tip de eveniment de telemetrie

- **Data.eventTagId"** - identificator unic al liniei de cod care a produs acest mesaj de telemetrie

- **Data.flights** - ediții flight activate

- **Data.innerHeight** - înălțime container panou lateral

- **Data.innerWidth** - lățime container panou lateral

- **Data.lookupSourceLang** - limba textului selectat în mod curent

- **Data.lookupTargetLang** - limba textului selectat în mod curent va fi tradusă în

- **Data.officeHost** - aplicație Office care găzduiește panoul lateral

- **Data.officeLocale** - limbă utilizatorului Office

- **Data.officeMachineId** - identificator unic al dispozitivului

- **Data.officePlatform** - platforma dispozitivului

- **Data.officeSessionId** - identificator al sesiunii Office

- **Data.officeUserId** - identificator unic utilizator Office

- **Data.officeVersion** - versiune de Office

- **Data.pageXOffset** - poziție de defilare orizontală panoul lateral din partea stângă a panoului

- **Data.pageYOffset** - poziție de defilare verticală panoul lateral din partea stângă a panoului

- **Data.pixelDepth** - rezoluția de culori a ecranului

- **Data.responseCode** - cod de răspuns solicitare de la serviciu

- **Data.responseTime** - timp scurs solicitare

- **Data.resultType** - rezultat solicitare

- **Data.screenHeight** - înălțime ecran în pixeli

- **Data.screenLeft** - coordonata orizontală a ferestrei față de ecran

- **Data.screenTop** - coordonata verticală a ferestrei față de ecran

- **Data.screenWidth** - lățime ecran în pixeli

- **Data.selectedTab** - care filă este selectată selecție sau document

- **Data.serverUrl** - URL serviciu de traducere

- **Data.sessionId** - identificator sesiune panoul lateral

- **Data.sessionStartTime** - marcă de timp UTC privind momentul în care a început sesiunea de traducere

- **Data.sourceTextHash** - codul hash al textului de tradus

- **Data.sourceTextLength** - lungime text de tradus

- **Data.sourceTextWords** - număr de cuvinte în textul de tradus

- **Data.warningMessage** - mesaj de avertisment raportat de serviciu


#### <a name="officevisiosharedfeatureexperimentation"></a>Office.Visio.Shared.FeatureExperimentation

Urmărește configurația „flighting” a caracteristicii pentru utilizatori. Acest eveniment ne ajută să determinăm succesul sau eșecul edițiilor flight ale caracteristicilor.

Se colectează următoarele câmpuri:

  - **Data\_Enable:bool** – true în cazul în care caracteristica este activată pentru utilizatorul curent

  - **Data\_Feature:string** – numele caracteristicii

  - **Data\_Flighted:bool** – true în cazul în care caracteristica este activată

  - **Data\_Licensed:bool** – true în cazul în care caracteristica este sub verificarea de licențiere

  - **Data\_Subscriber:bool** – true arată că utilizatorul are licență cu abonament

#### <a name="officevisiosharedrefreshsmartdiagram"></a>Office.Visio.Shared.RefreshSmartDiagram

Capturează erorile de reîmprospătare a diagramei atunci când fișierul este creat prin DV. Aceasta ne ajută să depanăm erorile și problemele din reîmprospătarea datelor dintr-o diagramă DV.

Se colectează următoarele câmpuri:

  - **Data\_ConnectorsBasedOnSequence:bool** – true dacă diagrama reîmprospătată a fost creată inițial utilizând conectorul bazat pe opțiunea „secvență”

  - **Data\_DialogError** : **string** – eroare în timpul reîmprospătării diagramei inteligente

  - **Data\_FileError:string** – șir de eroare atunci când fișierul Excel conectat este nevalid

  - **Data\_OverwriteSelected** : **bool** – true dacă utilizatorul a selectat opțiunea de înlocuire a diagramei în timpul reîmprospătării

  - **Data\_WarningShown** : **bool** – true dacă utilizatorul a văzut vreun avertisment în timpul reîmprospătării datelor

#### <a name="officevisiosharedwritebacktoexcel"></a>Office.Visio.Shared.WritebackToExcel

Capturează erorile de răspuns Excel atunci când fișierul este creat prin DV. Aceasta ne ajută să depanăm erorile și problemele din răspunsul la date Excel dintr-o diagramă DV.

Se colectează următoarele câmpuri:

  - **Data\_ConnectorsBasedOnSequence:bool** – true atunci când conectorii sunt creați în funcție de setările de secvență

  - **Data\_DataSourceType:string** – acest fișier indică dacă diagrama este creată din „Tabel” sau „Interval particularizat”

  - **Data\_DialogError:string** – tip de eroare particularizată în timpul creării diagramei inteligente prin Excel

  - **Data\_NoOfShapesAdded:int** – numărul de forme adăugate în timpul funcționalității writeback Excel

  - **Data\_NoOfShapesDeleted:int** – numărul de forme șterse în timpul funcționalității writeback Excel

  - **Data\_OverwriteSelected:bool** – true dacă utilizatorul a selectat opțiunea de înlocuire a datelor

  - **Data\_SourceDataModified:bool** – true dacă s-au modificat datele sursă

  - **Data\_WarningShown:bool** – true înseamnă că utilizatorul primește un avertisment privind actualizarea datelor

  - **Data\_WarningShownBecauseOfPresenceOfFormula:bool** – true înseamnă că utilizatorul primește un avertisment din cauza prezenței formulei în Excel

  - **Data\_WarningShownToAddNextStepID:bool** – true înseamnă că utilizatorul primește un avertisment, deoarece identificatorul pentru pasul următor lipsește din Excel

  - **Data\_WarningShownToConvertToTable:bool** – true înseamnă că utilizatorul primește un avertisment pentru a efectua conversia datelor Excel în format de tabel


#### <a name="officewordfilenewcreatenewfile"></a>Office.Word.FileNew.CreateNewFile

Acest eveniment indică faptul că un document nou este creat în Office Word și urmărește succesul sau nereușita operațiunii. Evenimentul este utilizat pentru a monitoriza dacă crearea noului document funcționează conform așteptărilor. În plus, se folosește pentru a calcula utilizatorii/dispozitivele active lunar și măsurătorile de fiabilitate cloud.

Se colectează următoarele câmpuri:

  - **Data\_DirtyState** - dacă documentul a fost creat într-o stare cu erori (cu modificări care trebuie salvate)

  - **Data\_ErrorID** - identificator de eroare în cazul unei operații nereușite

  - **Data\_MainPdod -** identificatorul documentului din timpul acestei sesiuni de proces

  - **Data\_UsesCustomTemplate** - indică dacă documentul a fost creat pornind de la un șablon particularizat

#### <a name="officewordfileopenuserinitiatedopen"></a>Office.Word.FileOpen.UserInitiatedOpen 

Acest eveniment indică faptul că Office Word deschide un document la inițiativa utilizatorului și nu prin programare de către Office Word. În plus, conține date esențiale despre performanța la deschiderea fișierelor și este un eveniment de pornire a aplicației din perspectiva utilizatorului.  Evenimentul monitorizează dacă deschiderea fișierelor funcționează așa cum trebuie. În plus, se folosește pentru a calcula utilizatorii/dispozitivele active lunar și măsurătorile de fiabilitate cloud. 
 
Se colectează următoarele câmpuri:

- **Data_AddDocTelemRes** - raportează dacă am putut completa corect alte valori legate de telemetria documentelor din eveniment. Utilizat pentru diagnostice privind calitatea datelor. 

- **Data_BytesAsynchronous** - numărul de byți (comprimat) fără care credem că putem deschide fișierul dacă îi obținem înainte ca utilizatorul să vrea să editeze sau să salveze. 

- **Data_BytesAsynchronousWithWork** - numărul de byți (comprimat) fără care credem că putem deschide fișierul, dar care ar necesita investiții de cod semnificative pentru a funcționa 

- **Data_BytesSynchronous** - numărul de byți (comprimat) de care avem nevoie înainte să putem deschide fișierul 

- **Data_BytesUnknown** - numărul de byți din părțile de documente pe care nu ne așteptăm să le găsim 

- **Data_Doc_AccessMode** - documentul este numai în citire/editabil 

- **Data_Doc_AssistedReadingReasons** - set predefinit de valori privind motivul pentru care documentul a fost deschis în modul de citire asistată 

- **Data_Doc_ChunkingType** - unități utilizate pentru deschiderea incrementală a documentelor 

- **Data_Doc_EdpState** - setare de protecție a datelor electronice pentru document 

- **Data_Doc_Ext** - extensia documentului (docx/xlsb/pptx etc.) 

- **Data_Doc_FileFormat** - versiunea de protocol pentru formatul fișierului 

- **Data_Doc_Fqdn** - numele de domeniu OneDrive sau SharePoint Online 

- **Data_Doc_FqdnHash** - codul hash unidirecțional pentru numele de domeniu identificabil al clientului 

- **Data_Doc_IdentityTelemetryId** - codul hash unidirecțional pentru identitatea de utilizator folosită pentru deschidere 

- **Data_Doc_InitializationScenario** - înregistrează cum a fost deschis documentul 

- **Data_Doc_IOFlags** - rapoarte privind semnalizările memorate în cache folosite pentru a seta opțiuni de solicitare deschise 

- **Data_Doc_IrmRights** - acțiunile permise de politica de protejare a datelor electronice aplicată pentru document/utilizator 

- **Data_Doc_IsIncrementalOpen** - semnalizare care indică faptul că documentul a fost deschis incremental 

- **Data_Doc_IsOcsSupported** - semnalizare care indică faptul că documentul este acceptat în serviciul de colaborare 

- **Data_Doc_IsOpeningOfflineCopy** - semnalizare care indică faptul că s-a deschis copia offline a unui document 

- **Data_Doc_IsSyncBacked** - semnalizare care indică faptul că pe computer există o copie sincronizată automat a documentului 

- **Data_Doc_Location** - indică ce serviciu a furnizat documentul (OneDrive, File Server, SharePoint) 

- **Data_Doc_LocationDetails** - indică ce Folder cunoscut a furnizat un document stocat local 

- **Data_Doc_NumberCoAuthors** - numărul de alți utilizatori dintr-o sesiune de editare în colaborare 

- **Data_Doc_PasswordFlags** - arată semnalizările de parole pentru citire sau citire/scriere setate 

- **Data_Doc_ReadOnlyReasons** - motivele pentru care documentul a fost deschis doar în citire 

- **Data_Doc_ResourceIdHash** - identificator de document anonimizat, folosit în diagnosticarea problemelor 

- **Data_Doc_ServerDocId** - identificator de document anonimizat și invariabil, folosit în diagnosticarea problemelor 

- **Data_Doc_ServerProtocol** - versiunea de protocol folosită în comunicarea cu serviciul 

- **Data_Doc_ServerType** - tipul de server care oferă serviciul (SharePoint, OneDrive, WOPI etc.) 

- **Data_Doc_ServerVersion** - versiunea serverului care oferă serviciul 

- **Data_Doc_SessionId** - versiunea serverului care oferă serviciul 

- **Data_Doc_SharePointServiceContext** - informații de diagnosticare din solicitările SharePoint Online 

- **Data_Doc_SizeInBytes** - indicator privind dimensiunea documentului 

- **Data_Doc_SpecialChars** - indicator privind caracterele speciale din calea sau adresa URL a documentului 

- **Data_Doc_StreamAvailability** - indicator care arată dacă șirul documentului este disponibil/dezactivat 

- **Data_Doc_SyncBackedType** - indicator privind tipul documentului (local sau bazat pe servicii) 

- **Data_Doc_UrlHash** - cod hash unidirecțional, pentru crearea unui identificator naiv de document 

- **Data_Doc_WopiServiceId** - conține identificatorul unic al furnizorului de servicii WOPI 

- **Data_EditorDisablingRename** - identificatorul primului editor care a provocat dezactivarea redenumirii 

- **Data_EditorsCount** - numărul de editori din document 

- **Data_ForceReadWriteReason** - valoare întreagă care reprezintă motivul pentru care fișierul a fost forțat în modul citire/scriere 

- **Data_FSucceededAfterRecoverableFailure** - arată că deschiderea a reușit după repararea unei erori la deschiderea documentului 

- **Data_LastLoggedTag** - etichetă unică pentru site-ul de apelare a codului folosit pentru a identifica momentele când încercăm să nu realizăm deschiderea de două ori (folosit pentru diagnosticarea calității datelor) 

- **Data_LinkStyles** - indică dacă asociem stiluri de șabloane 

- **Data_MainPdod** - identificatorul documentului din procesul Office Word 

- **Data_Measurements** - șir codificat cu detalii de timp pentru diferitele părți ale deschiderii. Utilizat pentru a diagnostica performanța de deschidere. 

- **Data_MoveDisabledReason** - eroarea care dezactivează mutarea pentru document 

- **Data_MoveFlightEnabled** - dacă ediția flight este activată pentru caracteristica de mutare 

- **Data_OpenInitiateKind** - tipul scenariului în care utilizatorii au pornit operațiunea de deschidere a fișierului. 

- **Data_PartsUnknown** - numărul de părți ale documentului pentru care nu am putut obține date 

- **Data_RecoverableFailureInitiationLocationTag** - etichetă unică pentru site-ul de apelare a codului folosit pentru a identifica locul din cod în care încercăm să remediem fișierul înainte de a-l deschide 

- **Data_RenameDisabledReason** - eroare care face redenumirea să fie dezactivată pentru acest document 

- **Data_RenameFlightEnabled** - dacă este activată ediția flight pentru caracteristica de redenumire 

- **Data_SecondaryTag** - etichetă unică pentru site-ul de apelare a codului folosit pentru a adăuga date suplimentare despre erori pentru deschidere. 

- **Data_TemplateFormat** - formatul de fișier al șablonului pe care se bazează documentul 

- **Data_UsesNormal** - indică dacă documentul deschis se bazează pe șablonul normal. 

- **Data_VerboseMeasurements** - șir codificat cu detalii de timp pentru diferitele părți ale deschiderii.  Utilizat pentru măsurarea performanței, activat doar pentru inelele interne. 



#### <a name="officewordfilesaveactcmdgosubsaveas"></a>Office.Word.FileSave.ActCmdGosubSaveAs

Acest eveniment indică faptul că un utilizator salvează modificările într-un document nou. Evenimentul monitorizează dacă salvarea într-un document nou funcționează conform așteptărilor. În plus, se folosește pentru a calcula utilizatorii/dispozitivele active lunar și măsurătorile de fiabilitate cloud.

Se colectează următoarele câmpuri:

- **Data_AddDocTelemRes** - raportează dacă am putut completa corect alte valori legate de telemetria documentelor din eveniment. Utilizat pentru diagnostice privind calitatea datelor.

- **Data_DetachedDuration** - cât timp a fost activitatea detașată de fir

- **Data_Doc_AccessMode** - documentul este numai în citire/editabil

- **Data_Doc_AssistedReadingReasons** - set predefinit de valori privind motivul pentru care documentul a fost deschis în modul de citire asistată

- **Data_Doc_AsyncOpenKind –** indică dacă s-a deschis o versiune memorată în cache a documentului cloud și ce logică de reîmprospătare asincronă s-a folosit.

- **Data_Doc_ChunkingType** - unități utilizate pentru deschiderea incrementală a documentelor

- **Data_Doc_EdpState** - setare de protecție a datelor electronice pentru document

- **Data_Doc_Ext** - extensia documentului (docx/xlsb/pptx etc.)

- **Data_Doc_FileFormat** - versiunea de protocol pentru formatul fișierului

- **Data_Doc_Fqdn** - numele de domeniu OneDrive sau SharePoint Online

- **Data_Doc_FqdnHash** - codul hash unidirecțional pentru numele de domeniu identificabil al clientului

- **Data_Doc_IdentityTelemetryId** - codul hash unidirecțional pentru identitatea de utilizator folosită pentru deschidere

- **Data_Doc_InitializationScenario** - înregistrează cum a fost deschis documentul

- **Data_Doc_IOFlags** - rapoarte privind semnalizările memorate în cache folosite pentru a seta opțiuni de solicitare deschise

- **Data_Doc_IrmRights** - acțiunile permise de politica de protejare a datelor electronice aplicată pentru document/utilizator
    
- **Data_Doc_IsIncrementalOpen** - semnalizare care indică faptul că documentul a fost deschis incremental

- **Data_Doc_IsOcsSupported** - semnalizare care indică faptul că documentul este acceptat în serviciul de colaborare
    
- **Data_Doc_IsOpeningOfflineCopy** - semnalizare care indică faptul că s-a deschis copia offline a unui document

- **Data_Doc_IsSyncBacked** - semnalizare care indică faptul că pe computer există o copie sincronizată automat a documentului

- **Data_Doc_Location** - indică ce serviciu a furnizat documentul (OneDrive, File Server, SharePoint etc.)

- **Data_Doc_LocationDetails** - indică ce Folder cunoscut a furnizat un document stocat local

- **Data_Doc_NumberCoAuthors** - numărul de alți utilizatori dintr-o sesiune de editare în colaborare

- **Data_Doc_PasswordFlags** - arată semnalizările de parole pentru citire sau citire/scriere setate

- **Data_Doc_ReadOnlyReasons** - motivele pentru care documentul a fost deschis doar în citire

- **Data_Doc_ResourceIdHash** - identificator de document anonimizat, folosit în diagnosticarea problemelor

- **Data_Doc_RtcType** - indică modul în care a fost configurat canalul în timp real (RTC) pentru fișierul curent (dezactivat, neacceptat, la cerere, activat permanent etc.).

- **Data_Doc_ServerDocId** - identificator de document anonimizat și invariabil, folosit în diagnosticarea problemelor

- **Data_Doc_ServerProtocol** - versiunea de protocol folosită în comunicarea cu serviciul

- **Data_Doc_ServerType** - tipul de server care oferă serviciul (SharePoint, OneDrive, WOPI etc.)

- **Data_Doc_ServerVersion** - versiunea serverului care oferă serviciul

- **Data_Doc_SessionId** - identifică o anumită sesiune de editare a documentului din sesiunea completă

- **Data_Doc_SharePointServiceContext** - informații de diagnosticare din solicitările SharePoint Online

- **Data_Doc_SizeInBytes** - indicator privind dimensiunea documentului

- **Data_Doc_SpecialChars** - indicator privind caracterele speciale din calea sau adresa URL a documentului

- **Data_Doc_StreamAvailability** - indicator care arată dacă șirul documentului este disponibil/dezactivat

- **Data_Doc_SyncBackedType** - indicator privind tipul documentului (local sau bazat pe servicii)

- **Data_Doc_UrlHash** - cod hash unidirecțional, pentru crearea unui identificator naiv de document

- **Data_EditorDisablingRename** - identificatorul primului editor care a provocat dezactivarea redenumirii

- **Data_EditorsCount** - numărul de editori din document

- **Data_LastLoggedTag** - etichetă unică pentru site-ul de apelare a codului folosit pentru a identifica momentele când nu reușim să încercăm salvarea de două ori (folosit pentru diagnosticarea calității datelor)

- **Data_MoveDisabledReason** - eroarea care dezactivează mutarea pentru document

- **Data_MoveFlightEnabled** - dacă ediția flight este activată pentru caracteristica de mutare

- **Data_RenameDisabledReason** - eroare care face redenumirea să fie dezactivată pentru document

- **Data_RenameFlightEnabled** - dacă este activată ediția flight pentru caracteristica de redenumire

    

#### <a name="officewordfilesaveactfconfirmsavedoccorequerysave"></a>Office.Word.FileSave.ActFConfirmSaveDocCoreQuerySave

Acest eveniment indică faptul că Office Word îi solicită utilizatorului să salveze modificările atunci când încearcă să închidă documentul. Acesta permite Microsoft să monitorizeze dacă salvare-la-ieșire funcționează conform așteptărilor pentru a se evita pierderea de date din documente. Evenimentul monitorizează dacă salvare-la-ieșire funcționează conform așteptărilor. În plus, se folosește pentru a calcula utilizatorii/dispozitivele active lunar și măsurătorile de fiabilitate cloud.

Se colectează următoarele câmpuri:

- **Data_AddDocTelemRes** - raportează dacă am putut completa corect alte valori legate de telemetria documentelor din eveniment. Utilizat pentru diagnostice privind calitatea datelor.

- **Data_DetachedDuration** - cât timp a fost activitatea detașată de fir

- **Data_Doc_AccessMode** - documentul este numai în citire/editabil

- **Data_Doc_AssistedReadingReasons** - set predefinit de valori privind motivul pentru care documentul a fost deschis în modul de citire asistată

- **Data_Doc_AsyncOpenKind –** indică dacă s-a deschis o versiune memorată în cache a documentului cloud și ce logică de reîmprospătare asincronă s-a folosit.

- **Data_Doc_ChunkingType** - unități utilizate pentru deschiderea incrementală a documentelor

- **Data_Doc_EdpState** - setare de protecție a datelor electronice pentru document

- **Data_Doc_Ext** - extensia documentului (docx/xlsb/pptx etc.)

- **Data_Doc_FileFormat** - versiunea de protocol pentru formatul fișierului

- **Data_Doc_Fqdn** - numele de domeniu OneDrive sau SharePoint Online

- **Data_Doc_FqdnHash** - codul hash unidirecțional pentru numele de domeniu identificabil al clientului

- **Data_Doc_IdentityTelemetryId** - codul hash unidirecțional pentru identitatea de utilizator folosită pentru deschidere

- **Data_Doc_InitializationScenario** - înregistrează cum a fost deschis documentul

- **Data_Doc_IOFlags** - rapoarte privind semnalizările memorate în cache folosite pentru a seta opțiuni de solicitare deschise

- **Data_Doc_IrmRights** - acțiunile permise de politica de protejare a datelor electronice aplicată pentru document/utilizator

- **Data_Doc_IsIncrementalOpen** - semnalizare care indică faptul că documentul a fost deschis incremental

- **Data_Doc_IsOcsSupported** - semnalizare care indică faptul că documentul este acceptat în serviciul de colaborare
    
- **Data_Doc_IsOpeningOfflineCopy** - semnalizare care indică faptul că s-a deschis copia offline a unui document

- **Data_Doc_IsSyncBacked** - semnalizare care indică faptul că pe computer există o copie sincronizată automat a documentului

- **Data_Doc_Location** - indică ce serviciu a furnizat documentul (OneDrive, File Server, SharePoint etc.)

- **Data_Doc_LocationDetails** - indică ce Folder cunoscut a furnizat un document stocat local

- **Data_Doc_NumberCoAuthors** - numărul de alți utilizatori dintr-o sesiune de editare în colaborare

- **Data_Doc_PasswordFlags** - arată semnalizările de parole pentru citire sau citire/scriere setate

- **Data_Doc_ReadOnlyReasons** - motivele pentru care documentul a fost deschis doar în citire

- **Data_Doc_ResourceIdHash** - identificator de document anonimizat, folosit în diagnosticarea problemelor

- **Data_Doc_RtcType** - indică modul în care a fost configurat canalul în timp real (RTC) pentru fișierul curent (dezactivat, neacceptat, la cerere, activat permanent etc.).

- **Data_Doc_ServerDocId** - identificator de document anonimizat și invariabil, folosit în diagnosticarea problemelor

- **Data_Doc_ServerProtocol** - versiunea de protocol folosită în comunicarea cu serviciul

- **Data_Doc_ServerType** - tipul de server care oferă serviciul (SharePoint, OneDrive, WOPI etc.)

- **Data_Doc_ServerVersion** - versiunea serverului care oferă serviciul

- **Data_Doc_SessionId** - identifică o anumită sesiune de editare a documentului din sesiunea completă

- **Data_Doc_SharePointServiceContext** - informații de diagnosticare din solicitările SharePoint Online

- **Data_Doc_SizeInBytes** - indicator privind dimensiunea documentului

- **Data_Doc_SpecialChars** - indicator privind caracterele speciale din calea sau adresa URL a documentului

- **Data_Doc_StreamAvailability** - indicator care arată dacă șirul documentului este disponibil/dezactivat

- **Data_Doc_SyncBackedType** - indicator privind tipul documentului (local sau bazat pe servicii)

- **Data_Doc_UrlHash** - cod hash unidirecțional, pentru crearea unui identificator naiv de document

- **Data_Doc_WopiServiceId** - conține identificatorul unic al furnizorului de servicii WOPI

- **Data_DstDoc_AccessMode** - documentul de destinație este doar în citire/editabil

- **Data_DstDoc_EdpState** - setare de protecție a datelor electronice pentru documentul de destinație

- **Data_DstDoc_Ext** - Extensia (docx/xlsb/pptx, etc.) documentului de destinație

- **Data_DstDoc_FileFormat** - Versiunea protocolului de format fișier pentru documentul de destinație

- **Data_DstDoc_Location** - indică serviciul care va oferi spațiu de stocare pentru documentul de destinație (OneDrive, File Server, SharePoint etc.)

- **Data_DstDoc_LocationDetails** - indică Folderul cunoscut local care a stocat documentul de destinație

- **Data_DstDoc_SessionId** - identifică o anumită sesiune de editare a documentului din sesiunea completă

- **Data_DstDoc_UrlHash** - cod hash într-o singură direcție pentru crearea unui identificator naiv pentru documentul de destinație

- **Data_FailureClass** - întreg care reprezintă clasa de eroare pentru erorile de tranziție OCS

- **Data_LocationPickerSaveStatus** - valoare întreagă care indică acțiunea care a declanșat salvarea din caseta de dialog salvare la ieșire

- **Data_MainPdod** - Identificatorul documentului din procesul Office Word

- **Data_MoveFlightEnabled** - dacă ediția flight este activată pentru caracteristica de mutare

- **Data_OCSSyncbackSaveStarted** - marcaj care arată că această salvare este legată de salvarea de sincronizare inversă 

- **Data_RenameDisabledReason** - eroare care face redenumirea să fie dezactivată pentru acest document

- **Data_RenameFlightEnabled** - dacă este activată ediția flight pentru caracteristica de redenumire

- **Data_SaveInitiateKind** - întreg care arată cum s-a inițiat salvarea

- **Data_SrcDocIsUnnamedOrNew** - indică dacă documentul pe care îl salvăm este nou


#### <a name="officewordfilesavesaveassavefile"></a>Office.Word.FileSave.SaveAsSaveFile

Acest eveniment indică faptul că Office Word salvează un document într-un document nou. Acest lucru permite ca Microsoft să detecteze erorile din acțiunea de „salvare ca”, lucru important pentru a evita pierderea datelor din documente. Evenimentul monitorizează dacă „salvarea ca” funcționează așa cum vă așteptați. În plus, se folosește pentru a calcula utilizatorii/dispozitivele active lunar și măsurătorile de fiabilitate cloud.

Se colectează următoarele câmpuri:

- **Data_AddDocTelemRes** - raportează dacă am putut completa corect alte valori legate de telemetria documentelor din eveniment. Utilizat pentru diagnostice privind calitatea datelor.

- **Data_AddDocTelemResDst** - raportează dacă am putut completa corect alte valori legate de telemetria documentelor din eveniment pentru documentul de destinație. Utilizat pentru diagnostice privind calitatea datelor.

- **Data_AddDocTelemResSrc** - raportează dacă am putut completa corect alte valori legate de telemetria documentelor din eveniment pentru documentul sursă. Utilizat pentru diagnostice privind calitatea datelor.

- **Data_DetachedDuration** - cât timp a fost activitatea detașată de fir

- **Data_Doc_AccessMode** - documentul este numai în citire/editabil

- **Data_Doc_AssistedReadingReasons** - set predefinit de valori privind motivul pentru care documentul a fost deschis în modul de citire asistată

- **Data_Doc_AsyncOpenKind –** indică dacă s-a deschis o versiune memorată în cache a documentului cloud și ce logică de reîmprospătare asincronă s-a folosit.

- **Data_Doc_ChunkingType** - unități utilizate pentru deschiderea incrementală a documentelor

- **Data_Doc_EdpState** - setare de protecție a datelor electronice pentru document

- **Data_Doc_Ext** - extensia documentului (docx/xlsb/pptx etc.)

- **Data_Doc_FileFormat** - versiunea de protocol pentru formatul fișierului

- **Data_Doc_Fqdn** - numele de domeniu OneDrive sau SharePoint Online

- **Data_Doc_FqdnHash** - codul hash unidirecțional pentru numele de domeniu identificabil al clientului

- **Data_Doc_IdentityTelemetryId** - codul hash unidirecțional pentru identitatea de utilizator folosită pentru deschidere

- **Data_Doc_IOFlags** - rapoarte privind semnalizările memorate în cache folosite pentru a seta opțiuni de solicitare deschise

- **Data_Doc_IrmRights** - acțiunile permise de politica de protejare a datelor electronice aplicată pentru document/utilizator

- **Data_Doc_IsIncrementalOpen** - semnalizare care indică faptul că documentul a fost deschis incremental

- **Data_Doc_IsOcsSupported** - semnalizare care indică faptul că documentul este acceptat în serviciul de colaborare

- **Data_Doc_IsOpeningOfflineCopy** - semnalizare care indică faptul că s-a deschis copia offline a unui document

- **Data_Doc_IsSyncBacked** - semnalizare care indică faptul că pe computer există o copie sincronizată automat a documentului

- **Data_Doc_Location** - indică ce serviciu a furnizat documentul (OneDrive, File Server, SharePoint etc.)

- **Data_Doc_LocationDetails** - indică ce Folder cunoscut a furnizat un document stocat local

- **Data_Doc_NumberCoAuthors** - numărul de alți utilizatori dintr-o sesiune de editare în colaborare

- **Data_Doc_ReadOnlyReasons** - motivele pentru care documentul a fost deschis doar în citire

- **Data_Doc_ResourceIdHash** - identificator de document anonimizat, folosit în diagnosticarea problemelor

- **Data_Doc_RtcType** - indică modul în care a fost configurat canalul în timp real (RTC) pentru fișierul curent (dezactivat, neacceptat, la cerere, activat permanent etc.).

- **Data_Doc_ServerDocId** - identificator de document anonimizat și invariabil, folosit în diagnosticarea problemelor

- **Data_Doc_ServerProtocol** - versiunea de protocol folosită în comunicarea cu serviciul

- **Data_Doc_ServerType** - tipul de server care oferă serviciul (SharePoint, OneDrive, WOPI etc.)

- **Data_Doc_ServerVersion** - versiunea serverului care oferă serviciul

- **Data_Doc_SessionId** - identifică o anumită sesiune de editare a documentului din sesiunea completă

- **Data_Doc_SharePointServiceContext** - informații de diagnosticare din solicitările SharePoint Online

- **Data_Doc_SizeInBytes** - indicator privind dimensiunea documentului

- **Data_Doc_SpecialChars** - indicator privind caracterele speciale din calea sau adresa URL a documentului

- **Data_Doc_StreamAvailability** - indicator care arată dacă șirul documentului este disponibil/dezactivat

- **Data_Doc_UrlHash** - cod hash unidirecțional, pentru crearea unui identificator naiv de document

- **Data_DstDoc_AccessMode** - documentul de destinație este doar în citire/editabil

- **Data_DstDoc_AssistedReadingReasons** - set predefinit de valori privind motivul pentru care documentul de destinație a fost deschis în modul de citire asistată

- **Data_DstDoc_AsyncOpenKind –** indică dacă s-a deschis o versiune memorată în cache a noului document cloud și ce logică de reîmprospătare asincronă s-a folosit.
    
- **Data_DstDoc_ChunkingType** - unități utilizate pentru deschiderea incrementală a documentelor

- **Data_DstDoc_EdpState** - setare de protecție a datelor electronice pentru documentul de destinație

- **Data_DstDoc_Ext** - extensia documentului (docx/xlsb/pptx etc.)

- **Data_DstDoc_FileFormat** - versiunea de protocol pentru formatul fișierului

- **Data_DstDoc_Fqdn** - numele de domeniu OneDrive sau SharePoint Online pentru documentul de destinație

- **Data_DstDoc_FqdnHash** - cod hash într-o singură direcție pentru numele de domeniu identificabil de client pentru documentul de destinație

- **Data_DstDoc_IdentityTelemetryId** - codul hash unidirecțional pentru identitatea de utilizator folosită pentru deschidere

- **Data_DstDoc_InitializationScenario** - înregistrează cum a fost deschis documentul de destinație

- **Data_DstDoc_IOFlags** - rapoarte privind marcajele memorate în cache folosite pentru a seta opțiunile de deschidere a solicitărilor pentru documentul de destinație
    
- **Data_DstDoc_IrmRights** - acțiunile permise de politica de protejare a datelor electronice aplicată pentru documentul de destinație/utilizator

- **Data_DstDoc_IsIncrementalOpen** - semnalizare care indică faptul că documentul a fost deschis incremental

- **Data_DstDoc_IsOcsSupported** - semnalizare care indică faptul că documentul este acceptat în serviciul de colaborare

- **Data_DstDoc_IsOpeningOfflineCopy** - semnalizare care indică faptul că s-a deschis copia offline a unui document

- **Data_DstDoc_IsSyncBacked** - semnalizare care arată că pe computer există o copie sincronizată automat a documentului

- **Data_DstDoc_Location** - indică serviciul care a oferit spațiul de stocare pentru documentul de destinație (OneDrive, File Server, SharePoint etc.)

- **Data_DstDoc_LocationDetails** - indică ce Folder cunoscut a furnizat un document stocat local

- **Data_DstDoc_NumberCoAuthors** - numărul de alți utilizatori dintr-o sesiune de editare în colaborare

- **Data_DstDoc_PasswordFlags** - arată marcajele de parole pentru citire sau citire/scriere setate pentru documentul de destinație

- **Data_DstDoc_ReadOnlyReasons** - motivele pentru care documentul de destinație a fost deschis doar în citire 

- **Data_DstDoc_ResourceIdHash** - identificator de document anonimizat, folosit în diagnosticarea problemelor

- **Data_DstDoc_ServerDocId** - identificator de document anonimizat și invariabil, folosit în diagnosticarea problemelor

- **Data_DstDoc_ServerProtocol** - versiunea de protocol folosită în comunicarea cu serviciul

- **Data_DstDoc_ServerType** - tipul de server care oferă serviciul (SharePoint, OneDrive, WOPI etc.)
    
- **Data_DstDoc_ServerVersion** - versiunea serverului care oferă serviciul

- **Data_DstDoc_SessionId** - identifică o anumită sesiune de editare a documentului din sesiunea completă

- **Data_DstDoc_SharePointServiceContext** - informații de diagnosticare din solicitările SharePoint Online

- **Data.Doc.SizeInBytes -** indicator privind dimensiunea documentului

- **Data_DstDoc_SpecialChars** - indicator privind caracterele speciale din calea sau adresa URL a documentului

- **Data_DstDoc_StreamAvailability** - indicator care arată dacă șirul documentului este disponibil/dezactivat

- **Data_DstDoc_SyncBackedType** - indicator privind tipul documentului (local sau bazat pe servicii)

- **Data_DstDoc_UrlHash** - cod hash într-o singură direcție pentru crearea unui identificator naiv pentru documentul de destinație
    
- **Data_DstDoc_WopiServiceId** - conține identificatorul unic al furnizorului de servicii WOPI

- **Data_FailureClass** - întreg care reprezintă clasa de eroare pentru erorile de tranziție OCS

- **Data_LocationPickerPropagateToSaveTime,spLapsedMsec** - măsoară timpul, în milisecunde, necesar pentru declanșarea salvării după ce s-a obținut un rezultat din selectorul de locații

- **Data_LocationPickerSaveStatus** - starea returnate de selectorul de locații

- **Data_MainPdod** - identificatorul documentului din procesul Office Word

- **Data_MoveDisabledReason** - eroarea care dezactivează mutarea pentru document

- **Data_MoveFlightEnabled** - dacă ediția flight este activată pentru caracteristica de mutare

- **Data_RenameDisabledReason** - eroare care face redenumirea să fie dezactivată pentru acest document

- **Data_RenameFlightEnabled** - dacă este activată ediția flight pentru caracteristica de redenumire

- **Data_SaveInitiateKind** - întreg care arată cum s-a inițiat salvarea

- **Data_SrcDoc_AccessMode** - documentul sursă este doar în citire/editabil

- **Data_SrcDoc_AssistedReadingReasons** - set predefinit de valori privind motivul pentru care documentul a fost deschis în modul de citire asistată

- **Data_SrcDoc_AsyncOpenKind –** indică dacă s-a deschis o versiune memorată în cache a documentului cloud original și ce logică de reîmprospătare asincronă s-a folosit.

- **Data_SrcDoc_ChunkingType** - unități utilizate pentru deschiderea incrementală a documentelor

- **Data_SrcDoc_EdpState** - setare de protecție a datelor electronice pentru documentul sursă

- **Data_SrcDoc_Ext** - Extensia documentului sursă (docx/xlsb/pptx etc.)

- **Data_SrcDoc_FileFormat** - Versiunea protocolului de format fișier pentru documentul sursă

- **Data_SrcDoc_Fqdn** - numele de domeniu OneDrive sau SharePoint Online pentru documentul sursă

- **Data_SrcDoc_FqdnHash** - cod hash într-o singură direcție pentru numele de domeniu identificabil de client pentru documentul sursă

- **Data_SrcDoc_IdentityTelemetryId** - codul hash unidirecțional pentru identitatea de utilizator folosită pentru deschidere

- **Data_SrcDoc_InitializationScenario** - înregistrează cum a fost deschis documentul

- **Data_SrcDoc_IOFlags** - rapoarte privind marcajele memorate în cache folosite pentru a seta opțiunile de deschidere a solicitărilor

- **Data_SrcDoc_IrmRights** - acțiunile permise de politica de protejare a datelor electronice aplicată pentru document/utilizator

- **Data_SrcDoc_IsIncrementalOpen** - semnalizare care indică faptul că documentul a fost deschis incremental

- **Data_SrcDoc_IsOcsSupported** - semnalizare care indică faptul că documentul este acceptat în serviciul de colaborare

- **Data_SrcDoc_IsOpeningOfflineCopy** - semnalizare care indică faptul că s-a deschis copia offline a unui document

- **Data_SrcDoc_IsSyncBacked** - semnalizare care arată că pe computer există o copie sincronizată automat a documentului
    
- **Data_SrcDoc_Location** - arată ce serviciu a furnizat documentul sursă (OneDrive, File Server, SharePoint etc.)

- **Data_SrcDoc_LocationDetails** - indică ce Folder cunoscut a furnizat un document stocat local

- **Data_SrcDoc_NumberCoAuthors** - numărul de alți utilizatori dintr-o sesiune de editare în colaborare

- **Data_SrcDoc_PasswordFlags** - arată semnalizările de parole pentru citire sau citire/scriere setate

- **Data_SrcDoc_ReadOnlyReasons** - motivele pentru care documentul a fost deschis doar în citire

- **Data_SrcDoc_ResourceIdHash** - identificator de document anonimizat, folosit în diagnosticarea problemelor

- **Data_SrcDoc_ServerDocId** - identificator de document anonimizat și invariabil, folosit în diagnosticarea problemelor

- **Data_SrcDoc_ServerProtocol** - versiunea de protocol folosită în comunicarea cu serviciul

- **Data_SrcDoc_ServerType** - tipul de server care oferă serviciul (SharePoint, OneDrive, WOPI etc.)

- **Data_SrcDoc_ServerVersion** - versiunea serverului care oferă serviciul

- **Data_SrcDoc_SessionId** - identifică o anumită sesiune de editare a documentului din sesiunea completă

- **Data_SrcDoc_SharePointServiceContext** - informații de diagnosticare din solicitările SharePoint Online

- **Data_SrcDoc_SizeInBytes** - indicator privind dimensiunea documentului

- **Data_SrcDoc_SpecialChars** - indicator privind caracterele speciale din calea sau adresa URL a documentului

- **Data_SrcDoc_StreamAvailability** - indicator care arată dacă șirul documentului este disponibil/dezactivat

- **Data_SrcDoc_SyncBackedType** - indicator privind tipul documentului (local sau bazat pe servicii)

- **Data_SrcDoc_UrlHash** - cod hash unidirecțional, pentru crearea unui identificator naiv de document

- **Data_SrcDoc_WopiServiceId** - conține identificatorul unic al furnizorului de servicii WOPI

- **Data_SrcDocIsUnnamedOrNew** - indică dacă documentul pe care îl salvăm este nou


#### <a name="officewordworddocumentdirtyflagchanged"></a>Office.Word.Word.DocumentDirtyFlagChanged

Acest eveniment indică faptul că Office Word editează un document care modifică starea internă a documentului în „defazată”. Astfel, Microsoft poate evalua starea de funcționare a caracteristicii pentru documentul editat. Evenimentul este un mesaj repetat din editările utilizatorului. În plus, se folosește pentru a calcula utilizatorii/dispozitivele active lunar.

Se colectează următoarele câmpuri:

  - **Data\_CollectionTime –** marca de timp a evenimentului

  - **Data\_DocumentLocation–** tipul locației documentului

  - **Data\_DocumentLocationDetails –** subtipul locației documentului

  - **Data\_FAlwaysSaveEnabled –** Indică dacă s-a activat salvarea permanentă

  - **Data\_FirstEditTime –** marca de timp a primei editări

  - **Data\_NumberCoAuthors –** numărul de coautori care editează documentul în timpul sesiunii

  - **Data\_NumberOfTimesDocumentDirtied –** numărul de editări ale documentului

  - **Data\_Pdod –** identificatorul documentului din procesul Office Word

  - **Data\_UrlHash –** codul hash din calea documentului

  - **Data\_ViewKind –** tipul de vizualizare Word

#### <a name="onenoteappnavigationratingreminderdialogshown"></a>OneNote.App.Navigation.RatingReminderDialogShown

Semnalul critic utilizată pentru măsurarea eficacității logicii de declanșare pentru memento de evaluare. Această casetă de dialog este afișată atunci când utilizatorul a îndeplinit toate condițiile pentru a vedea memento de evaluare (nr. de zile active, a evaluat anterior sau nu, etc.). Acest lucru este utilizat pentru a vă asigura că logica de interfață de declanșare pentru memento de evaluare. Dacă utilizatorii văd această casetă de dialog, ne va oferi moduri de a primi feedback de la clienți la momentul potrivit și de a îmbunătăți starea aplicațiilor.

Se colectează următoarele câmpuri:

- Fără

#### <a name="onenotecanvaspageopened-previous-name-officeonenoteandroidcanvaspageopened"></a>OneNote.Canvas.PageOpened *(nume anterior)* , Office.OneNote.Android.Canvas.PageOpened

Semnalul utilizată pentru a înregistra când este deschisă pagina.  Telemetria este folosită pentru a monitoriza, a detecta și a rezolva problemele cauzate când pagina este deschisă în OneNote.

Se colectează următoarele câmpuri: 

- **JOT_ID** - obiectul paginii deschise

- **TIME_TAKEN_IN_MS** - timp necesar pentru a deschide pagina

#### <a name="onenotecapturenewnotenewnotetaken-previous-name-officeonenoteandroidcapturenewnotenewnotetaken"></a>OneNote.Capture.NewNote.NewNoteTaken *(nume anterior)* , Office.OneNote.Android.Capture.NewNote.NewNoteTaken

Acest semnal este utilizat pentru a garanta că, după ce un utilizator se conectează la o aplicație OneNote Android, se acordă în mod corespunzător acces la blocnotesuri, iar utilizatorul creează cu succes o notă nouă.  Aceasta se folosește pentru a asigura detectarea regresiei critice pentru aplicația OneNote și starea serviciilor.

Se colectează următoarele câmpuri:

- Fără

#### <a name="onenotemessagebarmessagebarclicked-previous-name-officeonenoteandroidmessagebarmessagebarclicked"></a>OneNote.MessageBar.MessageBarClicked *(nume anterior)* , Office.OneNote.Android.MessageBar.MessageBarClicked

Semnalul utilizat pentru a indica probleme întâlnite în timp ce utilizați bara de mesaje.  Telemetria este folosită pentru a monitoriza, a detecta și a rezolva problemele cauzate în interacțiunea cu bara de mesaje

Se colectează următoarele câmpuri: 

- **Message_Bar_Type** - returnează dacă utilizatorul utilizează bara de mesaje veche sau nouă

- **Message_Type** - restaurează ID-ul la mesajul de eroare

#### <a name="parselicenseop"></a>ParseLicenseOp

Este colectat atunci când un utilizator încearcă să deschidă un document protejat prin IRM sau să aplice protecții IRM.  Acesta conține informațiile necesare pentru a investiga și a diagnostica corect problemele care apar atunci când se realizează operațiunea de analiză a licențelor. 

Se colectează următoarele câmpuri:

- **AppInfo.ClientHierarchy** - ierarhie client care indică faptul că aplicația rulează în mediul de producție sau în mediul de dezvoltator

- **AppInfo.Name** - nume aplicație

- **AppInfo.Version** - versiunea aplicației

- **iKey** - ID server înregistrator

- **RMS.ApplicationScenarioId** - ID al scenariului furnizat de aplicație

- **RMS.Duration** - timp total pentru finalizarea operațiunii

- **RMS.DurationWithoutExternalOps** - timp total minus operațiuni externe consumate, cum ar fi latența de rețea.

- **RMS.ErrorCode** - codul de eroare returnat de operațiune, dacă există

- **RMS.HttpCall** - indică dacă există operațiune HTTP

- **RMS.LicenseFormat** - formatul licenței: Xrml sau Json

- **RMS.Result** - succes sau eșec al operațiunii

- **RMS.ScenarioId** - ID al scenariului definit de clientul Serviciu de administrare a drepturilor

- **RMS.SDKVersion** - versiunea clientului pentru Serviciul de administrare a drepturilor

- **RMS.ServerType** - tipul de server al Serviciului de administrare a drepturilor 

- **RMS.StatusCode** - cod de stare al rezultatului operațiunii

- **RMS.VerifyCertChainDuration** - durată timp pentru a verifica lanțul de certificate

- **RMS.VerifySignatureDuration** - durată timp pentru a verifica semnătura

#### <a name="readconversation"></a>read.conversation

Este utilizat pentru a monitoriza posibilul impact negativ asupra stării și performanței de redare a unui mesaj de e-mail

Se colectează următoarele câmpuri: 

- **above_40fps** - numărul de cadre redate peste 40fps
 
- **above_50fps** - numărul de cadre redate peste 50fps
 
- **above_55fps** - numărul de cadre redate peste 55fps

- **adal_id** - ID-ul de autentificare Active Directory al contului, un identificator unic în sistemul de autentificare Microsoft 

- **component_name** - numele componentei/vizualizării care este activă în timpul filtrării

- **event_mode** - locul din aplicație în care utilizatorul a introdus o în conversație (grupuri sau altele)

- **internet_message_id** - un ID de urmărire pentru mesajul cel mai recent din conversație
      
- **orientation** - orientarea ecranului la ora evenimentului (portret sau peisaj)

- **recent_message_id** - ID-ul celui mai recent mesaj din conversație

- **suggested_reply_state** - starea răspunsurilor sugerate pentru această conversație (indisponibil, disponibil, afișat, utilizat sau eliminat)

- **suggested_reply_types** - indică tipul și numărul de răspunsuri sugerate afișate/utilizate pentru această conversație. Este un dicționar. De exemplu, {text: 2, send_avail: 1}.
  
- **total_count** - numărul total de cadre total afișat de componentă
 
- **view_duration** - cât timp a fost vizualizată componenta de către utilizator

#### <a name="saveattempt"></a>save.attempt

Ne permite să identificăm impactul problemelor cauzate de utilizatori în încercarea de a salva un fișier prin evaluarea numărului de sesiuni care sunt afectate și dacă există caracteristici comune ale sesiunilor respective.

Se colectează următoarele câmpuri: 

- **file_type** - tipul de fișier pe care utilizatorul a încercat să-l salveze (cum ar fi. doc)

- **origin** - care este originea încercării de salvare a fișierului (de ex. de la un mesaj de e-mail), astfel încât să putem detecta problemele asociate cu salvarea unui fișier dintr-un anumit loc din aplicație

- **token_type** - tipul de simbol utilizat pentru autentificarea contului pentru a salva fișierul, astfel încât să ne ajute să detectăm probleme de autentificare asociate cu salvarea unui fișier

#### <a name="searchsubtabselected"></a>search.subtab.selected

Acest eveniment colectează punctele originale pentru motivul pentru care a fost selectată o căutare sub_tab. Subfilele se află sub bara de căutare a aplicației principale, pentru a filtra datele. Acest eveniment ne permite să urmărim elementele fragment de tip (toate, corespondență, contacte și calendar) pe care le folosesc utilizatorii atunci când își realizează căutările, astfel încât să ne asigurăm că mecanismele de filtrare de căutare funcționează corect.

Se colectează următoarele câmpuri:

- **properties_general** - proprietățile generale pe care le colectează întregul eveniment Aria

- **selected_reason** - cauza pentru care este selectat un fragment de tip, care ar putea fi una dintre aceste trei valori: tap_on_header, tap_on_see_all, enter_search_mode

- **subtab_type** - fragmentul de tip care a fost selectat, care ar putea fi una dintre aceste patru valori: toate, e-mail, contact, eveniment.

#### <a name="sendmessage"></a>send.message

Este utilizat pentru a monitoriza posibilul impact negativ asupra performanței și stării trimiterii de mesaje de e-mail

Se colectează următoarele câmpuri:
  
- **account** - urmărește contul care a efectuat acțiunea

- **compose_duration** - urmărește timpul total necesar utilizatorului pentru a compune mesajul, inclusiv o sesiune cu mai multe schițe

- **draft_message_id** - urmărește ID-ul mesajului compus pentru mesajul trimis

- **event_mode** - urmărește modul de eveniment, dacă se aplică la mesaj, („grupuri” sau „altele”)

- **has_attachment** - indică dacă mesajul are atașări

- **has_mip_label** - indică dacă o etichetă MIP a fost atribuită sau nu mesajului

- **is_group_escalation** - este acesta un mesaj escaladat în grup, „mesajul escaladat” este un mesaj care a fost trimis la cutia poștală a utilizatorului din cauza unei escaladări (abonat la grup)

- **is_groups** - urmărește dacă mesajul trimis este un mesaj de grup sau nu

- **key_stroke_count** - urmărește numărul apăsărilor de taste pentru mesajul trimis

- **message_id** - urmărește ID-ul mesajului oferit ca răspuns/redirecționat

- **origin** - indică unde a fost compus, de ex., nou, răspuns, sau răspuns rapid etc.

- **send_draft_origin** - indică unde a fost inițiată trimiterea, de ex., compunere sau răspuns rapid

- **smart_compose_model_version** - urmărește ce versiune de model de compunere inteligentă este utilizată

- **source_inbox** - indică tipul de inbox sursă pentru mesajul de referință, 

- **suggested_reply_state** - capturarea stării răspunsurilor sugerate, de ex. indisponibil, disponibil, afișat, utilizat sau eliminat, pentru acest e-mail trimis

- **suggested_reply_types** - indică tipul și numărul de răspunsuri sugerate afișate/utilizate pentru acest mesaj de e-mail trimis. Este un dicționar. De exemplu, {text: 2, send_avail: 1}.

- **suggestions_requested** - indică câte sugestii de compunere inteligentă au fost solicitate

- **suggestions_results** - un rezultat al sugestiilor inteligente compuse, adică acceptat, respins

- **suggestions_returned** - indică numărul de sugestii de compunere inteligentă returnate de la server

- **suggestions_shown** - indică câte sugestii de compunere inteligentă sunt afișate utilizatorului

- **thread_id** - indică ID-ul firului de conversație răspuns/redirecționat

#### <a name="session"></a>sesiune

Ne permite să detectăm și să remediem situațiile în care utilizăm prea mult bateria dispozitivului și ne ajută să identificăm cauza.

Se colectează următoarele câmpuri: 

- **battery_level** - ne indică nivelul bateriei de pe dispozitiv pentru a ne ajuta să detectăm când aplicația noastră provoacă un impact negativ asupra nivelului bateriei dispozitivului.

- **has_hx** - ne spune că acest cont folosește noul nostru serviciu de sincronizare, pentru a ne ajuta să detectăm problemele provocate de serviciul nostru de sincronizare

#### <a name="settingsaction"></a>settings.action

Acest eveniment colectează informații de configurare din setări. Datele ne permit să detectăm situații în care există un posibil impact negativ asupra capacității utilizatorului de a configura setările de aplicație, cum ar fi setările de notificare, contul de e-mail principal și configurarea semnăturii de e-mail.

Se colectează următoarele câmpuri: 

- **account_order_changed** - pentru a verifica dacă ați modificat ordinea conturilor și pentru a vă asigura că această configurație funcționează corect 

- **action** - acțiunile posibile efectuate în Setări, cum ar fi ștergerea unui cont, pentru a ne ajuta să diagnosticăm probleme și să ne asigurăm că nu există un impact negativ

- **auth_type** - tipul de autentificare utilizat de cont, astfel încât să putem înțelege ce strat de sincronizare back-end utilizăm pentru a ne ajuta să diagnosticăm probleme 

- **changed_folder** - se capturează dacă s-a modificat un folder pentru a ne ajuta să diagnosticăm probleme. 

- **delete_scope** - în timpul unei ștergeri de cont, indiferent dacă ați șters contul de pe acest dispozitiv sau de pe toate dispozitivele cu Outlook.  

- **enabled_state** - dacă răspunsul dvs. automat, salvarea persoanelor de contact și blocarea setărilor de imagini externe sunt configurate corect  

- **notification_action** - pentru a verifica dacă ați configurat acțiuni de notificare pentru sortarea mesajelor de e-mail, pentru a ne ajuta să ne asigurăm că această setare funcționează cu succes 

- **notification_action_number** - pentru a verifica dacă acțiunile de notificare (acțiunea unu sau acțiunea doi) sunt configurate corect

- **server_type** - asemănător cu auth_type, ne spune ce tip de cont aveți pentru a ne ajuta să diagnosticăm mai bine problemele.  Exemple: Office365, Gmail, Outlook

- **setting_properties** - urmărește relația proprietăților cu acțiunea de setare detaliată mai jos: 
   - **alternate_app_icon_setting** - pictograma aplicației alternative selectate (luminos, întunecat)
   - **auth_type** - indică tipul de autentificare back-end care ne permite să știm dacă există o problemă cu un anumit tip de cont
   - **badge_count_state** - indică tipul de contor de ecusoane solicitat de utilizator, de ex. fără ecusoane, doar pentru mesajele prioritare etc. 
   - **changed_folder** - determină dacă această acțiune a fost arhivată, planificată sau altă acțiune.
   - **delete_scope** - urmărește dacă această acțiune are legătură cu ștergerea unei persoane doar pe acest dispozitiv sau pe toate dispozitivele, dacă este cazul. 
  - **enabled_state** - dacă starea asociată cu acțiunea este activată
  - **in_app_language** - limba selectată din aplicație, tipul de șir (implicit, en-US, fa, ru etc.)
  - **notification_action_setting** - indică detaliile, dacă este cazul, setărilor pentru acțiunile de notificare asociate cu această acțiune
    - **notification_action** - indică ce încerca să facă utilizatorul, de exemplu, să semnaleze, să șteargă, să arhiveze; ne permite să determinăm ce acțiune a încercat să efectueze utilizatorul asupra notificării și dacă acțiunea a fost realizată cu sau fără succes. 
    - **notification_action_number** - indică pentru ce număr de acțiune (două din trei acțiuni sunt particularizate) a fost atribuită o acțiune de notificare, de exemplu, acțiunea unu, acțiunea doi.  Acest lucru ne ajută să determinăm dacă există o problemă cu o anumită acțiune.
   - **notification_state** - indică tipul de contor de ecusoane solicitat de utilizator, de ex. fără ecusoane, doar pentru mesajele prioritare etc.
   - **server_type** - indică tipul de server back-end care ne permite să știm dacă există o problemă cu un anumit tip de server
   - **source** - indică sursa notificărilor, dacă este cazul, din setări sau setarea nu deranjați 
   - **swipe_setting** - indică detalii despre, dacă este cazul, setările de tragere cu degetul asociate cu această acțiune
     - **swipe_action** - indică ce încerca utilizatorul să facă, de ex. să semnaleze, să șteargă, să arhiveze, ne permite să determinăm acțiunea dorită de utilizator și dacă acțiunea nu a reușit sau nu. 
     - **swipe_direction** - indică modul în care utilizatorul a configurat glisarea, de ex. de la stânga la dreapta sau de la dreapta la stânga. Acest lucru ne permite să determinăm dacă există o problemă cu o anumită direcție de tragere cu degetul.
   - **ui_mode_setting** - modul selectat de UI (întunecat, luminos, setarea implicită a sistemului, baterie descărcată etc.)
   - **signature_setting** - indică dacă setarea a fost aplicată pentru întregul cont sau pentru un cont individual

- **state_changed_to** - pentru a verifica dacă setarea activat/dezactivat mesaje prioritare este configurată corect 

- **swipe_action** - pentru a verifica dacă ați configurat toate acțiunile de tragere cu degetul pentru sortarea mesajelor de e-mail, pentru a ne ajuta să ne asigurăm că această setare funcționează cu succes 

- **swipe_direction** - pentru a verifica dacă direcțiile de tragere (la stânga sau la dreapta) sunt configurate corect


#### <a name="sidebaraction"></a>sidebar.action

Ne permite să detectăm situațiile în care există un posibil impact negativ asupra capacității de a configura setările de aplicație, cum ar fi setările de notificare, contul de e-mail principal și configurarea semnăturii de corespondență.

Câmpurile de date care sunt comune pentru Outlook Mobile pentru acest eveniment pe iOS și Android:

- **Account** - urmărește contul și datele sale asociate evenimentului, valorile urmărite în aceste date se află în documentația de câmp comună om *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

- **action** - urmărește tipul de acțiune din bara laterală, de ex. butonul respins, Ajutor selectat, bara laterală corespondență etc., 

- **from_favorites** - urmărește dacă acțiunea provine de la un element din Preferințe 

- **mail_folder_type** - ce tip de folder a fost selectat în timpul acțiunii din bara laterală, dacă există.

- **sidebar_type** - urmărește tipul de bară laterală asociat cu acest eveniment, de ex. corespondență sau calendar pentru a ne ajuta să garantăm că navigarea din setarea Preferințe funcționează corect

Se colectează următoarele câmpuri: 

- **account_type** - indică tipul de autentificare al contului, de exemplu, Gmail, Outlook etc. 

- **account_has_groups** - ne ajută să ne asigurăm că în cont există grupuri, care sunt configurate corect

- **calendar_accounts_count** - numărul de conturi de calendar pe care îl aveți pentru a ne ajuta să ne asigurăm că conturile dvs. de calendar sunt configurate corect 

- **calendar_apps_count** - numărul de aplicații de calendar pe care îl aveți pentru a ne ajuta să ne asigurăm că aplicațiile dvs. de calendar interesant sunt configurate corect 

- **calendar_type** - tipul de calendar pe care îl aveți (calendar principal, calendar de grup etc.) 

- **has_favorite_folders** - ne ajută să ne asigurăm că folderele preferate sunt configurate corect 

- **has_favorite_people** - ne ajută să ne asigurăm că persoanele/persoanele de contact preferate sunt configurate corect 

- **has_group_calendar** - ne ajută să ne asigurăm că aveți calendare de grup, că sunt configurate corect 

- **has_group_calendar_account** - ne ajută să ne asigurăm că aveți calendare de grup, că sunt configurate corect 

- **has_group_toggled** - ne ajută să ne asigurăm că ați comutat calendare de grup, această setare este configurată corect 

- **interesting_calendars_accounts_count** - numărul de conturi de calendar interesant pe care îl aveți pentru a ne ajuta să ne asigurăm că conturile dvs. de calendar interesant sunt configurate corect 

- **mail_accounts_count** - numărul total de conturi de e-mail din bara laterală, pentru a vă asigura că acest lucru este configurat corect 

- **mail_folder_type** - tipul de folder pe care l-a accesat utilizatorul pentru a vă asigura că este configurat corect. Poate include Folderul șters, Spam sau Folderul trimis. 

- **mail_inbox_unread_count** - ne ajută să ne asigurăm că contorizarea necitită este afișată și configurată corect 

- **mail_subfolder_depth** - ne ajută să ne asigurăm că vom putea afișa cu succes configurațiile de subfolder de corespondență ale unui utilizator

#### <a name="storeop"></a>StoreOp

Este colectat atunci când un utilizator încearcă să deschidă un document protejat prin IRM sau să aplice protecții IRM.  Acesta conține informațiile necesare pentru a investiga și a diagnostica corect problemele care apar atunci când se realizează operațiunea de stocare a licențelor pentru Serviciul de administrare a drepturilor. 

Se colectează următoarele câmpuri:

- **AppInfo.ClientHierarchy** - ierarhie client care indică faptul că aplicația rulează în mediul de producție sau în mediul de dezvoltator

- **AppInfo.Name** - nume aplicație.

- **AppInfo.Version** - versiunea aplicației

- **iKey** - ID al serverului pentru servicii de înregistrare

- **RMS.ApplicationScenarioId** - ID al scenariului furnizat de aplicație

- **RMS.ContentId** - ID-ul de conținut din Licența pentru utilizatorul final

- **RMS.Duration** - timp total pentru finalizarea apelului API

- **RMS.DurationWithoutExternalOps** - timp total minus operațiuni externe consumate, cum ar fi latența de rețea.

- **RMS.ErrorCode** - codul de eroare returnat de operațiune, dacă există

- **RMS.HttpCall** - indică dacă există operațiune HTTP

- **RMS.LicenseFormat** - formatul licenței: Xrml sau Json

- **RMS.OperationName** - nume operațiune

- **RMS.Result** - succes sau eșec al operațiunii

- **RMS.ScenarioId** - ID al scenariului definit de clientul Serviciu de administrare a drepturilor

- **RMS.SDKVersion** - versiunea clientului pentru Serviciul de administrare a drepturilor

- **RMS.ServerType** - tipul de server al Serviciului de administrare a drepturilor 

- **RMS.StatusCode** - cod de stare al rezultatului operațiunii

- **RMS.Url** - URL-ul serverului pentru Serviciul de administrare a drepturilor

#### <a name="watchappv2"></a>watchAppV2

Acest eveniment ne permite să detectăm și să remediem eventualele probleme privind capacitățile de pe Apple Watch, cum ar fi primirea de notificări și răspunsul la mesajele de e-mail.

Se colectează următoarele câmpuri: 

- **app_action** - ne spune tipurile de acțiune pe care le-a întreprins utilizatorul privind Apple Watch, cum ar fi „archive_message”, pentru a ne ajuta să detectăm probleme legate de o acțiune specifică, cum ar fi imposibilitatea de a arhiva cu succes mesajele de pe Apple Watch

- **is_watch_app_installed** - ne spune dacă utilizatorul a instalat aplicația Apple Watch pe dispozitivul său

- **is_complication_enabled** - ne spune dacă utilizatorul a adăugat Outlook la ecranul Apple Watch, pentru a ne ajuta să detectăm probleme legate de ecrane Apple Watch

- **watch_os** - ne spune versiunea de sistem de operare Apple Watch instalată pentru a ne ajuta să detectăm probleme legate de anumite versiuni de sistem de operare Apple Watch


### <a name="application-status-and-boot-subtype"></a>*Subtipul de inițializare și starea aplicației*

Stabilește dacă au avut loc anumite evenimente de caracteristici, cum ar fi pornirea sau oprirea, și dacă respectiva caracteristică rulează.

#### <a name="appstartup"></a>app.startup

Acest eveniment ne permite să detectăm și să remediem probleme în care Outlook pornește lent sau incomplet, îngreunând utilizarea aplicației de către utilizatori.  Acesta include informații despre caracteristici specifice care au fost activate și despre durata de pornire al părților.

Se colectează următoarele câmpuri: 

- **attach_base_context_millis** - timp între începerea Contextului de bază și începerea onCreate()

- **device_ram_in_mb** - RAM disponibil pe dispozitiv

- **has_company_portal** - dacă este instalată aplicația portalul firmei

- **hx_okhttp_mode** - dacă noua componentă a serviciului de sincronizare a corespondenței utilizează OKHttp pentru trimiterea și primirea de solicitări de rețea bazate pe HTTP

- **initial_activity_name** - activitatea Android care a lansat aplicația

- **manufacturer** - producătorul dispozitivului

- **model** - modelul de dispozitiv

- **on_create_millis** - timpul necesar în metoda onCreate()

- **on_resume_millis** - timpul necesar în metoda onResume()

- **time_until_attach** - timp între încărcarea clasei și începerea Contextului de bază

- **total_millis** - timpul total de la începerea încărcării la finalizarea reluării Activității Android

#### <a name="boottime"></a>boot.time 

Acest eveniment ne permite să detectăm când s-au produs erori critice ale aplicațiilor, care ar putea duce la căderea aplicației dvs. sau la probleme serioase, cum ar fi vizualizarea unor rânduri goale în inboxul dvs. Acest eveniment colectează informații care ne permit să clasificăm și să dispunem pe categorii problemele pentru a ne ajuta să stabilim priorități în ceea ce privește impactul problemelor asupra clienților.

Se colectează următoarele câmpuri:

- **black_list_reason** - ne spune dacă există un motiv pentru care ar trebui să ignorăm aceste date. Printre exemple se numără lansarea din cauza unei notificări la distanță și lansarea din cauza unei preluări de fundal.

- **step_premain** - ne spune intervalul de timp necesar pentru ca Outlook să treacă de la atingerea pictogramei de către utilizator la pasul „principal” step0_main definit în acest document.

- **step0_main** - ne spune intervalul de timp necesar pentru ca Outlook să ajungă la pasul „principal”, care este un pas definit de Apple.

- **step1_appWillFinishLaunching** - ne spune intervalul de timp necesar pentru ca Outlook să treacă de la pasul „principal” la pasul „appWillFinishLaunching”, care este un pas definit de Apple.

- **step2_appDidFinishLaunching** - ne spune intervalul de timp necesar pentru ca Outlook să treacă de la pasul „appWillFinishLaunching” la pasul „appDidFinishLaunching”, care este un pas definit de Apple.

- **step3_engineStarted** - ne spune intervalul de timp necesar pentru ca Outlook să treacă de la pasul „appDidFinishLaunching” la pornirea motorului aplicației, care gestionează stocarea și sincronizarea datelor.

- **step4_runLoopFirstIdle** - ne spune intervalul de timp necesar pentru ca Outlook să treacă de la pasul „engineStarted” la cel de a nu mai avea lucru suplimentar de finalizat.

- **total_time** - ne spune intervalul de timp necesar pentru ca Outlook să finalizeze procesul de pornire.

#### <a name="dnslookupop"></a>DnsLookupOp

Este colectat atunci când un utilizator încearcă să deschidă un document protejat prin IRM sau să aplice protecții IRM.  Acesta conține informațiile necesare pentru a investiga și a diagnostica corect problemele care apar atunci când se realizează operațiunea de căutare a informațiilor DNS. 

Se colectează următoarele câmpuri:

- **AppInfo.ClientHierarchy** - ierarhie client care indică faptul că aplicația rulează în mediul de producție sau în mediul de dezvoltator

- **AppInfo.Name** - nume aplicație.

- **AppInfo.Version** - versiunea aplicației

- **iKey** - ID al serverului pentru servicii de înregistrare

- **RMS.ApplicationScenarioId** - ID al scenariului furnizat de aplicație

- **RMS.Duration** - timp total pentru finalizarea operațiunii

- **RMS.DurationWithoutExternalOps** - timp total minus operațiuni externe consumate, cum ar fi latența de rețea.

- **RMS.ErrorCode** - codul de eroare returnat de operațiune, dacă există

- **RMS.HttpCall** - indică dacă există operațiune http

- **RMS.LicenseFormat** - formatul licenței: Xrml sau Json

- **RMS.NoOfDomainsSearched** - numărul de domenii căutate    

- **RMS.NoOfDomainsSkipped** - numărul de domenii ignorate 

- **RMS.Result** - succes sau eșec al operațiunii

- **RMS.ScenarioId** - ID al scenariului definit de clientul Serviciu de administrare a drepturilor

- **RMS.SDKVersion** - versiunea clientului pentru Serviciul de administrare a drepturilor

- **RMS.ServerType** - tipul de server al Serviciului de administrare a drepturilor 

- **RMS.StatusCode** - cod de stare al rezultatului operațiunii

#### <a name="firstvisible"></a>first.visible

Acest eveniment ne permite să detectăm prima dată când aplicația este lansată în mod intenționat de către utilizator. Acest eveniment este necesar pentru a vă asigura că aplicația funcționează cu succes în compilările OEM (producător de echipamente originale).

Se colectează următoarele câmpuri:

- **is_oem** - un câmp de urmărire care indică dacă aplicația rulează pe o variantă OEM

- **is_system_install** - un câmp care urmărește prezența unui fișier proprietar preinstalat, care ar trebui să indice că această instalare este OEM 

- **manufacturer** - producătorul dispozitivului

- **model** - modelul dispozitivului

- **systemFlagSet** - valoarea semnalului de sistem Android (ApplicationInfo. FLAG_SYSTEM) care indică dacă aplicația a fost instalată ca parte a imaginii de sistem a dispozitivului

#### <a name="getuserop"></a>GetUserOp

Este colectat atunci când un utilizator încearcă să deschidă un document protejat prin IRM sau să aplice protecții IRM.  Acesta conține informațiile necesare pentru a investiga și a diagnostica corect problemele care apar atunci când se realizează operațiunea obținere a certificatelor de utilizator. 

Se colectează următoarele câmpuri:

- **AppInfo.ClientHierarchy** - ierarhie client care indică faptul că aplicația rulează în mediul de producție sau în mediul de dezvoltator

- **AppInfo.Name** - nume aplicație

- **AppInfo.Version** - versiunea aplicației

- **iKey** - ID al serverului pentru servicii de înregistrare

- **RMS.ApplicationScenarioId** - ID al scenariului furnizat de aplicație

- **RMS.ContentId** - ID-ul de conținut

- **RMS.Duration** - timp total pentru finalizarea operațiunii

- **RMS.DurationWithoutExternalOps** - timp total minus operațiuni externe consumate, cum ar fi latența de rețea.

- **RMS.ErrorCode** - codul de eroare returnat de operațiune

- **RMS.HttpCall** - indică dacă există operațiune HTTP

- **RMS.LicenseFormat** - formatul licenței: Xrml sau Json

- **RMS.Result** - succes sau eșec al operațiunii

- **RMS.ScenarioId** - ID al scenariului definit de clientul Serviciu de administrare a drepturilor

- **RMS.SDKVersion** - versiunea clientului pentru Serviciul de administrare a drepturilor

- **RMS.ServerType** - tipul de server al Serviciului de administrare a drepturilor 

- **RMS.StatusCode** - cod de stare al rezultatului operațiunii

- **RMS.Type** - tipul informațiilor despre utilizator

#### <a name="httpop"></a>HttpOp

Este colectat atunci când un utilizator încearcă să deschidă un document protejat prin IRM sau să aplice protecții IRM.  Acesta conține informațiile necesare pentru a investiga și a diagnostica corect problemele care apar atunci când se realizează operațiunea de solicitare http.

Se colectează următoarele câmpuri:

- **AppInfo.ClientHierarchy** - ierarhie client care indică faptul că aplicația rulează în mediul de producție sau în mediul de dezvoltator
    
- **AppInfo.Name** - nume aplicație

- **AppInfo.Version** - versiunea aplicației

- **iKey** - ID al serverului pentru servicii de înregistrare

- **RMS.ApplicationScenarioId** - ID al scenariului furnizat de aplicație

- **RMS.CallBackStatus** - starea rezultatului returnat de apelul invers de autentificare

- **RMS.CallbackTime** - timpul consumat de apelul invers de autentificare 

- **RMS.CorrelationId** - ID-ul de corelare a solicitării http

- **RMS.DataSize** - dimensiunea datelor din solicitarea HTTP

- **RMS.Duration** - timp total pentru finalizarea operațiunii

- **RMS.DurationWithoutExternalOps** - timp total minus operațiuni externe consumate, cum ar fi latența de rețea.

- **RMS.ErrorCode** - codul de eroare returnat de operațiune, dacă există

- **RMS.HttpCall** - indică dacă există operațiune http imbricată. 

- **RMS.LicenseFormat** - formatul licenței: Xrml sau Json

- **RMS.OperationName** - nume operațiune

- **RMS.Result** - succes sau eșec al operațiunii

- **RMS.ScenarioId** - ID al scenariului definit de clientul Serviciu de administrare a drepturilor

- **RMS.SDKVersion** - versiunea clientului pentru Serviciul de administrare a drepturilor

- **RMS.ServerType** - tipul de server al Serviciului de administrare a drepturilor 

- **RMS.StatusCode** - cod de stare al rezultatului operațiunii

- **RMS.Url** - URL-ul serverului pentru Serviciul de administrare a drepturilor

- **RMS.WinhttpCallbackStatus** - starea rezultatului apelului invers winhttp

#### <a name="initialized"></a>Inițializat

Ne permite să analizăm starea de funcționare a interfeței, care le permite aplicațiilor mobile să preia setările de utilizator și confidențialitate din serviciile Office și să diagnosticheze conectivitatea și setările de confidențialitate ale serviciului.

Se colectează următoarele câmpuri:

- **roamingSettingType** - identifică locația din care încercăm să citim setările

#### <a name="ipccreateoauth2token"></a>IpcCreateOauth2Token

Este colectat atunci când un utilizator încearcă să deschidă un document protejat prin IRM sau să aplice protecții IRM. Acesta conține informațiile necesare pentru a investiga și a diagnostica corect problemele care apar atunci când se realizează apelul API IpcCreateOauth2Token. 

Se colectează următoarele câmpuri:

- **AppInfo.ClientHierarchy** - ierarhie client care indică faptul că aplicația rulează în mediul de producție sau în mediul de dezvoltator
    
- **AppInfo.Name** - nume aplicație.

- **AppInfo.Version** - versiunea aplicației

- **iKey** - ID al serverului pentru servicii de înregistrare

- **RMS.Duration** - timp total pentru finalizarea apelului API

- **RMS.DurationWithoutExternalOps** - timp total minus operațiuni externe consumate, cum ar fi latența de rețea.

- **RMS.ErrorCode** - codul de eroare returnat de apelul API, dacă există.

- **RMS.HttpCall** - indică dacă există operațiune HTTP

- **RMS.Result** - succes sau eșec al apelului API

- **RMS.ScenarioId** - ID al scenariului definit de API

- **RMS.SDKVersion** - versiunea clientului pentru Serviciul de administrare a drepturilor

- **RMS.StatusCode** - cod de stare al rezultatului returnat


#### <a name="officeandroidaccountstorageinfo"></a>Office.Android.AccountStorageInfo

Acest eveniment determină numărul de conturi MSA și ADAL din registry și preferințele partajate. Aceasta permite analiza inconsistențelor între depozitele de date și ne ajută să stabilizăm performanța aplicațiilor.

Se colectează următoarele câmpuri:

- **RegistryADALCount** - indică numărul de conturi ADAL din registry.

- **RegistryLiveIdCount** - indică numărul de conturi MSA din registry.

- **SharedPrefADALCount** - indică numărul de conturi ADAL din preferințele partajate.

- **SharedPrefLiveIdCount** - indică numărul de conturi MSA din preferințele partajate.


#### <a name="officeandroidandroidoffice16bootlatency"></a>Office.Android.AndroidOffice16BootLatency

Critic pentru capturarea pentru performanța metrică a aplicațiilor în ceea ce privește timpul de răspuns al aplicației din boot.  Microsoft folosește acesta pentru a colecta timpul necesar pentru ca aplicația să fie receptivă și totodată, să detecteze scenarii care pot influența timpul de încărcare în Word, Excel sau PowerPoint.

Se colectează următoarele câmpuri:

- **AppLaunchResponsiveTimeInMilliSec** - Timpul de răspuns al lansării aplicației

- **AppSuspendedDuringBoot** - Boolean pentru a indica dacă aplicația a fost suspendată în timpul încărcării

- **CollectionTime** - ora evenimentului

- **FileActivationAttempted** - Boolean pentru a indica dacă s-a încercat activarea fișierului

- **FirstIdleOnAppThreadTimeInMilliSec** - timpul mort al firului aplicației

- **IsThisFirstLaunch** - Boolean pentru a indica dacă este lansarea aplicației în premieră

- **UserDialogInterruptionDuringBoot** - Boolean pentru a indica dacă a existat o interfață utilizator blocată în timpul pornirii

#### <a name="officeextensibilityofficejsappactivated"></a>Office.Extensibility.OfficeJS.Appactivated

Înregistrează informații despre opririle neașteptate Office. Acest lucru ne permite să identificăm blocările sau căderile produsului, astfel încât să le putem remedia.

Se colectează următoarele câmpuri:

  - **Data\_AirspaceInitTime:integer-** timpul pentru inițializarea componentei Airspace Office

  - **Data\_AllShapes:integer –** numărul de forme din document

  - **Data\_APIInitTime:integer –** timpul necesar pentru a inițializa modulul Visio API

  - **Data\_AppSizeHeight –** Adaugă **-** la înălțimea ferestrei

  - **Data\_AppSizeWidth –** Adaugă **-** la lățimea ferestrei

  - **Data\_AppURL –** URL-ul programului de completare; jurnalele adreselor URL complete pentru programele de completare din magazin și domeniul adreselor URL pentru cele din afara magazinului

  - **Data_Doc_AsyncOpenKind:long –** indică dacă s-a deschis o versiune memorată în cache a documentului cloud și ce logică de reîmprospătare asincronă s-a folosit.

  - **Data\_AuthorsCount:integer –** numărul de autori care au editat documentul în această sesiune

  - **Data\_BackgroundPages:integer –** numărul de pagini de fundal din diagramă

  - **Data\_BootTime:integer –** timpul necesar pentru a inițializa Visio

  - **Data\_Browser –** șir de browser cu informații despre acesta, cum ar fi tipul sau versiunea

  - **Data\_ChildWindowMixedModeTime:integer –** timpul necesar pentru a activa modul mixt în Visio (fereastra secundară poate avea altă valoare DpiAwareness decât cea principală)

  - **Data\_CommentsCount:integer –** numărul de comentarii din document

  - **Data\_ConnectionCount:integer –** numărul de conexiuni de date din diagramă

  - **Data\_ContentMgrInitTim:integer –** timpul necesar pentru a inițializa managerul de conținut

  - **Data\_CreateMainFrameTime:integer –** creați ora pentru mainframe

  - **Data\_CreatePaletteTime:integer –** timpul necesar pentru a crea paleta globală de culori

  - **Data\_DispFormatCount:integer –** numărul de grafice de date din diagramă

  - **Data\_Doc\_Ext:string –** extensia documentului

  - **Data\_Doc\_Fqdn:string –** unde este stocat documentul (SharePoint.com, live.net), disponibil numai pentru domeniile Office 365

  - **Data\_Doc\_FqdnHash:string –** codul hash al locului unde este stocat documentul

  - **Data\_Doc\_IsIncrementalOpen:bool –** : documentul a fost deschis incremental (caracteristică nouă care deschide documentul fără să-l descarce în totalitate)

  - **Data\_Doc\_IsOpeningOfflineCopy:bool –** documentul este deschis din memoria cache locală?

  - **Data\_Doc\_IsSyncBacked:bool –** true când acesta este un document de server care există la nivel local și este sincronizat cu serverul (de exemplu, prin aplicațiile client OneDrive sau ODB)

  - **Data\_Doc\_Location:long –** : setul predefinit de valori pentru locul unde este stocat documentul (Local, SharePoint, WOPI, Rețea etc.)

  - **Data\_Doc\_LocationDetails:long –** setul predefinit de valori pentru locația mai detaliată (folderul Temp, folderul de descărcări, Documente OneDrive, Imagini OneDrive

  - **Data\_Doc\_ResourceIdHash:string –** codul hash al identificatorului de resursă pentru documentele stocate în cloud

  - **Data_Doc_RtcType -**  indică modul în care a fost configurat canalul în timp real (RTC) pentru fișierul curent (dezactivat, neacceptat, la cerere, activat permanent etc.).

  - **Data\_Doc\_ServerDocId:string –** identificatorul imutabil pentru documentele stocate în cloud

  - **Data\_Doc\_SessionId:long –** GUID generat care identifică instanța documentului din aceeași sesiune de proces

  - **Data\_Doc\_SizeInBytes:long –** dimensiunea documentului în byți

  - **Data\_Doc\_SpecialChars:long –** Bitmask lung ce arată caracterele speciale din adresa URL sau calea documentului

  - **Data\_Doc\_SyncBackedType -** indicator privind tipul documentului (local sau bazat pe servicii) 

  - **Data\_Doc\_UrlHash:string –** codul hash pentru adresa URL completă a documentelor stocate în cloud

  - **Data\_DpiAwarenessTime:integer –** timpul necesar pentru a activa Per Monitor Dpi Awareness

  - **Data\_DurationToCompleteInMilliseconds:double –** durata pentru a finaliza salvarea, în milisecunde

  - **Data\_ErrorCode:int –** : 0 pentru succes, întreg pentru nereușita salvării

  - **Data\_FailureReason:integer –** motivul nereușitei pentru salvarea asincronă

  - **Data\_FileExtension –** extensia de fișier a diagramei deschise

  - **Data\_FileHasDGMaster:bool –** true când fișierul are Grafice de date

  - **Data\_FileHasImportedData:bool –** true când fișierul are date importate

  - **Data\_FileHasShapesLinked:bool –** true când fișierul a asociat forme la date

  - **Data\_FileIOBytesRead:int –** numărul total de byți citiți la salvare

  - **Data\_FileIOBytesReadSquared:int –** valoarea pătrată pentru Data\_FileIOBytesRead

  - **Data\_FileIOBytesWritten:int –** numărul total de byți scriși la salvare

  - **Data\_FileIOBytesWrittenSquared:int –** valoarea pătrată pentru Data\_FileIOBytesWritten

  - **Data\_FilePathHash:binary** – codul hash binar al căii fișierului

  - **Data\_FilePathHash: binary** – codul GUID pentru calea fișierului

  - **Data\_FileSize –** dimensiunea documentului în byți

  - **Data\_ForegroundPages:integer –** numărul de pagini de prim-plan din diagramă

  - **Data\_ForegroundShapes:integer –** numărul întreg de forme din paginile de Prim-plan

  - **Data\_GdiInitTime:integer –** timpul necesar pentru a inițializa modulul GDI

  - **Data\_HasCoauthUserEdit:bool –** true dacă documentul a fost editat într-o sesiune de elaborare în comun

  - **Data\_HasCustomPages:bool –** true dacă documentul conține pagini particularizate

  - **Data\_HasCustPatterns:bool –** true dacă fișierul are modele particularizate

  - **Data\_HasDynConn:bool –** true dacă documentul conține conexiuni dinamice

  - **Data\_HasScaledPages:bool –** true dacă documentul conține pagini scalate

  - **Data\_HasUserWaitTime:bool –** true dacă se afișează caseta de dialog a fișierului la salvare

  - **Data\_InitAddinsTime:integer –** timpul necesar pentru a inițializa și a încărca funcția COM Add

  - **Data\_InitBrandTime:integer -** perioada de timp pentru a inițializa ecranul de pornire și componentele marca Office 

  - **Data\_InitGimmeTime:integer -** timpul necesar pentru a inițializa componenta Office

  - **Data\_InitLicensingTime:integer -** timpul necesar pentru a inițializa componenta licenței Office

  - **Data\_InitMsoUtilsTime:integer -** timpul inițializării către componenta Office MSOUTILS

  - **Data\_InitPerfTime:integer -** durata inițializării componentei de performanță Office

  - **Data\_InitTCOTime:integer -** perioada de timp necesară pentru a inițializa managerul de componente Office

  - **Data\_InitTrustCenterTime:integer –** timpul necesar pentru a inițializa centrul de autorizare a componentelor Office

  - **Data\_InitVSSubSystemsTime:integer –** timpul necesar pentru a inițializa componentele Visio

  - **Data\_InternalFile:bool –** true dacă fișierul este unul intern. ex. tipar

  - **Data\_IsAsyncSave:bool –** true dacă salvarea a fost asincronă

  - **Data\_IsAutoRecoveredFile:bool –** true dacă fișierul a fost recuperat automat

  - **Data\_IsEmbedded:bool –** true dacă fișierul Visio a fost încorporat în altă aplicație

  - **Data\_IsInfinitePageDisabledForAllPages:bool –** true dacă opțiunea Pagină infinită este dezactivată pentru toate paginile documentului

  - **Data\_IsIRMProtected:bool –** true dacă fișierul este protejat prin Information Right

  - **Data\_IsLocal:bool –** true dacă fișierul este local

  - **Data\_IsRecoverySave:bool –** true dacă salvarea a fost declanșată de recuperare

  - **Data\_IsShapeSearchPaneHiddenState:bool –** true dacă panoul de căutare a formelor a fost ascuns pentru document

  - **Data\_IsSmartDiagramPresentInActivePageOfFile:bool –** bool, true dacă diagrama vizuală cu date inteligente este prezentă în pagina activă a fișierului

  - **Data\_IsSmartDiagramPresentInFile:bool –** bool, true dacă diagrama vizuală cu date inteligente este prezentă în fișier.

  - **Data\_IsUNC:bool –** true atunci când calea documentului aderă la Convenția Universală de Numire

  - **Data\_LandscapePgCount:integer –** numărul de pagini cu orientarea peisaj din diagramă

  - **Data\_Layers:integer–** numărul de niveluri din diagramă

  - **Data\_LoadProfileTime:integer –** timpul necesar pentru a încărca profilare Office

  - **Data\_LoadRichEditTim:integer –** timpul de încărcare a componentei de editare inteligentă

  - **Data\_LoadVisIntlTime:integer –** timpul necesar pentru a încărca fișierul DLL internațional Visio

  - **Data\_Location:integer –** locația din care a fost deschis fișierul 0 Local, 1, Rețea, 2, SharePoint, 3 – Web

  - **Data\_MasterCount:integer –** numărul de coordonatoare din diagramă

  - **Data\_MaxCoauthUsers:integer –** numărul maxim de utilizatori care colaborează la orice moment în componentele Filesystem, Registry, First Party sau SDX din sesiune

  - **Data\_MaxTilesAutoSizeOn:integer –** numărul maxim de dale a unei pagini pentru care s-a activat dimensiunea automată

  - **Data\_MsoBeginBootTime:integer –** timpul de inițializare MSO

  - **Data\_MsoDllLoadTime:integer –** timpul necesar pentru a încărca MSO DLL

  - **Data\_MsoEndBootTime:integer –** timpul necesar pentru a încheia inițializarea MSO

  - **Data\_MsoInitCoreTime:integer –** timpul necesar pentru a inițializa componenta Office MSO

  - **Data\_MsoInitUITime:integer –** timpul necesar pentru a inițializa interfața de utilizare a componentelor Office MSO

  - **Data\_MsoMigrateTime:integer –** timpul necesar pentru a migra setările de utilizator la prima inițializare, dacă utilizatorul a făcut upgrade de la versiunea anterioară

  - **Data\_NetworkIOBytesRead:int –** numărul total de byți din rețea citiți la salvare

  - **Data\_NetworkIOBytesReadSquared:int –** valoarea pătrată pentru Data\_NetworkIOBytesRead

  - **Data\_NetworkIOBytesWritten:int –** numărul total de byți din rețea scriși la salvare

  - **Data\_NetworkIOBytesWrittenSquared :int –** valoarea pătrată pentru NetworkIOBytesWritten

  - **Data\_OartStartupTime:integer –** timpul necesar pentru a inițializa componenta Office OART

  - **Data\_OleInitTime:integer –** timpul de inițializare a componentei Office OLE

  - **Data\_OpenDurationTimeInMs:integer –** durata pentru a deschide fișierul, în milisecunde

  - **Data\_OriginatedFromTemplateID:integer –** identificatorul șablonului din care s-a creat diagrama. NULL pentru șabloanele de la terți

  - **Data\_Pages:integer –** numărul de pagini din document

  - **Data\_PositionToolbarsTime:integer –** timpul necesar pentru a poziționa barele de instrumente

  - **Data\_ReadOnly:bool –** true dacă fișierul este doar în citire

  - **Data\_RecordSetCount:integer –** numărul de seturi de înregistrări din diagramă

  - **Data\_RecoveryTime:integer –** timpul necesar pentru a deschide fișierele de recuperare

  - **Data\_ReviewerPages:integer –** numărul de pagini revizuite din diagramă

  - **Data\_RibbonTime:integer –** timpul necesar pentru a afișa bara de stare

  - **Data\_RoamingSettingsStartupTime:integer –** timpul necesar pentru a crea și a încărca toate setările Visio transmise în prezent

  - **Data\_SchemeMgrStartupTime:integer –** timpul necesar pentru a inițializa managerul de scheme

  - **Data\_SDX\_AssetId –** există DOAR pentru programele de completare din magazin. OMEX oferă programului de completare un IDActiv când intră în magazin

  - **Data\_SDX\_BrowserToken –** identificatorul din memoria cache a browserului

  - **Data\_SDX\_HostJsVersion –** aceasta este versiunea de Office.js specifică platformei (de ex. outlook web16.01.js). Ea conține suprafața API pentru programele de completare

  - **Data\_SDX\_Id –** codul GUID al unui program de completare care îl identifică în mod unic

  - **Data\_SDX\_InstanceId –** reprezintă perechea de documente a programului de completare

  - **Data\_SDX\_MarketplaceType –** indică de unde este instalat programul de completare

  - **Data\_SDX\_OfficeJsVersion –** aceasta este versiunea de Office.js care se va redirecționa spre versiunea specifică platformei.

  - **Data\_SDX\_Version –** versiunea programului de completare

  - **Data\_ShellCmdLineTime:integer –** timpul necesar pentru a analiza și a executa orice comenzi shell în linia de comandă

  - **Data\_Size:long** – dimensiunea fișierului în byți

  - **Data\_StartEndTransactionTime:integer –** timpul necesar pentru a inițializa componentele Visio

  - **Data\_STNInitTime:integer –** timpul necesar pentru a inițializa configurația ferestrei de tipar

  - **Data\_Tag:string –** identificatorul unic al evenimentului Salvare ca

  - **Data\_ThemeCount:integer –** numărul de teme din diagramă

  - **Data\_TimeStamp –** marca de timp la care s-a închis documentul

  - **Data\_UIInitTime:integer –** timpul de inițializare a interfeței de utilizare

  - **Data\_WasSuccessful:bool –** true dacă „salvarea ca” a reușit

  - **Data\_WinLaunchTime:integer –** timpul necesar pentru a lansa panoul de pornire Visio etc.)

  - **Office.Visio.FileCharacteristicsVisio –** surprinde proprietățile fișierului la momentul inițializării acestuia pentru Visio C2R și Dev16. Acest eveniment ne ajută să clasificăm și să depanăm erorile privind proprietățile documentului, permițându-ne să stabilim mai repede cauza problemelor și să le remediem, pentru satisfacția clienților.

  - **Office.Visio.Shared.BootStats –** acest eveniment colectează timpii de inițializare pentru aplicația Visio Win32. El colectează diverse câmpuri pentru inițializarea mai multor componente, precum Timpul de încărcare a paginii sau Timpul de inițializare a aplicațiilor Evenimentul se folosește pentru a măsura performanța de inițializare pentru Visio.

  - **Office.Visio.Shared.FileOpen –** acest eveniment colectează statisticile de deschidere a fișierelor pentru Visio. Acest eveniment este utilizat pentru a monitoriza ratele de succes/insucces de la deschiderea fișierelor și le mapează cu câteva proprietăți, cum ar fi dimensiunea fișierelor. Proprietățile fișierelor ne permit să depanăm și să stabilim mai rapid cauza problemelor.

  - **Office.Visio.Shared.Filesave –** acest eveniment colectează statisticile de salvare a fișierelor pentru Visio. Evenimentul este utilizat pentru a monitoriza ratele de succes/insucces de la salvarea fișierelor și le mapează cu câteva proprietăți, cum ar fi dimensiunea fișierelor și locația în care sunt salvate (de ex. în cloud sau la nivel local). Proprietățile fișierelor ne permit să depanăm și să stabilim mai rapid cauza problemelor.

  - **Office.Visio.Shared.FilesaveAs –** acest eveniment colectează statisticile de „salvare ca” a fișierelor pentru Visio. Evenimentul este utilizat pentru a monitoriza ratele de succes/insucces de la salvarea fișierelor și le mapează cu câteva proprietăți, cum ar fi dimensiunea fișierelor și locația în care sunt salvate (de ex. în cloud sau la nivel local). Proprietățile fișierelor ne permit să depanăm și să stabilim mai rapid cauza problemelor.

  - **Office.Visio.Shared.PostSave –** acest eveniment surprinde motivul nereușitei salvării fișierelor

  - **Office.Visio.VisioFilesaveAs –** acest eveniment colectează statisticile de „salvare ca” a fișierelor pentru Visio Dev16. Evenimentul este utilizat pentru a monitoriza ratele de succes/insucces de la „salvarea ca” a fișierelor și le mapează cu câteva proprietăți, cum ar fi dimensiunea fișierelor și locația în care sunt salvate (de ex. în cloud sau la nivel local). Proprietățile fișierelor ne permit să depanăm și să stabilim mai rapid cauza problemelor.

  - **Office.Visio.VisioFileSaveAsync –** acest eveniment colectează statisticile asincrone de la salvarea fișierelor pentru Visio Dev16. Evenimentul este utilizat pentru a monitoriza ratele de succes/insucces asincrone de la salvarea fișierelor și le mapează cu câteva proprietăți, cum ar fi dimensiunea fișierelor și locația în care sunt salvate (de ex. în cloud sau la nivel local). Proprietățile fișierelor ne permit să depanăm și să stabilim mai rapid cauza problemelor.

  - **Office.Visio.VisioFileSaveSync –** acest eveniment colectează statisticile sincrone de la salvarea fișierelor pentru Visio Dev16. Evenimentul este utilizat pentru a monitoriza ratele de succes/insucces sincrone de la salvarea fișierelor și le mapează cu câteva proprietăți, cum ar fi dimensiunea fișierelor și locația în care sunt salvate (de ex. în cloud sau la nivel local). Proprietățile fișierelor ne permit să depanăm și să stabilim mai rapid cauza problemelor. Acest eveniment ne ajută să monitorizăm motivele de nereușită a salvării pentru un fișier.

#### <a name="officeextensibilitysandboxodpactivationhanging"></a>Office.Extensibility.Sandbox.ODPActivationHanging

Colectează atunci când un program de completare Office durează prea mult să se lanseze (> 5 sec). Utilizat pentru detectarea și remedierea problemelor cu lansarea programelor de completare Office.
 
Se colectează următoarele câmpuri:

- **AppID** - ID-ul aplicației

- **AppInfo** - date referitoare la tipul de program de completare (panou de activități sau UILess sau de conținut etc.) și la tipul de furnizor (Omen, SharePoint, sisteme de fișiere etc.)

- **AppInstanceId** - ID-ul instanței aplicației 

- **AssetId** - asset ID-ul aplicației

- **IsPreload** - indică dacă programul de completare este în curs de încărcare în fundal pentru îmbunătățirea performanței de activare

- **NumberOfAddinsActivated** - contor de programe de completare activate

- **RemoterType** - specifică tipul de program la distanță (de încredere, neautorizat, Win32webView, de încredere UDF etc.) utilizat pentru a activa programul de completare

- **StoreType** - origine a aplicației

- **TimeForAuth** - timp petrecut cu autentificarea 

- **TimeForSandbox** - timp petrecut în sandbox

- **TimeForServerCall** - timp petrecut cu apelarea serverului 

- **TotalTime** - timp total

- **UsesSharedRuntime** - arată dacă aplicația utilizează sau nu sharedRuntime.

#### <a name="officeofficemobileappactivationlaunch"></a>Office.OfficeMobile.AppActivation.Launch

Acest eveniment identifică prima dată și activările ulterioare prin triggere externe care activează aplicația. Activarea aplicației încarcă anumite dependențe responsabile pentru rularea fără probleme a aplicației și acest eveniment va înregistra dacă s-a încărcat cu succes. De asemenea, va înregistra sursa activării și intenția aplicației responsabilă pentru activarea aplicației

Se colectează următoarele câmpuri:

- **ActionName** - maparea valorilor întregi la numele acțiunii/caracteristicii invocate din punctul de activare.
 
- **ActivationType** - maparea valorilor întregi la sursa de activare
  
- **IsActionTriggered** - valoarea booleană pentru a stabili dacă acțiunea a fost declanșată după activarea cu succes a aplicației.

- **IsFirstRun** - valoarea booleană pentru a stabili dacă a fost prima rulare a aplicației sau o rulare ulterioară.
 

#### <a name="officeofficemobilefrefirstrunsetup"></a>Office.OfficeMobile.FRE.FirstRunSetup

Prima rulare a aplicației după instalare va declanșa acest eveniment repetat. Acesta va ajuta la identificarea instalărilor și actualizărilor automate din versiuni mai vechi ale aplicației și ne va permite să identificăm erorile actualizărilor automate, inclusiv cele de descărcare a încărcărilor de bibliotecă și a pachetelor de extindere/lingvistice.

Se colectează următoarele câmpuri:

- **IsFlightAssigned** - valoare booleană pentru a determina dacă utilizatorul a făcut parte dintr-un grup de pasageri preatribuiți care poate declanșa expunerea la anumite experiențe.

- **IsFRELoadSuccessful** - număr întreg menționând starea rezultatelor

#### <a name="onenoteappappbootcomplete-previous-name-officeonenoteandroidappappbootcomplete-officeandroidearlytelemetryappbootcomplete"></a>OneNote.App.AppBootComplete *(nume anterior)* , Office.OneNote.Android.App.AppBootComplete, Office.Android.EarlyTelemetry.AppBootComplete

Semnal critic utilizat pentru a ne asigura că utilizatorii consumatori noi (cont Microsoft) pot lansa și utiliza pentru prima dată cu succes OneNote.  Aceasta se folosește pentru a asigura detectarea regresiei critice pentru aplicația OneNote și starea serviciilor.  Dacă utilizatorii nu pot lansa aplicația pentru prima dată, acest lucru va declanșa un incident de severitate înaltă.

Se colectează următoarele câmpuri: 

- **ACTIVITY_BOOT_TIME_IN_MS** - timp necesar pentru a finaliza crearea activităților

- **Activity_Name** - numele activității deschise când pornește 

- **ANY_DIALOG_SHOWN** -indică dacă se afișează o casetă de dialog în timpul încărcării

- **APP_SUSPEND_DURING_EVENT** - indică dacă încărcarea a fost preinstalată

- **APP_THREAD_CREATION_WAIT_TIME_TIME_FOR_APP_THREAD_CREATION** - timp necesar pentru a crea fire de aplicație

- **AVAILABLE_MEMORY_IN_MB** - memorie totală disponibilă pe dispozitiv 

- **AVG_SNAPSHOT_POPULATION_TIME** - timp mediu necesar să preluați structurile de blocnotes în timp ce utilizați aplicația

- **BOOT_END_AT_VIEW** - sub-categoria de nume de activitate (numele vizualizării)

- **BOOT_SNAPSHOTS** - detaliul structurii blocnotesului preia pentru conturile utilizate în aplicația

- **COREAPP_STARTUP_ACCOUNT_SETUP_STARTUP_ACCOUNT_SETUP** - timp necesar pentru a verifica și a iniția experiența SSO

- **CRASH_INTERACTION_DURING_BOOT > 0** - pentru a indica dacă aplicația s-a defectat în timpul ultimei sesiuni

- **DALVIK_HEAP_LIMIT_IN_MB** - învechit

- **DELAY_LOAD_STICKY_NOTES** - indică dacă notele aderente sunt întârziate sau nu

- **FISHBOWL_SHOWN_DURING_EVENT** - indică cazurile în care conținutul nu este sincronizat

- **HAS_LOGCAT_LOGGING_IMPACT_ON_BOOT** - indică dacă timpul de încărcare este afectat din cauza jurnalelor

- **INIT_SNAPSHOT_DURATION** - timp necesar pentru a obține structura blocnotesului pentru conturile de utilizator

- **IS_COLD_BOOT** - indică dacă lansați aplicația când aceasta nu rulează în fundal

- **IS_FIRST_LAUNCH** - indică dacă aceasta este prima dată când aplicația a fost lansată pe dispozitiv

- **IS_FOLDABLE_TYPE** - indică dacă dispozitivul este un dispozitiv pliabil

- **IS_PHONE** - indică dacă dispozitivul este un telefon sau o tabletă

- **IS_RECENT_PAGES_AVAILABLE_ON_FRAGMENT_CREATION** - indică dacă interfața de utilizator este gata și așteaptă să fie pus la dispoziție conținutul  

- **IS_REHYDRATE_LAUNCH** - indică dacă aplicația a fost oprită de sistem

- **IS_UPGRADE** -indică dacă aplicația este lansată după upgrade

- **JOT_MAIN_APP_CREATE_TIME_MAIN_APP_CREATE_TIME** - timp necesar pentru a crea o componentă de notă (componentă de cod partajat) 

- **JOT_MAIN_APP_INIT_TIME_MAIN_APP_INIT_TIME** - timp necesar pentru a inițializa componenta NOTĂ

- **LAUNCH_POINT** - indică dacă aplicația este deschisă de pe widget sau de la pictograma de aplicație sau cu un hyperlink sau de la partajare la ON etc.

- **MSO_ACTIVATION_TIME_ACTIVATION_TIME** - timp necesar pentru inițializarea MSO

- **NATIVE_LIBRARIES_LOAD_TIME** - timp necesar pentru încărcarea bibliotecilor

- **NAVIGATION_CREATE_TO_NAVIGATION_RESUME_CREATE_TO_NAVIGATION_RESUME** - timp necesar pentru navigarea completă

- **NAVIGATION_RESUME_TO_BOOT_END_RESUME_TO_BOOT_END** - timp necesar pentru a măsura întârzierea în încărcarea paginilor după pornire

- **NAVIGATION_SET_CONTENT_VIEW_TIME_SET_CONTENT_VIEW_TIME** - timp necesar pentru a aduce conținut

- **NUMBER_Of_RUNNING_PROCESSES** - indică numărul de procese active care rulează

- **NUMBER_OF_SNAPSHOTS** - număr de preluări a structurii blocnotesului în timpul încărcării

- **OFFICEASSETMANAGER_INITIALIZATION_TIME** - timp necesar pentru a dezarhiva și a inițializa Asset Manager

- **PROCESS_BOOT_TIME_IN_MS** - timp necesar pentru a finaliza crearea activităților

- **ROOT_ACTIVITY_CREATE_ACTIVITY_CREATE** - timp de tranziție din stratul rădăcină 

- **ROOT_ACTIVITY_DISK_CHECK_ACTIVITY_DISK_CHECK** - învechit

- **ROOT_ACTIVITY_LAUNCH_NEXTACTIVITY_ACTIVITY_LAUNCH_NEXTACTIVITY** -învechit

- **ROOT_ACTIVITY_PROCESS_INTENT_ACTIVITY_PROCESS_INTENT** -învechit 

- **ROOT_ACTIVITY_SESSION_ACTIVITY_SESSION** - timp de tranziție din stratul rădăcină 

- **ROOT_TO_NAVIGATION_TRANSITION_TO_NAVIGATION_TRANSITION** - timp necesar pentru a gestiona navigarea din rădăcină

- **SNAPSHOT_PUBLISH_TO_RENDERING_END_PUBLISH_TO_RENDERING_END** - timp pentru a finaliza conținutul de randare

- **SPLASH_ACTIVITY_SESSION_ACTIVITY_SESSION** - timp necesar pentru afișarea ecranului de pornire

- **SPLASH_TO_ROOT_TRANSITION_TO_ROOT_TRANSITION** - timp de tranziție din stratul rădăcină 

- **TIME_BETWEEN_PROCESS_BOOT_AND_ACTIVITY_BEGIN_IN_MS** - Durata între proces & crearea activităților 

- **TIME_TAKEN_IN_MS** - timp necesar pentru a finaliza încărcarea
 
- **TOTAL_MEMORY_IN_MB** - total memorie de pe dispozitiv
 
- **USER_INTERACTED_DURING_EVENT** - indică dacă utilizatorul a interacționat în timpul încărcării

#### <a name="onenoteapponenoteappforeground-previous-name-officeonenoteandroidapponenoteappforeground-officeandroidearlytelemetryonenoteappforeground"></a>OneNote.App.OneNoteAppForeground *(nume anterior)* , Office.OneNote.Android.App.OneNoteAppForeground, Office.Android.EarlyTelemetry.OneNoteAppForeground

Semnalul folosit pentru a indica aplicația OneNote este în prim plan.  Telemetria se folosește pentru a asigura detectarea regresiei critice pentru aplicația OneNote și starea serviciilor. 

Următoarele câmpuri sunt colectate: Niciunul

#### <a name="onenoteapplaunch-previous-name-officeandroidearlytelemetryapplaunch-officeonenoteandroidapplaunch"></a>OneNote.AppLaunch *(nume anterior)* , Office.Android.EarlyTelemetry.AppLaunch, Office.OneNote.Android.AppLaunch

Semnal critic utilizat pentru a ne asigura că utilizatorii OneNote pot lansa cu succes aplicația.  Telemetria se folosește pentru a asigura detectarea regresiei critice pentru aplicația OneNote și starea serviciilor. 

Se colectează următoarele câmpuri: 

- **ANDROID_SDK_VERSION** - captează versiunea SDK Android

- **FirstLaunchTime** - timpul înregistrărilor când a fost lansată prima dată aplicația

- **InstallLocation** - indică dacă aplicația este preinstalată sau este descărcată din Store

- **is_boot_completed_ever** - indică dacă aplicația a fost lansată cu succes înainte pe dispozitiv

- **IS_DARK_MODE_ENABLED** - o valoare Booleană care indică dacă aplicația este în modul întunecat sau nu

- **NewOneNoteUser** - identificați dacă utilizatorul este nou

#### <a name="officeoutlookdesktopexchangepuidandtenantcorrelation"></a>Office.Outlook.Desktop.ExchangePuidAndTenantCorrelation

Colectează codul PUID al utilizatorului și identificatorul de entitate găzduită, o dată pe sesiune. Corelarea PUID cu entitatea găzduită este necesară pentru a înțelege și a diagnostica problemele cu Outlook pentru fiecare entitate găzduită.

Se colectează următoarele câmpuri:

  - **CollectionTime** – marca de timp a evenimentului

  - **ConnId** – identificatorul de conexiune care analizează PUID și identificatorul entității găzduite OMS

  - **OMSTenantId** – identificatorul unic generat de Microsoft al entității găzduite

  - **PUID** – codul PUID Exchange pentru a identifica în mod unic utilizatorii


#### <a name="officeoutlookmacmacolkactivationstate"></a>Office.Outlook.Mac.MacOLKActivationState

Colectează modul în care este activat Outlook, cum ar fi cu abonament sau cu o licență de volum. Datele sunt monitorizate pentru a garanta că nu vedem valori maxime în erori. De asemenea analizăm datele pentru a găsi zone care necesită îmbunătățiri. 

Se colectează următoarele câmpuri:

- **SetupUIActivationMethod** - metoda de activare Outlook, cum ar fi abonamentul sau licența de volum

#### <a name="officepowerpointdocoperationopen"></a>Office.PowerPoint.DocOperation.Open 

Colectat de câte ori PowerPoint deschide un fișier. Conține informații de succes, detalii despre erori, măsurători de performanță și detalii de bază despre fișier, inclusiv tipul de format și metadatele de document. Aceste informații sunt necesare pentru a vă asigura că PowerPoint poate deschide fișierele cu succes, fără degradarea performanței. Acest lucru ne permite să diagnosticăm orice probleme descoperite.

Se colectează următoarele câmpuri:

  - **Data\_AddDocTelemetryResult –** această intrare în jurnal are toate datele de telemetrie necesare pentru documente (câmpurile Data\_Doc\_\*)

  - **Data\_AddDocumentToMruList –** durata de executare a metodei AddDocumentToMruList

  - **Data\_AlreadyOpened –** acest document a fost deschis anterior (în contextul aceleiași sesiuni de proces)

  - **Data\_AntiVirusScanMethod –** setul predefinit de valori de tipul scanat (IOAV, AMSI, None etc.)

  - **Data\_AntiVirusScanStatus –** setul predefinit de valori pentru scanarea antivirus care apare pentru fiecare document deschis (NoThreatsDetected, Failed, MalwareDetected etc.)

  - **Data\_AsyncOpenKind –** setul predefinit de valori pentru opțiunile asincrone (Collab, ServerOnly, SyncBacked, NotAsync)

  - **Data\_CancelBackgroundDownloadHr –** s-a întrerupt descărcarea documentului? Dacă da, care a fost rezultatul întreruperii?

  - **Data\_CheckForAssistedReadingReasons –** durata executării metodei CheckForAssistedReadingReasons în milisecunde

  - **Data\_CheckForDisabledDocument –** durata executării metodei CheckForDisabledDocument în milisecunde

  - **Data\_CheckForExistingDocument –** durata executării metodei CheckForExistingDocument în milisecunde

  - **Data\_CheckIncOpenResult –** durata executării metodei CheckIncOpenResult în milisecunde

  - **Data\_CheckLambdaResult –** durata executării metodei CheckLambdaResult în milisecunde

  - **Data\_CheckPackageForRequiredParts –** durata executării metodei CheckPackageForRequiredParts în milisecunde

  - **Data\_CheckPackageForSpecialCases –** durata executării metodei CheckPackageForSpecialCases în milisecunde

  - **Data\_CheckRequiredPartsLoaded –** durata executării metodei CheckRequiredPartsLoaded în milisecunde

  - **Data\_CheckWebSharingViolationForIncOpen –** durata executării metodei CheckWebSharingViolationForIncOpen în milisecunde
   
  - **Data_CloseAndReopenWithoutDiscard -** dacă un document a fost închis și redeschis în timpul procesului de deschidere fără a fi eliminat.

  - **Data\_ContentTransaction –** set predefinit de valori pentru momentul când se poate crea tranzacția (AllowedOnLoadDocument, AllowedOnOpenComplete etc.)

  - **Data_CorrelationId -** un GUID a trecut la PowerPoint prin ProtocolHandler pentru corelarea telemetriei. ProtocolHandler este un proces separat care gestionează linkurile Office pentru sistemul de operare.

  - **Data\_CppUncaughtExceptionCount:long -** excepții native necaptate în timp ce rula activitatea

  - **Data\_CreateDocumentTimeMS –** durata executării metodei CreateDocumentTimeMS în milisecunde

  - **Data\_CreateDocumentToken –** durata executării metodei CreateDocumentToken în milisecunde

  - **Data\_CreateDocumentToW –** durata executării metodei CreateDocumentToW în milisecunde

  - **Data\_CreateDocWindow –** durata executării metodei CreateDocWindow în milisecunde

  - **Data\_CreateLocalTempFile –** durata executării metodei CreateLocalTempFile în milisecunde

  - **Data\_DetachedDuration:long –** timpul cât activitatea a fost detașată/nu a rulat

  - **Data\_DetermineFileType –** durata executării metodei DetermineFileType în milisecunde

  - **Data\_Doc\_AccessMode:long –** cum a fost deschis acest document (doar în citire/citire-scriere)

  - **Data\_Doc\_AssistedReadingReasons:long -** set predefinit de valori pentru care documentul a fost deschis în modul de citire asistată

  - **Data_Doc_AsyncOpenKind:long –** indică dacă s-a deschis o versiune memorată în cache a documentului cloud și ce logică de reîmprospătare asincronă s-a folosit.

  - **Data\_Doc\_ChunkingType:long -** cum este stocat documentul în SharePoint

  - **Data\_Doc\_EdpState:long -** starea Enterprise Data Protection a documentului

  - **Data\_Doc\_Ext:string -** extensia documentului

  - **Data\_Doc\_Extension:string -** extensia documentului

  - **Data\_Doc\_FileFormat:long -** set predefinit de valori pentru formatul fișierului (mai granular decât extensia)

  - **Data\_Doc\_Fqdn:string –** unde este stocat documentul (SharePoint.com, live.net), disponibil numai pentru domeniile Office 365

  - **Data\_Doc\_FqdnHash:string –** codul hash al locului unde este stocat documentul

  - **Data\_Doc\_IdentityTelemetryId:string –** GUID unic al utilizatorului

  - **Data\_Doc\_IdentityUniqueId:string –** identificator unic al identității folosite pentru acțiunea Documente partajate

  - **Data\_Doc\_IOFlags:long -** bitmask pentru diferite semnalizări legate de IO pentru un anumit document

  - **Data\_Doc\_IrmRights:long -** set predefinit de valori pentru tipul de Information Rights Management aplicat pentru acest document (Redirecționare, Răspuns, SecureReader, Editare etc.)

  - **Data\_Doc\_IsCloudCollabEnabled:bool –** true dacă antetul „IsCloudCollabEnabled” a fost deja primit dintr-o solicitare OPTIONS.

  - **Data\_Doc\_IsIncrementalOpen:bool –** documentul a fost deschis incremental (caracteristică nouă care deschide documentul fără să-l descarce în totalitate)

  - **Data\_Doc\_IsOcsSupported:bool -** dacă documentul acceptă elaborarea în comun folosind noul serviciu OCS

  - **Data\_Doc\_IsOpeningOfflineCopy:bool -** documentul este deschis din memoria cache locală?

  - **Data\_Doc\_IsSyncBacked:bool -** dacă documentul este deschis din folderul care folosește aplicația de sincronizare inversă OneDrive

  - **Data\_Doc\_Location:long -** set predefinit de valori privind locul de stocare a documentului (Local, SharePoint, WOPI, Rețea etc.)

  - **Data\_Doc\_LocationDetails:long –** set predefinit de valori privind locația mai detaliată (folderul Temp, folderul de descărcări, Documente OneDrive, Imagini OneDrive etc.)

  - **Data\_Doc\_NumberCoAuthors:long -** numărul de coautori la momentul deschiderii unui document

  - **Data\_Doc\_PasswordFlags:long -** set predefinit de valori privind modul în care documentul este criptat cu o parolă (Fără, parolă pentru citire, parolă pentru editare)

  - **Data\_Doc\_ReadOnlyReasons:long –** set predefinit de valori privind motivul pentru care acest document a fost marcat doar în citire (blocat pe server, document final, protejat prin parolă pentru editare etc.)

  - **Data\_Doc\_ResourceIdHash:string -** codul hash al identificatorului de resurse pentru documentele stocate în cloud

  - **Data_Doc_RtcType -**  indică modul în care a fost configurat canalul în timp real (RTC) pentru fișierul curent (dezactivat, neacceptat, la cerere, activat permanent etc.).

  - **Data\_Doc\_ServerDocId:string –** identificatorul imutabil pentru documentele stocate în cloud

  - **Data\_Doc\_ServerProtocol:long -** set predefinit de valori privind protocolul folosit în comunicarea cu serverul (Http, Cobalt, WOPI etc.)
 
  - **Data\_Doc\_ServerType:long –** set predefinit de valori privind tipul serverului (SharePoint, DropBox, WOPI)

  - **Data\_Doc\_ServerVersion:long –** dacă serverul se bazează pe Office14, Office15, Office 16

  - **Data\_Doc\_SessionId:long –** GUID generat care identifică instanța documentului din aceeași sesiune de proces

  - **Data\_Doc\_SharePointServiceContext:string -** un șir opac, de obicei GridManagerID.FarmID. Util pentru corelarea jurnalelor de la client și de pe server

  - **Data\_Doc\_SizeInBytes:long -** dimensiunea documentului în octeți

  - **Data\_Doc\_SpecialChars:long -** Bitmask ce arată caracterele speciale din adresa URL sau calea documentului

  - **Data\_Doc\_StorageProviderId:string -** șir care identifică furnizorul de stocare al documentului, precum „DropBox”

  - **Data\_Doc\_StreamAvailability:long –** set predefinit de valori privind starea șirului de document (disponibil, dezactivat definitiv, indisponibil)

  - **Data\_Doc\_UrlHash:string –** codul hash pentru adresa URL completă a documentelor stocate în cloud

  - **Data\_Doc\_UsedWrsDataOnOpen:bool –** true dacă fișierul a fost deschis incremental folosind datele WRS prememorate în cache pentru gazdă

  - **Data\_Doc\_WopiServiceId:string –** identificatorul serviciului WOPI, de ex. „Dropbox”

  - **Data\_DownloadExcludedData –** durata executării metodei DownloadExcludedData în milisecunde

  - **Data\_DownloadExcludedDataTelemetry –** set predefinit de valori privind starea de așteptare sincronă a descărcării (SynchronousLogicHit, UserCancelled RunModalTaskUnexpectedHResult etc.)

  - **Data\_DownloadFileInBGThread –** durata executării metodei DownloadFileInBGThread în milisecunde

  - **Data\_DownloadFragmentSize –** dimensiunea fragmentului (parte de fișier care se poate descărca), de obicei 3,5 MB

  - **Data\_ExcludedEmbeddedItems –** numărul de părți zip excluse pentru prima redare

  - **Data\_ExcludedEmbeddedItemsSize –** dimensiunea totală a părților zip excluse pentru prima redare

  - **Data\_ExcludedRequiredItems –** numărul de părți zip excluse, dar obligatorii pentru prima redare

  - **Data\_ExcludedRequiredItemsSize –** dimensiunea totală a părților zip excluse, dar obligatorii pentru prima redare

  - **Data\_ExecutionCount –** numărul de executări ale protocolului IncOpen

  - **Data\_FailureComponent:long -** set predefinit de valori privind componenta care a cauzat nereușita protocolului (Conflict, CSI, Internă etc.)

  - **Data\_FailureReason:long –** set predefinit de valori privind motivul nereușitei (FileIsCorrupt, BlockedByAntivirus etc.)

  - **Data\_FCreateNew –** este acesta un document nou și necompletat

  - **Data\_FCreateNewFromTemplate –** este acesta un document nou din șabloane

  - **Data_FErrorAfterDocWinCreation:boolean-**  s-a produs o eroare sau o excepție după ce a fost creată fereastra de document.

  - **Data\_FileUrlLocation –** set predefinit de valori privind locul unde este stocat documentul (NetworkShare, LocalDrive, ServerOther etc.)

  - **Data\_FirstSlideCompressedSize –** dimensiunea comprimată a părții zip din primul diapozitiv (de obicei Slide1.xml)

  - **Data_FIsAutoBackupFile-** Acest fișier este un fișier de backup automat?

  - **Data\_FIsDownloadFileInBgThreadEnabled –** este activată pentru șir descărcarea pe fundal?

  - **Data\_fLifeguarded:bool –** documentul a fost vreodată protejat (caracteristică pentru a remedia automat erorile din documente, fără intervenția utilizatorului)?

  - **Data\_ForceReopenOnIncOpenMergeFailure –** marcaj care arată dacă am fost obligați să redeschidem din cauza erorii de îmbinare din Inc Open

  - **Data\_ForegroundThreadPass0TimeMS –** (exclusiv pentru Mac) timpul total petrecut în firul din prim-plan la prima trecere

  - **Data\_ForegroundThreadPass1TimeMS –** (exclusiv pentru Mac) timpul total petrecut în firul din prim-plan la a doua trecere

  - **Data\_FWebCreatorDoc –** documentul este creat din șablon sau din QuickStarter

  - **Data\_HasDocToken –** acest document are un token CSI doc (cod intern)

  - **Data\_HasDocument –** acest document are un document CSI (cod intern)

  - **Data\_InclusiveMeasurements –** duratele de măsurare a metodelor includ durata de apelare a metodei secundare

  - **Data\_IncompleteDocReasons –** set predefinit de valori pentru care deschiderea a fost incompletă (Necunoscut, DiscardFailure etc.)

  - **Data\_IncOpenDisabledReasons –** set predefinit de valori ale motivelor pentru care deschiderea incrementală a fost dezactivată

  - **Data\_IncOpenFailureHr –** rezultatul motivului pentru cade deschiderea incrementală nu a reușit

  - **Data\_IncOpenFailureTag –** eticheta (indicator spre locația codului) locului în care nu a reușit deschiderea incrementală

  - **Data\_IncOpenFallbackReason –** de ce nu a rulat IncOpen

  - **Data\_IncOpenRequiredTypes –** set predefinit de valori pentru tipurile de conținut necesare pentru prima redare (RequiredXmlZipItem, RequiredNotesMaster etc.)

  - **Data\_IncOpenStatus –** set predefinit de valori pentru starea deschiderii incrementale (Încercată, FoundExcludedItems, DocIncOpenInfoCreated etc.)

  - **Data\_InitFileContents –** durata executării metodei InitFileContents în milisecunde

  - **Data\_InitialExcludedItems –** numărul de părți zip excluse inițial

  - **Data\_InitialExcludedItemsSize –** dimensiunea totală a părților zip excluse inițial

  - **Data\_InitializationTimeMS –** (exclusiv pentru Mac) timpul de inițializare

  - **Data\_InitialRoundtripCount –** numărul de răspunsuri de la server necesare pentru a forma arhiva zip inițială

  - **Data\_InitLoadProcess –** durata executării metodei InitLoadProcess în milisecunde

  - **Data\_InitPackage –** durata executării metodei InitPackage în milisecunde

  - **Data\_InitSecureReaderReasons –** durata executării metodei InitSecureReaderReasons în milisecunde

  - **Data\_IsIncOpenInProgressWhileOpen –** în cazul deschiderii multiple a aceluiași document, protocolul de deschidere Inc rulează împreună cu cel deschis?

  - **Data\_IsMultiOpen –** acceptăm deschiderea multiplă?

  - **Data\_IsOCS –** documentul a fost în modul OCS în ultima stare cunoscută

  - **Data\_IsODPFile –** documentul este în formatul „Open Document Format” folosit de OpenOffice.org

  - **Data\_IsPPTMetroFile –** documentul are format metro (pptx)

  - **Data\_LoadDocument –** durata executării metodei LoadDocument în milisecunde

  - **Data\_MeasurementBreakdown –** detalierea măsurătorii codificate (perf metodă detaliată scurtată)

  - **Data\_Measurements –** măsurători codificate

  - **Data\_MethodId –** ultima metodă executată

  - **Data\_NotRequiredExcludedItems –** numărul total de elemente din pachet PowerPoint care nu sunt necesare pentru prima redare și excluse

  - **Data\_NotRequiredExcludedItemsSize –** dimensiunea totală a elementelor din pachet PowerPoint care nu sunt necesare pentru prima redare și excluse

  - **Data\_NotRequiredExcludedParts –** numărul total de părți zip care nu sunt necesare pentru prima redare și excluse

  - **Data\_NotRequiredExcludedPartsSize –** numărul total de părți zip care nu sunt necesare pentru prima redare și excluse

  - **Data_OngoingBlockingOpenCount –** este numărul de protocoale deschise blocante deschise care rulează în prezent.
  
  - **Data_OngoingOpenCount –** este numărul de protocoale deschise care rulează în prezent.

  - **Data\_OpenCompleteFailureHR –** rezultatul motivului pentru care nu a funcționat protocolul OpenComplete

  - **Data\_OpenCompleteFailureTag –** eticheta (indicator spre locația codului) pentru locul în care nu a reușit protocolul OpenComplete

  - **Data\_OpenLifeguardOption –** set predefinit de valori ale opțiunilor pentru operațiunea de protejare (None, TryAgain, OpenInWebApp etc.)

  - **Data\_OpenReason –** set predefinit de valori privind modul în care a fost deschis documentul (FilePicker, OpenFromMru, FileDrop etc.)

  - **Data\_OSRPolicy –** politica SecureReader

  - **Data\_OSRReason –** motive pentru care acest document a fost deschis în Secure Reader

  - **Data\_OtherContentTypesWithRequiredParts –** tipurile de conținut nestandard care au fost excluse, dar obligatorii pentru prima redare

  - **Data\_PrepCacheAsync –** marcaj pentru OcsiOpenPerfPrepCacheAsync

  - **Data\_PreviousDiscardFailed –** indică faptul că încercarea anterioară de deschidere/închidere a documentului nu a eliberat corect toată memoria

  - **Data\_PreviousFailureHr –** în cazul redeschiderii aceluiași document, care a fost rezultatul ultimei erori

  - **Data\_PreviousFailureTag –** În cazul redeschiderii aceluiași document, care a fost eticheta ultimei erori (indicator spre locația codului)

  - **Data\_RemoteDocToken –** este activată Deschiderea de la distanță (caracteristica prototipului care activează deschiderea fișierului din serviciu, nu din gazdă)?

  - **Data\_Repair –** suntem în modul de reparare a documentelor (pentru documentele deteriorate care pot fi remediate)

  - **Data\_RequestPauseStats –** de câte ori a solicitat codul întreruperea înregistrării performanței

  - **Data\_RequiredPartsComressedSize –** dimensiunea totală a componentelor PowerPoint obligatorii pentru prima redare

  - **Data\_RequiredPartsDownload –** dimensiunea totală a componentelor PowerPoint care sunt descărcate

  - **Data\_RequiredPartsRoundtripCount –** numărul total de circuite (apelări ale gazdei) necesare pentru a obține toate componentele PowerPoint obligatorii pentru prima redare

  - **Data\_RequiredZipItemsDownload –** dimensiunea totală a elementelor zip obligatorii pentru prima redare

  - **Data\_RequiredZipItemsRoundtripCount –** numărul total de circuite (apelări ale gazdei) necesare pentru a obține toate elementele zip obligatorii pentru prima redare

  - **Data\_RoundtripsAfterMissingRequiredParts –** numărul total de circuite (apelări ale gazdei) necesare după ce am găsit componentele PowerPoint obligatorii lipsă

  - **Data\_RoundtripsAfterMissingRequiredZipItems –** numărul total de circuite (apelări ale gazdei) necesare după ce am găsit elementele zip obligatorii lipsă

  - **Data\_RoundtripsAfterRequiredPackage –** numărul total de circuite (apelări ale gazdei) necesare după ce am creat pachetul

  - **Data\_RoundtripsAfterRequiredParts –** numărul total de circuite (apelări ale gazdei) necesare după ce am descărcat toate componentele lipsă

  - **Data\_SetDocCoAuthAutoSaveable –** durata executării metodei SetDocCoAuthAutoSaveable în milisecunde

  - **Data\_SniffedFileType –** o estimare educată a tipului de fișier propus pentru documentul corupt

  - **Data\_StartTime –** contorul de performanță la pornirea deschiderii

  - **Data\_StopwatchDuration:long –** timpul total al activității

  - **Data\_SyncSlides –** durata executării metodei SyncSlides în milisecunde

  - **Data\_TimerStartReason –** set predefinit de valori privind pornirea temporizatorului (CatchMissedSyncStateNotification, WaitingForFirstDownload etc.)

  - **Data\_TimeSplitMeasurements –** detalierea măsurătorii codificate (performanța metodei detaliate scurtate)

  - **Data\_TimeToInitialPackage –** timpul necesar pentru a crea pachetul inițial

  - **Data\_TimeToRequiredPackage –** timpul necesar pentru a crea pachetul obligatoriu

  - **Data\_TimeToRequiredParts –** timpul necesar pentru a crea pachetul cu toate componentele obligatorii

  - **Data\_TotalRequiredParts –** numărul total de componente PowerPoint obligatorii pentru prima redare

  - **Data\_TotalRequiredParts –** numărul total de componente nestandard obligatorii pentru prima redare

  - **Data\_UnpackLinkWatsonId –** identificatorul Watson al erorii atunci când documentul este deschis prin adresa URL Share OneDrive

  - **Data\_UnpackResultHint –** set predefinit de valori privind rezultatele URL pentru partajare la dezarhivare (NavigateToWebWithoutError, UrlUnsupported, AttemptOpen etc.)

  - **Data\_UnpackUrl –** durata executării metodei UnpackUrl în milisecunde

  - **Data\_UpdateAppstateTimeMS –** durata executării metodei UpdateAppstate în milisecunde

  - **Data\_UpdateCoauthoringState –** durata executării metodei UpdateCoauthoringState în milisecunde

  - **Data\_UpdateReadOnlyState –** durata executării metodei UpdateReadOnlyState în milisecunde

  - **Data\_WACCorrelationId –** în caz că deschideți fișierul în browser, obțineți corelarea jurnalelor WebApp

  - **Data\_WasCachedOnInitialize –** acest document a fost memorat în cache în timpul inițializării

  - **Data\_WBDirtyBeforeDiscard –** dacă ramificația care funcționează a devenit defazată înainte de a redeschide documentul

  - **Data\_ZRTOpenDisabledReasons –** de ce nu am putut deschide documentul din cache (Zero circuite)

#### <a name="officepowerpointpptdesktopbootime"></a>Office.PowerPoint.PPT.Desktop.Bootime

Colectează modul în care se inițializează PowerPoint. Acesta include inițializarea PowerPoint în vizualizarea protejată, în modul de citire asistat, din macrocomenzi, din documente imprimate, din documente noi și necompletate, din recuperarea documentelor, din automatizare și dacă este clic și pornire. De asemenea, colectează durata necesară pentru încărcarea PowerPoint. Aceste date sunt esențiale pentru a garanta că PowerPoint se descurcă bine atunci când este inițializat din moduri diferite. Microsoft utilizează aceste date pentru a surprinde timpii lungi de inițializare la deschiderea PowerPoint din moduri diferite.

Se colectează următoarele câmpuri:

  - **AssistedReading –** în modul de citire asistată

  - **Automation –** din automatizare

  - **Benchmark –** rulați testul de performanță

  - **Blank –** document necompletat

  - **BootTime –** timpul de inițializare a sesiunii

  - **Embedding –** documentul de încorporare

  - **IsC2R –** este clic și pornire

  - **IsNew –** document nou

  - **IsOpen –** este deschis

  - **Macro1 –** rulați macrocomanda

  - **Macro2 –** rulați macrocomanda

  - **NonStandardSpaceInCmdLine** – există un spațiu nestandard în linia de comandă

  - **Print –** document imprimat

  - **PrintDialog –** document imprimat cu caseta de dialog

  - **PrintPrinter –** document imprimat cu imprimanta

  - **ProtectedView –** în vizualizarea protejată

  - **Regserver –** înregistrați PowerPoint ca server COM

  - **Restore –** restaurați documentul

  - **Show –** afișați documentul

  - **Time –** durata sesiunii

  - **UnprotectedView –** în vizualizarea neprotejată

#### <a name="officepowerpointppthasuserediteddocument"></a>Office.PowerPoint.PPT.HasUserEditedDocument

Colectat atunci când un utilizator începe să editeze un document. Microsoft utilizează aceste date pentru a calcula utilizatorii activi care au editat un document PowerPoint

Se colectează următoarele câmpuri:

  - **CorrelationId** – identificatorul de corelare al documentului

#### <a name="officeprojectbootandopenproject"></a>Office.Project.BootAndOpenProject

Proiect este inițializat prin deschiderea unui fișier. Acest eveniment indică faptul că un utilizator a deschis Office Project cu un fișier asociat. Acesta conține datele de succes critice pentru a vă asigura că Project poate să înceapă și să încarce un fișier.

Se colectează următoarele câmpuri:

  - **Data\_AlertTime –** durata cât a fost activă caseta de dialog de inițializare.

  - **Data\_BootTime –** timpul necesar pentru a inițializa Project

  - **Data\_CacheFileSize –** dacă fișierul a fost memorat în cache, dimensiunea fișierului

  - **Data\_EntDocType –** tipul de fișier care a fost deschis

  - **Data\_IsInCache –** dacă fișierul deschis a fost memorat în cache

  - **Data\_LoadSRAs –** dacă utilizatorul vrea să încarce SRA sau nu

  - **Data\_Outcome –** timpul total de inițializare și de deschidere a fișierelor.

  - **Data\_OpenFromDocLib –** dacă fișierul Project deschis a fost din biblioteca de documente

  - **Data\_ProjectServerVersion –** versiunea și compilarea în care se află momentan Project

#### <a name="officeprojectbootproject"></a>Office.Project.BootProject

Proiectul este inițializat fără a deschide un fișier. Acest eveniment indică faptul că un utilizator a deschis Office Project fără un fișier asociat. Acesta conține datele de succes critice pentru a vă asigura că Project poate să înceapă.

Se colectează următoarele câmpuri:

  - **Data\_BootTime –** timpul necesar pentru a inițializa Project

  - **Data\_FileLoaded –** false dacă se deschide din afara spațiului sau dintr-un proiect nou, necompletat

  - **Data\_IsEntOfflineWithProfile –** dacă utilizatorii sunt în SKU profesional și nu sunt conectați la server

  - **Data\_IsEntOnline –** dacă sesiunea de Project este conectată la un server Project cu funcționalități de întreprindere

  - **Data\_IsLocalProfile –** dacă sesiunea Project este conectată la un server Project cu funcționalități de întreprindere

  - **Data\_ProjectServerVersion –** versiunea și compilarea în care se află momentan Project


#### <a name="officeprojectopenproject"></a>Office.Project.OpenProject

Proiect deschide un fișier. Acest eveniment indică faptul că un utilizator deschide direct un fișier Project. Acesta conține datele de succes critice pentru a deschide fișiere în Project.

Se colectează următoarele câmpuri:

  - **Data\_AgileMode –** definește dacă proiectul deschis este de tip cascadă sau agil

  - **Data\_AlertTime –** durata cât a fost activă caseta de dialog de inițializare

  - **Data\_CacheFileSize –** dacă fișierul a fost memorat în cache, dimensiunea fișierului

  - **Data\_EntDocType –** tipul de fișier care a fost deschis

  - **Data\_IsInCache –** dacă fișierul deschis a fost memorat în cache

  - **Data\_LoadSRAs –** dacă utilizatorul vrea să încarce SRA sau nu

  - **Data\_OpenFromDocLib –** dacă fișierul Project deschis a fost din biblioteca de documente

  - **Data\_Outcome –** timpul total de inițializare și de deschidere a fișierelor

  - **Data\_Outcome –** timpul total de inițializare și de deschidere a fișierelor.

  - **Data\_ProjectServerVersion –** versiunea și compilarea în care se află momentan Project

#### <a name="officesessionidproviderofficeprocesssessionstart"></a>Office.SessionIdProvider.OfficeProcessSessionStart

Aplicabile pentru toate aplicațiile Office bazate pe Windows: win32 și UWP

Se colectează următoarele câmpuri:

- **OfficeProcessSessionStart** trimite informații de bază la începutul unei noi sesiuni Office. Acestea sunt utilizate pentru a contoriza numărul de sesiuni unice văzute pe un anumit dispozitiv. Acesta se folosește ca eveniment mesaj repetat pentru a vă asigura că aplicația rulează sau nu pe un dispozitiv. În plus, servește ca semnal critic pentru fiabilitatea generală a aplicației

- **AppSessionGuid** – identificator al unei anumite sesiuni de aplicație ce începe la ora de creare a procesului și persistă până la sfârșitul procesului. Este formatat ca GUID standard pe 128 de biți, dar alcătuit din 4 părți. Aceste patru părți sunt, în ordine: (1) ID-ul de proces pe 32 de biți (2) ID-ul de sesiune pe 16 biți (3) ID-ul de inițializare pe 16 biți (4) timpul de creare a procesului pe 64 de biți, în UTC 100ns

- **processSessionId** – GUID generat aleator pentru a identifica sesiunea de aplicație

- **UTCReplace_AppSessionGuid** Office valoare booleană constantă. Întotdeauna true.

#### <a name="officesystemsessionhandoff"></a>Office.System.SessionHandoff

Indică faptul că sesiunea Office curentă este o sesiune de predare. Acest lucru înseamnă că tratarea unei solicitări de la utilizator pentru a deschide un document este transmisă unei instanțe care rulează deja din aceeași aplicație.

Se colectează următoarele câmpuri.

- **ParentSessionId** - ID-ul sesiunii care va prelua procesarea cererii utilizatorilor.

#### <a name="officetelemetryengineisprelaunch"></a>Office.TelemetryEngine.IsPreLaunch

Se aplică pentru aplicațiile Office UWP.  Acest eveniment se declanșează când o aplicație Office este inițiată pentru prima dată după upgrade-ul/instalarea din magazin. El face parte din datele de diagnosticare de bază, utilizate pentru a urmări dacă o sesiune este de lansare sau nu.

Se colectează următoarele câmpuri:

- **appVersionBuild** – Numărul de versiune al aplicației.

- **appVersionMajor** - numărul de versiune majoră al aplicației.

- **appVersionMinor** – Numărul de versiune minoră al aplicației.

- **appVersionRev** – Numărul de versiune pentru revizuirea aplicației.

- **SessionID** – GUID generat aleator pentru a identifica sesiunea de aplicație

#### <a name="officetelemetryenginesessionhandoff"></a>Office.TelemetryEngine.SessionHandOff

Se aplică la aplicațiile Office Win32.  Acest eveniment ne ajută să înțelegem dacă a existat o nouă sesiune creată pentru a gestiona un eveniment inițiat de utilizatori pentru deschiderea fișierelor. Este o informație de diagnosticare esențială, utilizată pentru a genera semnalul de fiabilitate și a vă asigura că aplicația funcționează așa cum vă așteptați.

Se colectează următoarele câmpuri:

- **appVersionBuild** – Numărul de versiune al aplicației.

- **appVersionMajor** - numărul de versiune majoră al aplicației.

- **appVersionMinor** – Numărul de versiune minoră al aplicației.

- **appVersionRev** – Numărul de versiune pentru revizuirea aplicației.

- **childSessionID** – GUID generat aleator pentru a identifica sesiunea de aplicație

- **parentSessionID** – GUID generat aleator pentru a identifica sesiunea de aplicație

#### <a name="officevisiovisioiosappboottime"></a>Office.Visio.VisioIosAppBootTime

Acest lucru este declanșat de fiecare dată când se încarcă aplicația iOS Visio. Este esențial să înțelegeți performanța de pornire a aplicației iOS Visio. Se utilizează pentru a depana performanța slabă. 

Se colectează următoarele câmpuri:

- **Data_AppBootTime** - durata necesară pentru ca aplicația să se încarce, în milisecunde.

#### <a name="officevisiovisioiosappresumetime"></a>Office. Visio. VisioIosAppResumeTime 

Acest eveniment este declanșat de fiecare dată când aplicația iOS Visio reia focalizarea. Este esențial să măsurați performanța reluaării aplicațiilor și să depanați problemele de performanță ale aplicației iOS Visio.

Se colectează următoarele câmpuri:

- **Data_AppResumeTime** - durată pentru a relua aplicația în milisecunde.

#### <a name="officewordfileopenopencmdfilemrupriv"></a>Office.Word.FileOpen.OpenCmdFileMruPriv

Acest eveniment indică faptul că Office Word deschide un document din lista Cel mai recent utilizate (Most Recent Used – MRU). În plus, conține date esențiale despre performanța la deschiderea fișierelor și este un eveniment de pornire a aplicației din perspectiva utilizatorului. Evenimentul monitorizează dacă fileopen-from-MRU funcționează așa cum trebuie. În plus, se folosește pentru a calcula utilizatorii/dispozitivele active lunar și măsurătorile de fiabilitate cloud.

Se colectează următoarele câmpuri:

- **Data_AddDocTelemRes** - raportează dacă am putut completa corect alte valori legate de telemetria documentelor din eveniment. Utilizat pentru diagnostice privind calitatea datelor.

- **Data_BytesAsynchronous** - numărul de byți (comprimat) fără care credem că putem deschide fișierul dacă îi obținem înainte ca utilizatorul să vrea să editeze sau să salveze

- **Data_BytesAsynchronousWithWork** - numărul de byți (comprimat) fără care credem că putem deschide fișierul, dar care ar necesita investiții de cod semnificative pentru a funcționa

- **Data_BytesSynchronous** - numărul de byți (comprimat) de care avem nevoie înainte să putem deschide fișierul

- **Data_BytesUnknown** - numărul de byți din părțile de documente pe care nu ne așteptăm să le găsim 

- **Data_DetachedDuration** - cât timp a fost activitatea detașată de fir

- **Data_Doc_AccessMode** - documentul este numai în citire/editabil

- **Data_Doc_AssistedReadingReasons** - set predefinit de valori privind motivul pentru care documentul a fost deschis în modul de citire asistată

- **Data_Doc_AsyncOpenKind –** indică dacă s-a deschis o versiune memorată în cache a documentului cloud și ce logică de reîmprospătare asincronă s-a folosit.

- **Data_Doc_ChunkingType** - unități utilizate pentru deschiderea incrementală a documentelor

- **Data_Doc_EdpState** - setare de protecție a datelor electronice pentru document

- **Data_Doc_Ext** - extensia documentului (docx/xlsb/pptx etc.)

- **Data_Doc_FileFormat** - versiunea de protocol pentru formatul fișierului

- **Data_Doc_Fqdn** - numele de domeniu OneDrive sau SharePoint Online

- **Data_Doc_FqdnHash** - codul hash unidirecțional pentru numele de domeniu identificabil al clientului

- **Data_Doc_IdentityTelemetryId** - codul hash unidirecțional pentru identitatea de utilizator folosită pentru deschidere

- **Data_Doc_InitializationScenario** - înregistrează cum a fost deschis documentul

- **Data_Doc_IOFlags** - rapoarte privind semnalizările memorate în cache folosite pentru a seta opțiuni de solicitare deschise

- **Data_Doc_IrmRights** - acțiunile permise de politica de protejare a datelor electronice aplicată pentru document/utilizator

- **Data_Doc_IsIncrementalOpen** - semnalizare care indică faptul că documentul a fost deschis incremental

- **Data_Doc_IsOcsSupported** - semnalizare care indică faptul că documentul este acceptat în serviciul de colaborare

- **Data_Doc_IsOpeningOfflineCopy** - semnalizare care indică faptul că s-a deschis copia offline a unui document

- **Data_Doc_IsSyncBacked** - semnalizare care indică faptul că pe computer există o copie sincronizată automat a documentului

- **Data_Doc_Location** - indică ce serviciu a furnizat documentul (OneDrive, File Server, SharePoint etc.)

- **Data_Doc_LocationDetails** - indică ce Folder cunoscut a furnizat un document stocat local

- **Data_Doc_NumberCoAuthors** - numărul de alți utilizatori dintr-o sesiune de editare în colaborare

- **Data_Doc_PasswordFlags** - arată semnalizările de parole pentru citire sau citire/scriere setate

- **Data_Doc_ReadOnlyReasons** - motivele pentru care documentul a fost deschis doar în citire

- **Data_Doc_ResourceIdHash** - identificator de document anonimizat, folosit în diagnosticarea problemelor

- **Data_Doc_RtcType** - indică modul în care a fost configurat canalul în timp real (RTC) pentru fișierul curent (dezactivat, neacceptat, la cerere, activat permanent etc.).

- **Data_Doc_ServerDocId** - identificator de document anonimizat și invariabil, folosit în diagnosticarea problemelor 

- **Data_Doc_ServerProtocol** - versiunea de protocol folosită în comunicarea cu serviciul

- **Data_Doc_ServerType** - tipul de server care oferă serviciul (SharePoint, OneDrive, WOPI etc.)

- **Data_Doc_ServerVersion** - versiunea serverului care oferă serviciul

- **Data_Doc_SessionId** - identifică o anumită sesiune de editare a documentului din sesiunea completă

- **Data_Doc_SharePointServiceContext** - informații de diagnosticare din solicitările SharePoint Online

- **Data_Doc_SizeInBytes** - indicator privind dimensiunea documentului

- **Data_Doc_SpecialChars** - indicator privind caracterele speciale din adresa URL a documentului 

- **Data_Doc_SyncBackedType** - indicator privind tipul documentului (local sau bazat pe servicii)

- **Data_Doc_UrlHash** - cod hash unidirecțional, pentru crearea unui identificator naiv de document

- **Data_Doc_WopiServiceId** - conține identificatorul unic al furnizorului de servicii WOPI

- **Data_EditorDisablingRename** - identificatorul primului editor care a provocat dezactivarea redenumirii

- **Data_EditorsCount** - numărul de editori din document

- **Data_ForceReadWriteReason** - valoare întreagă care reprezintă motivul pentru care fișierul a fost forțat în modul citire/scriere

- **Data_FSucceededAfterRecoverableFailure** - arată că deschiderea a reușit după repararea unei erori la deschiderea documentului

- **Data_LastLoggedTag** - etichetă unică pentru site-ul de apelare a codului folosit pentru a identifica momentele când încercăm să nu realizăm deschiderea de două ori (folosit pentru diagnosticarea calității datelor)

- **Data_LinkStyles** - indică dacă asociem stiluri de șabloane

- **Data_MainPdod** - identificatorul documentului din procesul Office Word

- **Data_Measurements** - șir codificat cu detalii de timp pentru diferitele părți ale deschiderii. Utilizat pentru a măsura performanța.

- **Data_MoveDisabledReason** - eroarea care dezactivează mutarea pentru document

- **Data_MoveFlightEnabled** - dacă ediția flight este activată pentru caracteristica de mutare

- **Data_PartsUnknown** - numărul de părți ale documentului pentru care nu am putut obține date

- **Data_RecoverableFailureInitiationLocationTag** - etichetă unică pentru site-ul de apelare a codului folosit pentru a identifica locul din cod în care încercăm să remediem fișierul înainte de a-l deschide

- **Data_RenameDisabledReason** - eroare care face redenumirea să fie dezactivată pentru acest document

- **Data_RenameFlightEnabled** - dacă este activată ediția flight pentru caracteristica de redenumire

- **Data_SecondaryTag** - etichetă unică pentru site-ul de apelare a codului folosit pentru a adăuga date suplimentare despre erori pentru deschidere 

- **Data_TemplateFormat** - formatul de fișier al șablonului pe care se bazează documentul

- **Data_UsesNormal** - indică dacă documentul deschis se bazează pe șablonul normal

- **PathData_Doc_StreamAvailability** - indicator care arată dacă șirul documentului este disponibil/dezactivat


#### <a name="officewordfileopenopenffileopenxstzcore"></a>Office.Word.FileOpen.OpenFFileOpenXstzCore

Acest eveniment indică faptul că Office Word deschide un document pe care a făcut dublu clic un utilizator. În plus, conține date esențiale despre performanța la deschiderea fișierelor și este un eveniment de pornire a aplicației din perspectiva utilizatorului. Evenimentul monitorizează dacă file-openfrom-file-double-click funcționează așa cum vă așteptați. În plus, se folosește pentru a calcula utilizatorii/dispozitivele active lunar și măsurătorile de fiabilitate cloud.

Se colectează următoarele câmpuri:

- **Data_AddDocTelemRes** - raportează dacă am putut completa corect alte valori legate de telemetria documentelor din eveniment. Utilizat pentru diagnostice privind calitatea datelor
    
- **Data_BytesAsynchronous** - numărul de byți (comprimat) fără care credem că putem deschide fișierul dacă îi obținem înainte ca utilizatorul să vrea să editeze sau să salveze
    
- **Data_BytesAsynchronousWithWork** - numărul de byți (comprimat) fără care credem că putem deschide fișierul, dar care ar necesita investiții de cod semnificative pentru a funcționa

- **Data_BytesSynchronous** - numărul de byți (comprimat) de care avem nevoie înainte să putem deschide fișierul
    
- **Data_BytesUnknown** - numărul de byți din părțile de documente pe care nu ne așteptăm să le găsim

- **Data_DetachedDuration** - cât timp a fost activitatea detașată de fir

- **Data_Doc_AccessMode** - documentul este numai în citire/editabil

- **Data_Doc_AssistedReadingReasons** - set predefinit de valori privind motivul pentru care documentul a fost deschis în modul de citire asistată

- **Data_Doc_AsyncOpenKind –** indică dacă s-a deschis o versiune memorată în cache a documentului cloud și ce logică de reîmprospătare asincronă s-a folosit.

- **Data_Doc_ChunkingType** - unități utilizate pentru deschiderea incrementală a documentelor

- **Data_Doc_EdpState** - setare de protecție a datelor electronice pentru document

- **Data_Doc_Ext** - extensia documentului (docx/xlsb/pptx etc.)

- **Data_Doc_FileFormat** - versiunea de protocol pentru formatul fișierului

- **Data_Doc_Fqdn** - numele de domeniu OneDrive sau SharePoint Online

- **Data_Doc_FqdnHash** - codul hash unidirecțional pentru numele de domeniu identificabil al clientului

- **Data_Doc_IOFlags** - rapoarte privind semnalizările memorate în cache folosite pentru a seta opțiuni de solicitare deschise

- **Data_Doc_IdentityTelemetryId** - codul hash unidirecțional pentru identitatea de utilizator folosită pentru deschidere

- **Data_Doc_InitializationScenario** - înregistrează cum a fost deschis documentul

- **Data_Doc_IrmRights** - acțiunile permise de politica de protejare a datelor electronice aplicată pentru document/utilizator

- **Data_Doc_IsIncrementalOpen** - semnalizare care indică faptul că documentul a fost deschis incremental

- **Data_Doc_IsOcsSupported** - semnalizare care indică faptul că documentul este acceptat în serviciul de colaborare
    
- **Data_Doc_IsOpeningOfflineCopy** - semnalizare care indică faptul că s-a deschis copia offline a unui document

- **Data_Doc_IsSyncBacked** - semnalizare care indică faptul că pe computer există o copie sincronizată automat a documentului

- **Data_Doc_Location** - indică ce serviciu a furnizat documentul (OneDrive, File Server, SharePoint etc.)
    
- **Data_Doc_LocationDetails** - indică ce Folder cunoscut a furnizat un document stocat local

- **Data_Doc_NumberCoAuthors** - numărul de alți utilizatori dintr-o sesiune de editare în colaborare

- **Data_Doc_PasswordFlags** - arată semnalizările de parole pentru citire sau citire/scriere setate

- **Data_Doc_ReadOnlyReasons** - motivele pentru care documentul a fost deschis doar în citire

- **Data_Doc_ResourceIdHash** - identificator de document anonimizat, folosit în diagnosticarea problemelor

- **Data_Doc_RtcType** - indică modul în care a fost configurat canalul în timp real (RTC) pentru fișierul curent (dezactivat, neacceptat, la cerere, activat permanent etc.).

- **Data_Doc_ServerDocId** - identificator de document anonimizat și invariabil, folosit în diagnosticarea problemelor

- **Data_Doc_ServerProtocol** - versiunea de protocol folosită în comunicarea cu serviciul

- **Data_Doc_ServerType** - tipul de server care oferă serviciul (SharePoint, OneDrive, WOPI etc.)
    
- **Data_Doc_ServerVersion** - versiunea serverului care oferă serviciul 

- **Data_Doc_SessionId** - identifică o anumită sesiune de editare a documentului din sesiunea completă

- **Data_Doc_SharePointServiceContext** - informații de diagnosticare din solicitările SharePoint Online

- **Data_Doc_SizeInBytes** - indicator privind dimensiunea documentului

- **Data_Doc_SpecialChars** - indicator privind caracterele speciale din calea sau adresa URL a documentului

- **Data_Doc_StreamAvailability** - indicator care arată dacă șirul documentului este disponibil/dezactivat

- **Data_Doc_SyncBackedType** - indicator privind tipul documentului (local sau bazat pe servicii)

- **Data_Doc_UrlHash** - cod hash unidirecțional, pentru crearea unui identificator naiv de document

- **Data_Doc_WopiServiceId** - conține identificatorul unic al furnizorului de servicii WOPI

- **Data_EditorDisablingRename** - identificatorul primului editor care a provocat dezactivarea redenumirii

- **Data_EditorsCount** - numărul de editori din document

- **Data_FSucceededAfterRecoverableFailure** - arată că deschiderea a reușit după repararea unei erori la deschiderea documentului

- **Data_ForceReadWriteReason** - valoare întreagă care reprezintă motivul pentru care fișierul a fost forțat în modul citire/scriere
    
- **Data_LastLoggedTag** - etichetă unică pentru site-ul de apelare a codului folosit pentru a identifica momentele când încercăm să nu realizăm deschiderea de două ori (folosit pentru diagnosticarea calității datelor)

- **Data_LinkStyles** - indică dacă asociem stiluri de șabloane

- **Data_MainPdod** - identificatorul documentului din procesul Office Word

- **Data_Measurements** - șir codificat cu detalii de timp pentru diferitele părți ale deschiderii. Utilizat pentru a măsura performanța.
    
- **Data_MoveDisabledReason** - eroarea care dezactivează mutarea pentru document

- **Data_MoveFlightEnabled** - dacă ediția flight este activată pentru caracteristica de mutare

- **Data_PartsUnknown** - numărul de părți ale documentului pentru care nu am putut obține date

- **Data_RecoverableFailureInitiationLocationTag** - etichetă unică pentru site-ul de apelare a codului folosit pentru a identifica locul din cod în care încercăm să remediem fișierul înainte de a-l deschide.

- **Data_RenameDisabledReason** - eroare care face redenumirea să fie dezactivată pentru acest document

- **Data_RenameFlightEnabled** - dacă este activată ediția flight pentru caracteristica de redenumire

- **Data_SecondaryTag** - etichetă unică pentru site-ul de apelare a codului folosit pentru a adăuga date suplimentare despre erori pentru deschidere.

- **Data_TemplateFormat** - formatul de fișier al șablonului pe care se bazează documentul

- **Data_UsesNormal** - indică dacă documentul deschis se bazează pe șablonul normal.


#### <a name="officewordfileopenopenifrinitargs"></a>Office.Word.FileOpen.OpenIfrInitArgs

Acest eveniment indică faptul că Office Word deschide un document prin activare COM sau linia de comandă. În plus, conține date esențiale despre performanța la deschiderea fișierelor și este un eveniment de pornire a aplicației din perspectiva utilizatorului. Evenimentul monitorizează dacă file-open-from-command-line funcționează așa cum vă așteptați. În plus, se folosește pentru a calcula utilizatorii/dispozitivele active lunar și măsurătorile de fiabilitate cloud.

Se colectează următoarele câmpuri:

  - **Data\_AddDocTelemRes -** raportează dacă am putut completa corect alte valori legate de telemetria documentelor din eveniment. Utilizat pentru diagnostice privind calitatea datelor.

  - **Data\_BytesAsynchronous –** numărul de byți (comprimat) fără care credem că putem deschide fișierul dacă îi obținem înainte ca utilizatorul să vrea să editeze sau să salveze.

  - **Data\_BytesAsynchronousWithWork –** numărul de byți (comprimat) fără care credem că putem deschide fișierul, dar care ar necesita investiții de cod semnificative pentru a funcționa

  - **Data\_BytesSynchronous –** numărul de byți (comprimat) de care avem nevoie înainte să putem deschide fișierul

  - **Data\_BytesUnknown –** numărul de byți din părțile de documente pe care nu ne așteptăm să le găsim.

  - **Data\_Doc\_AccessMode –** documentul este doar în citire/editabil

  - **Data\_Doc\_AssistedReadingReasons -** set predefinit de valori privind motivul pentru care documentul a fost deschis în modul de citire asistată

  - **Data_Doc_AsyncOpenKind –** indică dacă s-a deschis o versiune memorată în cache a documentului cloud și ce logică de reîmprospătare asincronă s-a folosit.

  - **Data\_Doc\_ChunkingType -** unități utilizate pentru deschiderea incrementală a documentelor

  - **Data\_Doc\_EdpState –** setare de protecție a datelor electronice pentru document

  - **Data\_Doc\_Ext –** extensia documentului (docx/xlsb/pptx etc.)

  - **Data\_Doc\_FileFormat –** versiunea de protocol pentru formatul fișierului

  - **Data\_Doc\_Fqdn -** numele de domeniu OneDrive sau SharePoint Online

  - **Data\_Doc\_FqdnHash -** codul hash într-o singură direcție pentru numele de domeniu identificabil al clientului

  - **Data\_Doc\_IOFlags –** rapoarte privind marcajele memorate în cache folosite pentru a seta opțiunile de deschidere a solicitărilor

  - **Data\_Doc\_IdentityTelemetryId –** codul hash într-o singură direcție pentru identitatea de utilizator folosită pentru deschidere

  - **Data\_Doc\_InitializationScenario –** înregistrează cum a fost deschis documentul

  - **Data\_Doc\_IrmRights -** acțiunile permise de politica de protejare a datelor electronice aplicată pentru document/utilizator

  - **Data\_Doc\_IsIncrementalOpen -** semnalizare care arată că documentul a fost deschis incremental

  - **Data\_Doc\_IsOcsSupported -** semnalizare care arată că documentul este acceptat în serviciul de colaborare

  - **Data\_Doc\_IsOpeningOfflineCopy -** semnalizare care arată că s-a deschis copia offline a unui document

  - **Data\_Doc\_IsSyncBacked –** marcaj care arată că pe computer există o copie sincronizată automat a documentului

  - **Data\_Doc\_Location –** arată ce serviciu a furnizat documentul (OneDrive, File Server, SharePoint)

  - **Data\_Doc\_LocationDetails –** arată ce Folder cunoscut a furnizat un document stocat local

  - **Data\_Doc\_NumberCoAuthors -** numărul de alți utilizatori dintr-o sesiune de editare în colaborare

  - **Data\_Doc\_PasswordFlags -** arată semnalizările de parole pentru citire sau citire/scriere setate

  - **Data\_Doc\_ReadOnlyReasons –** motivele pentru care documentul a fost deschis doar în citire

  - **Data\_Doc\_ResourceIdHash –** un identificator de document anonimizat, folosit în diagnosticarea problemelor

  - **Data_Doc_RtcType -**  indică modul în care a fost configurat canalul în timp real (RTC) pentru fișierul curent (dezactivat, neacceptat, la cerere, activat permanent etc.).

  - **Data\_Doc\_ServerDocId –** un identificator de document anonimizat și imutabil, folosit în diagnosticarea problemelor

  - **Data\_Doc\_ServerProtocol –** versiunea de protocol folosită în comunicarea cu serviciul

  - **Data\_Doc\_ServerType -** tipul de server care oferă serviciul (SharePoint, OneDrive, WOPI etc.)

  - **Data\_Doc\_ServerVersion –** versiunea serverului care oferă serviciul

  - **Data\_Doc\_SessionId –** versiunea serverului care oferă serviciul

  - **Data\_Doc\_SharePointServiceContext –** informații de diagnosticare din solicitările SharePoint Online

  - **Data\_Doc\_SizeInBytes -** indicator privind dimensiunea documentului

  - **Data\_Doc\_SpecialChars -** indicator privind caracterele speciale din calea sau adresa URL a documentului

  - **Data\_Doc\_StreamAvailability -** indicator care arată dacă șirul documentului este disponibil/dezactivat

  - **Data\_Doc\_SyncBackedType -** indicator privind tipul documentului (local sau bazat pe servicii)

  - **Data\_Doc\_UrlHash -** cod hash într-o singură direcție, pentru crearea unui identificator naiv de document

  - **Data\_Doc\_WopiServiceId –** conține identificatorul unic al furnizorului de servicii WOPI

  - **Data\_EditorDisablingRename –** identificatorul primului editor care a provocat dezactivarea redenumirii

  - **Data\_EditorsCount –** numărul de editori din document

  - **Data\_FSucceededAfterRecoverableFailure –** arată că deschiderea a reușit după repararea unei erori la deschiderea documentului

  - **Data\_ForceReadWriteReason –** valoare întreagă care reprezintă motivul pentru care fișierul a fost forțat în modul citire/scriere

  - **Data\_LastLoggedTag –** etichetă unică pentru site-ul de apelare a codului folosit pentru a identifica momentele când încercăm să nu realizăm deschiderea de două ori (folosit pentru diagnosticarea calității datelor)

  - **Data\_LinkStyles –** indică dacă asociem stiluri de șabloane

  - **Data\_MainPdod –** Identificatorul documentului din procesul Office Word

  - **Data\_Measurements –** șir codificat cu detalii de timp pentru diferitele părți ale deschiderii. Utilizat pentru a diagnostica performanța de deschidere.

  - **Data\_MoveDisabledReason –** eroarea care dezactivează mutarea pentru document

  - **Data\_MoveFlightEnabled –** dacă ediția flight este activată pentru caracteristica de mutare

  - **Data\_PartsUnknown –** numărul de părți ale documentului pentru care nu am putut obține date

  - **Data\_RecoverableFailureInitiationLocationTag –** etichetă unică pentru site-ul de apelare a codului folosit pentru a identifica locul din cod în care încercăm să remediem fișierul înainte de a-l deschide

  - **Data\_RenameDisabledReason –** eroare care face redenumirea să fie dezactivată pentru acest document

  - **Data\_RenameFlightEnabled -** dacă este activată ediția flight pentru caracteristica de redenumire

  - **Data\_SecondaryTag –** etichetă unică pentru site-ul de apelare a codului folosit pentru a adăuga date suplimentare despre erori pentru deschidere.

  - **Data\_TemplateFormat –** formatul de fișier al șablonului pe care se bazează documentul.

  - **Data\_UsesNormal –** indică dacă documentul deschis se bazează pe șablonul normal.


#### <a name="officewordfileopenopenloadfile"></a>Office.Word.FileOpen.OpenLoadFile

Acest eveniment indică faptul că Office Word deschide un document prin caseta de dialog Deschidere. În plus, conține date esențiale despre performanța la deschiderea fișierelor și este un eveniment de pornire a aplicației din perspectiva utilizatorului. Evenimentul monitorizează dacă file-open-from-the-open-filedialog funcționează așa cum vă așteptați. În plus, se folosește pentru a calcula utilizatorii/dispozitivele active lunar și măsurătorile de fiabilitate cloud.

Se colectează următoarele câmpuri:

- **Data_AddDocTelemRes** - raportează dacă am putut completa corect alte valori legate de telemetria documentelor din eveniment. Utilizat pentru diagnostice privind calitatea datelor.

- **Data_BytesAsynchronous** - numărul de byți (comprimat) fără care credem că putem deschide fișierul dacă îi obținem înainte ca utilizatorul să vrea să editeze sau să salveze

- **Data_BytesAsynchronousWithWork** - numărul de byți (comprimat) fără care credem că putem deschide fișierul, dar care ar necesita investiții de cod semnificative pentru a funcționa
    
- **Data_BytesSynchronous** - numărul de byți (comprimat) de care avem nevoie înainte să putem deschide fișierul

- **Data_BytesUnknown** - numărul de byți din părțile de documente pe care nu ne așteptăm să le găsim

- **Data_DetachedDuration** - cât timp a fost activitatea detașată de fir

- **Data_Doc_AccessMode** - documentul este numai în citire/editabil

- **Data_Doc_AssistedReadingReasons** - set predefinit de valori privind motivul pentru care documentul a fost deschis în modul de citire asistată

- **Data_Doc_AsyncOpenKind –** indică dacă s-a deschis o versiune memorată în cache a documentului cloud și ce logică de reîmprospătare asincronă s-a folosit.

- **Data_Doc_ChunkingType** - unități utilizate pentru deschiderea incrementală a documentelor

- **Data_Doc_EdpState** - setare de protecție a datelor electronice pentru document

- **Data_Doc_Ext** - extensia documentului (docx/xlsb/pptx etc.)

- **Data_Doc_FileFormat** - versiunea de protocol pentru formatul fișierului

- **Data_Doc_Fqdn** - numele de domeniu OneDrive sau SharePoint Online

- **Data_Doc_FqdnHash** - codul hash unidirecțional pentru numele de domeniu identificabil al clientului

- **Data_Doc_IdentityTelemetryId** - codul hash unidirecțional pentru identitatea de utilizator folosită pentru deschidere

- **Data_Doc_InitializationScenario** - înregistrează cum a fost deschis documentul

- **Data_Doc_IOFlags** - rapoarte privind semnalizările memorate în cache folosite pentru a seta opțiuni de solicitare deschise

- **Data_Doc_IrmRights** - acțiunile permise de politica de protejare a datelor electronice aplicată pentru document/utilizator
    
- **Data_Doc_IsIncrementalOpen** - semnalizare care indică faptul că documentul a fost deschis incremental

- **Data_Doc_IsOcsSupported** - semnalizare care indică faptul că documentul este acceptat în serviciul de colaborare

- **Data_Doc_IsOpeningOfflineCopy** - semnalizare care indică faptul că s-a deschis copia offline a unui document

- **Data_Doc_IsSyncBacked** - semnalizare care indică faptul că pe computer există o copie sincronizată automat a documentului

- **Data_Doc_Location** - indică ce serviciu a furnizat documentul (OneDrive, File Server, SharePoint etc.)

- **Data_Doc_LocationDetails** - indică ce Folder cunoscut a furnizat un document stocat local

- **Data_Doc_NumberCoAuthors** - numărul de alți utilizatori dintr-o sesiune de editare în colaborare

- **Data_Doc_PasswordFlags** - arată semnalizările de parole pentru citire sau citire/scriere setate

- **Data_Doc_ReadOnlyReasons** - motivele pentru care documentul a fost deschis doar în citire

- **Data_Doc_ResourceIdHash** - identificator de document anonimizat, folosit în diagnosticarea problemelor

- **Data_Doc_RtcType** - indică modul în care a fost configurat canalul în timp real (RTC) pentru fișierul curent (dezactivat, neacceptat, la cerere, activat permanent etc.).

- **Data_Doc_ServerDocId** - identificator de document anonimizat și invariabil, folosit în diagnosticarea problemelor 

- **Data_Doc_ServerProtocol** - versiunea de protocol folosită în comunicarea cu serviciul

- **Data_Doc_ServerType** - tipul de server care oferă serviciul (SharePoint, OneDrive, WOPI etc.)

- **Data_Doc_ServerVersion** - versiunea serverului care oferă serviciul

- **Data_Doc_SessionId** - identifică o anumită sesiune de editare a documentului din sesiunea completă

- **Data_Doc_SharePointServiceContext** - informații de diagnosticare din solicitările SharePoint Online

- **Data_Doc_SizeInBytes** - indicator privind dimensiunea documentului

- **Data_Doc_SpecialChars** - indicator privind caracterele speciale din calea sau adresa URL a documentului

- **Data_Doc_StreamAvailability** - indicator care arată dacă șirul documentului este disponibil/dezactivat

- **Data_Doc_SyncBackedType** - indicator privind tipul documentului (local sau bazat pe servicii)

- **Data_Doc_UrlHash** - cod hash unidirecțional, pentru crearea unui identificator naiv de document

- **Data_EditorDisablingRename** - identificatorul primului editor care a provocat dezactivarea redenumirii

- **Data_EditorsCount** - numărul de editori din document

- **Data_ForceReadWriteReason** - valoare întreagă care reprezintă motivul pentru care fișierul a fost forțat în modul citire/scriere
    
- **Data_FSucceededAfterRecoverableFailure** - arată că deschiderea a reușit după repararea unei erori la deschiderea documentului

- **Data_LastLoggedTag** - etichetă unică pentru site-ul de apelare a codului folosit pentru a identifica momentele când nu reușim să încercăm salvarea de două ori (folosit pentru diagnosticarea calității datelor)

- **Data_LinkStyles** - indică dacă asociem stiluri de șabloane

- **Data_MainPdod** - identificatorul documentului din procesul Office Word

- **Data_Measurements** - șir codificat cu detalii de timp pentru diferitele părți ale deschiderii. Utilizat pentru a măsura performanța.

- **Data_MoveDisabledReason** - eroarea care dezactivează mutarea pentru document

- **Data_MoveFlightEnabled** - dacă ediția flight este activată pentru caracteristica de mutare

- **Data_PartsUnknown** - numărul de părți ale documentului pentru care nu am putut obține date

- **Data_RecoverableFailureInitiationLocationTag** - etichetă unică pentru site-ul de apelare a codului folosit pentru a identifica locul din cod în care încercăm să remediem fișierul înainte de a-l deschide

- **Data_RenameDisabledReason** - eroare care face redenumirea să fie dezactivată pentru acest document

- **Data_RenameFlightEnabled** - dacă este activată ediția flight pentru caracteristica de redenumire

- **Data_SecondaryTag** - etichetă unică pentru site-ul de apelare a codului folosit pentru a adăuga date suplimentare despre erori pentru deschidere

- **Data_TemplateFormat** - formatul de fișier al șablonului pe care se bazează documentul

- **Data_UsesNormal** - indică dacă documentul deschis se bazează pe șablonul normal


#### <a name="renewuserop"></a>RenewUserOp

Este colectat atunci când un utilizator încearcă să deschidă un document protejat prin IRM sau să aplice protecții IRM.  Acesta conține informațiile necesare pentru a investiga și a diagnostica corect problemele care apar atunci când se realizează operațiunea înnoire a certificatelor de utilizator. 

Se colectează următoarele câmpuri:

- **AppInfo.ClientHierarchy** - ierarhie client care indică faptul că aplicația rulează în mediul de producție sau în mediul de dezvoltator

- **AppInfo.Name** - nume aplicație.

- **AppInfo.Version** - versiunea aplicației

- **iKey** - ID server înregistrator

- **RMS.ApplicationScenarioId** - ID al scenariului furnizat de aplicație

- **RMS.Duration** - timp total pentru finalizarea operațiunii

- **RMS.DurationWithoutExternalOps** - timp total minus operațiuni externe consumate, cum ar fi latența de rețea.

- **RMS.ErrorCode** - codul de eroare returnat de operațiune, dacă există

- **RMS.HttpCall** - indică dacă există o operațiune HTTP

- **RMS.LicenseFormat** - formatul licenței: Xrml sau Json

- **RMS.Result** - succes sau eșec al operațiunii

- **RMS.ScenarioId** - ID al scenariului definit de clientul Serviciu de administrare a drepturilor

- **RMS.SDKVersion** - versiunea clientului pentru Serviciul de administrare a drepturilor

- **RMS.ServerType** - tipul de server al Serviciului de administrare a drepturilor 

- **RMS.StatusCode** - cod de stare al rezultatului operațiunii

- **RMS.Type** - tipul informațiilor despre utilizator

#### <a name="servicediscoveryop"></a>ServiceDiscoveryOp

Este colectat atunci când un utilizator încearcă să deschidă un document protejat prin IRM sau să aplice protecții IRM.  Acesta conține informațiile necesare pentru a investiga și a diagnostica corect problemele care apar atunci când se realizează operațiunea de descoperire a serviciului. 

Se colectează următoarele câmpuri:

- **AppInfo.ClientHierarchy** - ierarhie client care indică faptul că aplicația rulează în mediul de producție sau în mediul de dezvoltator

- **AppInfo.Name** - nume aplicație.

- **AppInfo.Version** - versiunea aplicației

- **iKey** - ID al serverului pentru servicii de înregistrare

- **RMS.ApplicationScenarioId** - ID al scenariului furnizat de aplicație

- **RMS.Duration** - timp total pentru finalizarea operațiunii

- **RMS.DurationWithoutExternalOps** - timp total minus operațiuni externe consumate, cum ar fi latența de rețea.

- **RMS.ErrorCode** - codul de eroare returnat de operațiune, dacă există

- **RMS.HttpCall** - indică dacă există operațiune HTTP

- **RMS.LicenseFormat** - formatul licenței: Xrml sau Json

- **RMS.OperationName** - nume operațiune

- **RMS.Result** - succes sau eșec al operațiunii

- **RMS.ScenarioId** - ID al scenariului definit de clientul Serviciu de administrare a drepturilor

- **RMS.SDKVersion** - versiunea clientului pentru Serviciul de administrare a drepturilor

- **RMS.ServerType** - tipul de server al Serviciului de administrare a drepturilor 

- **RMS.StatusCode** - cod de stare al rezultatului operațiunii


### <a name="office-accessibility-configuration-subtype"></a>*Subtip de configurație accesibilitate Office*

Caracteristici de accesibilitate în Office

#### <a name="officeaccessibilityaccessibilitytoolsessionpresencewin32"></a>Office.Accessibility.AccessibilityToolSessionPresenceWin32

Ne permite să detectăm că utilizatorul are un instrument de tehnologie de asistare și numele său. Acest lucru ne permite să înțelegem dacă un utilizator Office se confruntă cu probleme cu un anumit instrument din Tehnologiile de asistare.

Se colectează următoarele câmpuri:

  - **Data\_Data\_Jaws –** indică dacă Jaws rula în timpul sesiunii **Data\_Data\_Magic –** indică dacă Magic rula în timpul sesiunii

  - **Data\_Data\_Magnify –** indică dacă Magnify rula în timpul sesiunii

  - **Data\_Data\_Narrator –** indică dacă Narrator rula în timpul sesiunii

  - **Data\_Data\_NVDA –** indică dacă NVDA rula în timpul sesiunii

  - **Data\_Data\_SA –** indică dacă SA rula în timpul sesiunii

  - **Data\_Data\_Supernova –** indică dacă Supernova rula în timpul sesiunii

  - **Data\_Data\_SuperNovaessSuite –** indică dacă SuperNovaAccessSuite rula în timpul sesiunii

  - **Data\_Data\_WinEyes –** indică dacă WinEyes rula în timpul sesiunii

  - **Data\_Data\_ZoomText –** indică dacă ZoomText rula în timpul sesiunii

#### <a name="officeappledarkmode"></a>Office.Apple.DarkMode

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Evenimentul ne spune dacă utilizatorul rulează un sistem pe DarkMode și dacă utilizatorul a suprascris setarea sistemului DarkMode în Office.  Utilizăm acest eveniment pentru a asigura accesibilitatea și a acorda prioritate optimizării experienței de utilizator.

Se colectează următoarele câmpuri:

- **Data_DarkModeIsEnabled** - dacă DarkMode este activat în sistem.

- **Data_RequiresAquaSystemAppearanceEnabled** - dacă DarkMode este suprascris în Office.

#### <a name="officeapplehardwarekeyboardinuseapple"></a>Office.Apple.HardwareKeyboardInUse.Apple

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Evenimentul ne spune că un utilizator atașează o tastatură la dispozitivul său mobil. Evenimentul ne ajută să îmbunătățim accesibilitatea și să optimizăm experiența noastră de utilizator.

Se colectează următoarele câmpuri:

- **Data_CollectionTime** - un marcaj de timp care denotă data colecției evenimentului.

#### <a name="officeapplembuinstrumentdeviceaccessibilitysettings"></a>Office.Apple.MbuInstrument.DeviceAccessibilitySettings

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Evenimentul colectează starea diferitelor opțiuni de accesibilitate disponibile în timpul unei sesiuni. Utilizăm acest eveniment pentru a asigura accesibilitatea și a acorda prioritate optimizării experienței de utilizator.

Se colectează următoarele câmpuri:

- **Data_AccessibilityContentSize** - o semnalizare care indică dacă această setare este activată

- **Data_AssistiveTouchRunning** - o semnalizare care indică dacă această setare este activată

- **Data_BoldTextEnabled** - o semnalizare care indică dacă această setare este activată

- **Data_CollectionTime** - o semnalizare care indică dacă această setare este activată

- **Data_DarkerSystemColorsEnabled** - o semnalizare care indică dacă această setare este activată

- **Data_DifferentiateWithoutColor** - o semnalizare care indică dacă această setare este activată

- **Data_GrayscaleEnabled** - o semnalizare care indică dacă această setare este activată

- **Data_GuidedAccessEnabled** - o semnalizare care indică dacă această setare este activată

- **Data_IncreaseContrast** - o semnalizare care indică dacă această setare este activată

- **Data_InvertColorsEnabled** - o semnalizare care indică dacă această setare este activată

- **Data_PreferredContentSizeCategory** - o semnalizare care indică dacă această setare este activată

- **Data_ReduceMotionEnabled** - o semnalizare care indică dacă această setare este activată

- **Data_ReduceTransparency** - o semnalizare care indică dacă această setare este activată

- **Data_ReduceTransparencyEnabled** - o semnalizare care indică dacă această setare este activată

- **Data_ShakeToUndeEnabled** - o semnalizare care indică dacă această setare este activată (Perimat - utilizat doar pentru compilările vechi.)

- **Data_ShakeToUndoEnabled** - o semnalizare care indică dacă această setare este activată

- **Data_SpeakScreenEnabled** - o semnalizare care indică dacă această setare este activată

- **Data_SpeakSelectionEnabled** - o semnalizare care indică dacă această setare este activată

- **Data_SwitchControlRunning** - o semnalizare care indică dacă această setare este activată

- **Data_UAZoomEnabled** - o semnalizare care indică dacă această setare este activată

- **Data_VoiceOverRunning** - o semnalizare care indică dacă această setare este activată

#### <a name="officewordaccessibilitylearningtoolsreadaloudplayreadaloud"></a>Office.Word.Accessibility.LearningTools.ReadAloud.PlayReadAloud

Acest eveniment indică faptul că Office Word citește cu voce tare textul din document. Evenimentul este un mesaj repetat al caracteristicii de accesibilitate care permite ca Microsoft să evalueze starea de funcționare a caracteristicii textului citit cu voce tare.

Se colectează următoarele câmpuri:

  - **Data\_ParagraphCount –** numărul de paragrafe al documentului

  - **Data\_Play –** este prima dată când Word citește cu voce tare

  - **Data\_ViewKind –** tipul de vizualizare al documentului

#### <a name="officewordaccessibilitylearningtoolsreadaloudstopreadaloud"></a>Office.Word.Accessibility.LearningTools.ReadAloud.StopReadAloud

Acest eveniment indică faptul că Office Word întrerupe citirea cu voce tare a textului din document. Evenimentul permite ca Microsoft să evalueze starea de funcționare a caracteristicii de citire cu voce tare a textului, măsurând durata de lucru.

Se colectează următoarele câmpuri:

  - Fără

### <a name="privacy-subtype"></a>*Subtip de confidențialitate*

Setări de confidențialitate în Office 

#### <a name="officeintelligentserviceprivacyconsentprivacyevent"></a>Office.IntelligentService.PrivacyConsent.PrivacyEvent

Acest eveniment reprezintă o acțiune inițiată de utilizator sau de sistem, care face parte din experiența de utilizator privind confidențialitatea pentru Office. Este declanșat în casetele de dialog referitoare la confidențialitate la prima rulare, în caseta de dialog Confidențialitatea contului și în notificările de confidențialitate. Evenimentul este utilizat pentru a înțelege următoarele situații: când utilizatorii sunt de acord cu setările de confidențialitate Office, când utilizatorii modifică setările de confidențialitate Office și când setările de confidențialitate Office se actualizează în sesiunile de utilizator.

Se colectează următoarele câmpuri:

  - **Data_ActionId -** acțiune de utilizator într-o casetă de dialog privind confidențialitatea

  - **Data_ControllerConnectedServicesState -** setare de politică de utilizator pentru experiențe de mod conectat opționale suplimentare

  - **Data_DownloadedContentServiceGroupState -** setare de utilizatorului pentru conținutul descărcat 
 
  - **Data_ForwardLinkId -** link la documentația de confidențialitate pentru scenariu utilizator

  - **Data_HRESULT -** înregistrarea erorilor în timpul interacțiunii cu o casetă de dialog privind confidențialitatea

  - **Data_IsEnterpriseUser -** categoria de licență de utilizator

  - **Data_OfficeServiceConnectionState -** setare de utilizator pentru servicii conectate

  - **Data_RecordRegistry -** înregistrarea afișării casetei de dialog privind confidențialitate la nivel de întreprindere

  - **Data_Scenario -** scenariu de primă rulare bazat pe licența de utilizator și pe categorie

  - **Data_SeenInsidersDialog -** înregistrarea afișării casetei de dialog privind confidențialitatea pentru utilizatori Insider

  - **Data_SendTelemetryOption -** setare de utilizator pentru telemetrie

  - **Data_SendTelemetryOptionPolicy -** setare de politică de utilizator pentru telemetrie

  - **Data_UserCategory -** tip cont utilizator  

  - **Data_UserCCSDisabled -** înlocuire de utilizator pentru experiențe de mod conectat opționale suplimentare

   - **Data_UserContentServiceGroupState -** setare de utilizator pentru analiza conținutului

  - **Data_WillShowDialogs -** înregistrarea unui utilizator care trebuie să vadă casetele de dialog privind confidențialitatea la prima rulare



## <a name="product-and-service-performance-data-events"></a>Evenimente privind datele despre performanța produselor și a serviciilor

Iată subtipurile de date din această categorie:
- [Ieșire neașteptată a aplicației (cădere)](#unexpected-application-exit-crash-subtype)
- [Performanța caracteristicii aplicației](#application-feature-performance-subtype)
- [Eroare de activitate a aplicației](#application-activity-error-subtype)

### <a name="unexpected-application-exit-crash-subtype"></a>*Subtip de ieșire neașteptată a aplicației (cădere)*

Ieșirile neașteptate ale aplicației și starea aplicației atunci când se întâmplă acest lucru.

#### <a name="appstartupreason"></a>app.startup.reason

Acest eveniment ne permite să detectăm și să remediem problemele în care Outlook a înregistrat o cădere în timpul pornirii aplicației.  Acest eveniment include informații referitoare la motivul pentru care s-a produs căderea, pentru ca noi să putem să remediem problema rapid.

Se colectează următoarele câmpuri: 

- **app_background_time** - durata în care aplicația a fost în fundal cu ocazia ultimei sesiuni

- **startup_reason_type** - indică motivul pentru care pornește aplicația, acest lucru va indica dacă a fost din cauza unei închideri forțate sau din alt motiv. 

- **watch_status_info** - urmărește informațiile următoare, dacă este cazul. 

  - **is_watch_app_installed** - determină dacă utilizatorul are aplicația Watch instalată

  - **is_watch_paired** - determină dacă dispozitivul iOS este asociat cu un ceas

  - **is_watch_supported_and_active** - indică dacă este acceptat un ceas și dacă este activ în timpul sesiunii

Câmpurile următoare sunt colectate doar pentru Outlook Mobile pentru iOS:

- **clean_exit_reason** - un șir de cuvinte care indică dacă a existat un motiv pentru oprirea aplicației

- **is_agenda_user** - indică dacă utilizatorul a deschis agenda recent, ceea ce indică dacă scriem pe disc la pornire

- **is_watch_supported_and_active** - indică dacă este acceptat un ceas și dacă este activ în timpul sesiunii


#### <a name="applicationcrash"></a>application.crash

Utilizat pentru monitorizarea căderilor critice ale aplicației și ne ajută să colectăm informații despre motivul pentru care s-a blocat aplicația și cum să o preveniți.

Se colectează următoarele câmpuri: 

- **android.hardware.** - (de ex., android.hardware.bluetooth) valori de configurație hardware oferite de platforma Android

- **android.software.** - (de ex., android.software.device_admin) valori de configurație software oferite de platforma Android

- **android_version** - nume versiune dispozitiv Android, așa cum este indicat de android.os.Build.VERSION#RELEASE

- **application_package_name** - nume pachet de aplicații, așa cum se indică în android.content.Context#getPackageName()

- **application_stack_trace** - trasarea stivei de cădere

- **application_version_code** - cod de versiune a aplicației definit de aplicația Outlook

- **application_version_name** - numele versiunii aplicației definit de aplicația Outlook 

- **com.** (de ex., com.google.android.feature.FASTPASS_BUILD, com.amazon.feature.PRELOAD, com.samsung.android.bio.face) Anumite valori de configurare specifice pentru fabricant oferite de platforma Android

- **crash_report_sdk** - SDK pentru trimiterea jurnalelor de avarie. Hockey sau AppCenter

- **crash_type** - crash_type va avea ca tipuri java, nativ, non-fatal.

     - java - dacă avaria a fost înregistrată pe stratul de aplicație.

     - nativ - dacă avaria a fost înregistrată pe stratul nativ din aplicație. 

     - non-fatal - avariile non-fatale sunt înregistrate pentru a depana orice caracteristică. Aplicația nu se va bloca, dar va încărca jurnalele de avarii non-fatale, pentru a vă ajuta să depanați o caracteristică.

- **device_brand** - marcă de dispozitiv (producătorul sau operatorul mobil), așa cum se indică în android.os.Build#BRAND

- **device_ID** - ID-ul unic al dispozitivului (IMEI)

- **device_manufacturer** - producătorul dispozitivului așa cum este indicat de android.os.Build#MANUFACTURER

- **device_model** - modelul de dispozitiv așa cum este indicat de android.os.Build#MODEL

- **device_model** - numele dispozitivului așa cum este indicat de android.os.Build#DEVICE

- **device_total_memory** - estimarea dimensiunii totale a memoriei dispozitivului pe baza statisticii sistemului de fișiere.

- **glEsVersion** - cheie de versiune de sisteme încorporate OpenGL


#### <a name="crashevent"></a>crash.event

Ne permite să detectăm și să remediem situațiile în care s-au produs căderi critice ale aplicației și ne ajută să colectăm informații despre motivul pentru care a căzut aplicația și cum să preveniți căderea.

Se colectează următoarele câmpuri: 

- **crashTime** - data și ora la care s-a produs căderea pentru a ajuta la investigare

- **crash_time_from_start** – timpul scurs de la pornirea aplicației până la cădere, pentru a ajuta la investigație

- **exceptionName** - numele excepției care a declanșat căderea pentru a ajuta la investigare

- **exception_reason** – motivul excepției care a declanșat căderea pentru a ajuta la investigație

- **hasHx** - ne spune că acest cont folosește noul nostru serviciu de sincronizare, pentru a ne ajuta să detectăm problemele provocate de serviciul nostru de sincronizare

- **incidentIdentifier** - un ID unic pentru raportul de cădere, astfel încât să găsim problema corespunzătoare

- **isAppKill** - ne ajută să înțelegem dacă aplicația respectivă a fost oprită sau închisă pe dispozitiv

- **is_crashloop** - ne ajută să înțelegem dacă această cădere poate fi o cădere cu buclă.

- **reportKey** - un ID unic pentru instalarea aplicației pe dispozitivul pentru investigarea problemei

- **semnal** - un semnal care a cauzat căderea pentru a ne oferi mai multe detalii pentru a investiga acest accident


#### <a name="error"></a>Eroare

Ne permite să înțelegem problemele cu care se confruntă aplicațiile mobile atunci când încercați să preluați setările de confidențialitate de pe server.

Se colectează următoarele câmpuri:

- **correlationId** - un identificator unic pentru o conexiune de serviciu care a dus la o eroare, permițându-ne să diagnosticăm ce nu a funcționat bine

- **errorCode** - identifică codul de eroare relevant primit de la serviciul care poate fi utilizat pentru diagnosticarea problemei

- **exceptionType** - tipul de eroare pe care l-a întâmpinat biblioteca atunci când a preluat setarea

- **message** - identifică mesajul de eroare primit de serviciu

- **roamingSettingType** - identifică locația din care încercăm să citim setările

- **settingId** - setarea încercată de preluare

#### <a name="officeappdomainunhandledexceptionhandlerfailed"></a>Office.AppDomain.UnhandledExceptionHandlerFailed

Colectează informații pentru orice excepții netratate, utilizând aplicația Data Streamer. Aceste date se utilizează pentru a monitoriza starea de funcționare a aplicației. Evenimentul este generat de Microsoft Data Streamer pentru programul de completare Excel.

Se colectează următoarele câmpuri:

- **Exception** – stiva de apeluri pentru excepție

- **Event name** – categoria evenimentului și eticheta acestuia.

#### <a name="officeappleidentitydomainname"></a>Office.Apple.IdentityDomainName

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Acest eveniment este utilizat pentru a monitoriza starea de funcționare a sistemului nostru, precum și pentru a investiga cauzele erorilor unor utilizatori de domeniu. Colectăm domeniul utilizat de utilizatorii noștri atunci când aceștia se autentifică.  Utilizăm aceste date pentru a ne ajuta să identificăm și să remediem problemele care să nu pară că au un impact mare la un nivel mai larg, dar acest lucru poate afecta un anumit domeniu de utilizatori.

Se colectează următoarele câmpuri:

- **Data_Domain** - domeniul utilizat pentru autentificare

- **Data_IdentityProvider** - numele furnizorului de identitate de autentificare. (i.e. LiveId sau ADAL)

- **Data_IdentityProviderEnum** - codul furnizorului de identitate de autentificare. (Un număr)

#### <a name="officeapplesystemhealthappexitmacandios"></a>Office.Apple.SystemHealthAppExitMacAndiOS

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Evenimentul este utilizat pentru a monitoriza starea de funcționare a aplicațiilor noastre Office, precum și pentru a investiga cauzele erorilor. Colectăm date la fiecare ieșire din aplicație pentru a determina dacă o aplicație a ieșit cu corect.

Se colectează următoarele câmpuri:

- **Data_AffectedProcessSessionID** - identificatorul pentru sesiunea care prezintă ieșirea din aplicație.

- **Data_AffectedSessionBuildNumber** - versiunea minoră a aplicației în care a fost observată o ieșire din aplicație.

- **Data_AffectedSessionDuration** - durata sesiunii de la început la ieșire

- **Data_AffectedSessionIDSMatch** - un indicator de stare de telemetrie.

- **Data_AffectedSessionMERPSessionID** - un indicator de stare de telemetrie.

- **Data_AffectedSessionOSLocale** - setările regionale ale sistemului de operare sub care a fost observată ieșirea din aplicație.

- **Data_AffectedSessionOSVersion** - versiunea sistemului de operare sub care a fost observată ieșirea din aplicație.

- **Data_AffectedSessionResidentMemoryOnCrash** - volumul de memorie rezidentă care a fost consumat atunci când s-a produs ieșirea din aplicație

- **Data_AffectedSessionStackHash** - un identificator care va indica eroarea specifică atinsă.

- **Data_AffectedSessionStartTime** - ora la care a început sesiunea.

- **Data_AffectedSessionUAEType** - tipul de ieșire din aplicație observată (dacă a fost o ieșire nereușită, acest cod va indica tipul de eroare observată)

- **Data_AffectedSessionVersion** - versiunea majoră a aplicației în care a fost observată o ieșire din aplicație.

- **Data_AffectedSessionVirtualMemoryOnCrash** - volumul de memorie virtuală care a fost consumat atunci când s-a produs ieșirea din aplicație

- **Data_ExitWasGraceful** - dacă ieșirea din aplicație a fost corectă sau incorectă.

#### <a name="officeextensibilitycomaddinunhandledexception"></a>Office.Extensibility.COMAddinUnhandledException

Eveniment generat când cade programul de completare COM pe o versiune de aplicații de Office pentru consumatori. 

Utilizare: se utilizează pentru a calcula „adoptarea” globală, care nu ține de întreprindere a Aplicațiilor Microsoft 365 pentru întreprindere, pentru un program de completare care este apoi utilizat de instrumente, cum ar fi Readiness Toolkit. Acest lucru le permite clienților întreprindere să valideze dacă programele de completare pe care le-au implementat în organizațiile lor sunt compatibile cu cele mai recente versiuni de Aplicații Microsoft 365 pentru întreprindere și își planifică upgrade-urile în consecință. 

Se colectează următoarele câmpuri:

- **ScopeId** – domeniul firului curent

- **Method** – metoda Office unde a apărut excepția

- **Interface** – interfața Office în care a apărut excepția

- **AddinId** – ID-ul clasei programului de completare

- **AddinProgId** - perimat

- **AddinFriendlyName** - perimat

- **AddinTimeDateStamp** – marca de timp a programului de completare din metadatele DLL

- **AddinVersion** - perimat

- **AddinFileName** - perimat

- **VSTOAddIn** – dacă programul de completare este VSTO

- **AddinConnectFlag** – comportamentul curent de încărcare

- **LoadAttempts** – numărul de încercări pentru a încărca programul de completare

#### <a name="officeextensibilitycomaddinunhandledexceptionenterprise"></a>Office.Extensibility.COMAddinUnhandledExceptionEnterprise

Eveniment generat când cade programul de completare COM pe o versiune de aplicații Office Enterprise.

Utilizare: se utilizează pentru a calcula „adoptarea” globală, care nu ține de întreprindere a Aplicațiilor Microsoft 365 pentru întreprindere, pentru un program de completare care este apoi utilizat de instrumente, cum ar fi Readiness Toolkit. Acest lucru le permite clienților întreprindere să valideze dacă programele de completare pe care le-au implementat în organizațiile lor sunt compatibile cu cele mai recente versiuni de Aplicații Microsoft 365 pentru întreprindere și își planifică upgrade-urile în consecință. 

- **ScopeId** – domeniul firului curent

- **Method** – metoda Office unde a apărut excepția

- **Interface** – interfața Office în care a apărut excepția

- **AddinId** – ID-ul clasei programului de completare

- **AddinProgId** - perimat

- **AddinFriendlyName** - perimat

- **AddinTimeDateStamp** – marca de timp a programului de completare din metadatele DLL

- **AddinVersion** - perimat

- **AddinFileName** - perimat

- **VSTOAddIn** – dacă programul de completare este VSTO

- **AddinConnectFlag** – comportamentul curent de încărcare

- **LoadAttempts** – numărul de încercări pentru a încărca programul de completare

#### <a name="officeextensibilitysandboxodpactivationheartbeat"></a>Office.Extensibility.Sandbox.ODPActivationHeartbeat

Programele de completare Office rulează într-un sandbox. Acest eveniment colectează informațiile despre mesajele repetate pentru activări. Atunci când un program de completare se blochează, acest eveniment colectează motivul pentru care s-a defectat în cazul în care are legătură cu sandbox-ul. Folosit pentru a investiga când comunică clienții problemele.
 
Se colectează următoarele câmpuri:

- **AppID** - ID-ul aplicației

- **AppInfo** - date referitoare la tipul de program de completare (panou de activități sau UILess sau de conținut etc.) și la tipul de furnizor (Omen, SharePoint, sisteme de fișiere etc.)

- **AppInstanceId** - ID-ul instanței aplicației 

- **AssetId** - Asset ID-ul aplicației

- **ErrorCode** - timp total

- **IsAugmentationScenario** - indică dacă bucla de sincronizare este răspunzătoare de inițializarea comenzii Office Solutions Framework control

- **IsDebug** - indică dacă sesiunea este o sesiune de depanare

- **IsPreload** - indică dacă programul de completare este în curs de încărcare în fundal pentru îmbunătățirea performanței de activare.

- **IsWdagContainer** - indică dacă activarea programului de completare este efectuată într-un container de Protecție aplicații Windows Defender.

- **NumberOfAddinsActivated** - contor de programe de completare activate

- **RemoterType** - specifică tipul de program la distanță (de încredere, neautorizat, Win32webView, de încredere UDF etc.) utilizat pentru a activa programul de completare

- **StoreType** - origine a aplicației

- **Eticheta** - specifică unde anume s-a defectat codul utilizând eticheta unică asociată cu acesta.

- **UsesSharedRuntime** - indică faptul că aplicația utilizează sau nu sharedRuntime.


#### <a name="officeextensibilityvbatelemetrybreak"></a>Office.Extensibility.VbaTelemetryBreak

Eveniment generat atunci când un fișier activat pentru macrocomenzi întâmpină o eroare de compilare sau de rulare

Analiză desktop: aceasta este utilizată ca numărător în calculul stării de funcționare specifice pentru întreprindere a tipurilor de macrocomenzi (de exemplu, macrocomenzi Word, Excel etc.), utilizată pentru a deduce în timpul programului pilot dacă programul de completare este „gata de upgrade” în cercul de producție.

Se colectează următoarele câmpuri:

- **TagId** – ID-ul etichetei de telemetrie

- **BreakReason** – motivul întreruperii (rulare, compilare, altă eroare)

- **SolutionType** – tipul soluției (document, șablon, program de completare pentru aplicație, program de completare COM)

- **Data.ErrorCode** – codul de eroare raportat de motorul VBA


#### <a name="officefindtimeappfailedtostart"></a>Office.FindTime.AppFailedToStart

Colectat atunci când aplicația nu reușește să pornească din cauza unei erori în timpul pornirii. Utilizat pentru a urmări excepții și căderi.  Ajută la monitorizarea și depanarea stării aplicației.

Se colectează următoarele câmpuri: 

- **DateTime** - marcă de timp privind momentul în care evenimentul este înregistrat în jurnal.

- **EventName** - numele evenimentului conectat.

#### <a name="officeoutlookdesktophangbucketmetrics"></a>Office.Outlook.Desktop.HangBucketMetrics

Colectează timpul blocării pentru blocările Outlook – un identificator unic pentru fiecare blocare, timpul trecut și informații despre stiva de apeluri. Datele se utilizează pentru a detecta și a identifica blocările aplicației care vor fi remediate în viitoarele actualizări.

Se colectează următoarele câmpuri:

  - **BucketId** – codul hash al stivei de apeluri

  - **ElapsedTotal** – timpul total petrecut în apel

  - **ElapsedHanging** – timpul de blocare petrecut în apel

#### <a name="officeoutlookdesktophangreportingscopeperfmetrics"></a>Office.Outlook.Desktop.HangReportingScopePerfMetrics

Colectează timpul necesar pentru scenarii de bază Outlook: switchfolder switchmodule, sendmailoutbox, openitemclassic, sendmailtransport. Datele sunt monitorizate activ pentru probleme de performanță anormală. Acestea se folosesc pentru a detecta și a diagnostica problemele de performanță și pentru a îmbunătăți performanța cu fiecare actualizare.

Se colectează următoarele câmpuri:

  - **ElapsedTotal** – timpul total petrecut în acest apel

  - **ScopeId** – numele funcției care conține declarația sau un nume particularizat oferit prin definiția domeniului

#### <a name="officeoutlookdesktopwatsonbuckets"></a>Office.Outlook.Desktop.WatsonBuckets

Această regulă colectează informațiile despre erori din jurnalele de evenimente create când Outlook s-a defectat în sesiunea anterioară.

Datele sunt monitorizate activ pentru blocări anormale. Ele se utilizează pentru a detecta și a identifica blocările și a le remedia în viitoarele actualizări.

Se colectează următoarele câmpuri:

  - **BucketId** – codul hash al stivei de apeluri

  - **ElapsedTotal** – timpul total petrecut în apel

  - **ElapsedHanging** – timpul de blocare petrecut în apel

#### <a name="officepowerpointsession"></a>Office.PowerPoint.Session

Se colectează utilizarea caracteristicilor pentru fiecare sesiune PowerPoint.  Aceste date se utilizează pentru a calcula raportul de închideri neplanificate PowerPoint la utilizarea unei caracteristici. Raportul de închideri neplanificate PowerPoint este un semnal cheie pentru a garanta că PowerPoint funcționează așa cum vă așteptați.

Se colectează următoarele câmpuri:

  - **Flag** – marcaje de sesiune

  - **Usage** – utilizarea caracteristicilor

#### <a name="officepowerpointuaedialog"></a>Office.PowerPoint.UAE.Dialog

Se colectează de fiecare dată când PowerPoint s-a închis pe neașteptate cu o casetă de dialog deschisă în partea de sus a ferestrei principale PowerPoint. Aceste informații sunt esențiale pentru a surprinde închiderile neplanificate PowerPoint cauzate de o casetă de dialog activă care blochează fereastra principală PowerPoint. Microsoft utilizează aceste date pentru a diagnostica problema și a garanta că PowerPoint rulează așa cum vă așteptați.

Se colectează următoarele câmpuri:

  - **DlgCnt** – numărul total de casete de dialog deschise când s-a blocat sesiunea

  - **DlgId** – identificatorul casetei de dialog deschise

  - **IdType** – tipul de identificator al casetei de dialog deschise

  - **InitTime** – ora de inițializare a sesiunii blocate

  - **SessionId** – identificatorul sesiunii blocate

  - **TopId** – identificatorul casetei de dialog de sus

  - **Version** – versiunea sesiunii blocate

#### <a name="officepowerpointuaedocument"></a>Office.PowerPoint.UAE.Document

Se colectează caracteristica utilizată într-un document atunci când PowerPoint s-a închis pe neașteptate. Aceste caracteristici includ expunerea de diapozitive, deschiderea, salvarea, editarea sau elaborarea în comun a documentelor sau închiderea. Aceste informații sunt esențiale pentru a surprinde închiderile neașteptate PowerPoint în timp ce utilizați o caracteristică. Microsoft utilizează aceste date pentru a diagnostica problema și a garanta că PowerPoint rulează așa cum vă așteptați.

Se colectează următoarele câmpuri:

  - **CoauthFlag** – marcaje de utilizare pentru elaborarea în comun

  - **CommandFlag** – marcaje de modificare a documentelor

  - **FileIOFlag** – marcaje de utilizare IO a fișierelor

  - **InitTime** – ora de inițializare a sesiunii blocate

  - **Location** – locația documentului

  - **ServerDocId** – identificatorul documentului de pe server

  - **SessionId** – identificatorul sesiunii blocate

  - **UrlHash** – codul hash al adresei URL a documentului

  - **Usage** – utilizarea caracteristicilor

  - **Version** – versiunea sesiunii blocate

#### <a name="officepowerpointuaeopen"></a>Office.PowerPoint.UAE.Open

Se colectează de fiecare dată când PowerPoint se închide pe neașteptate atunci când deschideți un document. Aceste informații sunt esențiale pentru a surprinde închiderile neașteptate PowerPoint în timp ce deschideți un document. Microsoft utilizează aceste date pentru a diagnostica problema și a garanta că PowerPoint rulează așa cum vă așteptați.

Se colectează următoarele câmpuri:

  - **FileUrlLocation** – locația adresei URL a documentului

  - **Flag** – marcajele de deschidere

  - **InitTime** – ora de inițializare a sesiunii blocate

  - **Location** – locația documentului

  - **OpenReason** – motivul deschiderii

  - **ServerDocId** – identificatorul documentului de pe server

  - **SessionId** – identificatorul sesiunii blocate

  - **UrlHash** – codul hash al adresei URL a documentului

  - **Version** – versiunea sesiunii blocate

#### <a name="officepowerpointuaesession"></a>Office.PowerPoint.UAE.Session

Se colectează caracteristica utilizată când sesiunea PowerPoint s-a închis pe neașteptate.  Aceste informații sunt esențiale pentru a surprinde închiderile neașteptate PowerPoint. Microsoft utilizează aceste date pentru a diagnostica problema și a garanta că PowerPoint rulează așa cum vă așteptați.

Se colectează următoarele câmpuri:

  - **Flag** – marcaje de sesiune

  - **InitTime** – ora de inițializare a sesiunii blocate

  - **PreviousSessionId** – identificatorul sesiunii blocate

  - **Usage** – utilizarea caracteristicilor

  - **Version** – versiunea sesiunii blocate

#### <a name="officepowerpointuaeshutdown"></a>Office.PowerPoint.UAE.Shutdown

Se colectează închiderile neașteptate PowerPoint în timpul închiderii. Aceste informații sunt esențiale pentru a surprinde închiderile neașteptate PowerPoint în timpul închiderii. Microsoft utilizează aceste date pentru a diagnostica problema și a garanta că PowerPoint rulează așa cum vă așteptați.

Se colectează următoarele câmpuri:

  - **InitTime** – ora de inițializare a sesiunii blocate

  - **SessionId** – identificatorul sesiunii blocate

  - **Etapa** – etapa de închidere

  - **Version** – versiunea sesiunii blocate

#### <a name="officepowerpointuaeslideshow"></a>Office.PowerPoint.UAE.SlideShow

Se colectează închiderile neașteptate PowerPoint în timpul închiderii. Aceste informații sunt esențiale pentru a surprinde închiderile neașteptate PowerPoint în timpul închiderii. Microsoft utilizează aceste date pentru a diagnostica problema și a garanta că PowerPoint rulează așa cum vă așteptați.

Se colectează următoarele câmpuri:

  - **InitTime** – ora de inițializare a sesiunii blocate

  - **Mode** – modul expunere de diapozitive

  - **SessionId** – identificatorul sesiunii blocate

  - **State** – starea expunerii de diapozitive

  - **Version** – versiunea sesiunii blocate

#### <a name="officeprogrammabilitytelemetryaddincrash"></a>Office.Programmability.Telemetry.AddInCrash

Eveniment generat la încărcarea unui program de completare COM. Aceste informații sunt esențiale pentru a determina dacă un program de completare a cauzat blocarea unei aplicații Office. Ele se utilizează pentru a evalua compatibilitatea globală a programelor de completare cu aplicațiile Office.

Se colectează următoarele câmpuri:

  - **CLSID** – identificatorul de clasă al programului de completare

  - **ConnectFlag** – comportamentul de încărcare al programului de completare curent

  - **FileName** – numele fișierului program de completare, exclusiv calea fișierului

  - **FriendlyName** – numele prietenos al programului de completare

  - **Interface** – interfața Office în care a apărut excepția

  - **LoadAttempts** – numărul de încercări pentru a încărca programul de completare

  - **Method** – metoda Office în care a apărut excepția

  - **OfficeApplication** – aplicația Office în care a apărut excepția

  - **OfficeVersion** – versiunile Office

  - **ProgID** – identificator de program de completare

#### <a name="officeprogrammabilitytelemetrymacrofileopened"></a>Office.Programmability.Telemetry.MacroFileOpened 

Declanșată la deschiderea unui fișier care conține macrocomenzi (VBA) pe un dispozitiv care a fost înscris la aplicațiile Office ca serviciu (OAAS) de către administratorul IT și unde Aplicațiile Microsoft 365 pentru întreprindere au fost activate cu o licență de întreprindere. Evenimentul este utilizat pentru a înțelege starea fișierelor care conțin macrocomenzi (VBA) într-o entitate găzduită și este comparat cu Office.Programmability.Telemetry.VbaTelemetryBreak care urmărește erorile din fișierele care conțin VBA. 

Nu se colectează câmpuri.

#### <a name="officesystemsystemhealthungracefulappexitmacandios"></a>Office.System.SystemHealthUngracefulAppExitMacAndiOS

Eveniment de inițializare care captează ieșirile neelegante din aplicație pentru investigații suplimentare.

Se colectează următoarele câmpuri:

- **AffectedProcessAppBuild** - numărul compilării

- **AffectedProcessAppBuildRevision** - număr revizuire compilare

- **AffectedProcessAppMajorVer** - numărul de versiune major al aplicației

- **AffectedProcessAppMinorVer** - numărul de versiune minor al aplicației

- **AffectedProcessAppName** - nume aplicație

- **AffectedProcessResidentMemoryOnCrash** - memoria rezidentă a aplicației căzute

- **AffectedProcessUnsymbolicatedChecksum** - merge cu codul hash al stivei pentru simbolizare

- **AffectedProcessVirtualMemoryOnCrash** - memoria virtuală a aplicației căzute

- **AffectedSessionDuration** - durata sesiunii în secunde înainte de cădere

- **AffectedSessionLongBuildNumber** - număr de compilare lung

- **CrashedProcessSessionID** - SessionID pentru proces la căderea aplicației

- **DetectionTime** - DateTime pentru căderea aplicației
    
- **DeviceModel** - model de hardware

- **MERPSessionID** - ID-ul sesiunii de MERP

- **ReportingOsLocaleTag** - setări regionale ale sistemului de operare

- **ReportingOSVerStr** - versiunea sistemului de operare

- **SessionBuildNumber** - versiunea aplicației care a suferit căderea

- **SessionIDSMatch** - valoare Booleană utilizată pentru a verifica dacă ID-ul sesiunii de raportare este la fel ca cel preluat de Merp

- **SessionVersion** - versiunea aplicației care a suferit căderea - **Stackhash** - codul hash pentru trasarea stivei aplicației care a suferit căderea

- **UAEType** - enum care oferă informații despre ce tip de cădere a fost

#### <a name="officethisaddinstartupfailed"></a>Office.ThisAddIn.StartupFailed

Colectează informațiile pentru excepția care apare la pornirea aplicației Data Streamer. Aceste date se utilizează pentru a monitoriza starea de funcționare a aplicației. Evenimentul este generat de Microsoft Data Streamer pentru programul de completare Excel.

Se colectează următoarele câmpuri:

- **Exception** – stiva de apeluri pentru excepție

- **Event name** – categoria evenimentului și eticheta acestuia.

#### <a name="onenotesafebootresetcrashcounteronappsuspend-officeonenoteandroidsafebootresetcrashcounteronappsuspend-officeandroidearlytelemetry-safebootresetcrashcounteronappsuspend"></a>OneNote.SafeBootResetCrashCounterOnAppSuspend, Office.OneNote.Android.SafeBootResetCrashCounterOnAppSuspend, Office.Android.EarlyTelemetry. SafeBootResetCrashCounterOnAppSuspend

Semnalizarea critică este trimisă atunci când resetăm contorul de avarie din suspendarea aplicațiilor înainte de a se afișa caseta de dialog boot în condiții de siguranță. Acest marcator este necesar pentru a urmări și a diagnostica starea aplicației. Se afișează o casetă de dialog de încărcare sigură atunci când aplicația se defectează de mai multe ori în mod continuu. Oferă utilizatorului opțiunea de a reseta aplicația. Acest marcator vă va ajuta să vă dați seama dacă nu s-a afișat caseta de dialog boot în condiții de siguranță pentru un utilizator, în ciuda atingerii criteriilor de declanșare. 

Se colectează următoarele câmpuri:

- Fără


#### <a name="telemetryerror"></a>telemetry.error

Acest eveniment ne permite să diagnosticăm și să remediem problemele care împiedică generarea sau trimiterea datelor de diagnostic necesare. Aceste evenimente ne permit să înțelegem dacă lipsesc date critice necesare pentru a identifica probleme de securitate sau probleme majore referitoare la modul în care funcționează aplicația.

Se colectează următoarele câmpuri: 

- **timer_name** - ne spune unde se produce problema de telemetrie, de ex., în componenta cutie poștală sau în calendar. Acest lucru vă ajută să detectați și să rezolvați problemele de telemetrie care au loc dintr-o anumită parte a aplicației

- **type** - ne spune tipul de eroare de temporizator pentru a ne ajuta să detectăm când întâmpină aplicația noastră probleme privind trimiterea de date de telemetrie de diagnosticare


#### <a name="watchdoganr"></a>watchdog.anr

Este necesar pentru monitorizarea erorilor de performanță ale aplicațiilor pentru a împiedica cazurile în care aplicația nu mai răspunde, iar ecranul se blochează în aplicație (denumită ANR - aplicația nu răspunde).

Se colectează următoarele câmpuri: 

- **callstack** - stivă de apeluri pentru cod, în care s-a produs ANR
 
- **caused_restart** - dacă aplicația a fost obligată să repornească din cauza ANR
 
- **duration** - intervalul de timp în care dispozitivul a fost blocat
 
- **id** - identificator unic pentru ANR
 
- **interval** - pragul configurat pentru declanșarea ANR
 
- **is_application_object_initialized** - dacă ANR s-a produs după ce aplicația a fost inițializată complet sau înainte
 
- **last_known_is_in_foreground** - dacă aplicația a fost mai recent în prim plan sau în fundal


### <a name="application-feature-performance-subtype"></a>*Subtipul de performanță al caracteristicii aplicației*

Timpii de răspuns slabi sau performanțele scăzute pentru scenarii precum pornirea aplicației sau deschiderea unui fișier.

#### <a name="androidframemetrics"></a>android.frame.metrics

Ne permite să detectăm și să remediem situațiile în care componentele aplicațiilor noastre Android cauzează probleme de performanță, de exemplu, dacă inboxul dvs. defilează fără probleme.

Se colectează următoarele câmpuri: 

- **animation_duration** - durata redării animației în milisecunde

- **command_issue_duration** - durata de emitere a comenzilor pe platformă în milisecunde 

- **draw_duration** - durata de desenare a UI în milisecunde 

- **input_handling_duration** - durata manipulării de intrare în milisecunde 

- **layout_measure_duration** - durata măsurării aspectului în milisecunde

- **origin** - componenta de aplicație măsurată, de exemplu, calendar sau e-mail

- **sync_duration** - durată de sincronizare a cadrului în milisecunde

- **swap_buffers_duration** - durata de comutare între tampoane în milisecunde

- **total_duration** - durata totală de redare a cadrelor în milisecunde

- **unknown_delay** - întârziere cauzată de surse necunoscute, altele decât duratele urmărite în mod explicit

#### <a name="calcomponent"></a>cal.component

Acest eveniment ne permite să detectăm și să remediem problemele cu impact de performanță perceptibil asupra componentelor UI de calendar, care ar putea cauza probleme de defilare la nivelul calendarului.

Se colectează următoarele câmpuri: 

- **account_counter** - urmărește numărul de conturi asociate pentru fiecare tip de calendar, de ex. 2 pentru calendarul Gmail și dacă acel cont utilizează noul nostru serviciu de sincronizare

- **app_instance** - Outlook are 2 puncte de intrare pentru Duo, unul este pentru calendar și altul este pentru Mail, iar ambele pot fi lansate alăturat într-un mediu cu mai multe instanțe. Acest lucru ne va permite să știm ce instanță face acest apel de raportare, Mail sau Calendar

- **component_name** - ne spune numele componentei de calendar, cum ar fi vizualizarea Agendă sau vizualizarea Zi, pentru a ne ajuta să detectăm probleme de performanță care au impact asupra unei anumite componente din calendar

- **display_frame_data** - urmărește timpul petrecut cu afișarea a 60 de cadre, pentru a determina dacă există probleme de performanță. 

- **orientation** - ne spune dacă dispozitivul a fost în modul portret sau peisaj, pentru a ne ajuta să detectăm probleme de performanță care au impact asupra unei anumite orientări a dispozitivelor

- **taskId** - TaskId ne va oferi identificatorul activității al instanței curente. Acest lucru va fi necesar în medii cu mai multe instanțe, dacă utilizatorul dorește să lanseze aceeași instanță (Calendar, Calendar sau Mail, Mail) alăturat

- **view_duration** - ne spune cât timp a fost necesar pentru a reda diferitele componente de calendar UI pentru a ne ajuta să detectăm probleme de performanță care influențează experiența dvs. de calendar

#### <a name="contactaction"></a>contact.action

Acest eveniment este declanșat de acțiuni diferite pentru persoanele de contact, vizualizarea, actualizarea și ștergerea persoanelor de contact, precum și vizualizarea listei de persoane de contact. Acest lucru este utilizat pentru a determina dacă există regresii de performanță care au legătură cu persoanele de contact.

Se colectează următoarele câmpuri: 

- **accounts_with_filters** - numărul conturilor cu filtre aplicate la lista de persoane de contact

- **action** - acțiunea efectuată, de exemplu, vizualizarea unei persoane de contact
 
- **duration_initial_view_load** - durata de la deschiderea vizualizării până la încărcarea inițială a listei de persoane de contact

- **duration_show_contacts** - durata de la deschiderea vizualizării până la afișarea listei de persoane de contact
 
- **total_contacts** - numărul persoanelor de contact fără filtre aplicate
 
- **total_filtered_contacts** - numărul persoanelor de contact cu filtre aplicate

#### <a name="conversationloadtime"></a>conversation.load.time

Acest eveniment ne permite să detectăm și să remediem problemele în care există un impact de performanță perceptibil asupra încărcării conversațiilor de e-mail pentru a vă asigura că e-mailurile se încarcă așa cum vă așteptați.

Se colectează următoarele câmpuri: 

- **time** - ne spune intervalul de timp necesar pentru încărcarea conversației de e-mail.

#### <a name="coredatamigration"></a>core.data.migration

Ne permite să detectăm și să remediem situațiile în care s-a produs o eroare la actualizarea datelor de e-mail de pe dispozitivul dvs. la o versiune mai nouă.

Se colectează următoarele câmpuri:

- **db_size_megabytes** - urmărește dimensiunea bazei de date nucleu rotunjită la cei mai apropiați 25 de megaocteți și cu un număr maxim de MB de 500

- **db_wal_size_megabytes** - urmărește dimensiunea bazei de date nucleu rotunjită la cel mai apropiat 1 megaoctet și cu un număr maxim de MB de 10

- **free_space_megabytes** - urmărește spațiul liber disponibil în bucketuri 10, 100, 1000, 10.000, apoi 100.000. 

- **migration_duration_seconds** - urmărește durata de migrare rotunjită la unul dintre aceste segmente de timp: 0, 10, 20, 30, 40, 50, 60, 70, 80, 90, 100, 110, 120, 130, 140, 150, 160, 170, 180 (180 și după aceea ar trebui să fie doar 180)

#### <a name="coredataperformance"></a>core.data.performance

Ne permite să detectăm și să remediem situațiile în care datele de e-mail pe care le stocăm pe dispozitivul dvs. cauzează probleme de performanță.

Se colectează următoarele câmpuri:

- **Caller** - urmărește numele entității care apelează operațiunea salvare

- **db_size_megabytes** - urmărește dimensiunea bazei de date nucleu rotunjită la cei mai apropiați 25 de megaocteți și cu un număr maxim de MB de 500

- **duration** - urmărește intervalul de timp necesar pentru a finaliza operațiunea

- **entity** - urmărește numele entității care a apelat operațiunea de preluare

- **operation** - valoarea brută a operațiunii, indiferent că este vorba despre salvare, preluare sau „coadă citire scriere blocată”

#### <a name="inboxcomponent"></a>inbox.component

Acest eveniment colectează două tipuri de date: starea abonamentului Microsoft 365 și dacă utilizatorul vede anunțuri.  Acest eveniment ne ajută să detectăm și să remediem problemele în care există un impact de performanță perceptibil asupra componentelor UI ale utilizatorului din inbox care ar putea face ca e-mailurile, avatarul, starea citit/necitit să nu se încarce sau să nu se afișeze corect.

Se colectează următoarele câmpuri: 

- **above_40fps** - numărul de cadre redate peste 40fps

- **above_50fps** - numărul de cadre redate peste 50fps

- **above_55fps** - numărul de cadre redate peste 55fps

- **account_counter** - numărul corespunzător fiecărui tip de cont prezent pe dispozitiv, de exemplu, un cont Office 365 = 1 cont, un cont Outlook.com = 1 cont.

- **ad_not_shown_reason** - motivul pentru care nu sunt afișate reclame

- **ad_shown** - dacă a fost afișată o reclamă (dacă sunt activate reclamele)

- **ad_shown_for_premium** - afișarea în mod neașteptat a anunțului utilizatorilor premium 

- **age** - vârsta persoanei (utilizată pentru a confirma conformitatea cu limitările de vârstă a anunțurilor) *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

- **app_instance** - Outlook are 2 puncte de intrare pentru Duo, unul este pentru calendar și altul este pentru Mail, iar ambele pot fi lansate alăturat într-un mediu cu mai multe instanțe. Acest lucru ne va permite să știm ce instanță face acest apel de raportare, Mail sau Calendar

- **component_name** - numele componentei/vizualizării care este activă în timpul filtrării

- **has_hx** - dacă dispozitivul are cel puțin un cont Hx (noul nostru serviciu de sincronizare a e-mailului)

- **has_subscription** - dacă dispozitivul are un abonament cu reclame

- **is_all_accounts_inbox** - dacă inboxul curent este folderul „toate conturile”

- **is_current_account** - dacă contul activ curent este cont cu reclame

- **load_error_code** - cod de eroare atunci când încărcați reclame

- **network_error_code** - cod de eroare de rețea atunci când solicitați reclame

- **orientation** - orientarea ecranului la ora evenimentului (portret sau peisaj)

- **provider** – furnizorul (Xandr sau Facebook) anunțului curent afișat

- **sub_error_type** - tip de eroare detaliat

- **taskId** - TaskId ne va oferi identificatorul activității al instanței curente. Acest lucru va fi necesar în medii cu mai multe instanțe, dacă utilizatorul dorește să lanseze aceeași instanță (Calendar, Calendar sau Mail, Mail) alăturat

- **total_count** - numărul total de cadre total afișat de componentă

- **view_duration** - cât timp a fost vizualizată componenta de către utilizator

#### <a name="initialpagelanding"></a>Initial.page.landing 
 
Acest eveniment ajută urmărirea tipului de experiență pe care o văd utilizatorii atunci când aterizează în pagina noastră de aplicații.  Aceste date se utilizează pentru a determina traficul de utilizatori canalizat în fiecare experiență din aplicația noastră și, de asemenea, ne ajută să sintetizăm cu ușurință rezultatele experimentale.
 
Se colectează următoarele câmpuri: 

- **Page** - acest lucru este utilizat pentru a urmări tipul de experiență pe care utilizatorul o vede prima dată când aterizează pe pagina noastră. Valorile posibile sunt „versiune de încercare“, „ignorare“, „pre-cuplat“, „abonament“ etc.

- **storeExperience** - acest lucru este utilizat pentru a determina dacă utilizatorul a fost eligibil pentru a vedea experiența din magazinul SDK.

- **stringVariant** - acest lucru este utilizat pentru a determina tipul de șiruri pe care le vede utilizatorul atunci când aterizează pe pagina noastră. Rețineți că, pentru orice pagină, cum ar fi „Versiune de încercare“, utilizatorul poate fi eligibil pentru a vedea șiruri diferite, în funcție de faptul dacă a instalat Office Legacy sau dacă a activat anterior Office. Eventualele enumerări ale acestei proprietăți sunt „LegacyUpsell“, „OfficeOpened“, „implicit“, „YesIntent“, „NoIntent“ etc.

- **windowsBuildType** - acesta este utilizat pentru a urmări tipul de WindowsBuildType pe care este utilizatorul. i.e. „RS4“, „RS5“, „RS19H1“, „Vibranium“ etc. Pe măsură ce experiențele noastre sunt, de obicei, direcționate către diferite WindowsBuildTypes, această proprietate este esențială pentru diferențierea între lansări. 

#### <a name="ipcpbootstrapuser"></a>IpcpBootstrapUser

Este colectat atunci când un utilizator încearcă să deschidă un document protejat prin IRM sau să aplice protecții IRM. Acesta conține informațiile necesare pentru a investiga și a diagnostica corect problemele care apar atunci când se realizează apelul API IpcpBootstrapUser. 

Se colectează următoarele câmpuri:

- **AppInfo.ClientHierarchy** - ierarhie client care indică faptul că aplicația rulează în mediul de producție sau în mediul de dezvoltator

- **AppInfo.Name** - nume aplicație.

- **AppInfo.Version** - versiunea aplicației

- **iKey** - ID al serverului pentru servicii de înregistrare

- **RMS.ApplicationScenarioId** - ID al scenariului furnizat de aplicație

- **RMS.AuthCallbackProvided** - indică dacă se furnizează apelare inversă pentru autentificare ca intrare pentru apelul API sau nu

- **RMS.ConnectionInfo.ExtranetUrl** - URL de extranet din informațiile de conexiune

- **RMS.ConnectionInfo.IntranetUrl** - URL de intranet din informațiile de conexiune

- **RMS.ConnectionMode** - modul de conexiune între clientul Serviciu de administrare a drepturilor și server: online sau offline

- **RMS.Duration** - timp total pentru finalizarea apelului API

- **RMS.DurationWithoutExternalOps** - timp total minus operațiuni externe consumate, cum ar fi latența de rețea.

- **RMS.ErrorCode** - codul de eroare returnat de apelul API, dacă există.

- **RMS.GuestTenant** - ID-ul entității găzduite invitat pentru utilizator

- **RMS.HomeTenant** - ID-ul entității găzduite domiciliu pentru utilizator

- **RMS.HttpCall** - indică dacă există operațiune HTTP

- **RMS.Identity.ExtranetUrl** - URL-ul de extranet pentru serverul Serviciului de administrare a drepturilor pentru utilizator, colectat în timpul obținerii unui nou Certificat de cont de drepturi de la server

- **RMS.Identity.IntranetUrl** - URL-ul de intranet pentru serverul Serviciului de administrare a drepturilor pentru utilizator, colectat în timpul obținerii unui nou Certificat de cont de drepturi de la server

- **RMS.Identity.Status** - prima dată când se obține Certificatul de cont de drepturi de la server sau când se reînnoiește Certificatul de cont de drepturi 

- **RMS.Identity.Type** - tipul de cont de utilizator, cum ar fi cont Windows sau cont live

- **RMS.Identity.UserProvided** - indică dacă adresa de e-mail a utilizatorului a fost furnizată sau nu în timpul obținerii unui nou Certificat de cont de drepturi de la server

- **RMS.IssuerId** - ID-ul serverului Serviciului de administrare a drepturilor care emite Certificatul de cont de drepturi  

- **RMS.LicenseFormat** - formatul licenței: Xrml sau Json

- **RMS.RACType** - tipul Certificatului de cont de drepturi

- **RMS.Result** - succes sau eșec al apelului API

- **RMS.ScenarioId** - ID al scenariului definit de API

- **RMS.SDKVersion** - versiunea clientului pentru Serviciul de administrare a drepturilor

- **RMS.ServerType** - tipul de server al Serviciului de administrare a drepturilor 

- **RMS.StatusCode** - cod de stare al rezultatului returnat

- **RMS.TemplatesCount** - numărul de șabloane

- **RMS.TokenProvided** - indică dacă se furnizează tokenul ca intrare pentru apelul API sau nu 

- **RMS.UserProvided** - indică dacă se furnizează consumatorul ca intrare pentru apelul API sau nu 

- **UserInfo.UserObjectId** - ID al obiectului utilizator

#### <a name="ipcpgetkey"></a>IpcpGetKey

Se colectează atunci când un utilizator încearcă să deschidă un document protejat cu IRM (Information Rights Management) sau să aplice protecții IRM. Acesta conține informațiile necesare pentru a investiga și a diagnostica corect problemele care apar atunci când se realizează apelul API IpcpGetKey. 

Se colectează următoarele câmpuri:

- **AppInfo.ClientHierarchy** - ierarhie client care indică faptul că aplicația rulează în mediul de producție sau în mediul de dezvoltator

- **AppInfo.Name** - nume aplicație.

- **AppInfo.Version** - versiunea aplicației

- **iKey** - ID al serverului pentru servicii de înregistrare

- **RMS.ApplicationScenarioId** - ID-ul scenariului furnizat de aplicație

- **RMS.AuthCallbackProvided** - indică dacă se furnizează callback pentru autentificare ca intrare pentru apelul API sau nu

- **RMS.ConnectionMode** - modul de conexiune între clientul Serviciu de administrare a drepturilor și server: online sau offline

- **RMS.ContentId** - ID-ul de conținut al documentului

- **RMS.Duration** - timp total pentru finalizarea apelului API

- **RMS.DurationWithoutExternalOps** - timp total minus operațiuni externe consumate, cum ar fi latența de rețea.

- **RMS.ErrorCode** - codul de eroare returnat de apelul API, dacă există.

- **RMS. EulId** - ID-ul licenței pentru utilizatorul final

- **RMS. EulProvided** - indică dacă furnizează licența de utilizator final ca intrare a apelului API sau nu

- **RMS.GuestTenant** - ID-ul entității găzduite invitat pentru utilizator 

- **RMS.HomeTenant** - ID-ul entității găzduite de domiciliu pentru utilizator

- **RMS.HttpCall** - indică dacă există operațiune http

- **RMS.Identity.ExtranetUrl** - URL-ul de extranet pentru serverul Serviciului de administrare a drepturilor pentru utilizator, colectat în timpul obținerii unui nou Certificat de cont de drepturi de la server

- **RMS.Identity.IntranetUrl** - URL-ul de intranet pentru serverul Serviciului de administrare a drepturilor pentru utilizator, colectat în timpul obținerii unui nou Certificat de cont de drepturi de la server

- **RMS.Identity.Status** - prima dată când se obține Certificatul de cont de drepturi de la server sau când se reînnoiește Certificatul de cont de drepturi 

- **RMS.Identity.Type** - tipul de cont de utilizator, cum ar fi cont Windows sau cont live

- **RMS.Identity.UserProvided** - indică dacă adresa de e-mail a utilizatorului a fost furnizată sau nu în timpul obținerii unui nou Certificat de cont de drepturi de la server

- **RMS.IssuerId** - ID-ul serverului RMS (Rights Management Service) care emite Certificatul de cont de drepturi 

- **RMS.KeyHandle** - adresa de memorie pentru handle-ul de cheie

- **RMS.LicenseFormat** - formatul licenței: Xrml sau Json

- **RMS.PL. ExtranetUrl** - URL-ul extranet din licența de publicare

- **RMS.PL. IntranetUrl** - URL-ul intranet din licența de publicare

- **RMS.PL. KeyType** - valorile „single” sau „double” indică dacă PL a fost protejat cu o singură cheie de protecție sau cu o cheie de protecție dublă

- **RMS.RACType** - tipul Certificatului de cont de drepturi

- **RMS.Result** - succes sau eșec al apelului API

- **RMS.ScenarioId** - ID-ul scenariului definit de API

- **RMS.SDKVersion** - versiunea clientului pentru Serviciul de administrare a drepturilor

- **RMS.ServerType** - tipul de server al Serviciului de administrare a drepturilor

- **RMS.StatusCode** - cod de stare al rezultatului returnat

- **RMS.TemplatesCount** - numărul de șabloane

- **RMS.TokenProvided** - indică dacă se furnizează tokenul ca intrare pentru apelul API sau nu 

- **RMS.UserProvided** - indică dacă se furnizează consumatorul ca intrare pentru apelul API sau nu 

- **UserInfo.UserObjectId** - ID-ul obiectului utilizator

#### <a name="jsonparseerror"></a>json.parse.error 
 
Acest eveniment indică faptul că a fost lansată o eroare de către parserul json.  Vom putea depana șirul de regiștrii citiți care a fost trimis la parserul json, pentru a permite o experiență netedă pentru utilizatorii noștri.
 
Se colectează următoarele câmpuri: 

- **Error** - acest lucru constă în mesajul de eroare pe care îl returnează obiectul de eroare.

#### <a name="mailfiltercomponent"></a>mail.filter.component

Acest eveniment ne permite să detectăm și să remediem problemele în care există un impact de performanță perceptibil asupra experienței de filtrare a e-mailului, care ar putea face ca filtrele dvs. să nu se încarce sau să nu se afișeze corect.

Se colectează următoarele câmpuri: 

- **above_40fps** - numărul de cadre redate peste 40fps
 
- **above_50fps** - numărul de cadre redate peste 50fps
 
- **above_55fps** - numărul de cadre redate peste 55fps
 
- **account_counter** - numărul corespunzător fiecărui tip de cont prezent pe dispozitiv, de exemplu, un cont Office 365 = 1 cont, un cont Outlook.com = 1 cont.
 
- **ad_not_shown_reason** - motivul pentru care nu sunt afișate reclame
 
- **ad_shown** - dacă a fost afișată o reclamă (dacă sunt activate reclamele)
 
- **age** - vârsta persoanei (utilizată pentru a confirma conformitatea cu limitările de vârstă pentru reclame)

- **app_instance** - Outlook are 2 puncte de intrare pentru Duo, unul este pentru calendar și altul este pentru Mail, iar ambele pot fi lansate alăturat într-un mediu cu mai multe instanțe. Acest lucru ne va permite să știm ce instanță face acest apel de raportare, Mail sau Calendar
 
- **component_name** - numele componentei/vizualizării care este activă în timpul filtrării
 
- **folder_type** - tipul de folder filtrat (e.g. Inbox, Coș de gunoi, Nonsistem)
 
- **has_hx** - dacă dispozitivul are cel puțin un cont Hx (noul serviciu de sincronizare a corespondenței)
 
- **has_subscription** - dacă dispozitivul are un abonament cu reclame
 
- **is_all_accounts_inbox** - dacă inboxul curent este folderul „toate conturile”
 
- **is_current_account** - dacă contul activ curent este cont cu reclame
 
- **load_error_code** - cod de eroare atunci când încărcați reclame
 
- **network_error_code** - cod de eroare de rețea atunci când solicitați reclame
 
- **orientation** - orientarea ecranului la ora evenimentului (portret sau peisaj)
 
- **sub_error_type** - tip de eroare detaliat

- **taskId** - TaskId ne va oferi identificatorul activității al instanței curente. Acest lucru va fi necesar în medii cu mai multe instanțe, dacă utilizatorul dorește să lanseze aceeași instanță (Calendar, Calendar sau Mail, Mail) alăturat
 
- **total_count** - numărul total de cadre total afișat de componentă
 
- **view_duration** - cât timp a fost vizualizată componenta de către utilizator

#### <a name="officeandroidandroidofficelaunchtolandingpagelatency"></a>Office. Android. AndroidOfficeLaunchToLandingPageLatency

Critic pentru capturarea pentru performanța metrică a aplicațiilor în ceea ce privește timpul de răspuns al aplicației din boot.  Microsoft folosește acesta pentru a colecta timpul necesar pentru ca aplicația să fie receptivă și totodată, să detecteze scenarii care pot influența timpul de încărcare în Word, Excel sau PowerPoint.

Se colectează următoarele câmpuri:
 
- **AnyCrashInteractionDuringBoot** -Boolean pentru orice accident întâlnit în timpul încărcării

- **AppActivationTimeInMs** - durata fazei de aplicație

- **AppSuspendedDuringBoot** - Boolean pentru suspendarea aplicațiilor în timpul încărcării

- **AvailableMemoryInMB** -memorie disponibilă

- **CollectionTime** - ora evenimentului

- **DalvikHeapLimitInMB** - informații ajutor

- **DocumentRecoveryInvoked** - Boolean pentru a indica dacă un document a fost recuperat

- **ExtractionDone** - durata extragerii librăriei native

- **FastBootGainTimeInMs** - timpul pentru completarea încărcării rapide

- **FileActivationAttempted** - Boolean pentru a indica dacă aplicația a fost lansată datorită activării fișerului

- **HasLogcatLoggingImpactOnBoot** - Boolean pentru a indica dacă logcat a afectat timpul încărcării 

- **IsThisFirstLaunch** - Boolean pentru a indica dacă se lansează aplicația pentru prima dată

- **LatencyTimeInMilliSec** - timp de așteptare în milisecunde

- **LibrarySharingTimeInMs** - timp pentru partajarea bibliotecilor

- **LoadMinLibsTimeInMs** - timp de încărcare pentru setul minim de biblioteci

- **MruListingTimeInMs** -timp pentru a încărca MRU

- **NativeLibrariesLoadTime** - timpul de încărcare al bibliotecii CPP

- **NumberOfRunningProcesses** - numărul de procese în execuție

- **NumberOfRunningProcesses** - numărul de procese în derulare

- **NumberOfRunningServices** - numărul de servicii care rulează

- **OfficeActivityTimeInMs** timp pentru inițializare OfficeActivity

- **PostAppInitTimeInMs** - durata fazei de aplicație

- **PreAppInitializationTime** - timp de inițializare a fazei de aplicație

- **PreAppInitTimeInMs** - durata fazei de aplicație

- **TotalMemoryInMB** -total memorie

- **UIRaaSDownloadLanguagePackageBoot** - informații legate de descărcarea pachetului lingvistic

- **UserDialogInterruptionDuringBoot** - Boolean pentru orice casetă de dialog de blocare afișată în timpul încărcării


#### <a name="officeappleappleappbootmac"></a>Office.Apple.Apple.AppBoot.Mac

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Evenimentul este utilizat pentru a colecta timpul necesar pentru a încărca aplicația, precum și câteva detalii despre tipul de încărcare efectuat. Acest eveniment ne ajută să monitorizăm performanța și să furnizăm îmbunătățiri ale acesteia.

Se colectează următoarele câmpuri:

- **Data_ Data_EvtBootTimerDocStageReady** - timpul scurs până când ajungeți la un anumit punct în cod.

- **Data_DocumentRecoveryInvoked** - dacă s-au invocat recuperări de documente în timpul încărcării.

- **Data_EvtBootTimerBootIdle** - timpul scurs până când ajungeți la un anumit punct în cod.

- **Data_EvtBootTimerFinishLaunchEnd** - timpul scurs până când ajungeți la un anumit punct în cod.

- **Data_EvtBootTimerLaunchDidFinish** - timpul scurs până când ajungeți la un anumit punct în cod.

- **Data_EvtBootTimerLaunchStart** - timpul scurs până când ajungeți la un anumit punct în cod.

- **Data_EvtBootTimerMainStart** - timpul scurs până când ajungeți la un anumit punct în cod.

- **Data_EvtBootTimerStaticInit** - timpul scurs până când ajungeți la un anumit punct în cod.

- **Data_EvtDockStageReady** - timpul scurs până când ajungeți la un anumit punct în cod.

- **Data_IsFileOpenAttempted** - dacă s-a încercat deschiderea unui fișier în timpul încărcării.

- **Data_IsFirstRunAttempted** - dacă încărcarea aplicației a trecut prin prima experiență de rulare.

- **Data_SentToBackground** - dacă aplicația a fost trimisă în fundal în timpul încărcării.

#### <a name="officeapplediskruleresultserializererroronstreamop"></a>Office.Apple.DiskRuleResultSerializerErrorOnStreamOp

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Evenimentul este utilizat pentru a monitoriza starea infrastructurilor noastre de telemetrie. Acest eveniment indică faptul că s-a produs o eroare.

Se colectează următoarele câmpuri:

- **Data_ActualBytesModified** - numărul de octeți modificați.

- **Data_BytesRequested** - număr de octeți de procesat.

- **Data_IsWriteOp** - dacă suntem pe punctul de a executa o operațiune de scriere

#### <a name="officeapplemacbootresourceusage"></a>Office.Apple.MacBootResourceUsage

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Evenimentul este utilizat pentru a colecta mai mulți indicatori din jurul resurselor consumate în timpul încărcării de aplicații Office. Acest eveniment ne ajută să monitorizăm performanța și să furnizăm îmbunătățiri ale acesteia.

Se colectează următoarele câmpuri:

- **Data_BlockInputOperations** - un contor de operațiuni de intrare în bloc

- **Data_BlockInputOperations** - un contor de operațiuni de ieșire în bloc

- **Data_InvoluntaryContextSwitches** - numărul de comutatoare de context involuntar

- **Data_MainThreadCPUTime** - o măsurătoare de timp scursă

- **Data_MaxResidentSize** - o măsurătoare de dimensiune de memorie

- **Data_MessagesReceived** - numărul de mesaje primite

- **Data_MessagesSent** - numărul de mesaje trimise

- **Data_PageFaults** - o contorizare a revendicărilor paginilor

- **Data_PageReclaims** - o contorizare a revendicărilor paginilor

- **Data_ProcessCPUTime** - o măsurătoare de timp scurs

- **Data_SharedTextMemorySize** - o măsurătoare de dimensiune de memorie

- **Data_SignalsReceived** - numărul semnalelor primite

- **Data_Swaps** - un contor de comutare de date

- **Data_SystemCPUTime** - o măsurătoare de timp scurs

- **Data_SystemUpTime** - o măsurătoare de timp scurs

- **Data_UnsharedDataSize** - o măsurătoare de dimensiune de date

- **Data_UnsharedStackSize** - o măsurătoare de dimensiune de stivă

- **Data_UserCPUTime** - o măsurătoare de timp scurs

- **Data_VoluntaryContextSwitchesNvcsw** - numărul de comutatoare de context involuntar

#### <a name="officeapplemauvalidation"></a>Office.Apple.MAU.Validation

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Evenimentul este utilizat pentru a monitoriza starea componentei de actualizare automată Microsoft, care este utilizată pentru a distribui și a instala actualizările aplicațiilor. Datele colectate sunt utilizate pentru detectarea erorilor și pentru investigarea cauzelor acestora.

Se colectează următoarele câmpuri:

- **Data_EventID** - colectăm un șir reprezentând un cod de eroare

- **Data_Message** - colectăm un șir care conține o descriere a erorii

#### <a name="officeapplembuinstrumenthangdetectionspincontrol"></a>Office.Apple.MbuInstrument.Hang.Detection.Spin.Control

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Evenimentul este înregistrat de fiecare dată când o aplicație pare că nu răspunde. Acest eveniment ne ajută să monitorizăm performanța și să furnizăm îmbunătățiri ale acesteia.

Se colectează următoarele câmpuri:

- **Data_CountSpinControlStart** - un marcator decât indică faptul că aplicația pare să nu răspundă (sau este lentă în a răspunde)

#### <a name="officeapplembuinstrumentvmondocumentclose"></a>Office.Apple.MbuInstrument.VMOnDocumentClose

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Evenimentul este utilizat pentru a colecta un instantaneu al stării de memorie în timpul închiderii documentului. Acest eveniment ne ajută să monitorizăm performanța și să furnizăm îmbunătățiri ale acesteia.

Se colectează următoarele câmpuri:

- **Data_CollectionTime** - un marcator de timp din momentul în care au fost colectate datele

- **Data_ResidentMemory** - valoarea de memorie de rezident observată

- **Data_VirtualMemory** - valoarea de memorie virtuală observată

#### <a name="officeapplembuinstrumentvmonshutdown"></a>Office.Apple.MbuInstrument.VMOnShutdown

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Evenimentul este utilizat pentru a colecta un instantaneu al stării de memorie în timpul închiderii aplicației. Acest eveniment ne ajută să monitorizăm performanța și să furnizăm îmbunătățiri ale acesteia.

Se colectează următoarele câmpuri:

- **Data_CollectionTime** - un marcator de timp din momentul în care au fost colectate datele

- **Data_ResidentMemory** - valoarea de memorie de rezident observată

- **Data_VirtualMemory** - valoarea de memorie virtuală observată

#### <a name="officeapplembuinstrumentvmonstart"></a>Office.Apple.MbuInstrument.VMOnStart

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Evenimentul este utilizat pentru a colecta un instantaneu al stării de memorie în timpul pornirii aplicației. Acest eveniment ne ajută să monitorizăm performanța și să furnizăm îmbunătățiri ale acesteia.

Se colectează următoarele câmpuri:

- **Data_CollectionTime** - un marcator de timp din momentul în care au fost colectate datele

- **Data_ResidentMemory** - valoarea de memorie de rezident observată

- **Data_VirtualMemory** - valoarea de memorie virtuală observată

#### <a name="officeapplemsoappdelegatebootperf"></a>Office.Apple.MsoAppDelegate.BootPerf

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Evenimentul este utilizat pentru a colecta timp și memorie consumate în timpul încărcării de aplicații Office, precum și câteva detalii despre tipul de încărcare efectuat. Acest eveniment ne ajută să monitorizăm performanța și să furnizăm îmbunătățiri ale acesteia.

Se colectează următoarele câmpuri:

- **Data_AppLaunchDurationMicroSec** - durata procesului de încărcare

- **Data_AppLaunchFinishSystemTime** - un marcaj de temporal la un anumit marcator de cod de încărcare

- **Data_AppLaunchFinishSystemTime** - un marcaj temporal la un anumit marcator de cod de încărcare

- **Data_ResidentMemory** - un instantaneu al memoriei rezidente disponibile în timpul încărcării

- **Data_VirtualMemory** - un instantaneu al memoriei rezidente disponibile în timpul încărcării

#### <a name="officeappleungracefulappexithangsinprevioussession"></a>Office.Apple.UngracefulAppExitHangsInPreviousSession

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Evenimentul este utilizat pentru a monitoriza starea de funcționare a aplicațiilor noastre Office, precum și pentru a investiga cauzele erorilor. Colectăm de câte ori a apărut o aplicație care nu răspunde înainte de a atinge o ieșire incorectă de aplicație.

Se colectează următoarele câmpuri:

- **Data_HangsDetected** - de câte ori o aplicație pare că nu răspunde înainte de a atinge o ieșire incorectă.

- **Data_LastSessionId** - identificatorul pentru sesiunea în care a fost observată ieșirea din aplicația incorectă.

- **Data_SessionSessionBuildNumber** - versiunea minoră a aplicației în care a fost observată o ieșire din aplicație.

- **Data_SessionVersion** - versiunea majoră a aplicației în care a fost observată o ieșire incorectă.

#### <a name="officeapplewhatsnewerrorandwarning"></a>Office.Apple.WhatsNewErrorAndWarning

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Evenimentul este utilizat pentru a monitoriza starea caracteristicii Noutăți. Acest eveniment denotă faptul că s-a produs o eroare/avertisment în timp ce analizați conținutul Noutăți, indicând probleme potențiale de creare de conținut.

Se colectează următoarele câmpuri:

- **Data_ContentKey** - un indicator către secțiunea de conținut care poate să fi cauzat eroarea.

- **Data_ErrorCode** - codul de eroare observat (dacă este disponibil)

- **Data_Error_Description** - o descriere a erorii (dacă este disponibilă)

- **Data_EventID** - colectăm un șir reprezentând un cod de eroare observată.

- **Data_IncludesHTMLTag** - dacă conținutul conține HTML îmbogățit

- **Data_IncludesItemsTag** - dacă conținutul conține o ierarhie de elemente

- **Data_LengthOfRawData** - dimensiunea conținutului

- **Data_RequestURL** - adresa URL de la care s-a descărcat conținutul

- **Data_ServerLanguageTag** - limba în care se afla conținutul.

- **Data_StatusCode** - starea erorii (dacă este disponibilă)

#### <a name="officeextensibilityrichapimethodinvocation"></a>Office.Extensibility.RichApiMethodInvocation

Atunci când clientul utilizează un program de completare Office și apelează Rich API pentru furnizarea serviciului, va fi declanșat acest eveniment. Utilizat pentru a măsura fiabilitatea serviciului, performanța și gradul de utilizare pentru invocarea metodelor Rich API.
 
Se colectează următoarele câmpuri:

- **Api** - nume complet API

- **DispFlag** - o semnalizare bit care descrie tipul de apel de metodă (de exemplu: 0x1 = METHOD, 0x2 = PROPERTYGET, 0x4 = PROPERTYPUT, 0x8 = PROPERTYPUTREF)

- **DispId** - ID-ul de expediție pentru metoda apelată

- **HResult** - HResult pentru apelul de metodă

- **Latency** - latența apelului, în microsecunde

- **ReqId** - GUID pentru solicitarea de grup căreia îi aparține această metodă

- **TypeId** - GUID pentru interfața pe care se apelează această metodă

#### <a name="officeiospaywallfailedscreenretrybuttontap"></a>Office.iOS.Paywall.FailedScreen.RetryButtonTap

Această telemetrie de utilizare este colectată pentru a afla când a eșuat Achiziționarea/Asigurarea accesului/Activarea, iar utilizatorul a apăsat butonul „Reîncercare”.  Utilizat pentru a depana scenariile de erori de achiziție care duc la reîncercarea și îmbunătățirea fiabilității procesului.

Se colectează următoarele câmpuri:

- **failureReason** - Șir – indică eroarea pentru care utilizatorul reîncearcă. Cum ar fi „provisioningFailed”, „purchaseFailed”, „activationFailed”.

- **productid** - Șir – ID-ul produsului din App Store pentru care utilizatorul reîncearcă solicitarea nereușită


#### <a name="officemanageabilityserviceapplypolicy"></a>Office.Manageability.Service.ApplyPolicy

Telemetria critică pentru a urmări erorile\\Succesul de la aplicarea setărilor privind politica cloud în registry. LastError spune de ce și unde nu a reușit aplicarea politicii în registry.

Se colectează următoarele câmpuri:

  - **Data.ApplyLogMsg** – mesajul de excepție, dacă este cazul, în timp ce se aplica politica

  - **Data.Cid** – identificator de corelare generat dinamic și trimis la serviciu, atunci când apelarea serviciului s-a făcut pentru a prelua politica privind mediul cloud. Utilizat pentru a corela apelul care a provocat o problemă în timp ce se aplicau politicile în cloud.

  - **Data.Last Error** – una din cinci valori șir (enumeratori) pentru a înregistra în jurnal etapa de aplicare a politicii care se executa când a avut loc excepția

#### <a name="officeonenoteandroidsyncprovisioningerror"></a>Office.OneNote.Android.Sync.ProvisioningError

Semnalul critic este utilizat pentru a garanta că, după ce un utilizator se conectează la o aplicație OneNote Android, se acordă acces în mod corespunzător la blocnotesuri, astfel încât să fie accesate cu ușurință. Aceasta se folosește pentru a asigura detectarea regresiei critice pentru aplicația OneNote și starea serviciilor.

Se colectează următoarele câmpuri:

- **AppSuspendedDuringEvent** : Returnează valoare booleană pentru a indica dacă aplicația a fost suspendată în timpul asigurării accesului

- **ErrorCode** - returnează codul de eroare responsabil pentru eșecul asigurării accesului 

- **NetworkConnection** : tipul de conectivitate de rețea a dispozitivului utilizat

- **NetworkDataExchange** - înregistrează numărul de byți schimbați în timpul asigurării accesului.

- **ServerType** : returnează tipul de server care oferă serviciul

- **TimeTakenInMilliSeconds** : returnează timpul necesar pentru a finaliza asigurarea accesului în milisecunde


#### <a name="officeonenotesystembootdialogssafebootdialogpending"></a>Office.OneNote.System.BootDialogs.SafeBootDialogPending 

Semnalizarea critică utilizată pentru a urmări când ne-am decis să afișăm utilizatorului o casetă de dialog de bootare în siguranță la următoarea bootare, deoarece am avut căderi la bootare de mai multe ori, în mod continuu. Aceasta se folosește pentru a asigura detectarea regresiei critice pentru aplicația OneNote și starea serviciilor. Dacă utilizatorii văd caseta de dialog de bootare sigură când avem o eroare critică de bootare și aceste informații ne vor ajuta să aflăm câți utilizatori se confruntă cu această problemă și câți utilizatori bootează aplicația din nou pentru a vedea de fapt caseta de dialog de bootare în siguranță, comparativ cu numărul celor care nu revin.

Se colectează următoarele câmpuri:

 - Fără

#### <a name="officeoutlookdesktopbootperfmetrics"></a>Office.Outlook.Desktop.BootPerfMetrics

Colectează timpul necesar pentru a inițializa Outlook. Timpul de inițializare Outlook este monitorizat activ pentru a detecta și a diagnostica regresiile. De asemenea, este utilizat pentru a diagnostica escaladările de la client și pentru a îmbunătăți performanța de inițializare în timp.

Se colectează următoarele câmpuri:

  - **AddinElapsedTotal** – timpul total petrecut la încărcarea programelor de completare

  - **CredPromptCount** – numărul de solicitări de acreditare afișate

  - **ElapsedTotal** – timpul total petrecut pentru inițializare

  - **IsLoggingEnabled** – înregistrarea în jurnal este activată

  - **ShowChooseProfileDlg** – dacă s-a afișat caseta de dialog Alegeți profilul

  - **ShowFirstRunDlg** – Outlook s-a lansat pentru prima dată

  - **ShowIMAPSrchfldWarningDlg** – avertismente dacă avem un cont IMAP cu un PST ANSI

  - **ShowNeedSupportDlg** – caseta de dialog de asistență declanșată de nereușita inițializării

  - **ShowSafeModeDlg** – sesiunea este deschisă în modul de siguranță

  - **ShowScanPstDlg** – mesajul de eroare afișat la verificarea reparării din depozit


#### <a name="officeoutlookmacbootperf"></a>Office.Outlook.Mac.BootPerf

Colectează timpul necesar pentru a inițializa Outlook. Timpul de inițializare Outlook este monitorizat activ pentru a detecta și a diagnostica regresiile. De asemenea, este utilizat pentru a diagnostica escaladările de la client și pentru a îmbunătăți performanța de inițializare în timp.

Se colectează următoarele câmpuri:

- **MacOLKBootPerfDuration** - timp total de încărcare

- **MacOLKBootPerfID** - identificator pentru timpul de încărcare


#### <a name="officeoutlookmacperformanceunresponsive"></a>Office.Outlook.Mac.PerformanceUnresponsive

Utilizat pentru a identifica probleme care afectează utilizatorul în Outlook și care se pot manifesta prin degradarea performanței. 

Se colectează următoarele câmpuri:

- **Duration** - perioadă cu performanța degradată

- **EventType** - tip de eveniment care se confruntă cu performanță degradată


#### <a name="officeperformanceboot"></a>Office.Performance.Boot

Colectat atunci când o aplicație Office este inițializată. Include dacă inițializarea a fost inițiată prin deschiderea unui fișier sau prin lansarea din meniul Start, dacă aceasta a fost prima inițializare a aplicației, cantitatea de memorie utilizată de aplicație și dacă a existat o interfață utilizator de blocare afișată utilizatorului. Utilizat pentru a măsura cât de repede se încarcă aplicațiile Office și cantitatea de memorie utilizată atunci când pornesc, pentru a vă asigura că există o experiență de utilizator acceptabilă.

Se colectează următoarele câmpuri:

- **ActivationKind** - dacă aplicația a fost pornită prin lansare din meniul Start, prin deschiderea unui fișier sau prin automatizare OLE.
  
- **BootToStart** - dacă utilizatorul a ales să afișeze ecranul de start când începe această aplicație.

- **ColdBoot** - dacă este prima dată când aplicația Office rulează după ce un sistem repornește sau un cod binar de aplicație trebuia să fie încărcat de pe disc.

- **DeviceModel** - Modelul de dispozitiv.

- **DocLocation** - când se deschide un document arată ce serviciu a furnizat documentul (OneDrive, server de fișiere, SharePoint etc.)

- **DurationUntilMso20Initialization** - durata în microsecunde între momentul când procesul Office a fost inițializat și mso20win32client.dll a fost încărcat.

- **Încorporarea** – dacă aplicația a fost deschisă pentru încorporarea OLE.

- **FirstBoot** – dacă aceasta a fost prima inițializare a aplicației.

- **InitializationDuration** – durata necesară în microsecunde pentru a inițializa prima dată procesul Office.

- **InterruptionMessageId** – dacă inițializarea a fost întreruptă de o casetă de dialog care solicită introducerea utilizatorului, ID-ul casetei de dialog.

- **LegacyDuration** - durata de timp pentru execuția activității, măsurată utilizând puncte de început și de sfârșit, diferite de Activity.Duration.

- **OpenAsNew** – dacă aplicația a fost pornită prin deschiderea unui document ca șablonul pentru unul nou. 

- **TotalWorkingSetMB** – volumul de memorie în megabyți din setul de lucru al procesului.

- **VirtualSetMB** – volumul de memorie în megabyți din setul virtual al procesului. (Numai MacOS/iOS)

- **WorkingSetPeakMB** – cel mai mare volum de memorie în megabyți care a fost vreodată în setul de lucru al procesului până acum.


#### <a name="officepowerpointpptandroidrehearseview"></a>Office.PowerPoint.PPT.Android.RehearseView

Acest eveniment denotă faptul că utilizatorul a oprit sesiunea de repetiție. În combinație cu Office.PowerPoint.PPT.Android.RehearseView.StartSession acesta va fi primul indicator pentru orice avarie sau eroare cu care se confruntă utilizatorul.

Se colectează următoarele câmpuri:

- **ConnectionCreationTime** - timpul necesar pentru crearea conexiunilor din partea serviciului.

- **CountDownAlertTime** – timpul în care a fost afișată alerta pentru numărătoarea inversă.

- **CountdownInitTime–** timpul între finalizarea încărcării diapozitivelor și începutul numărătorii inverse.

- **CritiqueSummary** - rezumat a ceea ce au văzut toate criticile cu numărul de utilizatori.

- **ExitEventCode** - cod pentru a identifica sub care dintre scenarii utilizatorul a ieșit din sesiunea de repetare, fie că a fost scenariul erorii, fie că a ieșit cu succes. 

- **FRETime** - timpul între începutul afișării ecranului FRE și momentul în care utilizatorul l-a dezactivat. 

- **MicrophonePermissionTime** - timpul în care a fost afișată alerta pentru permisiunea pentru microfon, până când utilizator a selectat una dintre opțiuni.

- **PauseRehearsingCount** - numărul de clicuri ale unui utilizator pe pauză de repetiție.

- **RehearsalInitTime** - timp necesar pentru ca repetiția să se inițializeze.

- **ResumeRehearsingCount** - numărul de clicuri ale unui utilizator pe reluarea repetiției.

- **Sessionid** - acesta este ID-ul sesiunii de discurs oficial. Îl putem utiliza pentru a depana jurnalele de servicii.

- **SlideshowViewLoadTime** - timpul necesar pentru încărcarea diapozitivelor.


#### <a name="officepowerpointpptandroidrehearseviewerrors"></a>Office.PowerPoint.PPT.Android.RehearseView.Errors

Eveniment declanșat atunci când apare o eroare. Acest eveniment ne va ajuta să aflăm erorile cu care s-a confruntat utilizatorul și ne vor ajuta să menținem Îndrumătorul pentru prezentatori performant pe dispozitive mobile.

Se colectează următoarele câmpuri:

- **Session id:string** - ID de sesiune de repetiție

- **RehearsalEventCode:int** - cod de eroare de repetiție


#### <a name="officepowerpointpptandroidrehearseviewrehearsalsummarypage"></a>Office.PowerPoint.PPT.Android.RehearseView.RehearsalSummaryPage 

Eveniment declanșat când se încarcă pagina rezumativă. Acest eveniment ne ajută să capturăm performanța paginii rezumative. Aceasta anunță cât timp durează încărcarea paginii de servicii de rezumat al repetițiilor pentru client. Este necesar să păstrați caracteristica performantă. 

Se colectează următoarele câmpuri:

- **PayloadCreationTime** – timpul necesar în milisecunde pentru a crea sarcina. 

- **PostUrlCallTime** – timpul necesar în milisecunde pentru a trimite apelul URL de publicare. 

- **RehearseSessionid** - acesta este ID-ul sesiunii de discurs oficial. Îl putem utiliza pentru a depana jurnalele de servicii.

- **RequestPayloadSize** – aceasta este dimensiunea sarcinii de solicitare. 

- **ResourcesLoadTime** – timpul necesar în milisecunde pentru a încărca resursele (js, css). 

- **SummaryPageErrorReceived** – aceasta este o valoare booleană care indică dacă a fost primită pagina rezumativă sau dacă a apărut o problemă.

- **SummaryPageHtmlLoadTime** – timpul necesar în milisecunde pentru a încărca summarypageHtml. 

- **SummaryPageLoadStartTime** – timpul necesar în milisecunde pentru a primi primul răspuns de la server. 

- **SummaryPageLoadTime** - timpul (în ms) necesar pentru a încărca pagina rezumativă. Printre acestea se numără timpul de creare a sarcinilor 

- **ThumbnailsCount** – acesta este numărul total de imagini reduse care vor face parte din pagina rezumativă. 

#### <a name="officepowerpointpptandroidrehearseviewstartsession"></a>Office.PowerPoint.PPT.Android.RehearseView.StartSession

Eveniment declanșat atunci când utilizatorul face clic pe pornirea sesiunii. Acest eveniment ne ajută să capturăm numărul de utilizatori care utilizează caracteristica Îndrumător pentru prezentatori pe Android. Atunci când este combinat cu Office.PowerPoint.PPT.Android.RehearseView, ne va spune câți utilizatori au finalizat cu succes sesiunea de repetiții și câți nu au reușit. Acesta este primul nostru indicator de căderi sau erori din caracteristică.
 
Se colectează următoarele câmpuri:

 - Fără

#### <a name="officepowerpointrehearsalsessionmetrics"></a>Office.PowerPoint.Rehearsal.SessionMetrics 

Eveniment declanșat atunci când sesiunea de vorbire este oprită pentru Îndrumătorul pentru prezentări. Acest eveniment ne ajută să capturăm măsurători pentru o sesiune de repetiție în Îndrumătorul pentru prezentări. Acesta va ajuta să păstrați o calitate de serviciu înaltă pentru această caracteristică.

Se colectează următoarele câmpuri:

- **ActualRehearseBootTimeInMs** – timpul real necesar pentru crearea conexiunilor.

- **AdaptationTextSize** – dimensiunea textului trimis serviciului.

- **AuthDurationInMs** - acesta este timpul necesar pentru autentificare în milisecunde (reîmprospătați simbolul de autentificare).

- **AuthError** - acesta descrie eroarea de autentificare care a avut loc (dacă există).

- **AvgFragmentLatencyInMs** - acesta este timpul mediu de revenire al mesajelor de vorbire în rețea.

- **ConnectDurationInMs** - acesta este timpul necesar în milisecunde pentru sesiunea de completare a conexiunii. 

- **FirstAudioDelayInMs** - acesta este timpul necesar în milisecunde pentru primirea primelor date audio.

- **FRetriedOnOpenConnection** – aceasta este o valoare booleeană, care indică dacă reîncercați să aibă loc pentru OpenConnection sau nu.

- **InitMediaCaptureLayerDurationInMs** – acesta este timpul necesar în milisecunde pentru a inițializa stratul de captură media/audio.

- **LocallyDroppedMessageCount** - acesta este numărul total de mesaje abandonate local.

- **NumReconnectAttemptsDuringSession** – acesta indică numărul de ori când s-a efectuat o încercare de a se reconecta la servicii de vorbire.

- **NumTriesDuringEachReconnectAttempt** – aceasta este o matrice care indică numărul de încercări efectuate în timpul încercării de reconectare.

- **OpenFrontDoorConnectionDurationInMs** - acesta este timpul necesar în milisecunde pentru a deschide conexiunea la serviciul FrontDoor.

- **SendAdaptationTextDurationInMs** - acesta este timpul necesar în milisecunde pentru a trimite textul de adaptare la serviciu.

- **ServiceDroppedMessageCount** - acesta este numărul total de mesaje abandonate de serviciu.

- **SessionDurationInMs** – aceasta este durata de timp a întregii sesiuni, de la momentul în care utilizatorul face clic pe pornire, până la momentul în care utilizatorul face clic pe oprire.

- **SessionId** - acesta este ID-ul de sesiune de discurs oficial. Îl putem utiliza pentru a depana jurnalele de servicii.

- **SpeechClientResultEventsWithTimestamps** - acesta este un șir de coduri de eroare primite împreună cu mărci de timp, care vă pot ajuta să depanați.

- **SpeechHResultsWithTimestamps** - acesta este un șir de coduri de eroare primite împreună cu mărci de timp, care vă pot ajuta să depanați.

- **StartSpeechCaptureDurationInMs** - acesta este timpul necesar în milisecunde pentru a începe capturarea vorbirii.

- **StartSpeechServiceDurationInMs** – aceasta este o matrice de timp necesar pentru a porni sesiunea de vorbire de fiecare dată când există o reconectare, inclusiv durata pornirii primei sesiuni de vorbire. 

- **TotalMessageCount** - acesta este numărul total de mesaje audio trimise la serviciu.

- **WebSocketConnectDurationInMs** - acesta este timpul necesar în milisecunde pentru a finaliza conexiunea de soclu web.


#### <a name="officeuxofficeinsidercanshowofficeinsiderslab"></a>Office.UX.OfficeInsider.CanShowOfficeInsiderSlab

Activitate prin care se urmărește dacă secțiunea Office Insider poate fi afișată utilizatorului de pe fila Cont din interfața cu utilizatorul Office Backstage.

Se colectează următoarele câmpuri:

  - **Data_CanShow** – indică dacă secțiunea Office Insider poate fi afișată utilizatorului de pe fila Cont din interfața cu utilizatorul Office Backstage.
  
  - **Data_Event** – neutilizat

  - **Data_EventInfo** – neutilizat

  - **Data_Reason** - neutilizat
 

#### <a name="officeuxofficeinsiderregistercurrentinsider"></a>Office.UX.OfficeInsider.RegisterCurrentInsider

Semnal critic pentru urmărirea succesului sau eșecului înregistrării utilizatorilor care utilizează compilări Office Insider și nu au fost înregistrați anterior ca utilizatori Office Insider. Scenariul principal aici sunt utilizatorii Office Insider actuali care s-au alăturat programului Office Insider înainte ca înregistrarea utilizatorilor Office Insider să fie adăugată.

Se colectează următoarele câmpuri:

- **Data_RegisterInsider** - starea înregistrării Office Insider

- **Data_RegisterInsiderHr** - codul rezultatului pentru înregistrarea în Office Insider

- **Data_RegistrationStateCurrent** - starea curentă a înregistrării

- **Data_RegistrationStateDesired** - starea înregistrării solicitate


#### <a name="officeuxofficeinsidershowofficeinsiderdlg"></a>Office.UX.OfficeInsider.ShowOfficeInsiderDlg

Semnal critic care urmărește interacțiunea utilizatorului cu caseta de dialog Asociați-vă la Office Insider. Este utilizat pentru a identifica problemele cu efectuarea modificărilor inițiate de utilizator, precum asocierea la/părăsirea programului Office Insider și modificarea nivelului Office Insider.

Se colectează următoarele câmpuri:

- **Data_AcceptedContactMeNew** - indică dacă un utilizator a acceptat să fie contactat de către Microsoft pentru aderarea la programul Office Insider

- **Data_InsiderLevel** - nivelul Insider la deschiderea casetei de dialog „Alăturați-vă programului Office Insider”

- **Data_InsiderLevelNew** - nivelul Insider la închiderea casetei de dialog „Alăturați-vă programului Office Insider”

- **Data_IsInternalUser** - indică dacă aplicația se execută sub acreditările unui cont Microsoft corporativ.

- **Data_IsInternalUserInit** - indică dacă codul ar putea determina dacă aplicația se execută sub acreditările unui cont Microsoft corporativ.

- **Data_OpenNewsletterWebpage** - indică dacă link-ul de abonare la buletinul informativ Office Insider a fost declanșat cu condiția ca utilizatorul să se fi alăturat programului Office Insider, caracteristica de abonare la buletinul informativ este activată, iar utilizatorul nu a anulat deschiderea paginii web de abonare la buletinul informativ Office Insider.
    
- **Data_RegisterInsider** - starea înregistrării Office Insider

- **Data_RegisterInsiderHr** - codul rezultatului pentru înregistrarea în Office Insider

- **Data_RegistrationStateCurrent** - starea curentă a înregistrării

- **Data_RegistrationStateDesired** - starea înregistrării solicitate


#### <a name="officevisiosharedvisiofilerender"></a>Office.Visio.Shared.VisioFileRender

Acest eveniment capturează timpul de redare a fișierului. Acest eveniment ne ajută să controlăm performanța de redare a fișierelor.

Se colectează următoarele câmpuri:

  - **Data\_AvgTime: integer** – timpul mediu necesar pentru a reda desenul Visio într-o sesiune

  - **Data\_CompositeSurfEnabled: bool** – true dacă modul de redare compusă este activat

  - **Data\_Count: integer** – numărul de situații în care Visio redă desenul într-o sesiune

  - **Data\_FirstRenderTime: long** – durata de redare a fișierului la prima lansare, în milisecunde

  - **Data\_MaxTime: integer** – timpul maxim necesar pentru a reda desenul Visio într-o sesiune


#### <a name="officevisiovisiofileopenreliability"></a>Office.Visio.VisioFileOpenReliability

Acest eveniment colectează date privind performanța de deschidere a fișierelor pentru Visio Dev16. Acest eveniment este utilizat pentru a monitoriza performanța la deschiderea fișierelor și o asociază cu proprietăți de fișier, cum ar fi dimensiunea pentru Visio Dev16. Proprietățile fișierelor ne permit să depanăm și să stabilim mai rapid cauza problemelor.

Se colectează următoarele câmpuri:

  - **Data\_CorrelationId: string –** identificatorul de corelare al documentelor

  - **Data\_DocIsEnterpriseProtected: bool –** true dacă documentul este protejat folosind protecția informațiilor Windows

  - **Data\_DocumentId: string –** GUID pentru calea fișierelor

  - **Data\_DurationToCompleteInMilliseconds: double –** durata de finalizare a salvării în milisecunde

  - **Data\_DurationToCompleteInMillisecondsSquared: double –** valoarea pătrată pentru DurationToCompleteInMilliseconds

  - **Data\_ErrorCode: integer –** codul de eroare internă pentru nereușita deschiderii unui fișier

  - **Data\_Extension\_Docs: string –** extensia de fișier a diagramei deschise

  - **Data\_FileIOBytesRead: int –** numărul total de byți citiți la salvare

  - **Data\_FileIOBytesReadSquared: int –** valoarea pătrată pentru Data\_FileIOBytesRead

  - **Data\_FileIOBytesWritten: int –** numărul total de byți scriși la salvare

  - **Data\_FileIOBytesWrittenSquared: int –** valoarea pătrată pentru Data\_FileIOBytesWritten

  - **Data\_FilePathHash: binary** – codul hash binar al numelui fișierului

  - **Data\_FileOpenDownloadDurationInMs: long –** durata de deschidere a fișierului în milisecunde

  - **Data\_FileOpenEndDurationInMs: long: –** durata de deschidere a fișierului în milisecunde

  - **Data\_FileOpenTimeStamp: time: –** marca de timp de când a început să se deschidă fișierul

  - **Data\_FilePathHash: binary –** GUID pentru calea fișierului

  - **Data\_FileSize: long –** dimensiunea documentului în byți

  - **Data\_FileType: string –** extensia de fișier a diagramei deschise

  - **Data\_IsInternalFile: bool –** true dacă fișierul este intern. ex. tipar

  - **Data\_IsIRM: bool –** true dacă fișierul este protejat prin Information Right

  - **Data\_IsReadOnly: bool –** true dacă fișierul este doar în citire

  - **Data\_IsSuccess: bool –** true când deschiderea fișierului a reușit

  - **Data\_Location: string –** locația fișierului, de exemplu Local, SharePoint, OneDrive, WopiConsumer, WopiBusiness, GenericThirdPartyConsumer

  - **Data\_NetworkIOBytesRead: int –** numărul total de byți de rețea citiți la salvare

  - **Data\_NetworkIOBytesReadSquared: int –** valoarea pătrată pentru Data\_NetworkIOBytesRead

  - **Data\_NetworkIOBytesWritten: int –** numărul total de byți din rețea scriși la salvare

  - **Data\_NetworkIOBytesWrittenSquared: int –** valoarea pătrată pentru NetworkIOBytesWritten

  - **Data\_OpenLocation: integer –** locația din care s-a deschis fișierul 0 , Local, 1, Rețea, 2, SharePoint, 3 – Web

  - **Data\_Size\_Docs: integer –** dimensiunea documentului în byți

  - **Data\_Tag: string –** identificatorul unic pentru evenimentul Salvare ca

  - **Data\_WasSuccessful: bool –** true dacă deschiderea a reușit


#### <a name="onenoteappsafebootdialogactiontaken-officeonenoteandroidsafebootdialogactiontaken-officeandroidearlytelemetrysafebootdialogactiontaken"></a>OneNote.App.SafeBootDialogActionTaken, Office.OneNote.Android.SafeBootDialogActionTaken, Office.Android.EarlyTelemetry.SafeBootDialogActionTaken

Semnalizarea critică utilizată pentru a urmări răspunsul utilizatorului când vede o casetă de dialog de bootare în siguranță. Caseta de dialog de bootare în siguranță este afișată atunci când nu am reușit să lansăm în mod repetat. Opțiunea utilizatorului pentru bootare în siguranță este utilizată ca permisiune pentru a șterge datele de aplicație pentru reuși lansarea. Aceasta se folosește pentru a asigura detectarea regresiei critice pentru aplicația OneNote și starea serviciilor. Utilizatorul vede când întâmpină o eroare critică de blocare a bootării. Aceste informații vor ajuta să urmăriți dacă a fost rezolvată cauza blocării și dacă utilizatorul poate sau nu lansa aplicația cu succes.

Se colectează următoarele câmpuri: 

- **DIALOG_ACTION** - pe ce buton al casetei de dialog a făcut clic utilizatorul: butonul Pozitiv sau butonul Negativ


#### <a name="onenotesyncprovisioningcompleted-previous-name-officeonenoteandroidsyncprovisioningcompleted"></a>OneNote.Sync.ProvisioningCompleted *(nume anterior)* , Office.OneNote.Android.Sync.ProvisioningCompleted

Semnalul critic este utilizat pentru a garanta că, după ce un utilizator se conectează la o aplicație OneNote Android, se acordă acces în mod corespunzător la blocnotesuri, astfel încât să fie accesate cu ușurință. Aceasta se folosește pentru a asigura detectarea regresiei critice pentru aplicația OneNote și starea serviciilor

Se colectează următoarele câmpuri: 

- **AppSuspendedDuringEvent** - Returnează valoare booleană pentru a indica dacă aplicația a fost suspendată în timpul acordării accesului

- **NetworkConnection** - tipul de conectivitate de rețea a dispozitivului utilizat

- **NetworkDataExchange** - înregistrează numărul de octeți schimbați în timpul acordării accesului.

- **ServerType** - returnează tipul de server care oferă serviciul

- **TimeTakenInMilliSeconds** - returnează timpul necesar pentru a finaliza asigurarea accesului în milisecunde

#### <a name="onenotesyncprovisioningstarted-previous-name-officeonenoteandroidsyncprovisioningstarted"></a>OneNote.Sync.ProvisioningStarted *(nume anterior)* , Office.OneNote.Android.Sync.ProvisioningStarted

Semnalul critic este utilizat pentru a garanta că, după ce un utilizator se conectează la o aplicație OneNote Android, se acordă în mod corespunzător acces la blocnotesuri, astfel încât să fie accesate cu succes.  Aceasta se folosește pentru a asigura detectarea regresiei critice pentru aplicația OneNote și starea serviciilor

Se colectează următoarele câmpuri: 

- **NetworkConnection** - tipul de conectivitate de rețea a dispozitivului utilizat

- **ServerType** - returnează tipul de server care oferă serviciul

#### <a name="perfevent"></a>perf.event

Este utilizat pentru a monitoriza posibilul impact negativ asupra performanței de încărcare a diferitelor părți ale aplicației, de ex. pentru a vă asigura că, atunci când deschideți pentru prima dată aplicația, inboxul se încarcă rapid.

Se colectează următoarele câmpuri: 

- **app_start_show_message_list** - aceasta înseamnă că a fost o problemă de performanță la pornirea aplicației ceea ce face ca lista de mesaje din inbox să aibă nevoie de mai mult timp pentru a se încărca

- **event_type** - ne spune tipul de eveniment de performanță care a cauzat o problemă de performanță, pentru a ne ajuta să detectăm probleme care au legătură cu un anumit tip.   

- **extra_params** - un dezvoltator poate adăuga parametri suplimentari aici pentru a ne oferi mai multe detalii despre ceea ce ar putea cauza această problemă de performanță, de exemplu, atunci când această acțiune s-a produs și s-a încheiat etc. 

- **profiling_summary** - furnizează informații despre grupul de activități, numărul de activități și timpul mediu pentru acele grupuri, pentru a ajuta la înțelegerea regresiilor potențiale din anumite zone atunci când se încarcă aplicația

- **total_time_elapsed** - ne spune cât timp a durat evenimentul de performanță pentru a ne ajuta să înțelegem gravitatea problemei de performanță

#### <a name="performancerecord"></a>performance.record

Acest eveniment colectează măsurătorile de performanță ale aplicației. Acesta ne permite să detectăm și să remediem situații în care utilizarea memoriei de aplicație și utilizarea CPU devin extrem de ridicate sau au alte probleme de performanță care pot determina încetinirea dispozitivului.

Se colectează următoarele câmpuri: 

- **app_exit_metric** - ne spune măsurătorile despre contorizări de diverse tipuri de performanță pentru ieșirile din aplicații în prim-plan și din cele în fundal, pentru a ne ajuta să înțelegem ieșirile din aplicație în mod neașteptat cu motive de performanță negativă.

- **average_suspended_memory** - ne spune volumul mediu de memorie utilizată de către aplicație atunci când este suspendată, pentru a avea un termen de comparație și pentru a ne ajuta să înțelegem impactul de performanță negativ.

- **category** - ne spune dacă aplicația se află în prim plan sau în fundal în acel moment. Posibilele valori includ prim plan și fundal.

- **cpu_usage** - ne spune cât CPU a fost utilizat de aplicație astfel încât să avem un termen de comparație, pentru a ne ajuta să înțelegem impactul de performanță negativ

- **cumulative_CPU_time** - ne spune volumul total de CPU utilizat de către aplicație cu măsurarea duratei de timp, pentru a avea un termen de comparație și pentru a ne ajuta să înțelegem impactul de performanță negativ.

- **cumulative_GPU_time** - ne spune volumul total de GPU utilizat de către aplicație pentru a avea un termen de comparație și pentru a ne ajuta să înțelegem impactul negativ al duratei de viață a bateriei.

- **is_watch_app_installed** - ne spune dacă utilizatorul utilizează în prezent un Apple Watch și dacă este instalat, pentru a ne ajuta să înțelegem impactul negativ asupra performanței cauzat de Watch

- **is_watch_paired** - ne spune dacă utilizatorul utilizează în prezent un Apple Watch și dacă este asociat cu dispozitivul pentru a ne ajuta să înțelegem impactul negativ asupra performanței cauzat de Watch

- **is_watch_supported_and_active** - ne spune dacă utilizatorul utilizează în prezent un Apple Watch și dacă este activ pentru a ne ajuta să înțelegem impactul negativ asupra performanței cauzat de Watch

- **memoAry_used_percentage** - ne spune ce procent din memorie a fost utilizat de aplicație, pentru a avea un termen de comparație și pentru a ne ajuta să înțelegem impactul negativ asupra performanței

- **memory_used** - ne spune câtă memorie a fost utilizată de aplicație pentru a avea un termen de comparație și pentru a ne ajuta să înțelegem impactul de performanță negativ

- **peak_memory_usage** - ne spune cel mai mare volum de memorie utilizată de către aplicație pentru a avea un termen de comparație și pentru a ne ajuta să înțelegem impactul de performanță negativ.

- **scroll_hitch_time_ratio** - ne spune raportul timpului petrecut conectându-vă în timp ce defilați pe interfața utilizatorului, pentru a ne ajuta să înțelegem impactul negativ asupra performanței interfeței utilizatorului.


### <a name="application-activity-error-subtype"></a>*Subtipul de eroare de activitate a aplicației*

Erorile în funcționalitatea unei caracteristici sau a unei experiențe de utilizator.

#### <a name="assertion"></a>assertion

Acest eveniment ne permite să detectăm când s-au produs erori critice ale aplicațiilor, care ar putea duce la căderea aplicației dvs. sau la probleme serioase, cum ar fi vizualizarea unor rânduri goale în inboxul dvs.

Se colectează următoarele câmpuri:

- **count** - numărul total de elemente asociate erorii; de exemplu, numărul de calendare care au erori

- **has_hx** - ne spune că acest cont folosește noul nostru serviciu de sincronizare, pentru a ne ajuta să detectăm problemele provocate de serviciul nostru de sincronizare

- **host_name** - numele gazdei serviciului care a fost implicată în eroare, pentru a ne ajuta să detectăm probleme legate de o anumită gazdă

- **host_type** - tipul de gazdă implicată în eroare, pentru a ne ajuta să detectăm probleme legate de un anumit tip de gazdă

- **message** - mesaj particularizat pentru afirmația utilizată pentru diagnosticarea problemei 

- **origin** - originea erorii din cod pentru a ne ajuta să detectăm probleme legate de o anumită parte a codului

- **stacktrace** - trasarea stivei în care a apărut afirmația pentru a ne ajuta să detectăm probleme legate de o anumită parte a codului

- **type** - tipul de eroare pentru afirmație care a apărut, de ex. null_folder_name, compose_selected_null_account, pentru a ne ajuta să detectăm probleme legate de o anumită parte a codului

#### <a name="editcontacterror"></a>edit.contact.error

Ne permite să detectăm și să remediem situațiile în care s-au produs erori atunci când ați încercat să vizualizați sau să editați persoanele de contact prin intermediul aplicației.

Se colectează următoarele câmpuri: 

- **errorType** - tipul de eroare care a avut loc pentru a ne ajuta să diagnosticăm problema

- **field** - câmpul de persoane de contact pe care utilizatorul a încercat să-l editeze pentru a ne ajuta să diagnosticăm problema

- **version** - versiunea serviciului de cărți de vizită pe care îl utilizăm pentru a ne ajuta să diagnosticăm problema

#### <a name="errorreport"></a>error.report

Acest eveniment ne permite să detectăm unde s-au produs erorile critice ale aplicației astfel încât să putem preveni problemele care ar putea determina căderea aplicației sau care ar putea să vă împiedice să citiți e-mailurile. 

Se colectează următoarele câmpuri: 

- **client-request-id** - identificator solicitare client pentru solicitarea care a cauzat eroarea
 
- **date** - marca de dată a solicitării care a cauzat eroarea

- **error** - tipul de eroare, de ex., get_mailbox_location_failed
 
- **error_body** - corpul mesajului de eroare
 
- **is_x_mailbox_anchor_set** - dacă s-a setat proprietatea X-AnchorMailbox la solicitare
 
- **reason** - motivul erorii, de ex. un mesaj de eroare
 
- **request-id** - identificator solicitare server pentru solicitarea care a determinat eroarea
 
- **source** - sursa erorii din infrastructura OM, de obicei, una dintre „BE” sau „FE”


#### <a name="officeairspacebackendwin32graphicsdriversofthang"></a>Office.AirSpace.Backend.Win32.GraphicsDriverSoftHang 

Ajută Microsoft să separe blocările lungi ale driverului de placă video de cele scurte, pentru a lua decizii despre driverele de placă video care pot avea probleme. Driverul de placă video al utilizatorului a făcut Office să se blocheze, dar impactul blocării nu este cunoscut încă

Se colectează următoarele câmpuri:

  - **Data\_InDeviceCall** – metoda apelată pe placa video care a produs blocarea

  - **Data\_Timeout** – cât a durat blocarea

  #### <a name="officeandroidadalsigninuiprompts"></a>Office.Android.ADALSignInUIPrompts

Acest eveniment indică faptul că solicitarea de conectare a fost livrată utilizatorului, pentru contul de la școală sau de la locul de muncă.  Acest eveniment vă ajută să înțelegeți starea de funcționare a aplicațiilor noastre și să luați măsurile corespunzătoare, atunci când observăm solicitările de conectare neașteptate. 

Se colectează următoarele câmpuri:

- **LastLoginDelta** - delta timp de la ultima logare reușită

- **PreviousIdentityCredProviderState** - indică starea contului.

- **PreviousIdentityState** - indică starea contului, dacă sesiunea a expirat. 

- **SignInResultCode** - indică codul rezultat al solicitării de la sfârșitul conectării.

- **UseCache** - indică dacă am forțat să-i solicităm utilizatorului să furnizeze din nou parola.

- **UserType** - indică dacă acesta este cont este nou sau nu

#### <a name="officeandroidandroidappdocsfileoperationends"></a>Office.Android.AndroidAppDocsFileOperationEnds

Documente critice doar pentru Android (AppDocs) date de telemetrie pentru fișiere Nou/Deschide/Salvare ca. Acesta captează codurile de eroare pentru erorile din aceste AppDocsOperations.  Microsoft îl utilizează pentru a identifica erorile din diverse operațiuni cu fișiere și stratul exact la care s-a produs eroarea în Word, Excel sau PowerPoint.

Se colectează următoarele câmpuri:

- **AccessMode** - valoare de enumerare pentru modul de acces pentru fișier. Values- None, ReadOnly, ReadOnlyUpgradable, ReadWrite

- **BlockingUIShown** - Boolean pentru a indica dacă blocarea UI a fost afișată în flux de oriunde.

- **ContentUriAuthority** - autoritatea URL de conținut de la SAF

- **Corelarea** - GUID pentru ID-ul de corespondență corelat cu operațiunea

- **DocId** - ID-ul de document generat de AppDocs

- **DocInstanceId** - DocInstanceId ID-ul de instanță din document generat de AppDocs, care este definit într-o instanță de operațiune dintr-un document

- **DocIsEnterpriseProtected** - Boolean pentru a indica dacă documentul este protejat.

- **DocUserId** - ID-ul de utilizator din stratul MS de autentificare

- **DocUserIdProvider** - enumerare care reprezintă furnizorul ID utilizatorului, 0 = Necunoscut, 1 = LiveID, 2 = OrgId, 3 = SSPI, 4 = ADAL

- **DurationInMs** - timp în milisecundă pentru ca operațiunea de fișier să se termine

- **EndReason** - valoare de enumerare pentru motivul final.  Valori-fără, reușită, eșec, anulare

- **ErrorCode** - cod de eroare pentru operațiunea de fișier

- **Extensia** - extinderea fișierului deschis.

- **FileSourceLocation** - valoare de enumerare pentru locația fișierului. Valori posibile: niciunul, local, UncOrMappedNetworkDrive, SkyDrive, App, Microsoft Office SharePoint Online, UnknownServer

- **FILETIME** - ora evenimentului

- **FirstBCSClientError_Info** - informații despre codul de eroare corelat cu conversiile fișierelor

- **HttpStatusCode** - cod de răspuns HTTP pentru solicitarea de servicii web

- **InitalizationReason** - punct de intrare pentru deschiderea fișierului

- **K2FileIOHresult** - cod HRESULT pentru terminarea operațiunii de deschidere a fișierului

- **LastBCSClientError_TagId** - ultima eroare de client BCS (serviciul de conversie binară)

- **OfficeWebServiceApiStatusFlag** - semnalizarea de stare pentru solicitarea serviciului Web

- **OpEndEventId** - etichetă care reprezintă locul în care operațiunea s-a încheiat efectiv

- **OpFlags** - operațiunea de document semnalizările de param utilizate de stratul AppDocs.

- **OpSeqNum** - un număr care reprezintă succedarea apelurilor legate de operațiunea de fișier din stratul AppDocs

- **OpType** - enumerare tip operațiune. Valori: "fără", "CreateDocument", "OpenDocument", "CopyDocument", "CloseDocument", "SaveDocument", "OpenVersion", "CloseVersion"

- **PreFetchState** - enumerarea pentru preîncărcare stare de șabloane pentru noile operațiuni de creare a fișierelor.

- **ProviderApp** - nume pachet pentru aplicația din care se deschide fișierul

- **ScopeInstanceId** - ID instanță în domeniu utilizat pentru asocierea contextului de date la activități

- **Size** - dimensiune fișier

- **State** - valoare de enumerare pentru starea fișierului. Valori: fără, Creare, creat, CreateFailed, deschidere, deschis, OpenFailed, copiere, copiat, CopyFailed, închidere, închis, CloseFail

- **TemplateName** - numele șablonului binar al șablonului de document din serviciul de șabloane, de exemplu, TF10002009. dotx

- **UriScheme** - schema URL

#### <a name="officeandroidandroidautherror"></a>Office. Android. AndroidAuthError

Acest eveniment denotă erorile de autentificare de bază în timpul reîmprospătării simbolurilor neasistate, încărcarea paginii de conectare din serviciu etc.  Acest eveniment vă ajută să înțelegeți starea de funcționare a conectărilor în aplicațiile noastre, conectările efectuate și să luați măsurile corespunzătoare, atunci când observăm solicitările de conectare neașteptate. 

Se colectează următoarele câmpuri:

- **ADALErrorCode** - indică codul de eroare în timp ce afișează solicitarea de conectare sau încercarea de preluare a simbolului silențios pentru a vă conecta la contul de la locul de muncă.

- **ADALRawErrorCode** - indică codul de eroare simplu în timp ce afișează solicitarea de conectare sau încercarea de preluare a simbolului silențios pentru a vă conecta la contul de la locul de muncă.

- **ErrorGroup** - indică tipul de cont, cum ar fi contul personal sau contul de la locul de muncă sau contul local de la locul de muncă.

- **IDCRLErrorCode** - indică codul de eroare în timp ce afișează solicitarea de conectare pentru contul personal.

- **IDCRLRawErrorCode** - indică codul de eroare simplu în timp ce afișează solicitarea de conectare pentru contul personal.

- **LiveOAuthErrorCode** - indică codul de eroare în timpul încercării de reîmprospătare a simbolului silențios pentru contul personal.

- **LiveOAuthRawErrorCode** - indică codul de eroare simplu în timpul încercării de reîmprospătare a simbolului silențios pentru contul personal.

- **NTLMErrorCode** - indică codul de eroare în timp ce afișează solicitarea de conectare pentru contul personal local.

#### <a name="officeandroidandroidfileasyncsavestatus"></a>Office.Android.AndroidFileAsyncSaveStatus

Capturi de salvare a datelor de stare din fișierul asincron și diverse coduri de eroare din componente diferite.  Microsoft utilizează aceste date pentru a analiza dacă există vreo pierdere de date de utilizator în aplicație în timpul salvării fișierelor din Word, Excel sau PowerPoint.

Se colectează următoarele câmpuri:

- **FileExtension** - extensie de fișier

- **FileIOSaveHResult** - HResult pentru operațiunea salvare fișier

- **FileIOSaveIsCopy** - Boolean pentru a indica dacă operațiunea salvează o copie.

- **FileSize** - dimensiunea fișierului

- **FileSourceLocation** - enumerare pentru locația sursei fișierului. Valori: niciunul, local, UncOrMappedNetworkDrive, SkyDrive, App, Microsoft Office SharePoint Online, UnknownServer

#### <a name="officeandroidandroidfileopenreliability"></a>Office.Android.AndroidFileOpenReliability

Acesta captează date de stare deschise pentru fișiere și diverse coduri de eroare pentru a identifica ce erori de deschidere a fișierului sunt așteptate comparativ cu cele neașteptate și care parte din cod le raportează.  Microsoft utilizează aceste date pentru a analiza motivele pentru erori de deschidere a fișierelor și pentru a calcula o rată critică de succes de deschidere a fișierului în Word, Excel sau PowerPoint.

Se colectează următoarele câmpuri:

- **AccessMode** - enumerarea modului de acces

- **AppDocsFileOpenErrorCode** - cod de eroare din AppDocs pentru deschiderea fișierului nereușită

- **ContentUriAuthority** - autoritatea URL-ului de conținut de la SAF

- **DownloadCsiError** - mesajul de eroare de descărcare de la CSI

- **FileExtension** - extensie de fișier

- **FileOpenEndErrorCode** - cod de eroare pentru nereușita deschiderii fișierului 

- **FileOpenStatus** - enumerare stare deschidere fișier

- **FileSize** - dimensiune fișier

- **FileSourceLocation** - enumerare pentru locația fișierului

- **FirstBCSClientError_Info** - ultima eroare a clientului BCS (serviciul de conversie binară)

- **IfWordFileOpenCancelled** - dacă fișierul deschis a fost anulat de utilizator în Word

- **InitializationReason** - enumerare pentru punctul de intrare pentru fișierul deschis

- **IsAutoSaveDisabled** - salvarea automată este dezactivată în timpul deschiderii fișierelor

- **IsFileEmpty** - Boolean pentru a indica dacă fișierul este gol

- **K2FileIOHresult** - HRESULT pentru încheierea operațiunii fișierului

- **OpenCsiError** - mesaj de eroare pentru deschiderea fișierului în stratul CSI

- **OpEndEventId** - etichetă care reprezintă locul în care operațiunea s-a încheiat

- **PPTHresult** -Hresult în PPT

- **PPTIsExpectedError** - clasificarea erorilor în PPT pentru eroarea așteptată/neașteptată la deschiderea fișierului  

- **PPTTag** -eticheta de eroare din PPT

- **ProviderApp** - nume pachet pentru aplicația din care se deschide fișierul

- **ProviderFileSize** - mărime fișier capturată în timp ce deschideți fișierul prin activarea fișierelor

- **State** - enumerare de stare deschidere fișier

- **UriScheme** - schema URL-ului

- **WordErrortag** - eticheta de eroare din Word

- **WordFileCorruptionReason** - motivul pentru corupție din cauza căruia fișierul Word poate să nu reușească la deschidere

- **WordFileOpenErrorCode** - cod de eroare la deschiderea fișierului specific Word-ului.

- **WordFileTypeFromDod** - tip de fișier determinat de Word pe baza formatului de fișier actual

- **WordFileTypeFromExtension** - tip de fișier determinat de Word bazat pe extinderea formatului

#### <a name="officeandroidandroidfilesavestatus"></a>Office.Android.AndroidFileSaveStatus

Critic pentru capturarea salvării fișierului cu datele de stare și diverse coduri de eroare din componente diferite.  Microsoft utilizează aceste date pentru a analiza dacă există vreo pierdere de date de utilizator în aplicație în timpul salvării fișierelor din Word, Excel sau PowerPoint.

Se colectează următoarele câmpuri:

- **AccessMode** - Valori**- niciuna, ReadOnly, ReadOnlyUpgradable, ReadWrite

- **AppDocsEndReason** - enumerare pentru fișierul Salvați AppdocEndReason.  Valori: fără, reușită, eșec, anulare

- **AppDocsErrorCode** - cod de eroare final pentru nereușita salvării fișierului

- **AppDocsTriggeringSaveDetails** - câmp pentru a indica dacă AppDocs declanșează salvarea

- **DocInstanceId** - DocInstanceId ID-ul de instanță din document generat de AppDocs, care este definit într-o instanță de operațiune dintr-un document

- **ExcelFileSaveResult** - HResult specific pentru Excel

- **FileExtension** - extindere fișier.

- **FileIOSaveErrorCode** - cod de eroare din FileIO

- **FileIOSaveHResult** - Hresult din FileIO

- **FileIOSaveIsCopy** - Boolean pentru a indica dacă operațiunea de copiere

- **FileSize** - dimensiune fișier

- **FileSourceLocation** - enumerare a locației fișierului  Valori: niciunul, local, UncOrMappedNetworkDrive, SkyDrive, App, Microsoft Office SharePoint Online, UnknownServer

- **OpFlags** -semnalizări de operațiune pentru salvare

- **PPTFileSaveFailHresult** - PPT Hresult pentru salvarea erorii

- **PPTFileSaveFailTag** - eticheta PPT pentru salvarea erorii

- **State** - enumerare de stare a deschiderii fișierului 

- **Values** : fără, Creare, creat, CreateFailed, deschidere, deschis, OpenFailed, copiere, copiat, CopyFailed, închidere, închis, CloseFail

- **WordFileCopyErrorTrackbackTag** - eticheta urmărire pentru eșec este etapa CopyDocument în Word

- **WordFileSaveCancelReason** -eticheta urmărire pentru anulările din Word

- **WordFileSaveEid** - cod de eroare specific pentru Word

- **WordFileSaveErrorTrackbackTag** - eticheta urmărire pentru salvarea erorilor

- **WordFileSaveOpResult** - enumerare pentru starea rezultatelor 0 dacă s-a reușit, 1 dacă nu a reușit, 2 dacă a fost anulat

- **WordFileSaveSuccess** - enumerare pentru detalii specifice Word pentru succesul operațiunii salvare fișier.

#### <a name="officeandroidandroidofficeactivationlatency"></a>Office. Android.AndroidOfficeActivationLatency

Date critice pentru a colecta timp de deschidere a fișierului final pentru tot fișierul se deschide în aplicațiile Windows, Excel, PowerPoint.  Acest lucru este utilizat de Microsoft pentru a afla măsurătoarea pentru deschiderea fișierului pentru performanța aplicațiilor noastre

Se colectează următoarele câmpuri:

- **AppBootingOccured** - Boolean pentru a verifica dacă s-a finalizat încărcarea aplicațiilor

- **ApplicationBootTime** - timpul necesar unei anumite faze de încărcare a aplicațiilor

- **AppSuspendedDuringBoot** - Boolean pentru a verifica dacă aplicația a fost suspendată în timpul încărcării

- **BlockingUIShownDuringFileOpen** - Boolean pentru a indica dacă există o casetă de dialog de blocare în timpul operațiunii deschidere fișier

- **CachedInfoAvailable** - Boolean pentru a căuta informații memorate în cache specifice operațiunii deschidere fișier

- **DocumentRecoveryInvoked** - Boolean pentru a indica dacă un document a fost recuperat

- **EndToEndActivationTime** - timp necesar pentru a reda fișierul pentru fișierele deschise din afara aplicației

- **EndToEndFileOpenTime** - timp necesar pentru a reda fișierul pentru fișierele deschise din afara aplicației

- **FileOpenPhaseDurationInMs** - timpul operațiunii de deschidere a fișierului consumat de anumite faze

- **FileSourceLocation** - valoare de enumerare pentru locația fișierelor, precum: niciunul, local, UncOrMappedNetworkDrive, SkyDrive, App, Microsoft Office SharePoint Online, UnknownServer

- **InitalizationReason** - punct de intrare pentru deschiderea fișierului

- **InitialBootPhaseTime** - timpul necesar unei anumite faze de încărcare a aplicațiilor

- **IsThisFirstLaunch** - Boolean pentru a indica dacă se lansează aplicația prima dată

- **MinimumLibraryLoadPhaseTime** - timpul necesar unei anumite faze de încărcare a aplicațiilor

- **MinimumLibraryLoadPhaseTime** - timpul necesar unei anumite faze de încărcare a aplicațiilor

- **MinimumLibraryLoadPhaseTime** - timpul necesar unei anumite faze de încărcare a aplicațiilor

- **PostAppInitTimeInMs** - timpul necesar unei anumite faze de încărcare a aplicațiilor

- **PPTRenderPhase** - oră corelată cu anumite faze din randarea PPT

- **PreAppInitTimeInMs** - timpul necesar unei anumite faze de încărcare a aplicațiilor

- **ProviderApp** - nume pachet pentru aplicația din care se deschide fișierul

- **TelemetryReason** - similară cu InitialisationReason, dar valoare de enumerare mai detaliată a punctului de intrare pentru fișierul deschis.

- **UserDialogInterruptionDuringBoot** - Boolean pentru a indica dacă a existat vreun dialog care blochează în timpul încălcării

- **XLRenderPhase** - ora corelată cu anumite faze din randarea Excel

#### <a name="officeandroidappdocsfileoperationends"></a>Office. Android. AppDocsFileOperationEnds

Documente critice doar pentru Android (AppDocs) date de telemetrie pentru fișiere Nou/Deschide/Salvare ca. Acesta captează codurile de eroare pentru erorile din aceste AppDocsOperations.  Microsoft îl utilizează pentru a identifica erorile din diverse operațiuni cu fișiere și stratul exact la care s-a produs eroarea în Word, Excel sau PowerPoint.

Se colectează următoarele câmpuri:

- **AccessMode** - valoare de enumerare pentru modul de acces pentru fișier.  Values- niciuna, ReadOnly, ReadOnlyUpgradable, ReadWrite

- **BlockingUIShown** - Boolean pentru a indica dacă blocarea UI a fost afișată în flux de oriunde.

- **ContentUriAuthority** - autoritatea URL de conținut de la SAF

- **Correlation** - GUID pentru ID-ul de corespondență corelat cu operațiunea

- **DocId** - ID-ul documentului generat de AppDocs

- **DocInstanceId** - DocInstanceId ID-ul de instanță din document generat de AppDocs, care este definit într-o instanță de operațiune dintr-un document

- **DocIsEnterpriseProtected** - Boolean pentru a indica dacă documentul este protejat.

- **DocUserId** - ID-ul de utilizator din stratul MS de autentificare

- **DocUserIdProvider** - enumerare care reprezintă furnizorul ID-ului de utilizator, 0 = Necunoscut, 1 = LiveID, 2 = OrgId, 3 = SSPI, 4 = ADAL

- **DurationInMs** - timp în milisecundă pentru ca operațiunea de fișier să se încheie

- **EndReason** - valoare de enumerare pentru motivul final.  Valori: fără, reușită, eroare, anulare

- **ErrorCode** - cod de eroare pentru operațiunea de fișier

- **Extinderea** - primele patru caractere din extinderea fișierului în curs de deschidere.

- **FileSourceLocation** - valoare de enumerare pentru locația fișierului. Valori posibile: niciunul, local, UncOrMappedNetworkDrive, SkyDrive, App, Microsoft Office SharePoint Online, UnknownServer

- **FILETIME** - ora evenimentului

- **FirstBCSClientError_Info** - informații despre codul de eroare corelat cu conversiile fișierelor

- **HttpStatusCode** - cod de răspuns HTTP pentru solicitarea de servicii Web

- **InitalizationReason** - punct de intrare pentru deschiderea fișierului

- **K2FileIOHresult** - cod HRESULT pentru terminarea operațiunii de deschidere a fișierului

- **LastBCSClientError_TagId** - ultima eroare de client BCS (serviciul de conversie binară)

- **OfficeWebServiceApiStatusFlag** - semnalizarea de stare pentru solicitarea serviciului Web

- **OpEndEventId** - etichetă care reprezintă locul în care operațiunea s-a încheiat efectiv

- **OpFlags** - operațiunea de document semnalizările de param utilizate de stratul AppDocs.

- **OpSeqNum** - un număr care reprezintă succedarea apelurilor legate de operațiunea de fișier din stratul AppDocs

- **OpType** - enumerare tip operațiune. Valori: "fără", "CreateDocument", "OpenDocument", "CopyDocument", "CloseDocument", "SaveDocument", "OpenVersion", "CloseVersion"

- **PreFetchState** - enumerarea pentru preîncărcare stare de șabloane pentru noile operațiuni de creare a fișierelor.

- **ProviderApp** - nume pachet pentru aplicația din care se deschide fișierul

- **ScopeInstanceId** - ID instanță în domeniu utilizat pentru asocierea contextului de date la activități

- **Size** - dimensiune fișier

- **State** - valoare de enumerare pentru starea fișierului. Valori: fără, Creare, creat, CreateFailed, deschidere, deschis, OpenFailed, copiere, copiat, CopyFailed, închidere, închis, CloseFail

- **TemplateName** - numele șablonului binar al șablonului de document din serviciul de șabloane, de exemplu, TF10002009. dotx

- **UriScheme** - schema URL

#### <a name="officeandroidauthaceerrors"></a>Office.Android.AuthACEErrors

Acest eveniment utilizează contul Microsoft (MAS) pentru a determina utilizatorul care încearcă să se conecteze la aplicație, timp în care este declanșată telemetria în discuție, ca parte a unei încercări nereușite.  

Acest eveniment ajută cu analiza de distribuire pentru eroarea de conectare MSA care ajută la înțelegerea motivelor din spatele fluxului de conectare nereușite MSA.

Se colectează următoarele câmpuri:

- **ExceptionsName** - indică clasele de excepție cu privire la etichetele de excepție care au loc în timpul fluxului de conectare la contul Microsoft.

- **ExceptionsTag** - indică ce excepții de flux prezente în uniune au loc pentru fluxul de conectare MSA.

- **IDCRLACEErrorCode** - oferă codul de eroare care apare în timpul fluxului de conectare MSA. Coduri de eroare diferite menționate la %SRCROOT%\identity\coreapi\public\IdentityData.h

- **IDCRLAuthenticationStatusErrorCode** - indică codurile de eroare pentru stările nevalide a rezultatului de autentificare din contul Microsoft (MSA).

- **IDCRLUserInteractionMissingError** - indică dacă fluxul de conectare în contul Microsoft (MSA) invocat cu semnalizarea showUI ca false determină accesarea.


#### <a name="officeandroidbcserrors"></a>Erori Office. Android. BCS.

Telemetrie erori de conversie binare pentru imprimare și partajare ca PDF.  Microsoft îl utilizează pentru a identifica punctele de eroare în timpul conversiilor BCS în Word, Excel sau PowerPoint.

Se colectează următoarele câmpuri:

- **DocumentFileSize** - dimensiune fișier

- **FileExtension** - primele patru caractere din extinderea fișierului.

- **IsFileDirty** -Boolean pentru a indica dacă există modificări nesalvate în fișier.

- **Location** - enumerare locația fișierului.  Valori: OneDrive, Microsoft Office SharePoint Online, Dropbox, altele

- **PDFConversionError** - eticheta la care apare eroarea pentru conversia PDF

- **PdfConversionErrorCode** - cod de eroare de conversie PDF

- **PdfConversionHRStatus** - Cod stare conversie PDF

- **PdfConversionResult** - PDF reconversie rezultat-enumerare.  Valori: „Succes”, „Nereușit” și „Anulat”

- **PdfFileSize -** - Dimensiunea PDF-ului

#### <a name="officeandroidclientsideiap"></a>Office.Android.ClientSideIAP

Telemetrie cu erori critice pentru erori de bază de date în timp ce răsfoiți fișiere și adaugați locuri.  Microsoft îl utilizează pentru a identifica problemele de corupție DB din aplicațiile care pot împiedica utilizatorul să adauge locuri sau să le răsfoiți din aplicație în Word, Excel sau PowerPoint.

Se colectează următoarele câmpuri:

- **ClientTransactionId** - GUID a trecut la DSC pentru o anumită solicitare de răscumpărare.

- **CollectionTime** - timp de finalizarea achiziționării abonamentului

- **Codţară** - cod de țară client, care este trimis către DSC pentru solicitarea de răscumpărare a clientului

- **GoPremiumEntryPoint** - punct de intrare pentru activarea achiziționării 

- **IsActivateExistingSubscription** - Boolean pentru a indica dacă există un abonament existent, care a fost activat

- **IsErrorRetriable** - Boolean pentru a indica dacă răscumpărarea poate fi reîncercată

- **IsPreviousPurchase** - Boolean pentru a indica dacă activarea s-a produs cu o achiziție anterioară de abonament

- **IsProvisioningTriggeredByRetry** - Boolean pentru a indica dacă s-a încercat din nou

- **LanguageCode** - cod de țară client, care este trimis către DSC pentru solicitarea de răscumpărare a clientului

- **ProductIdentifier** - nume SKU pe care clientul încearcă să-l achiziționeze

- **ProvisioningHttpStatusCode** - asigurarea accesului codului de stare HTTP

- **ProvisioningStatusCode** - asigurarea accesului codului de stare 

- **PurchaseOrderId** - identificator comenzi de achiziționare de la Google/Samsung 

- **RedemptionTaskHR** - HResult pentru rambursarea activității abonamentului

- **SubscriptionProvisioningSucceeded** - Boolean pentru reușita rezultatului furnizării abonamentului

- **SubscriptionPurchaseHR** - Hresult pentru activitate de achiziție de abonament

- **SubscriptionType** - enumerare pentru tip de abonament sau SKU-uri.

- **TCID** - pictograma care declanșează fluxul de abonament

#### <a name="officeandroiddbfailurecause"></a>Office.Android.DBFailureCause

Telemetrie pentru erori critice pentru erori de bază de date în timp ce răsfoiți fișiere și adaugați locuri.  Microsoft îl utilizează pentru a identifica problemele de corupție DB din aplicațiile care pot împiedica utilizatorul să adauge locuri sau să le răsfoiți din aplicație în Word, Excel sau PowerPoint.

Se colectează următoarele câmpuri:

- **ErrorAt** - valoare etichetă: informații despre locul în care s-a produs eroarea

- **ExceptionErrorMessage** - mesaj de eroare detaliat

#### <a name="officeandroidearlytelemetryexpansionfileserrors"></a>Office.Android.EarlyTelemetry.ExpansionFilesErrors

Setul de extensii APK pentru aplicația mobilă Office sunt fișierele suplimentare de resurse pe care dezvoltatorii de aplicații Android le pot publica împreună cu aplicația lor. Pentru ca fișierele noastre de extindere să fie mai fiabile, înregistrăm în jurnal cauza erorilor care au loc în descărcarea fișierelor de extindere sau în timp ce se citesc fișierele de extindere descărcate.

Se colectează următoarele câmpuri:

- **Data_ClassName** - text ce reprezintă numele fișierului de cod sursă, în care există o eroare.

- **Data_ErrorMessage** - text ce reprezintă operațiunea care nu a reușit.

- **Data_ExceptionMessage** - un câmp text opțional care reprezintă cauza excepției.

- **Data_ExceptionType** - un câmp text opțional care reprezintă numele excepției lansat din codul sursă.

- **Data_MethodName** - text reprezentând numele metodei din codul sursă unde există o eroare.

#### <a name="officeandroidearlytelemetryextractionerror"></a>Office.Android.EarlyTelemetry.ExtractionError

Pentru a reduce dimensiunea aplicațiilor Office Android, aplicăm comprimarea resurselor în pachetul final. În timpul execuției, extragem mai întâi aceste resurse înainte de a le utiliza. Câteodată apar erori neașteptate în timpul efectuării extracțiilor, ceea ce duce la căderea aplicației. 

Prin intermediul acestui eveniment, colectăm informații de diagnosticare legate de extracție, precum numele resursei extrase, calea de extragere etc., spațiul liber disponibil pe disk etc. Aceste date sunt colectate doar atunci când există erori de extragere.

Utilizăm aceste date pentru a înțelege cauza erorilor de extragere, precum și pentru a îmbunătăți experiența de utilizator pentru aplicațiile noastre.

Se colectează următoarele câmpuri:

- **Data_ArchiveName** - numele resursei care este extrasă.

- **Data_ArchivePath** - calea în care resursa este memorată temporar în cache.

- **Data_ArchiveSizeKB** - dimensiunea resursei care este extrasă.
 
- **Data_ClassName** - numele fișierului în codul sursă în care apare eroarea.

- **Data_ErrorDetail** - textul care descrie mai multe detalii despre cauza erorii, precum codul de eroare etc.

- **Data_ErrorMessage** - textul care descrie tipul de eroare întâmpinată în timpul extragerii.

- **Data_ExtractionDestinationPath** - calea în care este salvată resursa după extragere.

- **Data_FreeDiskSpaceMB** - volumul spațiului liber pe disk disponibil pe dispozitiv, măsurat în megabyți. 

- **Data_ItemToExtract** - numele resursei care este extrasă.

- **Data_MethodName** - numele metodei în codul sursă în care s-a produs eroarea.


#### <a name="officeandroidearlytelemetryregistryerrors"></a>Office.Android.EarlyTelemetry.RegistryErrors

Acest eveniment capturează toate erorile cu care se confruntă în timpul accesului la registry Android. Aceste date ale evenimentului ne ajută să înțelegem erorile de utilizator și cum să realizăm o caracteristică de registry mai robustă.

Se colectează următoarele câmpuri:

- **App** – procesul aplicației care trimite evenimentul.

- **AppVersionLong** – versiunea aplicației.

- **Data_StackTrace** – urmărirea stivei erorii.

#### <a name="officeandroidearlytelemetrysharedlibraryloadersearchandloadlibraryerror"></a>Office. Android.EarlyTelemetry. SharedLibraryLoadersearchAndloadLibraryError 

Vom înregistra acest eveniment în cazul în care există erori în timpul încărcării bibliotecilor partajate. Pot exista erori de încărcare pentru biblioteci din două motive 1) APK instalat este incompatibil cu dispozitivul. 2) Biblioteca pe care încercăm să o încărcăm poate fi deteriorată, din cauza erorilor din extragerea ei din cauza spațiului de disc redus sau a memoriei insuficiente.

Se colectează următoarele câmpuri:

- **Data_ExceptionMessage** - mesaj de excepție generat de sistemul API Android.loadLibrary

- **Data_FreeSpaceInMB** - spațiu disponibil pe dispozitiv 

- **Data_nickName** - numele bibliotecii care nu poate fi încărcată.

#### <a name="officeandroidintuneintunejavacopyfailedattempts"></a>Office.Android.Intune.IntuneJavaCopyFailedAttempts

Telemetrie de eroare critică pentru a urmări erorile API-urilor Intune individuale; Această telemetrie este înregistrată în cazul erorilor pentru salvarea copiei locale a documentelor în cloud protejate cu Intune.  Microsoft utilizează aceste date pentru a identifica erorile din timpul și de după înscrierea în Intune din cadrul aplicației, conectarea publică la aplicație cu un cont de la locul de muncă

Se colectează următoarele câmpuri:

- **Data_FileCreationFailedErrorCode** - cod de eroare asociat cu fluxul

#### <a name="officeandroidintuneintunejavaexceptionadaltokenformam"></a>Office.Android.Intune.IntuneJavaExceptionADALTokenForMAM

Telemetrie de eroare critică pentru a urmări erorile API-urilor Intune individuale; Această telemetrie este înregistrată în cazul erorilor pentru a obține eticheta ADAL pentru resursele Intune.  Microsoft utilizează aceste date pentru a identifica erorile în timpul înscrierii la Intune din cadrul aplicației și conectarea imediată la aplicație cu un cont de la locul de muncă

Se colectează următoarele câmpuri:

- **Data_ErrorCode** - cod de eroare asociat cu fluxul

#### <a name="officeandroidintuneintunejavaexceptionapppolicy"></a>Office.Android.Intune.IntuneJavaExceptionAppPolicy

Telemetrie de eroare critică pentru a urmări erorile API-urilor Intune individuale; Această telemetrie este înregistrată în cazul erorilor pentru a contacta API-urile din Intune legat de politicile obținute pentru o identitate pentru procesul actual.  Microsoft utilizează aceste date pentru a identifica erorile din timpul și de după înscrierea în Intune din cadrul aplicației, conectarea publică la aplicație cu un cont de la locul de muncă

Se colectează următoarele câmpuri:
 
- Fără

#### <a name="officeandroidintuneintunejavaexceptionapppolicyforcontext"></a>Office.Android.Intune.IntuneJavaExceptionAppPolicyForContext

Telemetrie de eroare critică pentru a urmări erorile API-urilor Intune individuale; Această telemetrie este înregistrată în cazul erorilor pentru a contacta API-urile din Intune legat de politicile obținute pentru o identitate în procesul actual.  Microsoft utilizează aceste date pentru a identifica erorile din timpul și de după înscrierea în Intune din cadrul aplicației, conectarea publică la aplicație cu un cont de la locul de muncă

Se colectează următoarele câmpuri:
 
- Fără

#### <a name="officeandroidintuneintunejavaexceptionauthenticationcallback"></a>Office. Android.Intune.IntuneJavaExceptionAuthenticationCallback

Telemetrie de eroare critică pentru a urmări erorile API-urilor Intune individuale; Această telemetrie este înregistrată în cazul erorilor pentru a contacta API-urile din Intune legat de înregistrarea pentru apeluri de autentificare pentru conturile gestionate.  Microsoft utilizează aceste date pentru a identifica erorile din timpul și de după înscrierea în Intune din cadrul aplicației, conectarea publică la aplicație cu un cont de la locul de muncă

Se colectează următoarele câmpuri:

- Fără

#### <a name="officeandroidintuneintunejavaexceptiongetaccountstatesync"></a>Office.Android.Intune.IntuneJavaExceptionGetAccountStateSync

Telemetrie de eroare critică pentru a urmări erorile API-urilor Intune individuale; Această telemetrie este înregistrată în cazul erorilor pentru conectarea API-urilor Intune legate de contul gestionat.  Microsoft utilizează aceste date pentru a identifica erorile din timpul și de după înscrierea în Intune din cadrul aplicației, conectarea publică la aplicație cu un cont de la locul de muncă

Se colectează următoarele câmpuri:
 
- Fără

#### <a name="officeandroidintuneintunejavaexceptiongetissavetolocationallowed"></a>Office.Android.Intune.IntuneJavaExceptionGetIsSaveToLocationAllowed

Telemetrie de eroare critică pentru a urmări erorile API-urilor Intune individuale; Această telemetrie este înregistrată în cazul erorilor pentru preluarea politicii legate de salvare în local.   Microsoft utilizează aceste date pentru a identifica erorile din timpul și de după înscrierea în Intune din cadrul aplicației, conectarea publică la aplicație cu un cont de la locul de muncă

Se colectează următoarele câmpuri:

- Fără

#### <a name="officeandroidintuneintunejavaexceptiongetpolicyforidentity"></a>Office.Android.Intune.IntuneJavaExceptionGetPolicyForIdentity

Telemetrie de eroare critică pentru a urmări erorile API-urilor Intune individuale; Această telemetrie este înregistrată în cazul erorilor pentru a conecta API-urile din Intune legat de politicile obținute pentru o identitate.  Microsoft utilizează aceste date pentru a identifica erorile din timpul și de după înscrierea în Intune din cadrul aplicației, conectarea publică la aplicație cu un cont de la locul de muncă

Se colectează următoarele câmpuri:

- Fără

#### <a name="officeandroidintuneintunejavaexceptiongetprotectioninfofromdescriptor"></a>Office.Android.Intune.IntuneJavaExceptionGetProtectionInfoFromDescriptor

Telemetrie de eroare critică pentru a urmări erorile API-urilor Intune individuale; Această telemetrie este înregistrată în cazul erorilor pentru conectarea API-urilor Intune legate de informații de protecție.  Microsoft utilizează aceste date pentru a identifica erorile din timpul și de după înscrierea în Intune din cadrul aplicației, conectarea publică la aplicație cu un cont de la locul de muncă

Se colectează următoarele câmpuri:
  
- Fără

#### <a name="officeandroidintuneintunejavaexceptiongetprotectioninfofrompath"></a>Office.Android.Intune.IntuneJavaExceptionGetProtectionInfoFromPath

Telemetrie de eroare critică pentru a urmări erorile API-urilor Intune individuale; Această telemetrie este înregistrată în cazul erorilor pentru conectarea API-urilor Intune legate de informații de protecție.  Microsoft utilizează aceste date pentru a identifica erorile din timpul și de după înscrierea în Intune din cadrul aplicației, conectarea publică la aplicație cu un cont de la locul de muncă

Se colectează următoarele câmpuri:

- Fără

#### <a name="officeandroidintuneintunejavaexceptiongetuipolicyidentity"></a>Office. Android. Intune. IntuneJavaExceptionGetUIPolicyIdentity

Telemetrie de eroare critică pentru a urmări erorile API-urilor Intune individuale; Această telemetrie este înregistrată în cazul erorilor pentru a conecta API-urile din Intune legat de politicile obținute pentru interfața utilizator pentru un cont gestionat.  Microsoft utilizează aceste date pentru a identifica erorile din timpul și de după înscrierea în Intune din cadrul aplicației, conectarea publică la aplicație cu un cont de la locul de muncă

Se colectează următoarele câmpuri:

- Fără

#### <a name="officeandroidintuneintunejavaexceptionisidentitymanaged"></a>Office. Android.Intune.IntuneJavaExceptionIsIdentityManaged

Telemetrie de eroare critică pentru a urmări erorile API-urilor Intune individuale; Această telemetrie este înregistrată în cazul erorilor pentru conectarea API-urilor Intune legate de identificarea contului gestionat.  Microsoft utilizează aceste date pentru a identifica erorile din timpul și de după înscrierea la Intune din cadrul aplicației, conectarea imediată la aplicație cu un cont de la locul de muncă

Se colectează următoarele câmpuri:

- Fără

#### <a name="officeandroidintuneintunejavaexceptionnullenrollmentmanager"></a>Office.Android.Intune.IntuneJavaExceptionNullEnrollmentManager

Telemetrie de eroare critică pentru a urmări erorile API-urilor Intune individuale; Această telemetrie este înregistrată în cazul erorilor pentru a conecta API-urile din Intune legat de înregistrarea componentelor pentru apeluri.  Microsoft utilizează aceste date pentru a identifica erorile din timpul și de după înscrierea în Intune din cadrul aplicației, conectarea publică la aplicație cu un cont de la locul de muncă

Se colectează următoarele câmpuri:

- Fără

#### <a name="officeandroidintuneintunejavaexceptionprotect"></a>Office.Android.Intune.IntuneJavaExceptionProtect

Telemetrie de eroare critică pentru a urmări erorile API-urilor Intune individuale; Această telemetrie este înregistrată în cazul erorilor pentru conectarea API-urilor Intune legate de protecția documentului gestionat.  Microsoft utilizează aceste date pentru a identifica erorile din timpul și de după înscrierea la Intune din cadrul aplicației, conectarea imediată la aplicație cu un cont de la locul de muncă

Se colectează următoarele câmpuri:

- Fără

#### <a name="officeandroidintuneintunejavaexceptionprotectfromdescriptorifrequired"></a>Office. Android.Intune.UntuneJavaExceptionProtectFromDescriptorIfRequired

Telemetrie de eroare critică pentru a urmări erorile API-urilor Intune individuale; Această telemetrie este înregistrată în cazul erorilor pentru conectarea API-urilor Intune legate de protecția documentului gestionat.  Microsoft utilizează aceste date pentru a identifica erorile din timpul și de după înscrierea în Intune din cadrul aplicației, conectarea publică la aplicație cu un cont de la locul de muncă

Se colectează următoarele câmpuri:

- Fără

#### <a name="officeandroidintuneintunejavaexceptionregisteraccountsync"></a>Office.Android.Intune.IntuneJavaExceptionRegisterAccountSync

Telemetrie de eroare critică pentru a urmări erorile API-urilor Intune individuale; Această telemetrie este înregistrată în cazul erorilor pentru conectarea API-urilor Intune legate de contului în Management Intune.  Microsoft utilizează aceste date pentru a identifica erorile din timpul și de după înscrierea în Intune din cadrul aplicației, conectarea publică la aplicație cu un cont de la locul de muncă

Se colectează următoarele câmpuri:

- Fără

#### <a name="officeandroidintuneintunejavaexceptionsetuipolicyidentitysync"></a>Office. Android.Intune.IntuneJavaExceptionSetUIPolicyIdentitySync

Telemetrie de eroare critică pentru a urmări erorile API-urilor Intune individuale; Această telemetrie este înregistrată în cazul erorilor pentru a conecta API-urile din Intune legat de setarea politicilor pentru un cont gestionat.  Microsoft utilizează aceste date pentru a identifica erorile din timpul și de după înscrierea în Intune din cadrul aplicației, conectarea publică la aplicație cu un cont de la locul de muncă

Se colectează următoarele câmpuri:

- Fără

#### <a name="officeandroidintuneintunejavaexceptionunregisteraccountsync"></a>Office.Android.Intune.IntuneJavaExceptionUnregisterAccountSync

Telemetrie de eroare critică pentru a urmări erorile API-urilor Intune individuale; Această telemetrie este înregistrată în cazul erorilor pentru conectarea API-urilor Intune legat de golirea scenariilor la distanță în Management Intune.  Microsoft utilizează aceste date pentru a identifica erorile din timpul și de după înscrierea în Intune din cadrul aplicației, conectarea publică la aplicație cu un cont de la locul de muncă

Se colectează următoarele câmpuri:

- Fără

#### <a name="officeandroidintuneintunejavaexceptionupdatetoken"></a>Office.Android.Intune.IntuneJavaExceptionUpdateToken

Telemetrie de eroare critică pentru a urmări erorile API-urilor Intune individuale; Această telemetrie este înregistrată în cazul erorilor pentru a conecta API-urile din Intune legat de actualizarea etichetei de autorizare pentru un cont gestionat.  Microsoft utilizează aceste date pentru a identifica erorile din timpul și de după înscrierea în Intune din cadrul aplicației, conectarea publică la aplicație cu un cont de la locul de muncă

Se colectează următoarele câmpuri:

- Fără

#### <a name="officeandroidlicenseactivationfailure"></a>Office.Android.LicenseActivationFailure

Telemetrie de eroare critică pentru a urmări erorile de activare a licențelor pentru conturile Office 365 în Word, Excel sau PowerPoint.  Microsoft îl utilizează pentru a analiza erorile pentru activarea unei licență Office 365 achiziționată.

Se colectează următoarele câmpuri:

- **EntryPoint** - enumerare punct de intrare pentru declanșarea fluxului de activare a licenței

- **HResult** - cod de eroare pentru nereușită

- **IsGallatin** - Boolean pentru a verifica dacă este un cont Gallatin

- **MessageCode** - enumerare pentru a indica punctul de nereușită pentru activare

- **PreviousEntryPoint** - enumerare punct de intrare pentru declanșarea fluxului de activare a licenței

- **StateAfterActivation** - enumerare pentru a indica starea de licențiere a aplicației înainte de începerea fluxului de activare

- **StateBeforeActivation** - enumerare pentru a indica starea de licențiere a aplicației înainte de începerea fluxului de activare

- **UserAccountType** - enumerare pentru a indica dacă contul este personal sau de întreprindere.

#### <a name="officeandroidmsasigninuiprompts"></a>Office.Android.MSASignInUIPrompts

Acest eveniment indică faptul că solicitarea de conectare a fost livrată utilizatorului, pentru contul personal.  Acest eveniment vă ajută să înțelegeți starea de funcționare a aplicațiilor noastre și să luați măsurile corespunzătoare, atunci când observăm solicitările de conectare neașteptate. 

Se colectează următoarele câmpuri:

- **ExternalCacheRefreshError** - cod de eroare de încercare a reîmprospătării simbolului, înainte de a afișa solicitarea de conectare.

- **LastLoginDelta** - delta timp de la ultima logare reușită

- **MSAserverUAID** - ID-ul de corelare cu datele de telemetrie ale serviciului.

- **PreviousIdentityState** - indică starea contului, dacă sesiunea a expirat. 

- **SignInResultCode** - indică codul rezultat al solicitării de la sfârșitul conectării.

- **UseCache** - indică dacă am forțat să-i solicităm utilizatorului să furnizeze din nou parola.

- **UserType** - indică dacă acesta este cont este nou sau nu

- **WasIdentitySignedOut** - indică dacă contul a fost deconectat.


#### <a name="officeapplelicensingmacdractivationfailures"></a>Office.Apple.Licensing.Mac.DRActivationFailures

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Evenimentul este utilizat pentru capturarea erorilor de activare a fluviului digital (evenimentul înregistrează cheia și produsul utilizat pentru activare, precum și codul de eroare primit).  Acest eveniment este utilizat pentru detectarea și pentru a ajuta la depanarea erorilor activare (probleme Digital River).

Se colectează următoarele câmpuri:

- **Data_DigitalRiverID** - cod de produs Digital River, care mapează pentru acest produs Office SKY

- **Data_Error** - un șir reprezentând un cod de eroare de activare.

- **Data_ProductKey** - cheia de produs care a fost încercată să fie activată

- **Data_ProductKeyHash** - o cheie de produs codificată activată

#### <a name="officeapplelicensingmacgetmachinestatuserrors"></a>Office.Apple.Licensing.Mac.GetMachineStatusErrors

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Evenimentul colectează codul de eroare returnat în timp ce verifică periodic validitatea unei licențe de abonament. Codul de eroare poate însemna indisponibilitatea serverelor, dar și expirarea licenței, limita contorului de mașină, ID-ul de hardware nevalid etc. Acest eveniment este utilizat pentru a monitoriza starea serviciului de licențiere Office, dar și pentru a investiga problemele legate de managementul abonamentului computerului.

Se colectează următoarele câmpuri:

- **Data_Error** - colectăm un șir reprezentând un cod de eroare

#### <a name="officeextensibilitysandboxodperrornotification"></a>Office.Extensibility.Sandbox.ODPErrorNotification

Urmărește diferitele notificări de erori primite de la sandbox. Se utilizează pentru a detecta scenariile de eroare în sandbox și acolo prin remedierea acestora, să se îmbunătățească productivitatea utilizatorului
 
Se colectează următoarele câmpuri:

- **AppId** - ID-ul aplicației

- **AppUrl** - adresa URL a aplicației 

- **Result** - cod de eroare rezultat

#### <a name="officefirstrunapplemaconiolkfirstrunstarted"></a>Office.FirstRun.Apple.MacONIOLKFirstRunStarted

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Evenimentul ne anunță că un utilizator a intrat în prima experiență de rulare. Utilizăm acest eveniment pentru a ne da seama dacă prima experiență de rulare (FRE) a fost începută cu succes.

Se colectează următoarele câmpuri:

- **Data_FirstRunCollectionTime** - un marcaj de timp care înregistrează ora la care a început fluxul.

#### <a name="officegraphicsarcexceptions"></a>Office.Graphics.ARCExceptions 

Aceste informații de raportare a excepțiilor sunt importante pentru a evalua starea generală a stivei de elemente grafice și pentru a identifica părțile de cod în care apar erori cu o frecvență ridicată, pentru a stabili prioritatea investigațiilor. Aceste informații de raportare a excepțiilor sunt importante pentru a evalua starea generală a stivei de elemente grafice și pentru a identifica părțile de cod în care apar erori cu o frecvență ridicată. Acestea ajută inginerii să stabilească erorile de redare care afectează cei mai mulți utilizatori, permițându-ne să stabilim priorități pentru investigațiile noastre și să remediem problemele care vor aduce cele mai multe beneficii utilizatorilor.

Se colectează următoarele câmpuri:

  - **Data\_HResult** – codul de eroare returnat

  - **Data\_TagCount** – de căte ori a apărut fiecare eroare

  - **Data\_TagID** – identificatorul erorii care a apărut

#### <a name="officeoutlookdesktopcalendaracceptcalsharenavigatetosharedfoldererror"></a>Office.Outlook.Desktop.Calendar.AcceptCalShareNavigateToSharedFolder.Error

Colectează informații atunci când apare o eroare în timp ce se navighează la calendarul partajat. Aceste date se utilizează pentru a monitoriza starea API-ului de partajare a calendarelor și interacțiunea Outlook cu calendarele partajate.

Se colectează următoarele câmpuri:

  - **FailedCaseHResult** – codul de eroare returnat

#### <a name="officeoutlookdesktopedpedpopenstorefailure"></a>Office.Outlook.Desktop.EDP.EDPOpenStoreFailure

Reușita sau nereușita de a deschide sursa de e-mailuri protejate de Protecția datelor la nivel de întreprindere în funcție de rezultatul apelării API-ului Windows pentru a obține cheia și a decripta magazinul. Vom folosi acest lucru pentru a diagnostica una dintre principalele probleme Enterprise Data Protection care pot împiedica inițializarea Outlook. Cauza principală a erorii este interacțiunea Outlook cu API-urile Windows utilizate pentru a decripta cheia din magazin.

Se colectează următoarele câmpuri:

  - **HVA Activity** **-** cu câmpuri de date particularizate

  - **IsFlightOn** – indică dacă s-a activat EDPDecryption Flight

#### <a name="officeoutlookdesktopndbcorruptionresult"></a>Office.Outlook.Desktop.NdbCorruptionResult

Office.Outlook.Desktop.NdbCorruptionResult și Office.Outlook.Desktop.NDBCorruptStore.Warning sunt colectate atunci detectăm o deteriorare în PST/OST pentru un utilizator. Când detectăm o deteriorare, Microsoft colectează formatul bazei de date, locul unde s-a detectat și o cantitate mică de context despre deteriorare. Deteriorarea OST/PST împiedică utilizatorii să-și acceseze e-mailurile. Monitorizăm în mod activ aceste date pentru activitate anormală. Ne propunem să investigăm și să diagnosticăm problemele, pentru a limita pierderea de date de către clienți.

Se colectează următoarele câmpuri:

  - **0 –** numele de proces care a raportat deteriorarea

  - **1 –** valoarea bool care indică dacă utilizatorul alege noul fișier sau nu

  - **2 –** numărul de alte procese care au baza de date deschisă

#### <a name="officeoutlookdesktopndbcorruptstorewarning"></a>Office.Outlook.Desktop.NDBCorruptStore.Warning

Office.Outlook.Desktop.NdbCorruptionResult și Office.Outlook.Desktop.NDBCorruptStore.Warning sunt colectate atunci detectăm o deteriorare în PST/OST pentru un utilizator. Când detectăm o deteriorare, Microsoft colectează formatul bazei de date, locul unde s-a detectat și o cantitate mică de context despre deteriorare. Deteriorarea OST/PST împiedică utilizatorii să-și acceseze e-mailurile. Monitorizăm în mod activ aceste date pentru activitate anormală. Ne propunem să investigăm și să diagnosticăm problemele, pentru a limita pierderea de date de către clienți.

Se colectează următoarele câmpuri:

  - **CollectionTime** – ora colectării

  - **Context** – contextul Corrupt Store unde s-a detectat deteriorarea

  - **CreatedWithVersion** – câmpul (opțional) cu versiunea depozitului

  - **Details** – detalii despre eroare

  - **NdbType** – tipul de depozit, care poate fi 0 = NdbUndefined, 1 = NdbSmall, 2 = NdbLarge, 3 = NdbTardis

  - **ProcessName** – numele de proces care determină deteriorarea depozitului

  - **PstVersion** – versiunea MSPST32.DLL

  - **Version** – versiunea de format a fișierului de depozit

#### <a name="officeoutlookdesktopoutlookcalendarusageerrmeetrcptforwardactionsruleo16"></a>Office.Outlook.Desktop.OutlookCalendarUsageErr.MeetRcpt.ForwardActions.Rule.O16

Colectează reușitele și nereușitele acțiunilor Redirecționare, Redirecționare ca atașare și Redirecționare ca iCalendar pentru răspunsurile la întâlniri Unice, Recurente și Excepționale din vizualizarea Mail, Calendar și Inspector Outlook. Rata de erori pentru acțiunile Redirecționare, Redirecționare ca atașare și Redirecționare ca iCalendar este monitorizată activ pentru anomalii. Statisticile privind anomaliile indică o eroare în abilitatea Outlook de a efectua operațiuni de calendar de bază. Aceste date se utilizează, de asemenea, pentru a diagnostica alte probleme legate de Calendar care pot fi detectate.

Se colectează următoarele câmpuri:

  - **CountExceptionForward** - numărul de excepții de întâlnire redirecționate

  - **CountExceptionForwardAsiCal** - numărul de excepții de întâlnire redirecționate ca iCal

  - **CountExceptionForwardInSplit** - numărul de excepții de întâlnire redirecționate din meniul Scindare din panglică

  - **CountExceptionForwardWithAttach** - numărul de excepții de întâlnire redirecționate ca atașare

  - **CountRecurringForward** - numărul de întâlniri recurente redirecționate

  - **CountRecurringForwardAsiCal** - numărul de întâlniri recurente redirecționate ca iCal

  - **CountRecurringForwardInSplit** - numărul de întâlniri recurente redirecționate din meniul Scindare din panglică

  - **CountRecurringForwardWithAttach** - numărul de întâlniri recurente redirecționate ca atașare

  - **CountSingleForward** - numărul de întâlniri unice redirecționate

  - **CountSingleForwardAsiCal** - numărul de întâlniri unice redirecționate ca iCal

  - **CountSingleForwardInSplit** - numărul de întâlniri unice redirecționate din meniul Scindare din panglică

  - **CountSingleForwardWithAttach** - numărul de întâlniri unice redirecționate ca atașare

  - **HResult** - ErrorCode

  - **OlkViewName** - indică vizualizarea Mail, Calendar sau Inspector

#### <a name="officeoutlookdesktopoutlookcalendarusageerrmeetrcptreplyactionsruleo16"></a>Office.Outlook.Desktop.OutlookCalendarUsageErr.MeetRcpt.ReplyActions.Rule.O16

Colectează reușitele și nereușitele acțiunilor Răspuns, Răspuns tuturor, Răspuns cu mesaj instantaneu și Răspuns tuturor cu mesaj instantaneu pentru răspunsurile la întâlniri Unice, Recurente și Excepționale din vizualizarea Mail, Calendar și Inspector Outlook. Rata de nereușită a acțiunilor Răspuns, Răspuns tuturor, Răspuns cu mesaj instantaneu și Răspuns tuturor cu mesaj instantaneu este monitorizată activ pentru anomalii. Statisticile privind anomaliile indică o eroare în abilitatea Outlook de a efectua operațiuni de calendar de bază. Aceste date se utilizează, de asemenea, pentru a diagnostica alte probleme legate de Calendar care pot fi detectate.

Se colectează următoarele câmpuri:

  - **CountExceptionReply** - numărul de excepții de Răspuns la întâlnire

  - **CountExceptionReplyAll** - numărul de excepții de Răspuns tuturor la întâlnire

  - **CountExceptionReplyAllWithIM** - numărul de excepții de Răspuns tuturor cu mesaj instantaneu la întâlnire

  - **CountExceptionReplyWithIM** - numărul de excepții de Răspuns cu mesaj instantaneu la întâlnire

  - **CountRecurringReply** - numărul de răspunsuri la întâlniri recurente

  - **CountRecurringReplyAll** - numărul de răspunsuri de tip Răspuns tuturor la întâlniri recurente

  - **CountRecurringReplyAllWithIM** - numărul de răspunsuri tuturor cu mesaj instantaneu la întâlniri recurente

  - **CountRecurringReplyWithIM** - numărul de răspunsuri cu mesaj instantaneu la întâlniri recurente

  - **CountSingleReply** - numărul de răspunsuri la întâlniri unice

  - **CountSingleReplyAll** - numărul de răspunsuri tuturor la întâlniri unice

  - **CountSingleReplyAllWithIM** - numărul de răspunsuri tuturor cu mesaj instantaneu la întâlniri unice

  - **CountSingleReplyWithIM** - numărul de răspunsuri cu mesaj instantaneu la întâlniri unice

  - **HResult** - ErrorCode

  - **OlkViewName** - indică vizualizarea Mail, Calendar sau Inspector

#### <a name="officeoutlookdesktopoutlookprivsdlgsingleuserloadfail"></a>Office.Outlook.Desktop.OutlookPrivsDlgSingleUser.LoadFail

Această regulă colectează erorile de partajare a calendarelor atunci când se adaugă un utilizator nou (de tip EX sau SMTP) din agendă. Aceste date se utilizează pentru diagnosticarea și rezolvarea problemelor detectate în caseta de dialog Partajarea calendarelor

Se colectează următoarele câmpuri:

  - **CountAccountWizardEnd** – De câte ori s-a încheiat caseta de dialog pentru expertul moștenit

  - **CountCreatePIMAccount** – de câte ori utilizatorul a creat un profil PIM

#### <a name="officeoutlookmacmacolkasserts"></a>Office.Outlook.Mac.MacOLKAsserts

Utilizat pentru a identifica probleme care afectează utilizatorul în Outlook și care se pot manifesta prin căderi sau prin degradarea funcționalității. 

Se colectează următoarele câmpuri:

- **Category** - tip de aserțiune

- **CollectionTime** - momentul în care se colectează aserțiunea


#### <a name="officeoutlookmacmacolkerrors"></a>Office.Outlook.Mac.MacOLKErrors

Utilizat pentru a identifica probleme care afectează utilizatorul în Outlook și care se pot manifesta prin căderi sau prin degradarea funcționalității. 

Se colectează următoarele câmpuri:

- **Category** - tip de eroare

- **CollectionTime** - momentul în care se colectează eroarea

- **ThreadID** - identificator pentru fir


#### <a name="officesystemsystemhealthasserts"></a>Office.System.SystemHealthAsserts

Erorile pe care le identifică acest eveniment ne ajută să înțelegem când experiența clienților se degradează. Multe dintre aceste ShipAsserts duc la căderi, iar aceste informații ne ajută să le remediem. Colectează ShipAsserts din cadrul produsului, pentru a identifica erorile.

Se colectează următoarele câmpuri:

 - **Count** – numărul fiecărei aserțiuni raportate

  - **EndTime** – ora la care a apărut ultima aserțiune raportată

  - **ErrorGroup** – un identificator de bucket pentru fiecare aserțiune

  - **FirstTimeStamp** – prima oră la care a apărut aserțiunea

  - **Trackback** – un identificator unic pentru o anumită aserțiune

#### <a name="officesystemsystemhealtherrorsetwshim"></a>Office.System.SystemHealthErrorsEtwShim

Utilizat pentru a problemele din aplicația curentă care afectează clienții și care se pot manifesta drept căderi sau funcționalitate diminuată. Înregistrează erorile care apar la momentul rulării procesului.

Se colectează următoarele câmpuri:

  - **EndTime** – ora la care a apărut ultima eroare raportată

  - **Trackback** – un identificator unic pentru o anumită eroare

  - **ErrorGroup** – un identificator de bucket pentru fiecare eroare

  - **Count** – numărul fiecărei erori

  - **FirstTimeStamp** – prima oră la care a apărut eroarea

#### <a name="officesystemsystemhealtherrorsulsandasserts"></a>Office.System.SystemHealthErrorsUlsAndAsserts

Utilizat pentru a problemele din aplicația curentă care afectează clienții și care se pot manifesta drept căderi sau funcționalitate diminuată. Înregistrează erorile care apar la momentul rulării procesului.

Se colectează următoarele câmpuri:

  - **EndTime** – ora la care a apărut ultima eroare raportată

  - **Trackback** – un identificator unic pentru o anumită eroare

  - **ErrorGroup** – un identificator de bucket pentru fiecare eroare

  - **Count** – numărul fiecărei erori

  - **FirstTimeStamp** – prima oră la care a apărut eroarea

#### <a name="officesystemsystemhealtherrorsulsworkaround"></a>Office.System.SystemHealthErrorsUlsWorkaround

Utilizat pentru a problemele din aplicația curentă care afectează clienții și care se pot manifesta drept căderi sau funcționalitate diminuată. Înregistrează erorile care apar la momentul rulării procesului

Se colectează următoarele câmpuri:

  - **EndTime** – ora la care a apărut ultima eroare raportată

  - **Trackback** – un identificator unic pentru o anumită eroare

  - **ErrorGroup** – un identificator de bucket pentru fiecare eroare

  - **Count** – numărul fiecărei erori

#### <a name="officesystemsystemhealtherrorswithouttag"></a>Office.System.SystemHealthErrorsWithoutTag

Utilizat pentru a problemele din aplicația curentă care afectează clienții și care se pot manifesta drept căderi sau funcționalitate diminuată. Înregistrează erorile care apar la momentul rulării procesului.

Se colectează următoarele câmpuri:

Count – numărul fiecărei erori

  - **EndTime** – ora la care a apărut ultima eroare raportată

  - **ErrorCode** – un identificator pentru eroare

  - **ErrorGroup** – un identificator de bucket pentru fiecare eroare

  - **ErrorId** – un identificator pentru eroare

  - **FirstTimeStamp** – prima oră la care a apărut eroarea

  - **Trackback** – un identificator unic pentru o anumită eroare

#### <a name="officesystemsystemhealtherrorswithtag"></a>Office.System.SystemHealthErrorsWithTag

Utilizat pentru a problemele din aplicația curentă care afectează clienții și care se pot manifesta drept căderi sau funcționalitate diminuată. Înregistrează erorile care apar la momentul rulării procesului.

Se colectează următoarele câmpuri:

  - **Count** – numărul fiecărei erori

  - **EndTime** – ora la care a apărut ultima eroare raportată

  - **ErrorCode** – un identificator pentru eroare

  - **ErrorGroup** – un identificator de bucket pentru fiecare eroare

  - **ErrorId** – un identificator pentru eroare

  - **FirstTimeStamp** – prima oră la care a apărut eroarea

  - **Trackback** – un identificator unic pentru o anumită eroare

#### <a name="renewidentityfailure"></a>RenewIdentityFailure

Este colectat atunci când un utilizator încearcă să deschidă un document protejat prin IRM sau să aplice protecții IRM. Acesta conține informațiile necesare pentru a investiga și a diagnostica corect problemele care apar atunci când nu reușește înnoirea certificatelor de utilizator.

Se colectează următoarele câmpuri:

- **AppInfo.ClientHierarchy** - ierarhie client care indică faptul că aplicația rulează în mediul de producție sau în mediul de dezvoltator

- **AppInfo.Name** - nume aplicație.

- **AppInfo.Version** - versiunea aplicației

- **Failure.Category** - categoria erorii „UnhandledError”

- **Failure.Detail** - informațiile detaliate ale erorii

- **Failure.Id** - ID eroare

- **Failure.Signature** - semnătura erorii, care este aceeași cu numele evenimentului

- **iKey** - ID al serverului pentru servicii de înregistrare

- **RMS.HRESULT** - rezultatul reînnoirii certificatului de utilizator

- **RMS.ScenarioId** - ID al scenariului definit de clientul Serviciu de administrare a drepturilor

- **RMS.SDKVersion** - versiunea clientului pentru Serviciul de administrare a drepturilor

#### <a name="saveerror"></a>save.error

Ne permite să detectăm și să remediem situațiile în care s-a produs o eroare atunci când ați încercat să salvați un fișier.  Urmărește erorile cauzate de erori la salvarea unui fișier, inclusiv un mesaj de eroare descriptiv, pentru a ne ajuta să rezolvăm problema.

Se colectează următoarele câmpuri: 

- **error** - tipul de eroare care s-a produs pentru a ne ajuta să detectăm și să rezolvăm problemele legate de un anumit tip de eroare

- **file_type** - tipul de fișier pe care utilizatorul a încercat să-l salveze (cum ar fi. doc)

- **origin** - care este originea încercării de salvare a fișierului (de ex. de la un mesaj de e-mail), astfel încât să putem detecta problemele asociate cu salvarea unui fișier dintr-un anumit loc din aplicație

- **token_type** - tipul de simbol utilizat pentru autentificarea contului pentru a salva fișierul, astfel încât să ne ajute să detectăm probleme de autentificare asociate cu salvarea unui fișier


## <a name="device-connectivity-and-configuration-data-events"></a>Evenimente privind conectivitatea și datele de configurare ale dispozitivelor

Iată subtipurile de date din această categorie:

- [Conectivitatea și configurarea dispozitivelor](#device-connectivity-and-configuration-subtype)


### <a name="device-connectivity-and-configuration-subtype"></a>*Conectivitatea dispozitivelor și subtipul de configurare*

Starea conexiunii la rețea și setările dispozitivelor, cum ar fi memoria.

#### <a name="applicationdidreceivememorywarning"></a>application.did.receive.memory.warning

Acest eveniment este trimis atunci când Apple ne spune că aplicația nu mai are memorie suficientă. Aceasta ne spune că am introdus o problemă cu gestionarea memoriei pe dispozitivul dvs.

Se colectează următoarele câmpuri: 

- **current_memory_used** - ne spune cantitatea de memorie utilizată de aplicație în momentul în care aplicația nu mai are memorie suficientă.

- **current_memory_used_percentage** - ne spune procentul de memorie utilizat de aplicație din memoria totală disponibilă în momentul în care aplicația nu mai avea memorie suficientă.

- **currentVC** - ne spune vizualizarea afișată în prezent atunci când aplicația nu mai avea memorie suficientă.

- **has_hx** - ne spune că acest cont folosește noul nostru serviciu de sincronizare, pentru a ne ajuta să detectăm problemele provocate de serviciul nostru de sincronizare

- **is_watch_app_installed** - ne spune dacă utilizatorul utilizează în prezent un Apple Watch și dacă este instalat, pentru a ne ajuta să înțelegem impactul negativ asupra performanței cauzat de Watch

- **is_watch_paired** - ne spune dacă utilizatorul utilizează în prezent un Apple Watch și dacă este asociat cu dispozitivul pentru a ne ajuta să înțelegem impactul negativ asupra performanței cauzat de Watch

- **is_watch_supported_and_active** - ne spune dacă utilizatorul utilizează în prezent un Apple Watch și dacă este activ pentru a ne ajuta să înțelegem impactul negativ asupra performanței cauzat de Watch

- **rn_initialized** - ne spune dacă React Native a fost inițializat în momentul în care aplicația nu mai avea memorie suficientă.

- **running_time** - ne spune intervalul de timp petrecut de aplicație în momentul în care aplicația nu mai avea memorie suficientă.

#### <a name="conversationmemoryleak"></a>conversation.memory.leak

Ne permite să detectăm situațiile în care vizualizarea noastră de conversație prin e-mail ne determină să utilizăm mai mult spațiu de stocare pe dispozitivul dvs. decât era de așteptat.

Se colectează următoarele câmpuri:

- Nu s-au colectat câmpuri sau date suplimentare. Doar jurnalele sunt colectate dacă există o irosire de memorie corelată cu un fir de conversație.

#### <a name="coredatacorruption"></a>core.data.corruption

Ne permite să detectăm situațiile în care nu vă putem afișa e-mailul sau calendarul, deoarece locul în care stocăm e-mailul pe dispozitivul dvs. s-a deteriorat.

Se colectează următoarele câmpuri:

- **errorSource** - indică dacă provine de la o acțiune salvare sau creare

- **sqlError** - cod de eroare numeric listat la https://www.sqlite.org/c3ref/c_abort.html

#### <a name="coredatacorruptionuserreset"></a>core.data.corruption.user.reset

Ne permite să detectăm situațiile în care v-ați șters sau resetat contul din aplicația noastră, situație cauzată de o corupere în datele de e-mail pe care le-am stocat pe dispozitivul dvs.

Se colectează următoarele câmpuri:

- **errorSource** - dictează unde s-a produs corupția, fie în timpul salvării, fie în timpul creării

#### <a name="coredatadiagnostics"></a>core.data.diagnostics 

Ne permite să detectăm și să remediem situațiile în care spațiul nostru de stocare e-mailul utilizează prea mult din spațiul de stocare al dispozitivelor dvs.

Se colectează următoarele câmpuri:

- **db_size_megabytes** - urmărește dimensiunea bazei de date nucleu rotunjită la cei mai apropiați 25 de megaocteți și cu un număr maxim de MB de 500

#### <a name="generalpropertieslog"></a>general.properties.log

Acest eveniment colectează informații care ne permit să clasificăm și să dispunem pe categorii problemele din aplicația Outlook care sunt asociate cu setările de accesibilitate și de dispozitive.  Această clasificare este necesară pentru a prioritiza impactul problemelor asupra clienților.

Se colectează următoarele câmpuri pentru iOS:

- **bold_text** - ne spune dacă dispozitivul are textul cu caractere aldine activat pentru a ne ajuta să detectăm probleme legate de textul cu caractere aldine

- **closed_captioning** - ne spune dacă utilizatorul a activat subtitrarea complexă pe dispozitiv, pentru a ne ajuta să detectăm probleme legate de subtitrări

- **darker_system_colors** - ne spune dacă utilizatorul a activat întunecarea culorilor de sistem pe dispozitiv, pentru a ne ajuta să detectăm probleme legate de această setare

- **gray_scale** - ne spune dacă utilizatorul a activat tonuri de gri pe dispozitiv, pentru a ne ajuta să detectăm probleme legate de această setare

- **guided_access** - ne spune dacă utilizatorul a activat acces ghidat pe dispozitivul său, pentru a ne ajuta să detectăm probleme legate de această setare

- **invert_colors** - ne spune dacă utilizatorul a activat setarea pentru a inversa culorile pe dispozitiv, pentru a ne ajuta să detectăm probleme legate de această setare

- **mono_audio** - ne spune dacă utilizatorul a activat setarea Audio mono pe dispozitiv, pentru a ne ajuta să detectăm probleme legate de această setare

- **reduce_motion** - ne spune dacă utilizatorul a activat setarea de reducere a mișcării pe dispozitiv, pentru a ne ajuta să detectăm probleme legate de această setare

- **reduce_transparency** - ne spune dacă utilizatorul a activat setarea pentru a reduce transparența pe dispozitiv, pentru a ne ajuta să detectăm probleme legate de această setare

- **speak_screen** - ne spune dacă utilizatorul a activat setarea pentru Audio mono pe dispozitiv, pentru a ne ajuta să detectăm probleme legate de această setare

- **speak_selection** - ne spune dacă utilizatorul a activat setarea pentru Speak Selection pe dispozitiv, pentru a ne ajuta să detectăm probleme legate de această setare

- **switch_control** - ne spune dacă utilizatorul a activat setarea pentru Switch Control pe dispozitiv, pentru a ne ajuta să detectăm probleme legate de această setare

- **voice_over** - ne spune dacă utilizatorul a activat setarea pentru VoiceOver pe dispozitiv, pentru a ne ajuta să detectăm probleme legate de această setare

Se colectează următoarele câmpuri pentru Android:

- **braille** - ne spune dacă utilizatorul a activat setarea pentru a inversa culorile pe dispozitiv, pentru a ne ajuta să detectăm probleme legate de această setare

- **caption** - ne spune dacă utilizatorul a activat subtitrarea complexă pe dispozitiv, pentru a ne ajuta să detectăm probleme legate de subtitrări

- **color_inversion** - ne spune dacă utilizatorul a activat setarea pentru a inversa culorile pe dispozitiv, pentru a ne ajuta să detectăm probleme legate de această setare

- **high_contrast** - ne spune dacă utilizatorul a activat setarea pentru Contrast înalt pe dispozitiv, pentru a ne ajuta să detectăm probleme legate de această setare

- **large_text** - ne spune dacă dispozitivul are setarea text mare activată pentru a ne ajuta să detectăm probleme legate de această setare

- **oem_preinstall** - ne spune dacă aplicația noastră a fost preinstalată pe dispozitiv (aceasta se aplică numai la dispozitivele Samsung)

- **supported_abis** - ne spune ce tipuri de interfață binare de aplicație (ABI) sunt acceptate de platforma de dispozitive pentru a ne ajuta să detectăm probleme legate de această setare

- **switch_access** - ne spune dacă utilizatorul a activat setarea pentru Switch Access pe dispozitiv, pentru a ne ajuta să detectăm probleme legate de această setare

- **talkback** - ne spune dacă utilizatorul a activat setarea pentru Talkback pe dispozitivul său, pentru a ne ajuta să detectăm probleme legate de această setare

- **webview_kernel_version** : versiunea kernel-ului Chromium a vizualizării web de pe dispozitiv, pentru a ne ajuta să detectăm probleme de compatibilitate legate de versiunea de vizualizare web a paginii.

- **webview_package_name** : numele de pachet a vizualizării web de pe dispozitiv, pentru a ne ajuta să detectăm probleme de compatibilitate legate de versiunea de vizualizare web a paginii.

- **webview_package_version** : numele de versiune a vizualizării web de pe dispozitiv, pentru a ne ajuta să detectăm probleme de compatibilitate legate de versiunea de vizualizare web a paginii.

#### <a name="lowstoragewarning"></a>low.storage.warning

Acest lucru este necesar pentru a monitoriza dacă aplicația noastră ocupă brusc cea mai mare parte a spațiului de stocare al dispozitivului din cauza unei utilizări de memorie de înaltă calitate, indicând atunci când dispozitivul este redus la spațiu de stocare

Se colectează următoarele câmpuri: 

- **free_bytes** - volumul de spațiu de stocare gratuit disponibil pe dispozitiv

#### <a name="officeairspaceairspacelocalblocklistdriverupdated"></a>Office.AirSpace.AirSpaceLocalBlocklistDriverUpdated

Utilizatorul a actualizat un driver de placă video care cauza anterior blocări în Office și nu mai este utilizat pentru redare. Informează Microsoft că utilizatorii care au fost odată într-o stare de redare suboptimă sunt din nou în starea de redare recomandată.

Se colectează următoarele câmpuri:

  - **Data\_BlockedDriverVersion** – versiunea driverului blocklisted.

  - **Data\_DeviceId** – identificatorul dispozitivului cu placa video care a fost blocklisted.

  - **Data\_UpdatedDriverVersion** – versiunea driverului actualizat

#### <a name="officeairspaceairspacelocalblocklistinfo"></a>Office.AirSpace.AirSpaceLocalBlocklistInfo

Detalii despre driverul de placă video al utilizatorului care a cauzat mai multe blocări recente ale aplicațiilor Office. Office nu va utiliza această placă video în această sesiune Office (ci va folosi redarea software) până la actualizarea driverului. Informează Microsoft cu privire la driverele de placă video care provoacă probleme în Office, pentru a identifica tendințele și a analiza impactul acestor drivere. Anunțați Microsoft câți utilizatori sunt în această stare suboptimă.

Se colectează următoarele câmpuri:

  - **Data\_AllAppsBlocked** – dacă toate aplicațiile Office sunt pe lista de blocare

  - **Data\_BlockedDeviceId** – identificatorul dispozitivului cu placă video care a fost blocklisted

  - **Data\_BlockedDriverVersion** – versiunea de driver care a fost blocklisted

  - **Data\_CrashHistory** – un șir care reprezintă istoricul blocărilor cauzate de driverul plăcii video pentru analiză

  - **Data\_SecsBetweenCrashes** – cât de frecvent apar blocările driverului de placă video

#### <a name="officeairspaceairspacewincompisenabled"></a>Office.AirSpace.AirSpaceWinCompIsEnabled

Dacă se folosește cea mai recentă platformă de redare Office de nivel inferior bazată pe Windows Composition.

Pe măsură ce se dezvoltă cea mai recentă platformă de redare de nivel inferior Office și începe să fie lansată pentru clienți, acest lucru permite Microsoft să vadă câți utilizatori folosesc fiecare versiune, pentru a vă asigura că platforma rămâne fără erori.

Se colectează următoarele câmpuri:

  - **Data\_WinCompEnabled** – dacă se folosește un backend bazat pe Windows Composition

#### <a name="officeairspacebackendwin32graphicsdriverhangdetectorblocklistapp"></a>Office.AirSpace.Backend.Win32.GraphicsDriverHangDetectorBlocklistApp

Placa video a utilizatorului a fost detectată ca determinând blocări lungi sau irecuperabile. Office nu va utiliza această placă video în această sesiune Office (ci va folosi redarea software) până la actualizarea driverului. Informează Microsoft cu privire la driverele de placă video care provoacă probleme în Office, pentru a identifica tendințele și a analiza impactul acestor drivere. Anunță câți utilizatori sunt în această stare suboptimă.

Se colectează următoarele câmpuri:

  - **Data\_AppName** – ce aplicație a întâmpinat blocări ale driverului de placă video

#### <a name="officeairspacebackendwin32graphicsdriverhangdetectorregistrywrite"></a>Office.AirSpace.Backend.Win32.GraphicsDriverHangDetectorRegistryWrite

Office a identificat că driverul de placă video al utilizatorului a provocat o blocare care ar trebui analizată la următoarea inițializare a aplicației Office. Se folosește pentru a determina dacă utilizarea altui adaptor sau a altui driver de placă video ar oferi o experiență de utilizator mai bună. Pe măsură ce apar modele, Microsoft poate face ajustări pentru a păstra experiența Office cât mai fluidă cu putință.

Se colectează următoarele câmpuri:

  - **Data\_HangDetected** – dacă s-a detectat o blocare

  - **Data\_InDeviceCall** – în ce apel de redare a plăcii video se afla Office când a apărut blocarea

  - **Data\_Timeout** – cât timp a durat blocarea, dacă s-a recuperat

  - **Data\_UnrecoverableCommand** – dacă blocarea din această comandă de redare a plăcii video permite, de obicei, recuperarea

#### <a name="officeairspacebackendwin32localblocklistactivity"></a>Office.AirSpace.Backend.Win32.LocalBlocklistActivity

Detalii despre driverul de placă video al utilizatorului care a cauzat mai multe blocări recente ale aplicațiilor Office. Office nu va utiliza această placă video în această sesiune Office (ci va folosi redarea software) până la actualizarea driverului. Informează Microsoft cu privire la driverele de placă video care provoacă probleme în Office, pentru a identifica tendințele și a analiza impactul acestor drivere. Anunțați Microsoft câți utilizatori sunt în această stare suboptimă.

Se colectează următoarele câmpuri:

  - **Data.AllAppsBlocked** – dacă toate aplicațiile Office sunt pe lista de blocare

  - **Data.BlockedDeviceId** – identificatorul dispozitivului cu placă video care a fost blocat

  - **Data.BlockedDriverVersion** – versiunea de driver care a fost blocklisted

  - **Data.CrashHistory System.String** – un șir care reprezintă istoricul blocărilor cauzate de driverul plăcii video pentru analiză

  - **Data.SecsBetweenCrashes** – cât de frecvent apar blocările driverului de placă video

#### <a name="officeairspacebackendwin32localblocklistdriverupdatedactivity"></a>Office.AirSpace.Backend.Win32.LocalBlocklistDriverUpdatedActivity

Utilizatorul a actualizat un driver de placă video care cauza anterior blocări în Office și nu mai este utilizat pentru redare. Informează Microsoft că utilizatorii care au fost odată într-o stare de redare suboptimă sunt din nou în starea de redare recomandată.

Se colectează următoarele câmpuri:

  - **Data\_BlockedDeviceId** – identificatorul dispozitivului cu placă video care a fost blocklisted

  - **Data\_BlockedDriverVersion** – versiunea de driver care a fost blocklisted

  - **Data\_UpdatedDriverVersion** – versiunea driverului actualizat

#### <a name="officegraphicsspritememcorrupt"></a>Office.Graphics.SpriteMemCorrupt

Raportează erorile detectate în telemetria de contabilizare a memoriei sprite. Esențiale pentru a evalua starea telemetriei de utilizare a memoriei grafice. Aceste informații sunt necesare pentru a valida corectitudinea telemetriei SpriteMem.

Se colectează următoarele câmpuri:

  - **Data\_CurrentSpriteMem** – cantitatea totală de memorie alocată activ pentru a stoca elemente sprite (imagini) care creează conținut pe ecran.

  - **Data\_Function** – numele funcției care încearcă să elibereze memoria sprite.

  - **Data\_SpriteMemToRemove** – cantitatea de memorie de eliminat din alocarea sprite.

#### <a name="officepowerpointpptsharednointernetconnectivity"></a>Office.PowerPoint.PPT.Shared.NoInternetConnectivity

Se colectează de câte ori PowerPoint detectează că nu există conectivitate la internet. Microsoft utilizează aceste date pentru a obține informații de diagnostic despre conexiunea la internet a utilizatorului, spre a înțelege cum afectează aceasta conectivitatea la servicii Office.

Se colectează următoarele câmpuri:

- **Data\_IsNexusDetected:bool** – arată dacă avem starea de conectivitate la internet atunci când apelăm serviciul Nexus (valoarea true) sau când apelăm API-ul serviciului web generic (valoarea false)

#### <a name="officeserviceabilitymanagerofficesvcmgrprofile"></a>Office.ServiceabilityManager.OfficeSvcMgrProfile

Acest eveniment se declanșează atunci când Office Serviceability Manager pornește și este esențial pentru furnizarea de detalii exacte legate de starea de implementare și aplicație, iar programul de completare se blochează în entitatea găzduită a clientului, permițându-ne să generăm detalii pentru ca administratorul IT să poată să facă cu încredere actualizări pentru utilajele lor de întreprindere.  

Se colectează următoarele câmpuri:

- **DeviceIdJoinToken** -folosit pentru a accesa date de telemetrie din starea de bună funcționare și implementare cu alte date funcționale colectate prin intermediul canalului de servicii.

- **TenantAssociationKeyStamped** -un semnalizator Boolean folosit pentru a determina numărul de dispozitive gestionate din sistemul Eco Office.
