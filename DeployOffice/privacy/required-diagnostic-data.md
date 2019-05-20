---
title: Date de diagnosticare obligatorii pentru Office
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.audience: ITPro
ms.topic: reference
ms.service: o365-proplus-itpro
localization_priority: Priority
ms.collection: Ent_O365
ms.custom:
- Ent_Office_ProPlus
- Ent_Office_Privacy
description: Le oferă administratorilor Office informații despre datele de diagnosticare obligatorii în Office și le furnizează o listă de evenimente și câmpuri de date.
hideEdit: true
ms.openlocfilehash: 9b22b428999c51b46e6f6ce662fad99f5a727b4c
ms.sourcegitcommit: 6145cfe372725bedab7bc6a80adab100561f74fd
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/17/2019
ms.locfileid: "34106936"
---
# <a name="required-diagnostic-data-for-office"></a>Date de diagnosticare obligatorii pentru Office

> [!IMPORTANT]
> Informațiile din acest articol se aplică la versiunea 1904 sau la o versiune mai recentă a următorului software client Office instalat pe un computer care rulează Windows:
> - Office 365 ProPlus și Office 365 Business
> - Office 365 Personal, Office 365 pentru acasă sau alte versiuni de Office, care fac parte dintr-un abonament Office 365.
> - Project și Visio care sunt oferite cu anumite planuri de abonament, cum ar fi planul Project Online Professional sau Visio Online Plan 2.

Datele de diagnosticare se folosesc pentru a păstra Office în siguranță și la zi, pentru a detecta, a diagnostica și a remedia problemele și pentru a îmbunătăți produsele. Aceste date nu includ numele sau adresa de e-mail a unui utilizator, nici conținutul fișierelor acestuia sau informații despre aplicații care nu au legătură cu Office.

Datele de diagnosticare sunt colectate și trimise la Microsoft despre software-ul client Office utilizat pe computerele care rulează Windows. Anumite date de diagnosticare sunt obligatorii, în timp ce altele sunt opționale. Vă oferim posibilitatea de a alege dacă să ne trimiteți datele de diagnosticare obligatorii sau opționale, utilizând controalele de confidențialitate, cum ar fi setările de politici pentru organizații. Puteți vedea datele de diagnosticare care ne sunt trimise utilizând Vizualizatorul de date de diagnosticare.

***Datele de diagnosticare obligatorii*** sunt datele minime necesare pentru a păstra Office securizat, actualizat și într-o stare de funcționare conform așteptărilor pe dispozitivul pe care este instalat.

Datele de diagnosticare obligatorii ajută la identificarea problemelor cu Office care pot fi asociate cu o configurație de dispozitiv sau software. De exemplu, ne poate ajuta să stabilim dacă o caracteristică de Office înregistrează căderi mai frecvent într-o anumită versiune de sistem de operare, cu caracteristici nou-introduse, sau atunci când anumite caracteristici de Office sunt dezactivate. Datele de diagnosticare obligatorii ne ajută să detectăm, să diagnosticăm și să remediem aceste probleme mai rapid, astfel încât impactul asupra utilizatorilor sau organizațiilor este redus.

Pentru mai multe informații despre datele de diagnosticare, consultați linkul următor:

- [Date de diagnosticare opționale pentru Office](optional-diagnostic-data.md)
- [Utilizarea Vizualizatorului de date de diagnosticare cu Office](https://support.office.com/article/cf761ce9-d805-4c60-a339-4e07f3182855)

Dacă sunteți administratorul organizației dvs., ați putea fi interesat și de următoarele:

- [Prezentare generală a controalelor de confidențialitate pentru Office 365 ProPlus](overview-privacy-controls.md)
- [Utilizați setările de politică pentru a gestiona controalele de confidențialitate pentru Office 365 ProPlus](manage-privacy-controls.md)

## <a name="categories-data-subtypes-events-and-data-fields-for-required-diagnostic-data"></a>Categorii, subtipuri de date, evenimente și câmpuri de date pentru date de diagnosticare obligatorii

Datele de diagnosticare obligatorii sunt organizate în categorii și subtipuri de date. În fiecare subtip de date există evenimente care conțin câmpuri de date specifice respectivului eveniment.

Următorul tabel furnizează o listă de categorii pentru datele de diagnosticare obligatorii. Subtipurile de date din fiecare categorie sunt enumerate împreună cu o descriere a focalizării pentru acel subtip de date. Există linkuri la fiecare secțiune de subtip de date unde veți găsi informațiile următoare:

- O listă de evenimente din acel subtip de date
- O descriere a fiecărui eveniment
- O listă de câmpuri de date în fiecare eveniment
- O descriere a fiecărui câmp de date

| **Categorie**       | **Subtip de date**| **Descriere**    |
| ---------- | ------------- | ---- |
| **Inventar și instalare software** | [Inventar și instalare Office](#office-setup-and-inventory-subtype)   | Produsul instalat, versiunea și starea de instalare.  |
| | [Configurație program de completare Office](#office-add-in-configuration-subtype)  | Programele de completare software și setările lor.     |
| | [Securitatea](#security-subtype)  | Condițiile de eroare ale documentelor, caracteristicilor și programelor de completare care pot compromite securitatea, inclusiv pregătirea pentru actualizarea produselor.  |
| **Utilizarea produselor și a serviciilor**    | [Succesul caracteristicii aplicației](#application-feature-success-subtype)   | Succesul funcționalității aplicației. Limitat la deschiderea și închiderea aplicației și a documentelor, editarea fișierelor și partajarea fișierelor (colaborare). |
| | [Starea aplicației și inițializare](#application-status-and-boot-subtype)    | Stabilește dacă au avut loc anumite evenimente de caracteristici, cum ar fi pornirea sau oprirea, și dacă respectiva caracteristică rulează.   |
| | [Configurație accesibilitate Office](#office-accessibility-configuration-subtype)  | Caracteristici de accesibilitate în Office       |
| **Performanța produselor și a serviciilor**       | [Ieșire neașteptată a aplicației (cădere)](#unexpected-application-exit-crash-subtype)  | Ieșirile neașteptate ale aplicației și starea aplicației atunci când se întâmplă acest lucru.    |
|  | [Performanța caracteristicii aplicației](#application-feature-performance-subtype)  | Timpii de răspuns slabi sau performanțele scăzute pentru scenarii precum pornirea aplicației sau deschiderea unui fișier. |
|  | [Eroare de activitate a aplicației](#application-activity-error-subtype)   | Erorile în funcționalitatea unei caracteristici sau a unei experiențe de utilizator.  |
| **Conectivitatea și configurarea dispozitivelor** | [Conectivitatea și configurarea dispozitivelor](#device-connectivity-and-configuration-subtype) | Starea conexiunii la rețea și setările dispozitivelor, cum ar fi memoria. |


> [!NOTE]
> - Categoriile sunt afișate în Vizualizatorul de diagnosticare de date, dar subtipurile de date nu sunt afișate.
> - Un câmp de date marcat *Depășit* a fost sau va fi eliminat din datele de diagnosticare obligatorii. Unele dintre aceste câmpuri de date sunt dubluri care au apărut ca date de diagnosticare au fost modernizate și utilizate pentru a vă asigura că nu există întreruperi de serviciu pentru rapoarte de monitorizare de diagnosticare live.

## <a name="categories-and-data-fields-that-are-common-for-all-events"></a>Categorii și câmpuri de date comune pentru toate evenimentele

Există câteva informații despre evenimente comune pentru toate evenimentele, indiferent de categorie sau de subtipul de date. Aceste informații comune, denumite uneori *contracte de date*, sunt organizate în categorii. Fiecare categorie conține câmpuri, iar aceste câmpuri sunt metadatele și proprietățile unui eveniment individual. Puteți vizualiza aceste informații utilizând Vizualizatorul de date de diagnosticare.

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

  - **UserCategory -** identifică tipul de utilizatori care și-au exprimat consimțământul. Unul dintre MSAUser, AADUser sau LocalDeviceUser

  - **DiagnosticConsentLevel** - indică nivelul de consimțământ pentru datele de diagnosticare oferite de utilizator

  - **DiagnosticConsentSourceLocation** - indică modul în care utilizatorul și-a exprimat consimțământul pentru datele de diagnosticare

  - **DiagnosticConsentSourceLocation** - indică momentul în care utilizatorul și-a exprimat consimțământul pentru datele de diagnosticare

  - **ServiceConnectionState** - indică dacă utilizatorul a ales să utilizeze sau nu toate experiențele de mod conectat

  - **ServiceConnectionStateSourceLocation** -indică modul în care utilizatorul a furnizat opțiunea de a utiliza sau nu toate experiențele de mod conectat

  - **ServiceConnectionStateConsentTime** - indică momentul în care utilizatorul a ales dacă să utilizeze sau nu toate experiențele de mod conectat

  - **ControllerConnectedServicesState** - indică dacă utilizatorul are acces la experiențele de mod conectat opționale

  - **ControllerConnectedServicesStateSourceLocation**- indică modul în care a fost efectuată opțiunea utilizatorului pentru experiențe de mod conectat opționale

  - **ControllerConnectedServicesStateConsentTime** - indică momentul în care utilizatorul a ales starea experiențelor de mod conectat opționale

  - **UserContentDependentState** - indică dacă utilizatorul a ales să activeze sau să dezactiveze experiențe de mod conectat care analizează conținut

  - **UserContentDependentStateSourceLocation** - indică modul în care a fost efectuată opțiunea utilizatorului de a activa sau de a dezactiva experiențe de mod conectat care analizează conținut

  - **UserContentDependentStateConsentTime** - indică momentul în care utilizatorul a optat să activeze sau să dezactiveze experiențe de mod conectat care analizează conținut

  - **DownloadContentState** - indică dacă utilizatorul a ales să activeze sau să dezactiveze experiențe de mod conectat care descarcă online conținut

  - **DownloadContentStateSourceLocation** - indică modul în care utilizatorul a efectuat alegerea de a activa sau dezactiva experiențe de mod conectat care descarcă conținut online

  - **DownloadContentStateSourceLocation** - indică momentul în care utilizatorul a efectuat alegerea de a activa sau dezactiva experiențe de mod conectat care descarcă conținut online

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

  - **SamplingClientId** -ID-ul clientului utilizat pentru a stabili dacă face parte din eșantionare. Ne permite să stabilim de ce o sesiune individuală a fost inclusă sau exclusă din eșantionare.

#### <a name="user"></a>Utilizator

Furnizează informațiile de entitate găzduită pentru SKU-uri de software comerciale.

Această categorie conține următoarele câmpuri:

  - **PrimaryIdentityHash** - identificator sub pseudonim care reprezintă utilizatorul curent.

  - **PrimaryIdentitySpace** - tipul de identitate conținut în PrimaryIdentityHash. Unul dintre MASCID, OrgIdCID sau UserObjectId.

  - **TenantGroup** - tipul de entitate găzduită de care aparține abonamentul. Ne permite să clasificăm problemele și să identificăm dacă este o problemă pe scară largă sau una izolată la un set de utilizatori.

  - **TenantId** - entitatea găzduită la care este asociat abonamentul utilizatorului. Ne permite să clasificăm problemele și să identificăm dacă este o problemă pe scară largă sau una izolată la un set de utilizatori sau la o anumită entitate găzduită.

### <a name="information-that-specifically-supports-diagnostic-data-collection"></a>*Informațiile care acceptă în mod specific colectarea datelor de diagnosticare*

Informațiile care acceptă în mod specific colectarea datelor de diagnosticare sunt colectate în categoriile următoare.

#### <a name="activity"></a>Activitate

Informații pentru a înțelege succesul evenimentului de colectare în sine.

Această categorie conține următoarele câmpuri:

  - **AggMode** - comunică sistemului cum să realizeze agregarea rezultatelor activității. Ne permite să reducem volumul de informații încărcate de pe computerul unui utilizator, prin agregarea rezultatelor activității într-un singur eveniment care sunt trimise periodic.

  - **Count** - de câte ori s-a produs activitatea dacă numărul este de la un eveniment agregat. Ne permite să stabilim cât de des o activitate a reușit sau a eșuat pe baza modului de agregare a activității.

  - **CV** - valoare care identifică relația dintre activități și activități secundare. Ne permite să reconstruim relația dintre activități imbricate.

  - **Duration** - cât timp a fost necesar pentru executarea activității. Ne permite să identificăm probleme de performanță care au impact negativ asupra experienței utilizatorilor.

  - **Result**.**Code** - cod definit de aplicație pentru a identifica anumite rezultate. Ne permite să stabilim detalii mai specifice ale unei erori date, cum ar fi un cod de eroare care poate fi utilizat pentru a clasifica și a remedia problemele.

  - **Result.Tag** - etichetă întreagă, care identifică locația din codul unde a fost generat rezultatul. Ne permite să identificăm clar locația din cod unde a fost generat un rezultat, care permite clasificarea eșecurilor.

  - **Result**.**Type** - tipul codului de rezultat. Identifică tipul de cod de rezultat care a fost trimis, astfel încât valoarea poate fi interpretată corect.

  - **Success** - semnalizare care indică dacă activitatea a reușit sau nu. Ne permite să determinăm dacă acțiunile pe care le aplică utilizatorul în produs sunt reușite sau nereușite. Acest lucru ne permite să identificăm problemele care au impact asupra utilizatorului.

#### <a name="application"></a>Aplicație 

Informații despre instalarea aplicației din care sunt colectate evenimentele.

Această categorie conține următoarele câmpuri:

  - **Architecture** - arhitectura aplicației. Să clasificăm erorile care pot fi specifice unei arhitecturi a aplicației.

  - **Click2RunPackageVersion** - numărul de versiune al pachetului Clic și Pornire care a instalat aplicația. Ne permite să identificăm ce versiune a programului de instalare a fost utilizată pentru a instala Office, astfel încât să putem identifica probleme asociate de configurare.

  - **DistributionChannel** - canalul în care a fost implementată aplicația. Ne permite să realizăm partiția datelor de intrare, astfel încât să putem stabili dacă problemele afectează publicul.

  - **InstallMethod -** dacă pentru versiunea de compilare curentă de Office s-a efectuat upgrade de la o compilare mai veche, dacă s-a revenit la o compilare mai veche sau dacă este o instalare nouă.

  - **IsClickToRunInstall** - semnalizare care indică dacă instalarea a fost o instalare Clic și Pornire. Ne permite să identificăm problemele care pot fi specifice mecanismului de instalare Clic și Pornire.

  - **IsDebug** - semnalizare care indică dacă compilarea de Office este o compilare de depanare. Ne permite să identificăm dacă problemele provin de la compilări de depanare care se pot comporta diferit.

  - **IsInstalledOnExternalStorage** - semnalizare care indică dacă Office a fost instalat pe un dispozitiv de stocare extern. Să stabilim dacă problemele pot fi urmărite până într-o locație de stocare externă.

  - **IsOEMInstalled** - semnalizare care indică dacă Office a fost instalat de un producător original al echipamentului (OEM). Să stabilim dacă aplicația a fost instalată de un OEM care ne poate ajuta să clasificăm și să identificăm problemele.

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

  - **Name** - numele evenimentului. Permite să identificăm evenimentul care a fost trimis de la client.

  - **Rule** - identificator al regulii care a generat datele dacă acestea au fost generate de o regulă. Ne permite să identificăm sursa unor date, astfel încât să putem valida și gestiona parametrii acelor evenimente

  - **RuleId** - identificator al regulii care a generat datele dacă acestea au fost generate de o regulă. Ne permite să identificăm sursa unor date, astfel încât să putem valida și gestiona parametrii acelor evenimente.

  - **RuleInterfaces** - orice interfețe care sunt implementate de o regulă specifică. Ne permite să clasificăm și să importăm datele în funcție de structura sa, care simplifică procesarea datelor.

  - **RuleVersion** - identificator al regulii care a generat datele dacă acestea au fost generate de o regulă. Ne permite să identificăm sursa unor date, astfel încât să putem valida și gestiona parametrii acelor evenimente.

  - **SampleRate** - indicație legată de procentul de utilizatori care trimit aceste date Acest lucru ne permite să efectuăm analiza statistică a datelor, iar pentru punctele de date foarte obișnuite, nu trebuie să fie trimise de toți utilizatorii.

  - **SchemaVersion** - versiunea schemei utilizate pentru a genera datele de diagnosticare. Obligatoriu pentru a gestiona datele trimise de client. Acest lucru permite modificări în timp în care datele sunt trimise de la fiecare client.

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

  - **SamplingKey** - cheia este utilizată pentru a stabili dacă sesiunea este eșantionată sau nu. Ne permite să înțelegem cum aleg sesiunile individuale dacă să fie eșantionate sau nu.

  - **SamplingMethod** - metoda utilizată pentru a stabili politica de eșantionare. Ne permite să înțelegem ce date provin dintr-o sesiune.

  - **Sequence** - identificator numeric unic pentru sesiune. Permite ordonarea sesiunilor pentru analiza acelor probleme care este posibil să fi apărut.

  - **Start** - ora de inițializare a sesiunii de proces. Ne permite să stabilim când începe sesiunea.

  - **TimeZoneBiasInMinutes** - diferența în minute între UTC și ora locală. Permite normalizarea orelor UTC înapoi la ora locală.

  - **SamplingClientIdValue** - valoarea cheii utilizate pentru a determina eșantionarea. Ne permite să determinăm de ce o sesiune a fost eșantionată sau nu.

  - **SamplingDeviceIdValue** - valoarea cheii utilizate pentru a determina eșantionarea. Ne permite să determinăm de ce o sesiune a fost eșantionată sau nu.

  - **SamplingSessionKValue** - metadate complexe de eșantionare. Utilizate pentru a evalua semnificația statistică a datelor primite.

  - **SamplingSessionNValue** - metadate complexe de eșantionare. Utilizate pentru a evalua semnificația statistică a datelor primite.

  - **TelemetryPermissionLevel** - valoare care indică nivelul datelor de diagnosticare pentru care utilizatorul a optat. Ne permite să înțelegem la ce nivel de date de diagnosticare să ne așteptăm de la o sesiune.

## <a name="software-setup-and-inventory-data-events"></a>Evenimente despre instalare de software și date de inventar

Iată subtipurile de date din această categorie:
- [Inventar și instalare Office](#office-setup-and-inventory-subtype)
- [Configurație program de completare Office](#office-add-in-configuration-subtype)
- [Securitatea](#security-subtype)  

### <a name="office-setup-and-inventory-subtype"></a>*Subtip de instalare și inventar Office*

Produsul instalat, versiunea și starea de instalare.

#### <a name="officeclicktorunupdatestatus"></a>Office.ClickToRun.UpdateStatus

Se aplică la toate aplicațiile win32. Ne ajută să înțelegem starea procesului de actualizare a suitei Office (succes sau eșec cu detalii despre eroare)

Se colectează următoarele câmpuri:

- **build** - versiunea de Office instalată momentan

- **channel** - canalul prin care Office a fost distribuit

- **errorCode** - codul de eroare care indică eroarea

- **errorMessage** - informații suplimentare despre eroare

- **stare** - starea curentă a actualizării

- **targetBuild** - versiunea de Office la care este actualizată

#### <a name="officecorrelationmetadatautccorrelationmetadata"></a>Office.CorrelationMetadata.UTCCorrelationMetadata

Colectează metadatele Office prin UTC pentru a compara cu date echivalente, colectate prin canalul de telemetrie Office pentru a verifica corectitudinea și gradul de completitudine al datelor.

Se colectează următoarele câmpuri:

- **abConfigs** - ID-uri listă de caracteristici pentru a identifica acele caracteristici care sunt activate la client sau golite când aceste date nu sunt colectate.

- **abFlights** - „NoNL:NoFlights” atunci când caracteristicile flight nu sunt configurate. În caz contrar „holdoutinfo = unknown”.

- **AppSessionGuid** - identificator al unei anumite sesiuni de aplicație care începe la ora de creare a procesului și persistă până la sfârșitul procesului. Este formatat ca GUID standard pe 128 de biți, dar alcătuit din 4 părți. Aceste patru părți sunt în ordine: (1) ID-ul de proces pe 32 de biți (2) ID-ul de sesiune pe 16 biți (3) ID-ul de inițializare pe 16 biți (4) ora de creare a procesului pe 64 de biți, în UTC 100ns

- **appVersionBuild** - numărul de versiune al aplicației.

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

- **osEnvironment** - un întreg care indică spre sistemul de operare (Windows, Android, iOS, Mac etc).

- **osVersionString** - identificator al sistemului de operare

- **sessionID** - GUID generat aleator pentru a identifica sesiunea de aplicație

- **UTCReplace_AppSessionGuid** - valoare booleană constantă. Întotdeauna true.

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

  - **Data\_GetRelativePathsFailed -** calea corespunzătoare nu indică spre locația accesibilă

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

  - **Data\_VisioSKU**:**integer** - 0 pentru SKU Standard și 1 pentru SKU Profesional

### <a name="office-add-in-configuration-subtype"></a>*Subtip configurație program de completare Office*

Programele de completare software și setările lor.

#### <a name="officeextensibilityappcommandsappcmdprojectionstatus"></a>Office.Extensibility.AppCommands.AppCmdProjectionStatus

Colectează informațiile pentru a urmări care instalări de programe de completare Office au actualizat cu succes panglica versus care nu au reușit.

Utilizat pentru a remedia problemele comune de înregistrare în care programele de completare nu sunt instalate corect și nu se afișează niciodată, drept pentru care sunt inutilizabile.

Se colectează următoarele câmpuri:

  - Fără

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

Date privind succesul sau nereușita în ceea ce privește regăsirea necesității unor date actualizate privind programele de completare atribuite de administratorul de entitate găzduită Office 365. Utilizat pentru măsurători ale stării, diagrame și analiza problemelor clientului. ExchangeGetLastUpdate va rula întotdeauna la inițializare ca parte a codului gazdă și va determina dacă atribuirile de program de completare s-au modificat pentru un utilizator.  Dacă da, atunci osf.DLL va fi încărcat, astfel încât să putem apela ExchangeGetEntitlements pentru a obține anumite atribuiri (și ExchangeGetManifests va fi apelat pentru a regăsi orice manifest nou care este necesar).  ExchangeGetEntitlements (și ExchangeGetManifests) pot fi apelate și la cerere după ce aplicația-gazdă a rulat.  Ideea este de a nu încărca DLL mare în cazul în care nu este necesar.  Fără acest eveniment în Obligatoriu, nu am putea să spunem dacă utilizatorii nu reușesc să obțină programe de completare atribuite lor dacă primul apel de serviciu nu reușește.  Este, de asemenea, semnalul principal în orice problemă de autentificare cu care ne confruntăm când comunicăm cu serviciul nostru.

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

  - **NeedRefresh - ** acesta este un câmp true sau false, care indică dacă datele programului de completare au fost învechite și trebuie să le actualizăm.

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

  - **ManifestsReturned** - numărul de manifeste returnate de server

  - **ManifestsToRetrieve** - numărul de manifeste de obținut de la server

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

  - **Activitate HVA standard fără nicio sarcină particularizată**

#### <a name="officeprogrammabilityadd-insinternalsetconnectenterprise"></a>Office.Programmability.Add-ins.InternalSetConnectEnterprise

Eveniment generat atunci când un program de completare COM este încărcat pe un dispozitiv de întreprindere. Analiză desktop: \# de încărcări este utilizat ca numitor pentru calcularea stării (\# de căderi/\# de încărcări) pentru calculul măsurătorilor de stare pentru cercuri pilot și de producție în scenarii pentru întreprinderi. Aceasta solicită ca datele să fie precise, nu eșantionate întrucât numărul de dispozitive este mai mic (100-1000).

Se colectează următoarele câmpuri:

  - **Add-inconnectFlag** - comportamentul curent de încărcare

  - **Add-inDescription** - descrierea programului de completare

  - **Add-inFileName** - numele de fișier al programului de completare, exclusiv calea fișierului

  - **Add-inFriendlyName** - numele prietenos al programului de completare

  - **Add-inId** - ID-ul clasei programului de completare

  - **Add-inProgId** - ID-ul programului de completare

  - **Add-inProvider** - furnizorul programului de completare

  - **Add-inTimeDateStamp** - marca de timp a programului de completare din metadatele DLL

  - **Add-inVersion** - versiunea programului de completare

#### <a name="officevisiovisioaddonload"></a>Office.Visio.Visio.AddonLoad

Capturează erori atunci când o soluție nu reușește să se încarce. Esențial pentru a depana erorile de încărcare a programului de completare în Visio.

Se colectează următoarele câmpuri:

  - **Data\_Load1Error:integer** - valoarea de eroare în timpul încărcării programului de completare Visio

#### <a name="officevisiovisioaddonusage"></a>Office.Visio.Visio.AddonUsage

Capturează erori atunci când există o eroare în funcționalitatea soluției. Esențial pentru a depana erorile programului de completare în programe de completare.

Se colectează următoarele câmpuri:

  - **Data\_DocumentSessionLogID:string** - identificator sesiune document

  - **Data\_IsEnabled**:**bool** - true, dacă soluția este activată

  - **Data\_TemplateID:string** - GUID al șablonului în care a fost încărcată soluția. Conectat ca 0 pentru soluție particularizată

  - **Data\_AddOnID**:**string** - GUID pentru a identifica programul de completare încărcat

  - **Data\_Error**:**integer** - ID eroare

### <a name="security-subtype"></a>*Subtip de securitate*

Condițiile de eroare ale documentelor, caracteristicilor și programelor de completare care pot compromite securitatea, inclusiv pregătirea pentru actualizarea produselor.

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


### <a name="application-feature-success-subtype"></a>*Subtip privind succesul caracteristicii aplicației*

Succesul funcționalității aplicației. Limitat la deschiderea și închiderea aplicației și a documentelor, editarea fișierelor și partajarea fișierelor (colaborare).

#### <a name="officeappcompatappcompatagentscanandupload"></a>Office.AppCompat.AppCompat.AgentScanAndUpload

Colectat doar atunci când utilizatorul final a activat Tabloul de bord de telemetrie Office. Colectează informații privind momentul în care se execută Agentul de telemetrie Office.  Acest lucru se colectează doar atunci când Tabloul de bord de telemetrie Office este activat și este utilizat pentru a determina starea de funcționare a agentului de telemetrie Office.

Se colectează următoarele câmpuri:

  - **Data.AgentExit** - marcă de timp privind momentul în care ieșirea agentului de telemetrie se efectuează cu succes

  - **Data.AgentScan** - marcă de timp privind momentul în care agentul de telemetrie a finalizat cu succes o scanare

  - **Data.AgentUpload** - marcă de timp privind momentul în care agentul de telemetrie finalizează cu succes încărcarea

#### <a name="officeappcompatappcompattelemetrydashboardresiliencycrashlog"></a>Office.AppCompat.AppCompat.TelemetryDashboardResiliencyCrashLog

Colectat doar atunci când Tabloul de bord de telemetrie Office a fost activat de utilizatorul final (cel mai probabil un administrator). Colectează apariția unor căderi de documente și programe de completare Office. Se colectează doar atunci când utilizatorul a activat Tabloul de bord de telemetrie Office și este utilizat pentru a stabili dacă au loc mai multe căderi de programe de completare sau documente.

Se colectează următoarele câmpuri:

  - **Data.CollectionTime** - marcă de timp privind momentul în care a fost înregistrat în jurnal un eveniment de cădere

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

#### <a name="officeextensibilitycatalogexchangeprocessentitlement"></a>Office.Extensibility.Catalog.ExchangeProcessEntitlement

Date privind procesarea unui drept individual și program de completare atribuit unui administrator de entitate găzduită Office 365.

Utilizat la crearea de diagrame (solicitat de conducerea echipei) privind succesul clienților și analiza problemelor clienților.

Se colectează următoarele câmpuri:

  - **AppVersion** - versiunea aplicației gazdă a programului de completare

  - **SolutionId** - GUID care reprezintă un program de completare unic

  - **TelemetryId** - GUID care reprezintă un utilizator unic

#### <a name="officefileiocsiccachedfilecsiloadfilebasic"></a>Office.FileIO.CSI.CCachedFileCsiLoadFileBasic

Ne permite să știm dacă un fișier s-a deschis cu succes din nivelul FIO. Utilizat pentru starea și monitorizarea caracteristicilor.

Se colectează următoarele câmpuri:

  - **Activity.Group -** etichetă care permite gruparea unui set de evenimente de monitorizare pentru a gestiona succesul general

  - **Activity.IsHVA -** semnalizare care indică faptul că evenimentul este de importanță critică pentru succesul utilizatorului

  - **Data.AsyncOpen -** semnalizare care indică faptul că deschiderea prezenta conținut care a sosit după ce corpul principal a fost deschis

  - **Data.CacheFileId -** se conectează la telemetrie Cache pentru documente Office pentru a activa analize de impact ale problemelor cu memoria cache asupra experienței utilizatorului

  - **Data.CoauthStatus -** raportează starea de colaborare a documentului la deschidere

  - **Data.CountOfMultiRoundTripsDownload -** numărul de transferuri la serverul utilizat pentru a depana problemele privind performanța și rețeaua

  - **Data.CountOfMultiRoundTripsUpload -** numărul de transferuri la serverul utilizat pentru a depana problemele privind performanța și rețeaua

  - **Data.DialogId -** setați dacă o casetă de dialog UI a fost afișată în timpul deschiderii, ceea ce indică faptul că i s-a afișat un mesaj de avertizare utilizatorului

  - **Data.DidFallbackToDAV -** setați dacă documentul a fost deschis utilizându-se un protocol de transfer de fișiere mai vechi

  - **Data.Doc.AccessMode -** documentul este numai în citire/editabil

  - **Data.Doc.AssistedReadingReasons -** setați dacă documentul are implementată o protecție a datelor electronice

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

  - **Data.Input.FileOpenState -** starea solicitată de aplicație (Read/ReadWrite etc.) **-**

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

  - **Data.IsSyncBackedStateDifferentThanOnLastOpen -** starea documentului s-a modificat, este posibil ca modificările să se fi produs în timp ce documentul era deschis

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

  - **Data.DialogChoice -** înregistrează alegerea efectuată în toate casetele de dialog de eroare

  - **Data.DialogId -** înregistrează DialogId ale tuturor casetelor de dialog de eroare care se afișează în timpul salvării

  - **Data.Dmc.IsOcsSupported -** depășit

  - **Data.Doc.AccessMode -** documentul este numai în citire

  - **Data.Doc.AssistedReadingReasons -** setați dacă documentul are implementată o protecție a datelor electronice

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

  - **Data.DstDoc.IOFlags -** semnalizări opțiuni memorate în cache ale documentului nou la deschidere

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

  - **Data.IsSyncBackedStateDifferentThanOnLastOpen -** starea documentului s-a modificat, este posibil ca modificările să se fi produs în timp ce documentul era deschis

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

#### <a name="officeoutlookdesktopprovidersloadproviderlibrary"></a>Office.Outlook.Desktop.Providers.LoadProviderLibrary

Acest eveniment urmărește succesul sau eșecul MAPI când încearcă să încarce un furnizor DLL (de ex., contab32.dll, emsmdb32.dll, un DLL utilizat de un program de completare). Operațiunea MAPI responsabilă pentru încărcarea de DLL-uri de la furnizori este fundamentală pentru operațiunea obligatorie pentru Outlook, precum și extensibilitate (prin programe de completare sau furnizori de Spațiu de stocare/Transport/Agendă particularizată). Monitorizăm în mod activ succesul sau eșecul rezultat în urma acestei operațiuni pentru a ne asigura că această funcționalitate de bază MAPI continuă să funcționeze conform așteptărilor.

Se colectează următoarele câmpuri:

  - **Activitate HVA standard** fără nicio sarcină particularizată

#### <a name="officeoutlookdesktopstorescreatenewstore"></a>Office.Outlook.Desktop.Stores.CreateNewStore

Colectează rezultatul de creare a unui magazin nou (cu tip și versiune), precum și codul rezultat. Monitorizăm în mod activ acest eveniment pentru a urmări starea capacității unui utilizator de a sincroniza și stoca e-mailuri local, de a arhiva e-mailuri (într-un fișier PST) sau a utiliza Grupuri.

Se colectează următoarele câmpuri:

  - **Activitate HVA standard** cu nicio sarcină particularizată

  - **StoreType** - tipul de magazin creat OST/PST/NST

  - **StoreVersion** - versiunea de magazin creată Small/Large/Tardis

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

  - **Data\_Doc\_ChunkingType:long -** cum este stocat documentul în SharePoint

  - **Data\_Doc\_EdpState:long -** starea Enterprise Data Protection a documentului

  - **Data\_Doc\_Ext:string -** extensia documentului

  - **Data\_Doc\_Extension:string -** extensia documentului

  - **Data\_Doc\_FileFormat:long -** set predefinit de valori pentru formatul fișierului (mai granular decât extensia)

  - **Data\_Doc\_Fqdn:string -** unde este stocat documentul (SharePoint.com, live.net), disponibil numai pentru domeniile Office 365

  - **Data\_Doc\_FqdnHash:string -** codul hash al locului unde este stocat documentul

  - **Data\_Doc\_IdentityTelemetryId:string - **GUID unic al utilizatorului

  - **Data\_Doc\_IdentityUniqueId:string -** identificator unic al identității folosite pentru acțiunea Documente partajate

  - **Data\_Doc\_IOFlags:long -** bitmask pentru diferite semnalizări legate de IO pentru un anumit document

  - **Data\_Doc\_IrmRights:long -** set predefinit de valori pentru tipul de Information Rights Management aplicat pentru acest document (Redirecționare, Răspuns, SecureReader, Editare etc.)

  - **Data\_Doc\_IsCloudCollabEnabled:bool -** true dacă antetul „IsCloudCollabEnabled” a fost deja primit dintr-o solicitare OPTIONS.

  - **Data\_Doc\_IsIncrementalOpen:bool -** documentul a fost deschis incremental (caracteristică nouă care deschide documentul fără să-l descarce în totalitate)

  - **Data\_Doc\_IsOcsSupported:bool -** dacă documentul acceptă elaborarea în comun folosind noul serviciu OCS

  - **Data\_Doc\_IsOpeningOfflineCopy:bool -** verifică dacă documentul este deschis din memoria cache locală

  - **Data_Doc_IsRtcAlwaysOn -** true în cazul în care canalul în timp real (RTC) este întotdeauna activat pentru acest fișier.

  - **Data\_Doc\_IsSyncBacked:bool -** verifică dacă documentul este deschis din folderul care folosește aplicația de sincronizare inversă OneDrive

  - **Data\_Doc\_Location:long -** set predefinit de valori privind locul de stocare a documentului (Local, SharePoint, WOPI, Rețea etc.)

  - **Data\_Doc\_LocationDetails:long -** set predefinit de valori privind locația mai detaliată (folderul Temp, folderul de descărcări, Documente OneDrive, Imagini OneDrive etc.)

  - **Data\_Doc\_NumberCoAuthors:long -** numărul de coautori la momentul deschiderii unui document

  - **Data\_Doc\_PasswordFlags:long -** set predefinit de valori privind modul în care documentul este criptat cu o parolă (Fără, parolă pentru citire, parolă pentru editare)-

  - **Data\_Doc\_ReadOnlyReasons:long -** set predefinit de valori privind motivul pentru care acest document a fost marcat doar în citire (blocat pe server, document final, protejat prin parolă pentru editare etc.)

  - **Data\_Doc\_ResourceIdHash:string -** codul hash al identificatorului de resurse pentru documentele stocate în cloud

  - **Data\_Doc\_ServerDocId:string -** identificatorul invariabil pentru documentele stocate în cloud

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

  - **Data\_fLifeguarded:bool -** a fost documentul vreodată protejat (caracteristică pentru a remedia erorile din documente, fără a-i adresa solicitări utilizatorului)?

  - **Data\_IsDocAutoSaveable:bool -** se salvează prezentarea automat?

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

  - **Data\_StopwatchDuration:long -** timpul total al activității

  - **Data\_UserContinuedZRTClose:bool -** după afișarea casetei de dialog la închidere, a selectat utilizatorul „Continuare” pentru a închide?

#### <a name="officepowerpointdocoperationnewdocument"></a>Office.PowerPoint.DocOperation.NewDocument

Colectat când PowerPoint creează o prezentare nouă. Include măsurători de eroare și succes și performanță.

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

  - **Data\_Doc\_ChunkingType:long -** cum este stocat documentul în SharePoint

  - **Data\_Doc\_EdpState:long -** starea Enterprise Data Protection a documentului

  - **Data\_Doc\_Ext:string -** extensia documentului

  - **Data\_Doc\_Extension:string -** extensia documentului

  - **Data\_Doc\_FileFormat:long -** set predefinit de valori pentru formatul fișierului (mai granular decât extensia)

  - **Data\_Doc\_Fqdn:string -** unde este stocat documentul (SharePoint.com, live.net), disponibil numai pentru domeniile Office 365

  - **Data\_Doc\_FqdnHash:string -** codul hash al locului unde este stocat documentul

  - **Data\_Doc\_IdentityTelemetryId:string - **GUID unic al utilizatorului

  - **Data\_Doc\_IdentityUniqueId:string -** identificator unic al identității folosite pentru acțiunea Documente partajate

  - **Data\_Doc\_IOFlags:long -** bitmask pentru diferite semnalizări legate de IO pentru un anumit document

  - **Data\_Doc\_IrmRights:long -** set predefinit de valori pentru tipul de Information Rights Management aplicat pentru acest document (Redirecționare, Răspuns, SecureReader, Editare etc.)

  - **Data\_Doc\_IsCloudCollabEnabled:bool -** true dacă antetul „IsCloudCollabEnabled” a fost deja primit dintr-o solicitare OPTIONS.

  - **Data\_Doc\_IsIncrementalOpen:bool -** documentul a fost deschis incremental (caracteristică nouă care deschide documentul fără să-l descarce în totalitate)

  - **Data\_Doc\_IsOcsSupported:bool -** dacă documentul acceptă elaborarea în comun folosind noul serviciu OCS

  - **Data\_Doc\_IsOpeningOfflineCopy:bool -** documentul este deschis din memoria cache locală?

  - **Data_Doc_IsRtcAlwaysOn -** true în cazul în care canalul în timp real (RTC) este întotdeauna activat pentru acest fișier.

  - **Data\_Doc\_IsSyncBacked:bool -** dacă documentul este deschis din folderul care folosește aplicația de sincronizare inversă OneDrive

  - **Data\_Doc\_Location:long -** set predefinit de valori privind locul de stocare a documentului (Local, SharePoint, WOPI, Rețea etc.)

  - **Data\_Doc\_LocationDetails:long -** set predefinit de valori privind locația mai detaliată (folderul Temp, folderul de descărcări, Documente OneDrive, Imagini OneDrive etc.)

  - **Data\_Doc\_NumberCoAuthors:long -** numărul de coautori la momentul deschiderii unui document

  - **Data\_Doc\_PasswordFlags:long -** set predefinit de valori privind modul în care documentul este criptat cu o parolă (Fără, parolă pentru citire, parolă pentru editare)-

  - **Data\_Doc\_ReadOnlyReasons:long -** set predefinit de valori privind motivul pentru care acest document a fost marcat doar în citire (blocat pe server, document final, protejat prin parolă pentru editare etc.)

  - **Data\_Doc\_ResourceIdHash:string -** codul hash al identificatorului de resurse pentru documentele stocate în cloud

  - **Data\_Doc\_ServerDocId:string -** identificatorul invariabil pentru documentele stocate în cloud

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

  - **Data\_FailureReason:long -** set predefinit de valori privind motivul nereușitei (FileIsCorrupt, BlockedByAntivirus etc.)

  - **Data_FullDownloadRoundTripCount:long -** numărul de trasee dus-întors la server necesare pentru a descărca întregul document.
  
  - **Data_IsProtocolRunInIncOpenMode:bool -** a fost protocolul de execuție pentru o descărcare incrementală, care este o descărcare în care s-au descărcat părți ale documentului după o afișare inițială pentru utilizator.

  - **Data\_MethodId:long -** în plan intern, ce linie de cod a fost executată ultima

  - **Data\_StopwatchDuration:long -** timpul total al activității

  - **Data\_TimeToEdit:long -** timpul necesar pentru ca documentul să devină editabil

  - **Data\_TimeToView:long -** timpul necesar pentru ca primul diapozitiv al documentului să fie redat

  - **Data\_UnhandledException:bool -** orice excepție nativă netratată?

#### <a name="officepowerpointdocoperationsave"></a>Office.PowerPoint.DocOperation.Save

Colectată ori de câte ori PowerPoint efectuează o salvare utilizând calea de cod modernă. Include tipul de rezultat, succes sau eșec, al măsurătorilor performanței de salvare și metadatele relevante ale documentului.  Erorile de salvare pot duce la pierderea unor date. Microsoft utilizează aceste date pentru a garanta faptul că această caracteristică funcționează conform așteptărilor, iar conținutul utilizatorilor a persistat cu succes.

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

  - **Data\_Doc\_ChunkingType:long -** cum este stocat documentul în SharePoint

  - **Data\_Doc\_EdpState:long -** starea Enterprise Data Protection a documentului

  - **Data\_Doc\_Ext:string -** extensia documentului

  - **Data\_Doc\_Extension:string -** extensia documentului

  - **Data\_Doc\_FileFormat:long -** set predefinit de valori pentru formatul fișierului (mai granular decât extensia)

  - **Data\_Doc\_Fqdn:string -** unde este stocat documentul (SharePoint.com, live.net), disponibil numai pentru domeniile Office 365

  - **Data\_Doc\_FqdnHash:string -** codul hash al locului unde este stocat documentul

  - **Data\_Doc\_IdentityTelemetryId:string - **GUID unic al utilizatorului

  - **Data\_Doc\_IdentityUniqueId:string -** identificator unic al identității folosite pentru acțiunea Documente partajate

  - **Data\_Doc\_IOFlags:long -** bitmask pentru diferite semnalizări legate de IO pentru un anumit document

  - **Data\_Doc\_IrmRights:long -** set predefinit de valori pentru tipul de Information Rights Management aplicat pentru acest document (Redirecționare, Răspuns, SecureReader, Editare etc.)

  - **Data\_Doc\_IsCloudCollabEnabled:bool -** true dacă antetul „IsCloudCollabEnabled” a fost deja primit dintr-o solicitare OPTIONS.

  - **Data\_Doc\_IsIncrementalOpen:bool -** documentul a fost deschis incremental (caracteristică nouă care deschide documentul fără să-l descarce în totalitate)

  - **Data\_Doc\_IsOcsSupported:bool -** dacă documentul acceptă elaborarea în comun folosind noul serviciu OCS

  - **Data\_Doc\_IsOpeningOfflineCopy:bool -** verifică dacă documentul este deschis din memoria cache locală

  - **Data_Doc_IsRtcAlwaysOn -** true în cazul în care canalul în timp real (RTC) este întotdeauna activat pentru acest fișier.

  - **Data\_Doc\_IsSyncBacked:bool -** dacă documentul este deschis din folderul care folosește aplicația de sincronizare inversă OneDrive

  - **Data\_Doc\_Location:long -** set predefinit de valori privind locul de stocare a documentului (Local, SharePoint, WOPI, Rețea etc.)

  - **Data\_Doc\_LocationDetails:long -** set predefinit de valori privind locația mai detaliată (folderul Temp, folderul de descărcări, Documente OneDrive, Imagini OneDrive etc.)

  - **Data\_Doc\_NumberCoAuthors:long -** numărul de coautori la momentul deschiderii unui document

  - **Data\_Doc\_PasswordFlags:long -** set predefinit de valori privind modul în care documentul este criptat cu o parolă (Fără, parolă pentru citire, parolă pentru editare)

  - **Data\_Doc\_ReadOnlyReasons:long -** set predefinit de valori privind motivul pentru care acest document a fost marcat doar în citire (blocat pe server, document final, protejat prin parolă pentru editare etc.)

  - **Data\_Doc\_ResourceIdHash:string -** codul hash al identificatorului de resurse pentru documentele stocate în cloud

  - **Data\_Doc\_ServerDocId:string -** identificatorul invariabil pentru documentele stocate în cloud

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

  - **Data\_FailureReason:long -** set predefinit de valori privind motivul nereușitei (FileIsCorrupt, BlockedByAntivirus etc.)

  - **Data\_fLifeguarded:bool -** a fost documentul vreodată protejat (caracteristică pentru a remedia erorile din documente, fără a-i adresa solicitări utilizatorului)?

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

Colectat ori de câte ori PowerPoint efectuează o Salvare ca. Include tipul de rezultat, succes sau eșec, al măsurătorilor performanței de salvare și metadatele relevante ale documentului. Erorile de salvare pot duce la pierderea unor date.

Microsoft utilizează aceste date pentru a garanta faptul că această caracteristică funcționează conform așteptărilor, iar conținutul utilizatorilor a persistat cu succes.

Se colectează următoarele câmpuri:

  - **Data\_AddDocTelemetryResult:long -** această intrare în jurnal are toate datele de telemetrie necesare pentru documente (câmpurile Data\_Doc\_\*)? Dacă nu, de ce?

  - **Data\_CppUncaughtExceptionCount:long -** excepții native neprinse în timp ce rula activitatea

  - **Data\_DetachedDuration:long -** timpul cât activitatea a fost detașată/nu a rulat

  - **Data\_DstDoc\_AccessMode:long -** cum a fost deschis acest document (doar în citire | citire-scriere)

  - **Data\_DstDoc\_AssistedReadingReasons:long -** set predefinit de valori pentru care documentul a fost deschis în modul de citire asistată

  - **Data\_DstDoc\_ChunkingType:long -** cum este stocat documentul în SharePoint

  - **Data\_DstDoc\_EdpState:long -** starea Enterprise Data Protection a documentului

  - **Data\_DstDoc\_Ext:string -** extensia documentului

  - **Data\_DstDoc\_Extension:string -** extensia documentului

  - **Data\_DstDoc\_FileFormat:long -** set predefinit de valori pentru formatul fișierului (mai granular decât extensia)

  - **Data\_DstDoc\_Fqdn:string -** unde este stocat documentul (SharePoint.com, live.net), disponibil numai pentru domeniile Office 365

  - **Data\_DstDoc\_FqdnHash:string -** codul hash al locului unde este stocat documentul

  - **Data\_DstDoc\_IdentityTelemetryId:string - **GUID unic al utilizatorului

  - **Data\_DstDoc\_IdentityUniqueId:string -** identificator unic al identității folosite pentru acțiunea Documente partajate

  - **Data\_DstDoc\_IOFlags:long -** bitmask pentru diferite semnalizări legate de IO pentru un anumit document

  - **Data\_DstDoc\_IrmRights:long -** set predefinit de valori pentru tipul de Information Rights Management aplicat pentru acest document (Redirecționare, Răspuns, SecureReader, Editare etc.)

  - **Data\_DstDoc\_IsCloudCollabEnabled:bool -** true dacă antetul „IsCloudCollabEnabled” a fost deja primit dintr-o solicitare OPTIONS.

  - **Data\_DstDoc\_IsIncrementalOpen:bool -** documentul a fost deschis incremental (caracteristică nouă care deschide documentul fără să-l descarce în totalitate)

  - **Data\_DstDoc\_IsOcsSupported:bool -** dacă documentul acceptă elaborarea în comun folosind noul serviciu OCS

  - **Data\_DstDoc\_IsOpeningOfflineCopy:bool -** verifică dacă documentul este deschis din memoria cache locală

  - **Data\_DstDoc\_IsSyncBacked:bool -** dacă documentul este deschis din folderul care folosește aplicația de sincronizare inversă OneDrive

  - **Data\_DstDoc\_Location:long -** set predefinit de valori privind locul de stocare a documentului (Local, SharePoint, WOPI, Rețea etc.)

  - **Data\_DstDoc\_LocationDetails:long -** set predefinit de valori privind locația mai detaliată (folderul Temp, folderul de descărcări, Documente OneDrive, Imagini OneDrive etc.)

  - **Data\_DstDoc\_NumberCoAuthors:long -** numărul de coautori la momentul deschiderii unui document

  - **Data\_DstDoc\_PasswordFlags:long -** set predefinit de valori privind modul în care documentul este criptat cu o parolă (Fără, parolă pentru citire, parolă pentru editare)

  - **Data\_DstDoc\_ReadOnlyReasons:long -** set predefinit de valori privind motivul pentru care acest document a fost marcat doar în citire (blocat pe server, document final, protejat prin parolă pentru editare etc.)

  - **Data\_DstDoc\_ResourceIdHash:string -** codul hash al identificatorului de resurse pentru documentele stocate în cloud

  - **Data\_DstDoc\_ServerDocId:string -** identificatorul invariabil pentru documentele stocate în cloud

  - **Data\_DstDoc\_ServerProtocol:long -** set predefinit de valori privind protocolul folosit în comunicarea cu serverul (Http, Cobalt, WOPI etc.)

  - **Data\_DstDoc\_ServerType:long -** set predefinit de valori privind tipul serverului (SharePoint, DropBox, WOPI)

  - **Data\_DstDoc\_ServerVersion:long -** dacă serverul se bazează pe Office14, Office15, Office 16

  - **Data\_DstDoc\_SessionId:long -** GUID generat care identifică instanța documentului din aceeași sesiune de proces

  - **Data\_DstDoc\_SharePointServiceContext:string -** un șir opac, de obicei GridManagerID.FarmID. Util pentru corelarea jurnalelor de la client și de pe server

  - **Data\_DstDoc\_SizeInBytes:long -** dimensiunea documentului în octeți

  - **Data\_DstDoc\_SpecialChars:long -** Bitmask ce arată caracterele speciale din adresa URL sau calea documentului

  - **Data\_DstDoc\_StorageProviderId:string -** șir care identifică furnizorul de stocare al documentului, precum „DropBox”

  - **Data\_DstDoc\_StreamAvailability:long -** set predefinit de valori privind starea șirului de document (disponibil, dezactivat definitiv, indisponibil)

  - **Data\_DstDoc\_UrlHash:string -** codul hash pentru adresa URL completă a documentelor stocate în cloud

  - **Data\_DstDoc\_UsedWrsDataOnOpen:bool -** true dacă fișierul a fost deschis incremental folosind datele WRS prememorate în cache pentru gazdă

  - **Data\_DstDoc\_WopiServiceId:string -** identificatorul serviciului WOPI, de ex. „Dropbox”

  - **Data\_FileType:long -** set predefinit de valori al tipului de fișier intern

  - **Data\_fLifeguarded:bool -** a fost documentul vreodată protejat (caracteristică pentru a remedia erorile din documente, fără a-i adresa solicitări utilizatorului)?

  - **Data\_FWebCreated:bool -** are acest document o semnalizare WebCreator?

  - **Data\_SaveReason:long -** set predefinit de valori privind motivul pentru care s-a efectuat această salvare (AutoSave, ToOCSTransitionSave, ToCSITransitionSave etc.)

  - **Data\_SaveType:long -** set predefinit de valori privind tipul de salvare (Salvare ca, Publicare, Manual, Salvare OM etc.)

  - **Data\_SrcDoc\_AccessMode:long -** cum a fost deschis acest document (doar în citire | citire-scriere)

  - **Data\_SrcDoc\_AssistedReadingReasons:long -** set predefinit de valori pentru care documentul a fost deschis în modul de citire asistată

  - **Data\_SrcDoc\_ChunkingType:long -** cum este stocat documentul în SharePoint

  - **Data\_SrcDoc\_EdpState:long -** starea Enterprise Data Protection a documentului

  - **Data\_SrcDoc\_Ext:string -** extensia documentului

  - **Data\_SrcDoc\_Extension:string -** extensia documentului

  - **Data\_SrcDoc\_FileFormat:long -** set predefinit de valori pentru formatul fișierului (mai granular decât extensia)

  - **Data\_SrcDoc\_Fqdn:string -** unde este stocat documentul (SharePoint.com, live.net), disponibil numai pentru domeniile Office 365

  - **Data\_SrcDoc\_FqdnHash:string -** codul hash al locului unde este stocat documentul

  - **Data\_SrcDoc\_IdentityTelemetryId:string - **GUID unic al utilizatorului

  - **Data\_SrcDoc\_IdentityUniqueId:string -** identificator unic al identității folosite pentru acțiunea Documente partajate

  - **Data\_SrcDoc\_IOFlags:long -** bitmask pentru diferite semnalizări legate de IO pentru un anumit document

  - **Data\_SrcDoc\_IrmRights:long -** set predefinit de valori pentru tipul de Information Rights Management aplicat pentru acest document (Redirecționare, Răspuns, SecureReader, Editare etc.)

  - **Data\_SrcDoc\_IsCloudCollabEnabled:bool -** true dacă antetul „IsCloudCollabEnabled” a fost deja primit dintr-o solicitare OPTIONS.

  - **Data\_SrcDoc\_IsIncrementalOpen:bool -** documentul a fost deschis incremental (caracteristică nouă care deschide documentul fără să-l descarce în totalitate)

  - **Data\_SrcDoc\_IsOcsSupported:bool -** dacă documentul acceptă elaborarea în comun folosind noul serviciu OCS

  - **Data\_SrcDoc\_IsOpeningOfflineCopy:bool -** verifică dacă documentul este deschis din memoria cache locală

  - **Data\_SrcDoc\_IsSyncBacked:bool -** dacă documentul este deschis din folderul care folosește aplicația de sincronizare inversă OneDrive

  - **Data\_SrcDoc\_Location:long -** set predefinit de valori privind locul de stocare a documentului (Local, SharePoint, WOPI, Rețea etc.)

  - **Data\_SrcDoc\_LocationDetails:long -** set predefinit de valori privind locația mai detaliată (folderul Temp, folderul de descărcări, Documente OneDrive, Imagini OneDrive etc.)

  - **Data\_SrcDoc\_NumberCoAuthors:long -** numărul de coautori la momentul deschiderii unui document

  - **Data\_SrcDoc\_PasswordFlags:long -** set predefinit de valori privind modul în care documentul este criptat cu o parolă (Fără, parolă pentru citire, parolă pentru editare)

  - **Data\_SrcDoc\_ReadOnlyReasons:long -** set predefinit de valori privind motivul pentru care acest document a fost marcat doar în citire (blocat pe server, document final, protejat prin parolă pentru editare etc.)

  - **Data\_SrcDoc\_ResourceIdHash:string -** codul hash al identificatorului de resurse pentru documentele stocate în cloud

  - **Data\_SrcDoc\_ServerDocId:string -** identificatorul invariabil pentru documentele stocate în cloud

  - **Data\_SrcDoc\_ServerProtocol:long -** set predefinit de valori privind protocolul folosit în comunicarea cu serverul (Http, Cobalt, WOPI etc.)

  - **Data\_SrcDoc\_ServerType:long -** set predefinit de valori privind tipul serverului (SharePoint, DropBox, WOPI)

  - **Data\_SrcDoc\_ServerVersion:long -** verifică dacă serverul se bazează pe Office14, Office15 sau Office 16Data\_SrcDoc\_SessionId:long GUID generat care identifică instanța documentului din aceeași sesiune de proces

  - **Data\_SrcDoc\_SharePointServiceContext:string -** un șir opac, de obicei GridManagerID.FarmID. Util pentru corelarea jurnalelor de la client și de pe server

  - **Data\_SrcDoc\_SizeInBytes:long -** dimensiunea documentului în byți

  - **Data\_SrcDoc\_SpecialChars:long -** Bitmask ce arată caracterele speciale din adresa URL sau calea documentului

  - **Data\_SrcDoc\_StorageProviderId:string -** șir care identifică furnizorul de stocare al documentului, precum „DropBox”

  - **Data\_SrcDoc\_StreamAvailability:long -** set predefinit de valori privind starea șirului de document (disponibil, dezactivat definitiv, indisponibil)

  - **Data\_SrcDoc\_UrlHash:string -** codul hash pentru adresa URL completă a documentelor stocate în cloud

  - **Data\_SrcDoc\_UsedWrsDataOnOpen:bool -** true dacă fișierul a fost deschis incremental folosind datele WRS prememorate în cache pentru gazdă

  - **Data\_SrcDoc\_WopiServiceId:string -** identificatorul serviciului WOPI, de ex. „Dropbox”

  - **Data\_StopwatchDuration:long -** timpul total al activității

  - **Data\_TypeOfSaveDialog:long -** set predefinit de valori ale casetei de dialog (RUN\_SAVEAS\_DLG, RUN\_SAVEMEDIA\_DLG, RUN\_SAVEAS\_VIDEO\_DLG etc.)

  - **DstDoc -** noua locație a documentului

  - **SrcDoc -** locația inițială a documentului

#### <a name="officepowerpointdocoperationsavelegacy"></a>Office.PowerPoint.DocOperation.SaveLegacy

Colectat ori de câte ori PowerPoint efectuează o salvare utilizând calea de cod moștenită. Include tipul de rezultat, succes sau eșec, al măsurătorilor performanței de salvare și metadatele relevante ale documentului. Erorile de salvare pot duce la pierderea unor date. Microsoft utilizează aceste date pentru a garanta faptul că această caracteristică funcționează conform așteptărilor, iar conținutul utilizatorilor a persistat cu succes.

Se colectează următoarele câmpuri:

  - **Data\_AddDocTelemetryResult:long -** această intrare în jurnal are toate datele de telemetrie necesare pentru documente (câmpurile Data\_Doc\_\*)? Dacă nu, de ce?

  - **Data\_CppUncaughtExceptionCount:long -** excepții native neprinse în timp ce rula activitatea

  - **Data\_DetachedDuration:long -** timpul cât activitatea a fost detașată/nu a rulat

  - **Data\_Doc\_AccessMode:long -** cum a fost deschis acest document (doar în citire | citire-scriere)

  - **Data\_Doc\_AssistedReadingReasons:long -** set predefinit de valori pentru care documentul a fost deschis în modul de citire asistată

  - **Data\_Doc\_ChunkingType:long -** cum este stocat documentul în SharePoint

  - **Data\_Doc\_EdpState:long -** starea Enterprise Data Protection a documentului

  - **Data\_Doc\_Ext:string -** extensia documentului

  - **Data\_Doc\_Extension:string -** extensia documentului

  - **Data\_Doc\_FileFormat:long -** set predefinit de valori pentru formatul fișierului (mai granular decât extensia)

  - **Data\_Doc\_Fqdn:string -** unde este stocat documentul (SharePoint.com, live.net), disponibil numai pentru domeniile Office 365

  - **Data\_Doc\_FqdnHash:string -** codul hash al locului unde este stocat documentul

  - **Data\_Doc\_IdentityTelemetryId:string - **GUID unic al utilizatorului

  - **Data\_Doc\_IdentityUniqueId:string -** identificator unic al identității folosite pentru acțiunea Documente partajate

  - **Data\_Doc\_IOFlags:long -** bitmask pentru diferite semnalizări legate de IO pentru un anumit document

  - **Data\_Doc\_IrmRights:long -** set predefinit de valori pentru tipul de Information Rights Management aplicat pentru acest document (Redirecționare, Răspuns, SecureReader, Editare etc.)

  - **Data\_Doc\_IsCloudCollabEnabled:bool -** true dacă antetul „IsCloudCollabEnabled” a fost deja primit dintr-o solicitare OPTIONS.

  - **Data\_Doc\_IsIncrementalOpen:bool -** documentul a fost deschis incremental (caracteristică nouă care deschide documentul fără să-l descarce în totalitate)

  - **Data\_Doc\_IsOcsSupported:bool -** dacă documentul acceptă elaborarea în comun folosind noul serviciu OCS

  - **Data\_Doc\_IsOpeningOfflineCopy:bool -** verifică dacă documentul este deschis din memoria cache locală

  - **Data_Doc_IsRtcAlwaysOn -** true în cazul în care canalul în timp real (RTC) este întotdeauna activat pentru acest fișier.

  - **Data\_Doc\_IsSyncBacked:bool -** dacă documentul este deschis din folderul care folosește aplicația de sincronizare inversă OneDrive

  - **Data\_Doc\_Location:long -** set predefinit de valori privind locul de stocare a documentului (Local, SharePoint, WOPI, Rețea etc.)

  - **Data\_Doc\_LocationDetails:long -** set predefinit de valori privind locația mai detaliată (folderul Temp, folderul de descărcări, Documente OneDrive, Imagini OneDrive etc.)

  - **Data\_Doc\_NumberCoAuthors:long -** numărul de coautori la momentul deschiderii unui document

  - **Data\_Doc\_PasswordFlags:long -** set predefinit de valori privind modul în care documentul este criptat cu o parolă (Fără, parolă pentru citire, parolă pentru editare)

  - **Data\_Doc\_ReadOnlyReasons:long -** set predefinit de valori privind motivul pentru care acest document a fost marcat doar în citire (blocat pe server, document final, protejat prin parolă pentru editare etc.)

  - **Data\_Doc\_ResourceIdHash:string -** codul hash al identificatorului de resurse pentru documentele stocate în cloud

  - **Data\_Doc\_ServerDocId:string -** identificatorul invariabil pentru documentele stocate în cloud

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

  - **Data\_DstDoc\_AccessMode:long -** cum a fost deschis acest document (doar în citire | citire-scriere)

  - **Data\_DstDoc\_AssistedReadingReasons:long -** set predefinit de valori pentru care documentul a fost deschis în modul de citire asistată

  - **Data\_DstDoc\_ChunkingType:long -** cum este stocat documentul în SharePoint

  - **Data\_DstDoc\_EdpState:long -** starea Enterprise Data Protection a documentului

  - **Data\_DstDoc\_Ext:string -** extensia documentului

  - **Data\_DstDoc\_Extension:string -** extensia documentului

  - **Data\_DstDoc\_FileFormat:long -** set predefinit de valori pentru formatul fișierului (mai granular decât extensia)

  - **Data\_DstDoc\_Fqdn:string -** unde este stocat documentul (SharePoint.com, live.net), disponibil numai pentru domeniile Office 365

  - **Data\_DstDoc\_FqdnHash:string -** codul hash al locului unde este stocat documentul

  - **Data\_DstDoc\_IdentityTelemetryId:string - **GUID unic al utilizatorului

  - **Data\_DstDoc\_IdentityUniqueId:string -** identificator unic al identității folosite pentru acțiunea Documente partajate

  - **Data\_DstDoc\_IOFlags:long -** bitmask pentru diferite semnalizări legate de IO pentru un anumit document

  - **Data\_DstDoc\_IrmRights:long -** set predefinit de valori pentru tipul de Information Rights Management aplicat pentru acest document (Redirecționare, Răspuns, SecureReader, Editare etc.)

  - **Data\_DstDoc\_IsCloudCollabEnabled:bool -** true dacă antetul „IsCloudCollabEnabled” a fost deja primit dintr-o solicitare OPTIONS.

  - **Data\_DstDoc\_IsIncrementalOpen:bool -** documentul a fost deschis incremental (caracteristică nouă care deschide documentul fără să-l descarce în totalitate)

  - **Data\_DstDoc\_IsOcsSupported:bool -** dacă documentul acceptă elaborarea în comun folosind noul serviciu OCS

  - **Data\_DstDoc\_IsOpeningOfflineCopy:bool -** verifică dacă documentul este deschis din memoria cache locală

  - **Data\_DstDoc\_IsSyncBacked:bool -** dacă documentul este deschis din folderul care folosește aplicația de sincronizare inversă OneDrive

  - **Data\_DstDoc\_Location:long -** set predefinit de valori privind locul de stocare a documentului (Local, SharePoint, WOPI, Rețea etc.)

  - **Data\_DstDoc\_LocationDetails:long -** set predefinit de valori privind locația mai detaliată (folderul Temp, folderul de descărcări, Documente OneDrive, Imagini OneDrive etc.)

  - **Data\_DstDoc\_NumberCoAuthors:long -** numărul de coautori la momentul deschiderii unui document

  - **Data\_DstDoc\_PasswordFlags:long-** set predefinit de valori privind modul în care documentul este criptat cu o parolă (Fără, parolă pentru citire, parolă pentru editare)

  - **Data\_DstDoc\_ReadOnlyReasons:long -** set predefinit de valori privind motivul pentru care acest document a fost marcat doar în citire (blocat pe server, document final, protejat prin parolă pentru editare etc.)

  - **Data\_DstDoc\_ResourceIdHash:string -** codul hash al identificatorului de resurse pentru documentele stocate în cloud

  - **Data\_DstDoc\_ServerDocId:string -** identificatorul invariabil pentru documentele stocate în cloud

  - **Data\_DstDoc\_ServerProtocol:long -** set predefinit de valori privind protocolul folosit în comunicarea cu serverul (Http, Cobalt, WOPI etc.)

  - **Data\_DstDoc\_ServerType:long -** set predefinit de valori privind tipul serverului (SharePoint, DropBox, WOPI)

  - **Data\_DstDoc\_ServerVersion:long -** dacă serverul se bazează pe Office14, Office15, Office 16

  - **Data\_DstDoc\_SessionId:long -** GUID generat care identifică instanța documentului din aceeași sesiune de proces

  - **Data\_DstDoc\_SharePointServiceContext:string -** un șir opac, de obicei GridManagerID.FarmID. Util pentru corelarea jurnalelor de la client și de pe server

  - **Data\_DstDoc\_SizeInBytes:long -** dimensiunea documentului în octeți

  - **Data\_DstDoc\_SpecialChars:long -** Bitmask ce arată caracterele speciale din adresa URL sau calea documentului

  - **Data\_DstDoc\_StorageProviderId:string -** șir care identifică furnizorul de stocare al documentului, precum „DropBox”

  - **Data\_DstDoc\_StreamAvailability:long -** set predefinit de valori privind starea șirului de document (disponibil, dezactivat definitiv, indisponibil)

  - **Data\_DstDoc\_UrlHash:string -** codul hash pentru adresa URL completă a documentelor stocate în cloud

  - **Data\_DstDoc\_UsedWrsDataOnOpen:bool -** true dacă fișierul a fost deschis incremental folosind datele WRS prememorate în cache pentru gazdă

  - **Data\_DstDoc\_WopiServiceId:string -** identificatorul serviciului WOPI, de ex. „Dropbox”

  - **Data\_FileType:long -** set predefinit de valori al tipului de fișier intern

  - **Data\_fLifeguarded:bool -** a fost documentul vreodată protejat (caracteristică pentru a remedia erorile din documente, fără a-i adresa solicitări utilizatorului)?

  - **Data\_SaveReason:long -** set predefinit de valori privind motivul pentru care s-a efectuat această salvare (AutoSave, ToOCSTransitionSave, ToCSITransitionSave etc.)

  - **Data\_SaveType:long -** set predefinit de valori privind tipul de salvare (Salvare ca, Publicare, Manual, Salvare OM etc.)

  - **Data\_SrcDoc\_AccessMode:long -** cum a fost deschis acest document (doar în citire | citire-scriere)

  - **Data\_SrcDoc\_AssistedReadingReasons:long -** set predefinit de valori pentru care documentul a fost deschis în modul de citire asistată

  - **Data\_SrcDoc\_ChunkingType:long -** cum este stocat documentul în SharePoint

  - **Data\_SrcDoc\_EdpState:long -** starea Enterprise Data Protection a documentului

  - **Data\_SrcDoc\_Ext:string -** extensia documentului

  - **Data\_SrcDoc\_Extension:string -** extensia documentului

  - **Data\_SrcDoc\_FileFormat:long -** set predefinit de valori pentru formatul fișierului (mai granular decât extensia)

  - **Data\_SrcDoc\_Fqdn:string -** unde este stocat documentul (SharePoint.com, live.net), disponibil numai pentru domeniile Office 365

  - **Data\_SrcDoc\_FqdnHash:string -** codul hash al locului unde este stocat documentul

  - **Data\_SrcDoc\_IdentityTelemetryId:string - **GUID unic al utilizatorului

  - **Data\_SrcDoc\_IdentityUniqueId:string -** identificator unic al identității folosite pentru acțiunea Documente partajate

  - **Data\_SrcDoc\_IOFlags:long -** bitmask pentru diferite semnalizări legate de IO pentru un anumit document

  - **Data\_SrcDoc\_IrmRights:long -** set predefinit de valori pentru tipul de Information Rights Management aplicat pentru acest document (Redirecționare, Răspuns, SecureReader, Editare etc.)

  - **Data\_SrcDoc\_IsCloudCollabEnabled:bool -** true dacă antetul „IsCloudCollabEnabled” a fost deja primit dintr-o solicitare OPTIONS.

  - **Data\_SrcDoc\_IsIncrementalOpen:bool -** documentul a fost deschis incremental (caracteristică nouă care deschide documentul fără să-l descarce în totalitate)

  - **Data\_SrcDoc\_IsOcsSupported:bool -** dacă documentul acceptă elaborarea în comun folosind noul serviciu OCS

  - **Data\_SrcDoc\_IsOpeningOfflineCopy:bool -** verifică dacă documentul este deschis din memoria cache locală

  - **Data\_SrcDoc\_IsSyncBacked:bool -** dacă documentul este deschis din folderul care folosește aplicația de sincronizare inversă OneDrive

  - **Data\_SrcDoc\_Location:long -** set predefinit de valori privind locul de stocare a documentului (Local, SharePoint, WOPI, Rețea etc.)

  - **Data\_SrcDoc\_LocationDetails:long -** set predefinit de valori privind locația mai detaliată (folderul Temp, folderul de descărcări, Documente OneDrive, Imagini OneDrive etc.)

  - **Data\_SrcDoc\_NumberCoAuthors:long -** numărul de coautori la momentul deschiderii unui document

  - **Data\_SrcDoc\_PasswordFlags:long-** set predefinit de valori privind modul în care documentul este criptat cu o parolă (Fără, parolă pentru citire, parolă pentru editare)

  - **Data\_SrcDoc\_ReadOnlyReasons:long -** set predefinit de valori privind motivul pentru care acest document a fost marcat doar în citire (blocat pe server, document final, protejat prin parolă pentru editare etc.)

  - **Data\_SrcDoc\_ResourceIdHash:string -** codul hash al identificatorului de resurse pentru documentele stocate în cloud

  - **Data\_SrcDoc\_ServerDocId:string -** identificatorul invariabil pentru documentele stocate în cloud

  - **Data\_SrcDoc\_ServerProtocol:long -** set predefinit de valori privind protocolul folosit în comunicarea cu serverul (Http, Cobalt, WOPI etc.)

  - **Data\_SrcDoc\_ServerType:long -** set predefinit de valori privind tipul serverului (SharePoint, DropBox, WOPI)

  - **Data\_SrcDoc\_ServerVersion:long ** dacă serverul se bazează pe Office14, Office15, Office 16

  - **Data\_SrcDoc\_SessionId:long -** GUID generat care identifică instanța documentului din aceeași sesiune de proces

  - **Data\_SrcDoc\_SharePointServiceContext:string -** un șir opac, de obicei GridManagerID.FarmID. Util pentru corelarea jurnalelor de la client și de pe server

  - **Data\_SrcDoc\_SizeInBytes:long -** dimensiunea documentului în byți

  - **Data\_SrcDoc\_SpecialChars:long -** Bitmask ce arată caracterele speciale din adresa URL sau calea documentului

  - **Data\_SrcDoc\_StorageProviderId:string -** șir care identifică furnizorul de stocare al documentului, precum „DropBox”

  - **Data\_SrcDoc\_StreamAvailability:long -** set predefinit de valori privind starea șirului de document (disponibil, dezactivat definitiv, indisponibil)

  - **Data\_SrcDoc\_UrlHash:string -** codul hash pentru adresa URL completă a documentelor stocate în cloud

  - **Data\_SrcDoc\_UsedWrsDataOnOpen:bool -** true dacă fișierul a fost deschis incremental folosind datele WRS prememorate în cache pentru gazdă

  - **Data\_SrcDoc\_WopiServiceId:string -** identificatorul serviciului WOPI, de ex. „Dropbox”

  - **Data\_StopwatchDuration:long -** timpul total al activității

  - **Data\_TypeOfSaveDialog:long -** set predefinit de valori ale casetei de dialog (RUN\_SAVEAS\_DLG, RUN\_SAVEMEDIA\_DLG, RUN\_SAVEAS\_VIDEO\_DLG etc.)

  - **Doc -** document curent pentru Salvare

  - **DstDoc -** noua locație a documentului (în cazul Salvare ca)

  - **SrcDoc -** locația inițială a documentului (în cazul Salvare ca)

#### <a name="officepowerpointpptsharedslideshowfailure"></a>Office.PowerPoint.PPT.Shared.SlideShow.Failure

Colectarea erorilor în timpul expunerii de diapozitive. Expunerea de diapozitive este o caracteristică principală a PowerPoint. Microsoft colectează atunci când apare o eroare în timpul expunerii de diapozitive pentru a îmbunătăți experiența utilizatorului privind expunerea de diapozitive. Microsoft utilizează aceste date pentru a obține informații de diagnosticare privind locul unde apare eroarea în timp ce utilizatorul folosește expunerea de diapozitive

Se colectează următoarele câmpuri:

  - **CountSlideShowErrors** - numărul total de erori aferente expunerii de diapozitive

  - **CountPPTErrors** - numărul total de erori PPT

  - **CountOArtErrors** - numărul total de erori OArt

  - **CountOtherErrors** - numărul total de alte erori

  - **FirstSlideShowError** - prima eroare care a apărut în expunerea de diapozitive

  - **FirstOArtError** - prima eroare care a apărut în OArt

  - **FirstPPTError** - prima eroare care a apărut în PPT

  - **FirstOtherError** - prima eroare care a apărut în altă zonă

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

  - **Data.actionSource -** cum a fost declanșată traducerea selecției-

  - **Data.bodyBackgroundColor -** culoare de fundal container temă Office-

  - **Data.bodyForegroundColor -** culoare de prim-plan container temă Office-

  - **Data.browserLang -** limbă curentă afișaj browser-

  - **Data.browserOnline -** depășit -

  - **Data.browserPlatform -** platformă browser-

  - **Data.browserUserAgent -** agent utilizator browser-

  - **Data.colorDepth -** adâncime culoare sistem-

  - **Data.contentLanguage -** limbă detectată a conținutului de tradus-

  - **Data.controlBackgroundColor -** culoare de fundal control temă Office-

  - **Data.controlForegroundColor -** culoare de prim-plan container temă Office-

  - **Data.correlationId -** identificator unic al solicitării trimise la serviciu-

  - **Data.crossSessionId -** identificator unic al utilizatorului-

  - **Data.crossSessionStartTime -** marcă de timp UTC privind momentul în care a început sesiunea de traducere-

  - **Data.currentTime -** marcă de timp UTC privind momentul în care a fost trimis acest mesaj de telemetrie-

  - **Data.displayLanguage -** limbă afișaj Office-

  - **Data.documentSourceLang -** limbă conținut document-

  - **Data.documentTargetLang -** documentul Limbă va fi tradus în-

  - **Data.environment -** mediul de serviciu la care este trimisă solicitarea-

  - **Data.errorMessage -** mesaj de eroare raportat de serviciu-

  - **Data.eventActionType -** tip de eveniment de telemetrie-

  - **Data.eventTagId -** identificator unic al liniei de cod care a produs acest mesaj de telemetrie-

  - **Data.flights -** ediții flight activate-

  - **Data.fileSize -** dimensiunea fișierului Word de tradus-

  - **Data.fileSource -** unde este găzduit fișierul Word (offline, online)-

  - **Data.fileType -** extensia fișierului Word-

  - **Data.innerHeight"-** înălțime container panou lateral-

  - **Data.innerWidth"-** lățime container panou lateral-

  - **Data.lookupSourceLang -** neutilizat pentru traducerea documentului-

  - **Data.lookupTargetLang -** neutilizat pentru traducerea documentului 

  - **Data.officeHost -** aplicație Office care găzduiește panoul lateral-

  - **Data.officeLocale -** limbă utilizatorului Office-

  - **Data.officeMachineId-** identificator unic al dispozitivului-

  - **Data.officePlatform -** platforma dispozitivului-

  - **Data.officeSessionId -** identificator al sesiunii Office-

  - **Data.officeUserId -** identificator unic utilizator Office-

  - **Data.officeVersion -** versiune de Office-

  - **Data.pageXOffset -** poziție de defilare orizontală panoul lateral din partea stângă a panoului-

  - **Data.pageYOffset -** poziție de defilare verticală panoul lateral din partea stângă a panoului-

  - **Data.pixelDepth -** rezoluția de culori a ecranului-

  - **Data.responseCode -** cod de răspuns solicitare de la serviciu la serviciu-

  - **Data.responseTime -** timp scurs solicitare-

  - **Data.resultType -** rezultat solicitare-

  - **Data.screenHeight -** ecran înălțime în pixeli-

  - **Data.screenLeft -** coordonata orizontală a ferestrei față de ecran-

  - **Data.screenTop -** coordonata verticală a ferestrei față de ecran-

  - **Data.screenWidth -** lățime ecran în pixeli-

  - **Data.selectedTab -** care filă este selecția sau documentul selectat-

  - **Data.serverUrl -** URL serviciu de traducere-

  - **Data.sessionId -** identificator sesiune panoul lateral-

  - **Data.sessionStartTime -** marcă de timp UTC privind momentul în care a început sesiunea de traducere-

  - **Data.sourceTextHash -** codul hash al textului de tradus-

  - **Data.sourceTextLength -** lungime text de tradus-

  - **Data.sourceTextWords -** număr de cuvinte în textul de tradus-

  - **Data.warningMessage -** mesaj de avertisment raportat către serviciu-

#### <a name="officetranslatortexttranslated"></a>Office.Translator.TextTranslated

Colectează succesul sau nereușita traducerii unei selecții pe care acțiunea unui utilizator o declanșează în Translator SDX. Acest lucru este de importanță critică pentru a evalua starea caracteristicii de traducere și a reacționa la eventuale întreruperi. Utilizat pentru a monitoriza starea de funcționare a scenariului „Traducere selecție” în Excel, PowerPoint, Word.

Se colectează următoarele câmpuri:

  - **Data.actionSource -** cum a fost declanșată traducerea selecției

  - **Data.bodyBackgroundColor -** culoare de fundal container temă Office

  - **Data.bodyForegroundColor -** culoare de prim-plan container temă Office

  - **Data.browserLang -** limbă curentă afișaj browser

  - **Data.browserOnline -** depășit

  - **Data.browserPlatform -** platformă browser

  - **Data.browserUserAgent -** agent utilizator browser

  - **Data.colorDepth -** adâncime culoare sistem

  - **Data.contentLanguage -** limbă detectată a conținutului de tradus

  - **Data.controlBackgroundColor -** culoare de fundal control temă Office

  - **Data.controlForegroundColor -** culoare de prim-plan container temă Office

  - **Data.correlationId -** identificator unic al solicitării trimise la serviciu

  - **Data.crossSessionId -** identificator unic al utilizatorului

  - **Data.crossSessionStartTime -** marcă de timp UTC privind momentul în care a început sesiunea de traducere

  - **Data.currentTime -** marcă de timp UTC privind momentul în care a fost trimis acest mesaj de telemetrie

  - **Data.displayLanguage -** limbă afișaj Office

  - **Data.documentSourceLang -** nu se utilizează pentru selecție

  - **Data.documentTargetLang -** nu se utilizează pentru traducere selecție

  - **Data.environment -** mediul de serviciu la care este trimisă solicitarea

  - **Data.errorMessage -** mesaj de eroare raportat de serviciu

  - **Data.eventActionType -** tip de eveniment de telemetrie

  - **Data.eventTagId"-** identificator unic al liniei de cod care a produs acest mesaj de telemetrie

  - **Data.flights -** ediții flight activate

  - **Data.innerHeight-** înălțime container panou lateral

  - **Data.innerWidth-** lățime container panou lateral

  - **Data.lookupSourceLang -** limba textului selectat în mod curent

  - **Data.lookupTargetLang -** limba textului selectat în mod curent va fi tradusă în

  - **Data.officeHost -** aplicație Office care găzduiește panoul lateral

  - **Data.officeLocale -** limbă utilizatorului Office

  - **Data.officeMachineId-** identificator unic al dispozitivului

  - **Data.officePlatform -** platforma dispozitivului

  - **Data.officeSessionId -** identificator al sesiunii Office

  - **Data.officeUserId -** identificator unic utilizator Office

  - **Data.officeVersion -** versiune de Office

  - **Data.pageXOffset -** poziție de defilare orizontală panoul lateral din partea stângă a panoului

  - **Data.pageYOffset -** poziție de defilare verticală panoul lateral din partea stângă a panoului

  - **Data.pixelDepth -** rezoluția de culori a ecranului

  - **Data.responseCode -** cod de răspuns solicitare de la serviciu la serviciu

  - **Data.responseTime -** timp scurs solicitare

  - **Data.resultType -** rezultat solicitare

  - **Data.screenHeight -** ecran înălțime în pixeli

  - **Data.screenLeft -** coordonata orizontală a ferestrei față de ecran

  - **Data.screenTop -** coordonata verticală a ferestrei față de ecran

  - **Data.screenWidth -** lățime ecran în pixeli

  - **Data.selectedTab -** care filă este selecția sau documentul selectat

  - **Data.serverUrl -** URL serviciu de traducere

  - **Data.sessionId -** identificator sesiune panoul lateral

  - **Data.sessionStartTime -** marcă de timp UTC privind momentul în care a început sesiunea de traducere

  - **Data.sourceTextHash -** codul hash al textului de tradus

  - **Data.sourceTextLength -** lungime text de tradus

  - **Data.sourceTextWords -** număr de cuvinte în textul de tradus

  - **Data.warningMessage -** mesaj de avertisment raportat către serviciu

#### <a name="officewordexperimentationdocumentstatsoncloseandsuspend"></a>Office.Word.Experimentation.DocumentStatsOnCloseAndSuspend

Acest eveniment înregistrează în jurnal statistici de document pentru fiecare document atunci când Office Word este închis sau suspendat.

Evenimentul este utilizat pentru a corela editări în document, dimensiunea etc. cu erori de salvare documente, partajare de documente și colaborare online la documente.

Se colectează următoarele câmpuri:

  - **Data\_BkmkRefCount -** referințe număr de marcaj în document

  - **Data\_CharacterCount -** numărul de caractere din document

  - **Data\_CharactersWithSpaceCount -** număr de caractere și spații din document

  - **Data\_ChartCount -** numărul de diagrame din document

  - **Data\_CitationCount -** numărul de referințe din document

  - **Data\_DocumentLocation -** arată ce serviciu a furnizat documentul (OneDrive, File Server, SharePoint etc.)

  - **Data\_ETW\_TrackbackTag -** identifică locul din cod de unde a fost declanșat acest eveniment (Închidere sau Suspendare)

  - **Data\_EndnoteDocCount -** numărul de note de final din document

  - **Data\_FootnoteDocCount -** numărul de note de subsol din document

  - **Data\_HasBibliography -** indică dacă documentul conține bibliografie

  - **Data\_HasHeader -** indică dacă documentul conține antet

  - **Data\_IsImeUsed -** indică dacă intrare Editorul de metodă de intrare a fost utilizat în document

  - **Data\_IsPageCountInProgress -** indică dacă numărul de pagini este în prezent în curs pentru document.

  - **Data\_IsTouchUsed -** indică dacă intrarea tactilă a fost utilizată în document

  - **Data\_IsTrackChangesOn -** indică dacă urmărirea modificărilor a fost activată pentru document

  - **Data\_LineCount -** numărul de linii din document

  - **Data\_MainPdod -** identificatorul documentului din procesul Office Word.

  - **Data\_PageCount -** numărul de pagini din document

  - **Data\_PageNumberFieldCount -** numărul de câmpuri număr de pagină din document

  - **Data\_ParagraphCount -** numărul de paragrafe din document

  - **Data\_PicCount -** numărul de imagini din document

  - **Data\_RsidCount -** numărul de revizuiri identificator salvare din document

  - **Data\_TocCount -** număr de cuprinsuri din document

  - **Data\_UrlHash -** cod hash unidirecțional, pentru crearea unui identificator naiv de document

  - **Data\_UserActionID -** acest câmp de date nu este utilizat (valoarea este întotdeauna 0).

  - **Data\_UserActionName -** întotdeauna „DocumentStatsOnCloseAndSuspend”

  - **Data\_UserInteractionTimeMsec -** număr de milisecunde în care utilizatorul a interacționat activ cu documentul

  - **Data\_WordCount -** numărul de cuvinte din document

#### <a name="officewordfilenewcreatenewfile"></a>Office.Word.FileNew.CreateNewFile

Acest eveniment indică faptul că un document nou este creat în Office Word și urmărește succesul sau nereușita operațiunii. Evenimentul este utilizat pentru a monitoriza dacă crearea noului document funcționează conform așteptărilor. În plus, se folosește pentru a calcula utilizatorii/dispozitivele active lunar și măsurătorile de fiabilitate cloud.

Se colectează următoarele câmpuri:

  - **Data\_DirtyState** - dacă documentul a fost creat într-o stare cu erori (cu modificări care trebuie salvate)

  - **Data\_ErrorID** - identificator de eroare în cazul unei operații nereușite

  - **Data\_MainPdod -** identificatorul documentului din timpul acestei sesiuni de proces

  - **Data\_UsesCustomTemplate** - indică dacă documentul a fost creat pornind de la un șablon particularizat

#### <a name="officewordfilesaveactcmdgosubsaveas"></a>Office.Word.FileSave.ActCmdGosubSaveAs

Acest eveniment indică faptul că un utilizator salvează modificările într-un document nou. Evenimentul monitorizează dacă salvarea într-un document nou funcționează conform așteptărilor. În plus, se folosește pentru a calcula utilizatorii/dispozitivele active lunar și măsurătorile de fiabilitate cloud.

Se colectează următoarele câmpuri:

  - **Data\_AddDocTelemRes -** raportează dacă am putut completa corect alte valori legate de telemetria documentelor din eveniment. Utilizat pentru diagnostice privind calitatea datelor.

  - **Data\_DetachedDuration -** cât timp a fost activitatea detașată de fir

  - **Data\_Doc\_AccessMode -** documentul este doar în citire/editabil

  - **Data\_Doc\_AssistedReadingReasons -** set predefinit de valori privind motivul pentru care documentul a fost deschis în modul de citire asistată

  - **Data\_Doc\_ChunkingType -** unități utilizate pentru deschiderea incrementală a documentelor

  - **Data\_Doc\_EdpState -** setare de protecție a datelor electronice pentru document

  - **Data\_Doc\_Ext -** extensia documentului (docx/xlsb/pptx etc.)

  - **Data\_Doc\_FileFormat –** versiunea de protocol pentru formatul fișierului

  - **Data\_Doc\_Fqdn -** numele de domeniu OneDrive sau SharePoint Online

  - **Data\_Doc\_FqdnHash -** codul hash într-o singură direcție pentru numele de domeniu identificabil al clientului

  - **Data\_Doc\_IOFlags -** rapoarte privind semnalizările memorate în cache folosite pentru a seta opțiunile de deschidere a solicitărilor

  - **Data\_Doc\_IdentityTelemetryId -** codul hash într-o singură direcție pentru identitatea de utilizator folosită pentru deschidere

  - **Data\_DstDoc\_InitializationScenario -** înregistrează cum a fost deschis documentul

  - **Data\_Doc\_IrmRights -** acțiunile permise de politica de protejare a datelor electronice aplicată pentru document/utilizator

  - **Data\_Doc\_IsIncrementalOpen -** semnalizare care arată că documentul a fost deschis incremental

  - **Data\_Doc\_IsOcsSupported -** semnalizare care arată că documentul este acceptat în serviciul de colaborare

  - **Data\_Doc\_IsOpeningOfflineCopy -** semnalizare care arată că s-a deschis copia offline a unui document

  - **Data_Doc_IsRtcAlwaysOn -** true în cazul în care canalul în timp real (RTC) este întotdeauna activat pentru acest fișier.

  - **Data\_Doc\_IsSyncBacked -** semnalizare care arată că pe computer există o copie sincronizată automat a documentului

  - **Data\_Doc\_Location -** arată ce serviciu a furnizat documentul (OneDrive, File Server, SharePoint etc.)

  - **Data\_Doc\_LocationDetails -** arată ce Folder cunoscut a furnizat un document stocat local

  - **Data\_Doc\_NumberCoAuthors -** numărul de alți utilizatori dintr-o sesiune de editare în colaborare

  - **Data\_Doc\_PasswordFlags -** arată semnalizările de parole pentru citire sau citire/scriere setate

  - **Data\_Doc\_ReadOnlyReasons -** motivele pentru care documentul a fost deschis doar în citire

  - **Data\_Doc\_ResourceIdHash -** un identificator de document anonimizat, folosit în diagnosticarea problemelor

  - **Data\_Doc\_ServerDocId -** un identificator de document anonimizat și invariabil, folosit în diagnosticarea problemelor

  - **Data\_Doc\_ServerProtocol -** versiunea de protocol folosită în comunicarea cu serviciul

  - **Data\_Doc\_ServerType -** tipul de server care oferă serviciul (SharePoint, OneDrive, WOPI etc.)

  - **Data\_Doc\_ServerVersion -** versiunea serverului care oferă serviciul

  - **Data\_Doc\_SessionId -** identifică o anumită sesiune de editare a documentului din sesiunea completă

  - **Data\_Doc\_SharePointServiceContext -** informații de diagnosticare din solicitările SharePoint Online

  - **Data\_Doc\_SizeInBytes -** indicator privind dimensiunea documentului

  - **Data\_Doc\_SpecialChars -** indicator privind caracterele speciale din calea sau adresa URL a documentului

  - **Data\_Doc\_StreamAvailability -** indicator care arată dacă șirul documentului este disponibil/dezactivat

  - **Data\_Doc\_SyncBackedType -** indicator privind tipul documentului (local sau bazat pe servicii)

  - **Data\_Doc\_UrlHash -** cod hash într-o singură direcție, pentru crearea unui identificator naiv de document

  - **Data\_EditorDisablingRename -** identificatorul primului editor care a provocat dezactivarea redenumirii

  - **Data\_EditorsCount -** numărul de editori din document

  - **Data\_LastLoggedTag -** etichetă unică pentru site-ul de apelare a codului folosit pentru a identifica momentele când nu reușim să încercăm salvarea de două ori (folosit pentru diagnosticarea calității datelor)

  - **Data\_MoveDisabledReason -** eroarea care dezactivează mutarea pentru document

  - **Data\_MoveFlightEnabled -** dacă este activată ediția flight pentru caracteristica de mutare

  - **Data\_RenameDisabledReason -** eroare care face redenumirea să fie dezactivată pentru document

  - **Data\_RenameFlightEnabled -** dacă este activată ediția flight pentru caracteristica de redenumire

#### <a name="officewordfilesaveactfconfirmsavedoccoreautorecoverysave"></a>Office.Word.FileSave.ActFConfirmSaveDocCoreAutoRecoverySave

Acest eveniment indică faptul că Office Word salvează un document de recuperare automată care nu a fost salvat înainte. Acesta permite ca Microsoft să detecteze erori în recuperarea automată, ceea ce este important pentru siguranța datelor din documente.

Evenimentul monitorizează dacă salvarea de recuperare automată funcționează conform așteptărilor. În plus, se folosește pentru a calcula utilizatorii/dispozitivele active lunar și măsurătorile de fiabilitate cloud.

Se colectează următoarele câmpuri:

  - **Data\_DetachedDuration -** cât timp a fost activitatea detașată de fir

  - **Data\_Doc\_AccessMode -** documentul este doar în citire/editabil

  - **Data\_Doc\_AssistedReadingReasons -** set predefinit de valori privind motivul pentru care documentul a fost deschis în modul de citire asistată

  - **Data\_Doc\_ChunkingType -** unități utilizate pentru deschiderea incrementală a documentelor

  - **Data\_Doc\_EdpState -** setare de protecție a datelor electronice pentru document

  - **Data\_Doc\_Ext -** extensia documentului (docx/xlsb/pptx etc.)

  - **Data\_Doc\_FileFormat –** versiunea de protocol pentru formatul fișierului

  - **Data\_Doc\_Fqdn -** numele de domeniu OneDrive sau SharePoint Online

  - **Data\_Doc\_FqdnHash -** codul hash într-o singură direcție pentru numele de domeniu identificabil al clientului

  - **Data\_Doc\_IdentityTelemetryId -** codul hash într-o singură direcție pentru identitatea de utilizator folosită pentru deschidere

  - **Data\_DstDoc\_InitializationScenario -** înregistrează cum a fost deschis documentul

  - **Data\_Doc\_IOFlags -** rapoarte privind semnalizările memorate în cache folosite pentru a seta opțiunile de deschidere a solicitărilor

  - **Data\_Doc\_IrmRights -** acțiunile permise de politica de protejare a datelor electronice aplicată pentru document/utilizator

  - **Data\_Doc\_IsIncrementalOpen -** semnalizare care arată că documentul a fost deschis incremental

  - **Data\_Doc\_IsOcsSupported -** semnalizare care arată că documentul este acceptat în serviciul de colaborare

  - **Data\_Doc\_IsOpeningOfflineCopy -** semnalizare care arată că s-a deschis copia offline a unui document

  - **Data_Doc_IsRtcAlwaysOn -** true în cazul în care canalul în timp real (RTC) este întotdeauna activat pentru acest fișier.

  - **Data\_Doc\_IsSyncBacked -** semnalizare care arată că pe computer există o copie sincronizată automat a documentului

  - **Data\_Doc\_Location -** arată ce serviciu a furnizat documentul (OneDrive, File Server, SharePoint etc.)

  - **Data\_Doc\_LocationDetails -** arată ce Folder cunoscut a furnizat un document stocat local

  - **Data\_Doc\_NumberCoAuthors -** numărul de alți utilizatori dintr-o sesiune de editare în colaborare

  - **Data\_Doc\_PasswordFlags -** arată semnalizările de parole pentru citire sau citire/scriere setate

  - **Data\_Doc\_ReadOnlyReasons -** motivele pentru care documentul a fost deschis doar în citire

  - **Data\_Doc\_ResourceIdHash -** un identificator de document anonimizat, folosit în diagnosticarea problemelor

  - **Data\_Doc\_ServerDocId -** un identificator de document anonimizat și invariabil, folosit în diagnosticarea problemelor

  - **Data\_Doc\_ServerProtocol -** versiunea de protocol folosită în comunicarea cu serviciul

  - **Data\_Doc\_ServerType -** tipul de server care oferă serviciul (SharePoint, OneDrive, WOPI etc.)

  - **Data\_Doc\_ServerVersion -** versiunea serverului care oferă serviciul

  - **Data\_Doc\_SessionId -** identifică o anumită sesiune de editare a documentului din sesiunea completă

  - **Data\_Doc\_SharePointServiceContext -** informații de diagnosticare din solicitările SharePoint Online

  - **Data\_Doc\_SizeInBytes -** indicator privind dimensiunea documentului

  - **Data\_Doc\_SpecialChars -** indicator privind caracterele speciale din calea sau adresa URL a documentului

  - **Data\_Doc\_StreamAvailability -** indicator care arată dacă șirul documentului este disponibil/dezactivat

  - **Data\_Doc\_SyncBackedType -** indicator privind tipul documentului (local sau bazat pe servicii)

  - **Data\_Doc\_UrlHash -** cod hash într-o singură direcție, pentru crearea unui identificator naiv de document

  - **Data\_Doc\_WopiServiceId -** conține identificatorul unic al furnizorului de servicii WOPI

  - **Data\_FailureClass -** întreg care reprezintă clasa de eroare pentru erorile de tranziție Office Collaboration Services (OCS)

  - **Data\_MainPdod -** identificatorul documentului din procesul Office Word.

  - **Data\_MoveFlightEnabled –** dacă ediția flight este activată pentru caracteristica de mutare

  - **Data\_OCSSyncbackSaveStarted –** marcaj care arată că această salvare este legată de salvarea de sincronizare inversă

  - **Data\_RenameDisabledReason -** eroare care face redenumirea să fie dezactivată pentru acest document

  - **Data\_RenameFlightEnabled -** dacă este activată ediția flight pentru caracteristica de redenumire

  - **Data\_SaveInitiateKind -** întreg care indică modul în care s-a inițiat salvarea

  - **Data\_SrcDocIsUnnamedOrNew -** indică dacă documentul pe care îl salvăm este nou

#### <a name="officewordfilesaveactfconfirmsavedoccorequerysave"></a>Office.Word.FileSave.ActFConfirmSaveDocCoreQuerySave

Acest eveniment indică faptul că Office Word îi solicită utilizatorului să salveze modificările atunci când încearcă să închidă documentul. Acesta permite Microsoft să monitorizeze dacă salvare-la-ieșire funcționează conform așteptărilor pentru a se evita pierderea de date din documente. Evenimentul monitorizează dacă salvare-la-ieșire funcționează conform așteptărilor. În plus, se folosește pentru a calcula utilizatorii/dispozitivele active lunar și măsurătorile de fiabilitate cloud.

Se colectează următoarele câmpuri:

  - **Data\_AddDocTelemRes -** raportează dacă am putut completa corect alte valori legate de telemetria documentelor din eveniment. Utilizat pentru diagnostice privind calitatea datelor.

  - **Data\_DetachedDuration -** cât timp a fost activitatea detașată de fir

  - **Data\_Doc\_AccessMode -** documentul este doar în citire/editabil

  - **Data\_Doc\_AssistedReadingReasons -** set predefinit de valori privind motivul pentru care documentul a fost deschis în modul de citire asistată

  - **Data\_Doc\_ChunkingType -** unități utilizate pentru deschiderea incrementală a documentelor

  - **Data\_Doc\_EdpState -** setare de protecție a datelor electronice pentru document

  - **Data\_Doc\_Ext -** extensia documentului (docx/xlsb/pptx etc.)

  - **Data\_Doc\_FileFormat –** versiunea de protocol pentru formatul fișierului

  - **Data\_Doc\_Fqdn -** numele de domeniu OneDrive sau SharePoint Online

  - **Data\_Doc\_FqdnHash -** codul hash într-o singură direcție pentru numele de domeniu identificabil al clientului

  - **Data\_Doc\_IdentityTelemetryId -** codul hash într-o singură direcție pentru identitatea de utilizator folosită pentru deschidere

  - **Data\_DstDoc\_InitializationScenario -** înregistrează cum a fost deschis documentul

  - **Data\_Doc\_IOFlags -** rapoarte privind semnalizările memorate în cache folosite pentru a seta opțiunile de deschidere a solicitărilor

  - **Data\_Doc\_IrmRights -** acțiunile permise de politica de protejare a datelor electronice aplicată pentru document/utilizator

  - **Data\_Doc\_IsIncrementalOpen -** semnalizare care arată că documentul a fost deschis incremental

  - **Data\_Doc\_IsOcsSupported -** semnalizare care arată că documentul este acceptat în serviciul de colaborare

  - **Data\_Doc\_IsOpeningOfflineCopy -** semnalizare care arată că s-a deschis copia offline a unui document

  - **Data_Doc_IsRtcAlwaysOn -** true în cazul în care canalul în timp real (RTC) este întotdeauna activat pentru acest fișier.

  - **Data\_Doc\_IsSyncBacked -** semnalizare care arată că pe computer există o copie sincronizată automat a documentului

  - **Data\_Doc\_Location -** arată ce serviciu a furnizat documentul (OneDrive, File Server, SharePoint etc.)

  - **Data\_Doc\_LocationDetails -** arată ce Folder cunoscut a furnizat un document stocat local

  - **Data\_Doc\_NumberCoAuthors -** numărul de alți utilizatori dintr-o sesiune de editare în colaborare

  - **Data\_Doc\_PasswordFlags -** arată semnalizările de parole pentru citire sau citire/scriere setate

  - **Data\_Doc\_ReadOnlyReasons -** motivele pentru care documentul a fost deschis doar în citire

  - **Data\_Doc\_ResourceIdHash -** un identificator de document anonimizat, folosit în diagnosticarea problemelor

  - **Data\_Doc\_ServerDocId -** un identificator de document anonimizat și invariabil, folosit în diagnosticarea problemelor

  - **Data\_Doc\_ServerProtocol -** versiunea de protocol folosită în comunicarea cu serviciul

  - **Data\_Doc\_ServerType -** tipul de server care oferă serviciul (SharePoint, OneDrive, WOPI etc.)

  - **Data\_Doc\_ServerVersion -** versiunea serverului care oferă serviciul

  - **Data\_Doc\_SessionId -** identifică o anumită sesiune de editare a documentului din sesiunea completă

  - **Data\_Doc\_SharePointServiceContext -** informații de diagnosticare din solicitările SharePoint Online

  - **Data\_Doc\_SizeInBytes -** indicator privind dimensiunea documentului

  - **Data\_Doc\_SpecialChars -** indicator privind caracterele speciale din calea sau adresa URL a documentului

  - **Data\_Doc\_StreamAvailability -** indicator care arată dacă șirul documentului este disponibil/dezactivat

  - **Data\_Doc\_SyncBackedType -** indicator privind tipul documentului (local sau bazat pe servicii)

  - **Data\_Doc\_UrlHash -** cod hash într-o singură direcție, pentru crearea unui identificator naiv de document

  - **Data\_Doc\_WopiServiceId –** conține identificatorul unic al furnizorului de servicii WOPI

  - **Data\_DstDoc\_AccessMode –** documentul de destinație este doar în citire/editabil

  - **Data\_DstDoc\_EdpState – setare de protecție a datelor electronice pentru documentul de destinație**

  - **Data\_DstDoc\_Ext –** Extensia (docx/xlsb/pptx, etc.) documentului de destinație

  - **Data\_DstDoc\_FileFormat –** Versiunea protocolului de format fișier pentru documentul de destinație

  - **Data\_DstDoc\_Location –** indică serviciul care va oferi spațiu de stocare pentru documentul de destinație (OneDrive, File Server, SharePoint etc.)

  - **Data\_DstDoc\_LocationDetails –** indică Folderul cunoscut local care a stocat documentul de destinație

  - **Data\_DstDoc\_SessionId –** identifică o anumită sesiune de editare a documentului din sesiunea completă

  - **Data\_DstDoc\_UrlHash –** cod hash într-o singură direcție pentru crearea unui identificator naiv pentru documentul de destinație

  - **Data\_FailureClass –** întreg care reprezintă clasa de eroare pentru erorile de tranziție OCS

  - **Data\_LocationPickerSaveStatus –** valoare întreagă care indică acțiunea care a declanșat salvarea din caseta de dialog salvare la ieșire

  - **Data\_MainPdod –** Identificatorul documentului din procesul Office Word.

  - **Data\_MoveFlightEnabled –** dacă ediția flight este activată pentru caracteristica de mutare

  - **Data\_OCSSyncbackSaveStarted –** marcaj care arată că această salvare este legată de salvarea de sincronizare inversă

  - **Data\_RenameDisabledReason -** eroare care face redenumirea să fie dezactivată pentru acest document

  - **Data\_RenameFlightEnabled -** dacă este activată ediția flight pentru caracteristica de redenumire

  - **Data\_SaveInitiateKind -** întreg care indică modul în care s-a inițiat salvarea

  - **Data\_SrcDocIsUnnamedOrNew –** indică dacă documentul pe care îl salvăm este nou

#### <a name="officewordfilesavesaveassavefile"></a>Office.Word.FileSave.SaveAsSaveFile

Acest eveniment indică faptul că Office Word salvează un document într-un document nou. Acest lucru permite ca Microsoft să detecteze erorile din acțiunea de „salvare ca”, lucru important pentru a evita pierderea datelor din documente. Evenimentul monitorizează dacă „salvarea ca” funcționează așa cum vă așteptați. În plus, se folosește pentru a calcula utilizatorii/dispozitivele active lunar și măsurătorile de fiabilitate cloud.

Se colectează următoarele câmpuri:

  - **Data\_AddDocTelemRes -** raportează dacă am putut completa corect alte valori legate de telemetria documentelor din eveniment. Utilizat pentru diagnostice privind calitatea datelor.

  - **Data\_AddDocTelemResDst –** raportează dacă am putut completa corect alte valori legate de telemetria documentelor din eveniment pentru documentul de destinație. Utilizat pentru diagnostice privind calitatea datelor.

  - **Data\_AddDocTelemResSrc –** raportează dacă am putut completa corect alte valori legate de telemetria documentelor din eveniment pentru documentul sursă. Utilizat pentru diagnostice privind calitatea datelor.

  - **Data\_DetachedDuration -** cât timp a fost activitatea detașată de fir

  - **Data\_Doc\_AccessMode -** documentul este doar în citire/editabil

  - **Data\_Doc\_AssistedReadingReasons -** set predefinit de valori privind motivul pentru care documentul a fost deschis în modul de citire asistată

  - **Data\_Doc\_ChunkingType -** unități utilizate pentru deschiderea incrementală a documentelor

  - **Data\_Doc\_EdpState -** setare de protecție a datelor electronice pentru document

  - **Data\_Doc\_Ext -** extensia documentului (docx/xlsb/pptx etc.)

  - **Data\_Doc\_FileFormat –** versiunea de protocol pentru formatul fișierului

  - **Data\_Doc\_Fqdn -** numele de domeniu OneDrive sau SharePoint Online

  - **Data\_Doc\_FqdnHash -** codul hash într-o singură direcție pentru numele de domeniu identificabil al clientului

  - **Data\_Doc\_IdentityTelemetryId –** codul hash într-o singură direcție pentru identitatea de utilizator folosită pentru deschidere

  - **Data\_Doc\_IOFlags –** rapoarte privind marcajele memorate în cache folosite pentru a seta opțiunile de deschidere a solicitărilor

  - **Data\_Doc\_IrmRights -** acțiunile permise de politica de protejare a datelor electronice aplicată pentru document/utilizator

  - **Data\_Doc\_IsIncrementalOpen -** semnalizare care arată că documentul a fost deschis incremental

  - **Data\_Doc\_IsOcsSupported -** semnalizare care arată că documentul este acceptat în serviciul de colaborare

  - **Data\_Doc\_IsOpeningOfflineCopy -** semnalizare care arată că s-a deschis copia offline a unui document

  - **Data_Doc_IsRtcAlwaysOn -** true în cazul în care canalul în timp real (RTC) este întotdeauna activat pentru acest fișier.

  - **Data\_Doc\_IsSyncBacked -** semnalizare care arată că pe computer există o copie sincronizată automat a documentului

  - **Data\_Doc\_Location -** arată ce serviciu a furnizat documentul (OneDrive, File Server, SharePoint etc.)

  - **Data\_Doc\_LocationDetails -** arată ce Folder cunoscut a furnizat un document stocat local

  - **Data\_Doc\_NumberCoAuthors –** numărul de alți utilizatori dintr-o sesiune de editare în colaborare

  - **Data\_Doc\_ReadOnlyReasons –** motivele pentru care documentul a fost deschis doar în citire

  - **Data\_Doc\_ResourceIdHash -** un identificator de document anonimizat, folosit în diagnosticarea problemelor

  - **Data\_Doc\_ServerDocId -** un identificator de document anonimizat și invariabil, folosit în diagnosticarea problemelor

  - **Data\_Doc\_ServerProtocol -** versiunea de protocol folosită în comunicarea cu serviciul

  - **Data\_Doc\_ServerType -** tipul de server care oferă serviciul (SharePoint, OneDrive, WOPI etc.)

  - **Data\_Doc\_ServerVersion -** versiunea serverului care oferă serviciul

  - **Data\_Doc\_SessionId -** identifică o anumită sesiune de editare a documentului din sesiunea completă

  - **Data\_Doc\_SharePointServiceContext -** informații de diagnosticare din solicitările SharePoint Online

  - **Data\_Doc\_SizeInBytes -** indicator privind dimensiunea documentului

  - **Data\_Doc\_SpecialChars -** indicator privind caracterele speciale din calea sau adresa URL a documentului

  - **Data\_Doc\_StreamAvailability –** indicator care arată dacă șirul documentului este disponibil/dezactivat

  - **Data\_Doc\_UrlHash –** cod hash într-o singură direcție, pentru crearea unui identificator naiv de document

  - **Data\_DstDoc\_AccessMode –** documentul de destinație este doar în citire/editabil

  - **Data\_DstDoc\_AssistedReadingReasons –** set predefinit de valori privind motivul pentru care documentul de destinație a fost deschis în modul de citire asistată

  - **Data\_DstDoc\_ChunkingType –** unități utilizate pentru deschiderea incrementală a documentelor

  - **Data\_DstDoc\_EdpState –** setare de protecție a datelor electronice pentru documentul de destinație

  - **Data\_DstDoc\_Ext –** extensia documentului (docx/xlsb/pptx etc.)

  - **Data\_DstDoc\_FileFormat –** versiunea de protocol pentru formatul fișierului

  - **Data\_DstDoc\_Fqdn –** numele de domeniu OneDrive sau SharePoint Online pentru documentul de destinație

  - **Data\_DstDoc\_FqdnHash –** cod hash într-o singură direcție pentru numele de domeniu identificabil de client pentru documentul de destinație

  - **Data\_DstDoc\_IdentityTelemetryId –** codul hash într-o singură direcție pentru identitatea de utilizator folosită pentru deschidere

  - **Data\_DstDoc\_InitializationScenario –** înregistrează cum a fost deschis documentul de destinație

  - **Data\_DstDoc\_IOFlags –** rapoarte privind marcajele memorate în cache folosite pentru a seta opțiunile de deschidere a solicitărilor pentru documentul de destinație

  - **Data\_DstDoc\_IrmRights –** acțiunile permise de politica de protejare a datelor electronice aplicată pentru documentul de destinație/utilizator

  - **Data\_DstDoc\_IsIncrementalOpen –** marcaj care arată că documentul a fost deschis incremental

  - **Data\_DstDoc\_IsOcsSupported –** marcaj care arată că documentul este acceptat în serviciul de colaborare

  - **Data\_DstDoc\_IsOpeningOfflineCopy –** marcaj care arată că s-a deschis copia offline a unui document

  - **Data\_DstDoc\_IsSyncBacked –** marcaj care arată că pe computer există o copie sincronizată automat a documentului

  - **Data\_DstDoc\_Location –** indică serviciul care a oferit spațiul de stocare pentru documentul de destinație (OneDrive, File Server, SharePoint etc.)

  - **Data\_DstDoc\_LocationDetails –** arată ce Folder cunoscut a furnizat un document stocat local

  - **Data\_DstDoc\_NumberCoAuthors –** numărul de alți utilizatori dintr-o sesiune de editare în colaborare

  - **Data\_DstDoc\_PasswordFlags –** arată marcajele de parole pentru citire sau citire/scriere setate pentru documentul de destinație

  - **Data\_DstDoc\_ReadOnlyReasons –** motivele pentru care documentul de destinație a fost deschis doar în citire

  - **Data\_DstDoc\_ResourceIdHash –** un identificator de document anonimizat, folosit în diagnosticarea problemelor

  - **Data\_DstDoc\_ServerDocId –** un identificator de document anonimizat și imutabil, folosit în diagnosticarea problemelor

  - **Data\_DstDoc\_ServerProtocol –** versiunea de protocol folosită în comunicarea cu serviciul

  - **Data\_DstDoc\_ServerType –** tipul de server care oferă serviciul (SharePoint, OneDrive, WOPI etc.)

  - **Data\_DstDoc\_ServerVersion –** versiunea serverului care oferă serviciul

  - **Data\_DstDoc\_SessionId –** identifică o anumită sesiune de editare a documentului din sesiunea completă

  - **Data\_DstDoc\_SharePointServiceContext –** informații de diagnosticare din solicitările SharePoint Online

  - **Data\_DstDoc\_SizeInBytes –** indicator privind dimensiunea documentului

  - **Data\_DstDoc\_SpecialChars –** indicator privind caracterele speciale din calea sau adresa URL a documentului

  - **Data\_DstDoc\_StreamAvailability –** indicator care arată dacă șirul documentului este disponibil/dezactivat

  - **Data\_DstDoc\_SyncBackedType –** indicator privind tipul documentului (local sau bazat pe servicii)

  - **Data\_DstDoc\_UrlHash –** cod hash într-o singură direcție pentru crearea unui identificator naiv pentru documentul de destinație

  - **Data\_DstDoc\_WopiServiceId –** conține identificatorul unic al furnizorului de servicii WOPI

  - **Data\_FailureClass –** întreg care reprezintă clasa de eroare pentru erorile de tranziție OCS

  - **Data\_LocationPickerPropagateToSaveTime,spLapsedMsec –** măsoară timpul, în milisecunde, necesar pentru declanșarea salvării după ce s-a obținut un rezultat din selectorul de locații

  - **Data\_LocationPickerSaveStatus –** starea returnate de selectorul de locații

  - **Data\_MainPdod –** Identificatorul documentului din procesul Office Word

  - **Data\_MoveDisabledReason –** eroarea care dezactivează mutarea pentru document

  - **Data\_MoveFlightEnabled –** dacă ediția flight este activată pentru caracteristica de mutare

  - **Data\_RenameDisabledReason –** eroare care face redenumirea să fie dezactivată pentru acest document

  - **Data\_RenameFlightEnabled -** dacă este activată ediția flight pentru caracteristica de redenumire

  - **Data\_SaveInitiateKind –** întreg care arată cum s-a inițiat salvarea

  - **Data\_SrcDoc\_AccessMode –** documentul sursă este doar în citire/editabil

  - **Data\_SrcDoc\_AssistedReadingReasons –** set predefinit de valori privind motivul pentru care documentul a fost deschis în modul de citire asistată

  - **Data\_SrcDoc\_ChunkingType –** unități utilizate pentru deschiderea incrementală a documentelor

  - **Data\_SrcDoc\_EdpState –** setare de protecție a datelor electronice pentru documentul sursă

  - **Data\_SrcDoc\_Ext –** Extensia documentului sursă (docx/xlsb/pptx etc.)

  - **Data\_SrcDoc\_FileFormat –** Versiunea protocolului de format fișier pentru documentul sursă

  - **Data\_SrcDoc\_Fqdn –** numele de domeniu OneDrive sau SharePoint Online pentru documentul sursă

  - **Data\_SrcDoc\_FqdnHash –** cod hash într-o singură direcție pentru numele de domeniu identificabil de client pentru documentul sursă

  - **Data\_SrcDoc\_IdentityTelemetryId –** codul hash într-o singură direcție pentru identitatea de utilizator folosită pentru deschidere

  - **Data\_SrcDoc\_InitializationScenario –** înregistrează cum a fost deschis documentul

  - **Data\_SrcDoc\_IOFlags –** rapoarte privind marcajele memorate în cache folosite pentru a seta opțiunile de deschidere a solicitărilor

  - **Data\_SrcDoc\_IrmRights –** acțiunile permise de politica de protejare a datelor electronice aplicată pentru document/utilizator

  - **Data\_SrcDoc\_IsIncrementalOpen –** marcaj care arată că documentul a fost deschis incremental

  - **Data\_SrcDoc\_IsOcsSupported –** marcaj care arată că documentul este acceptat în serviciul de colaborare

  - **Data\_SrcDoc\_IsOpeningOfflineCopy –** marcaj care arată că s-a deschis copia offline a unui document

  - **Data\_SrcDoc\_IsSyncBacked –** marcaj care arată că pe computer există o copie sincronizată automat a documentului

  - **Data\_SrcDoc\_Location –** arată ce serviciu a furnizat documentul sursă (OneDrive, File Server, SharePoint etc.)

  - **Data\_SrcDoc\_LocationDetails –** arată ce Folder cunoscut a furnizat un document stocat local

  - **Data\_SrcDoc\_NumberCoAuthors –** numărul de alți utilizatori dintr-o sesiune de editare în colaborare

  - **Data\_SrcDoc\_PasswordFlags –** arată marcajele de parole pentru citire sau citire/scriere setate

  - **Data\_SrcDoc\_ReadOnlyReasons –** motivele pentru care documentul a fost deschis doar în citire

  - **Data\_SrcDoc\_ResourceIdHash –** un identificator de document anonimizat, folosit în diagnosticarea problemelor

  - **Data\_SrcDoc\_ServerDocId –** un identificator de document anonimizat și imutabil, folosit în diagnosticarea problemelor

  - **Data\_SrcDoc\_ServerProtocol –** versiunea de protocol folosită în comunicarea cu serviciul

  - **Data\_SrcDoc\_ServerType –** tipul de server care oferă serviciul (SharePoint, OneDrive, WOPI etc.)

  - **Data\_SrcDoc\_ServerVersion –** versiunea serverului care oferă serviciul

  - **Data\_SrcDoc\_SessionId –** identifică o anumită sesiune de editare a documentului din sesiunea completă

  - **Data\_SrcDoc\_SharePointServiceContext –** informații de diagnosticare din solicitările SharePoint Online

  - **Data\_SrcDoc\_SizeInBytes –** indicator privind dimensiunea documentului

  - **Data\_SrcDoc\_SpecialChars –** indicator privind caracterele speciale din calea sau adresa URL a documentului

  - **Data\_SrcDoc\_StreamAvailability –** indicator care arată dacă șirul documentului este disponibil/dezactivat

  - **Data\_SrcDoc\_SyncBackedType –** indicator privind tipul documentului (local sau bazat pe servicii)

  - **Data\_SrcDoc\_UrlHash –** cod hash într-o singură direcție, pentru crearea unui identificator naiv de document

  - **Data\_SrcDoc\_WopiServiceId –** conține identificatorul unic al furnizorului de servicii WOPI

  - **Data\_SrcDocIsUnnamedOrNew –** indică dacă documentul pe care îl salvăm este nou

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

#### <a name="officevisiosharedfeatureexperimentation"></a>Office.Visio.Shared.FeatureExperimentation

Urmărește configurația „flighting” a caracteristicii pentru utilizatori. Acest eveniment ne ajută să determinăm succesul sau eșecul edițiilor flight ale caracteristicilor.

Se colectează următoarele câmpuri:

  - **Data\_Enable:bool **– true în cazul în care caracteristica este activată pentru utilizatorul curent

  - **Data\_Feature:string** – numele caracteristicii

  - **Data\_Flighted:bool** – true în cazul în care caracteristica este activată

  - **Data\_Licensed:bool** – true în cazul în care caracteristica este sub verificarea de licențiere

  - **Data\_Subscriber:bool** – true arată că utilizatorul are licență cu abonament

#### <a name="officevisiosharedrefreshsmartdiagram"></a>Office.Visio.Shared.RefreshSmartDiagram

Capturează erorile de reîmprospătare a diagramei atunci când fișierul este creat prin DV. Aceasta ne ajută să depanăm erorile și problemele din reîmprospătarea datelor dintr-o diagramă DV.

Se colectează următoarele câmpuri:

  - **Data\_ConnectorsBasedOnSequence:bool** – true dacă diagrama reîmprospătată a fost creată inițial utilizând conectorul bazat pe opțiunea „secvență”

  - **Data\_DialogError**:**string** – eroare în timpul reîmprospătării diagramei inteligente

  - **Data\_FileError:string** – șir de eroare atunci când fișierul Excel conectat este nevalid

  - **Data\_OverwriteSelected**:**bool** – true dacă utilizatorul a selectat opțiunea de înlocuire a diagramei în timpul reîmprospătării

  - **Data\_WarningShown**:**bool** – true dacă utilizatorul a văzut vreun avertisment în timpul reîmprospătării datelor

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

### <a name="application-status-and-boot-subtype"></a>*Subtipul de inițializare și starea aplicației*

Stabilește dacă au avut loc anumite evenimente de caracteristici, cum ar fi pornirea sau oprirea, și dacă respectiva caracteristică rulează.

#### <a name="officeextensibilityofficejsappactivated"></a>Office.Extensibility.OfficeJS.Appactivated

Înregistrează informații despre opririle neașteptate Office. Acest lucru ne permite să identificăm blocările sau căderile produsului, astfel încât să le putem remedia.

Se colectează următoarele câmpuri:

  - **Data\_AirspaceInitTime:integer – ** timpul necesar pentru inițializa componenta office Airspace

  - **Data\_AllShapes:integer –** numărul de forme din document

  - **Data\_APIInitTime:integer –** timpul necesar pentru a inițializa modulul Visio API

  - **Data\_AppSizeHeight –** Adăugați**-** la înălțimea ferestrei

  - **Data\_AppSizeWidth –** Adăugați**-** la lățimea ferestrei

  - **Data\_AppURL –** URL-ul programului de completare; înregistrează adresa URL completă pentru programele de completare din magazin și domeniul adresei URL pentru cele din afara magazinului

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

  - **Data\_Doc\_IsOpeningOfflineCopy:bool -** documentul este deschis din memoria cache locală?

  - **Data_Doc_IsRtcAlwaysOn -** true în cazul în care canalul în timp real (RTC) este întotdeauna activat pentru acest fișier.

  - **Data\_Doc\_IsSyncBacked:bool –** true când acesta este un document de server care există la nivel local și este sincronizat cu serverul (de exemplu, prin aplicațiile client OneDrive sau ODB)

  - **Data\_Doc\_Location:long –**: setul predefinit de valori pentru locul unde este stocat documentul (Local, SharePoint, WOPI, Rețea etc.)

  - **Data\_Doc\_LocationDetails:long –** setul predefinit de valori pentru locația mai detaliată (folderul Temp, folderul de descărcări, Documente OneDrive, Imagini OneDrive

  - **Data\_Doc\_ResourceIdHash:string –** codul hash al identificatorului de resursă pentru documentele stocate în cloud

  - **Data\_Doc\_ServerDocId:string –** identificatorul imutabil pentru documentele stocate în cloud

  - **Data\_Doc\_SessionId:long –** GUID generat care identifică instanța documentului din aceeași sesiune de proces

  - **Data\_Doc\_SizeInBytes:long –** dimensiunea documentului în byți

  - **Data\_Doc\_SpecialChars:long –** Bitmask lung ce arată caracterele speciale din adresa URL sau calea documentului

  - **Data\_Doc\_SyncBackedType –** indicator privind tipul de document (local sau bazat pe servicii) 

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

  - **Data\_InitBrandTime:integer –** timpul necesar pentru a inițializa ecranul de pornire și componentele office de brand

  - **Data\_InitGimmeTime:integer – ** timpul necesar pentru a inițializa componenta office

  - **Data\_InitLicensingTime:integer – ** timpul necesar pentru a licenția componenta office

  - **Data\_InitMsoUtilsTime:integer –** timpul de inițializare a componentei office MSOUTILS

  - **Data\_InitPerfTime:integer –** timpul de inițializare a componentei office de performanță

  - **Data\_InitTCOTime:integer –** timpul necesar pentru a inițializa managerul de componente office

  - **Data\_InitTrustCenterTime:integer –** timpul necesar pentru a inițializa centrul de autorizare a componentelor office

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

  - **Data\_LoadProfileTime:integer –** timpul necesar pentru a încărca instrumentul de diagnosticare office

  - **Data\_LoadRichEditTim:integer –** timpul de încărcare a componentei de editare inteligentă

  - **Data\_LoadVisIntlTime:integer –** timpul necesar pentru a încărca fișierul DLL internațional Visio

  - **Data\_Location:integer –** locația din care a fost deschis fișierul 0 Local, 1, Rețea, 2, SharePoint, 3 – Web

  - **Data\_MasterCount:integer –** numărul de coordonatoare din diagramă

  - **Data\_MaxCoauthUsers:integer –** numărul maxim de utilizatori care colaborează la orice moment în componentele Filesystem, Registry, First Party sau SDX din sesiune

  - **Data\_MaxTilesAutoSizeOn:integer –** numărul maxim de dale a unei pagini pentru care s-a activat dimensiunea automată

  - **Data\_MsoBeginBootTime:integer –** timpul de inițializare MSO

  - **Data\_MsoDllLoadTime:integer –** timpul necesar pentru a încărca MSO DLL

  - **Data\_MsoEndBootTime:integer –** timpul necesar pentru a încheia inițializarea MSO

  - **Data\_MsoInitCoreTime:integer –** timpul necesar pentru a inițializa componenta office MSO

  - **Data\_MsoInitUITime:integer –** timpul necesar pentru a inițializa interfața de utilizare a componentelor office MSO

  - **Data\_MsoMigrateTime:integer –** timpul necesar pentru a migra setările de utilizator la prima inițializare, dacă utilizatorul a făcut upgrade de la versiunea anterioară

  - **Data\_NetworkIOBytesRead:int –** numărul total de byți din rețea citiți la salvare

  - **Data\_NetworkIOBytesReadSquared:int –** valoarea pătrată pentru Data\_NetworkIOBytesRead

  - **Data\_NetworkIOBytesWritten:int –** numărul total de byți din rețea scriși la salvare

  - **Data\_NetworkIOBytesWrittenSquared :int –** valoarea pătrată pentru NetworkIOBytesWritten

  - **Data\_OartStartupTime:integer –** timpul necesar pentru a inițializa componenta office OART

  - **Data\_OleInitTime:integer –** timpul de inițializare a componentei office OLE

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

  - **Data\_SDX\_AssetId –** există DOAR pentru programele de completare din magazin. OMEX oferă un AssetId programului de completare când ajunge în magazin

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

#### <a name="officeoutlookdesktopexchangepuidandtenantcorrelation"></a>Office.Outlook.Desktop.ExchangePuidAndTenantCorrelation

Colectează codul PUID al utilizatorului și identificatorul de entitate găzduită, o dată pe sesiune. Corelarea PUID cu entitatea găzduită este necesară pentru a înțelege și a diagnostica problemele cu Outlook pentru fiecare entitate găzduită.

Se colectează următoarele câmpuri:

  - **CollectionTime** – marca de timp a evenimentului

  - **ConnId** – identificatorul de conexiune care analizează PUID și identificatorul entității găzduite OMS

  - **OMSTenantId** – identificatorul unic generat de Microsoft al entității găzduite

  - **PUID** – codul PUID Exchange pentru a identifica în mod unic utilizatorii

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

  - **Data\_ContentTransaction –** set predefinit de valori pentru momentul când se poate crea tranzacția (AllowedOnLoadDocument, AllowedOnOpenComplete etc.)

  - **Data\_CppUncaughtExceptionCount:long –** excepții native neprinse în timp ce rula activitatea

  - **Data\_CreateDocumentTimeMS –** durata executării metodei CreateDocumentTimeMS în milisecunde

  - **Data\_CreateDocumentToken –** durata executării metodei CreateDocumentToken în milisecunde

  - **Data\_CreateDocumentToW –** durata executării metodei CreateDocumentToW în milisecunde

  - **Data\_CreateDocWindow –** durata executării metodei CreateDocWindow în milisecunde

  - **Data\_CreateLocalTempFile –** durata executării metodei CreateLocalTempFile în milisecunde

  - **Data\_DetachedDuration:long –** timpul cât activitatea a fost detașată/nu a rulat

  - **Data\_DetermineFileType –** durata executării metodei DetermineFileType în milisecunde

  - **Data\_Doc\_AccessMode:long –** cum a fost deschis acest document (doar în citire / citire-scriere)

  - **Data\_Doc\_AssistedReadingReasons:long –** set predefinit de valori pentru care documentul a fost deschis în modul de citire asistată

  - **Data\_Doc\_ChunkingType:long –** cum este stocat documentul în SharePoint

  - **Data\_Doc\_EdpState:long –** starea Enterprise Data Protection a documentului

  - **Data\_Doc\_Ext:string –** extensia documentului

  - **Data\_Doc\_Extension:string –** extensia documentului

  - **Data\_Doc\_FileFormat:long –** set predefinit de valori pentru formatul fișierului (mai granular decât extensia)

  - **Data\_Doc\_Fqdn:string –** unde este stocat documentul (SharePoint.com, live.net), disponibil numai pentru domeniile Office 365

  - **Data\_Doc\_FqdnHash:string –** codul hash al locului unde este stocat documentul

  - **Data\_Doc\_IdentityTelemetryId:string – **GUID unic al utilizatorului

  - **Data\_Doc\_IdentityUniqueId:string –** identificator unic al identității folosite pentru acțiunea Documente partajate

  - **Data\_Doc\_IOFlags:long -** bitmask pentru diferite semnalizări legate de IO pentru un anumit document

  - **Data\_Doc\_IrmRights:long -** set predefinit de valori pentru tipul de Information Rights Management aplicat pentru acest document (Redirecționare, Răspuns, SecureReader, Editare etc.)

  - **Data\_Doc\_IsCloudCollabEnabled:bool –** true dacă antetul „IsCloudCollabEnabled” a fost deja primit dintr-o solicitare OPTIONS.

  - **Data\_Doc\_IsIncrementalOpen:bool –** documentul a fost deschis incremental (caracteristică nouă care deschide documentul fără să-l descarce în totalitate)

  - **Data\_Doc\_IsOcsSupported:bool –** dacă documentul acceptă elaborarea în comun folosind noul serviciu OCS

  - **Data\_Doc\_IsOpeningOfflineCopy:bool –** dacă documentul este deschis din memoria cache locală?

  - **Data_Doc_IsRtcAlwaysOn -** true în cazul în care canalul în timp real (RTC) este întotdeauna activat pentru acest fișier.

  - **Data\_Doc\_IsSyncBacked:bool –** dacă documentul este deschis din folderul care folosește aplicația de sincronizare OneDrive

  - **Data\_Doc\_Location:long –** set predefinit de valori privind locul de stocare a documentului (Local, SharePoint, WOPI, Rețea etc.)

  - **Data\_Doc\_LocationDetails:long –** set predefinit de valori privind locația mai detaliată (folderul Temp, folderul de descărcări, Documente OneDrive, Imagini OneDrive etc.)

  - **Data\_Doc\_NumberCoAuthors:long –** numărul de coautori la momentul deschiderii unui document

  - **Data\_Doc\_PasswordFlags:long –** set predefinit de valori privind modul în care documentul este criptat cu o parolă (Niciunul, parolă pentru citire, parolă pentru editare)

  - **Data\_Doc\_ReadOnlyReasons:long –** set predefinit de valori privind motivul pentru care acest document a fost marcat doar în citire (blocat pe server, document final, protejat prin parolă pentru editare etc.)

  - **Data\_Doc\_ResourceIdHash:string –** codul hash al identificatorului de resurse pentru documentele stocate în cloud

  - **Data\_Doc\_ServerDocId:string –** identificator imutabil pentru documentele stocate în cloud

  - **Data\_Doc\_ServerProtocol:long –** set predefinit de valori privind protocolul folosit în comunicarea cu serverul (Http, Cobalt, WOPI etc.)

  - **Data\_Doc\_ServerType:long –** set predefinit de valori privind tipul serverului (SharePoint, DropBox, WOPI)

  - **Data\_Doc\_ServerVersion:long –** dacă serverul se bazează pe Office14, Office15, Office 16

  - **Data\_Doc\_SessionId:long –** GUID generat care identifică instanța documentului din aceeași sesiune de proces

  - **Data\_Doc\_SharePointServiceContext:string –** un șir opac, de obicei GridManagerID.FarmID. Util pentru corelarea jurnalelor de la client și de pe server

  - **Data\_Doc\_SizeInBytes:long –** dimensiunea documentului în byți

  - **Data\_Doc\_SpecialChars:long –** Bitmask ce arată caracterele speciale din adresa URL sau calea documentului

  - **Data\_Doc\_StorageProviderId:string –** șir care identifică furnizorul de stocare al documentului, precum „DropBox”

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

  - **Data\_FailureComponent:long –** set predefinit de valori privind componenta care a cauzat nereușita protocolului (Conflict, CSI, Internă etc.)

  - **Data\_FailureReason:long –** set predefinit de valori privind motivul nereușitei (FileIsCorrupt, BlockedByAntivirus etc.)

  - **Data\_FCreateNew –** este acesta un document nou și necompletat

  - **Data\_FCreateNewFromTemplate –** este acesta un document nou din șabloane

  - **Data_FErrorAfterDocWinCreation:boolean-**  s-a produs o eroare sau o excepție după ce a fost creată o fereastră de document.

  - **Data\_FileUrlLocation –** set predefinit de valori privind locul unde este stocat documentul (NetworkShare, LocalDrive, ServerOther etc.)

  - **Data\_FirstSlideCompressedSize –** dimensiunea comprimată a părții zip din primul diapozitiv (de obicei Slide1.xml)

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

#### <a name="officetelemetryengineisprelaunch"></a>Office.TelemetryEngine.IsPreLaunch

Se aplică pentru aplicațiile Office UWP.  Acest eveniment se declanșează când o aplicație office este inițiată pentru prima dată după upgrade-ul/instalarea din magazin. El face parte din datele de diagnosticare de bază, utilizate pentru a urmări dacă o sesiune este de lansare sau nu.

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

#### <a name="officewordfileopenopencmdfilemrupriv"></a>Office.Word.FileOpen.OpenCmdFileMruPriv

Acest eveniment indică faptul că Office Word deschide un document din lista Cel mai recent utilizate (Most Recent Used – MRU). În plus, conține date esențiale despre performanța la deschiderea fișierelor și este un eveniment de pornire a aplicației din perspectiva utilizatorului. Evenimentul monitorizează dacă file-open-from-MRU funcționează așa cum vă așteptați. În plus, se folosește pentru a calcula utilizatorii/dispozitivele active lunar și măsurătorile de fiabilitate cloud.

Se colectează următoarele câmpuri:

  - **Data\_AddDocTelemRes -** raportează dacă am putut completa corect alte valori legate de telemetria documentelor din eveniment. Utilizat pentru diagnostice privind calitatea datelor.

  - **Data\_BytesAsynchronous –** numărul de byți (comprimat) fără care credem că putem deschide fișierul dacă îi obținem înainte ca utilizatorul să vrea să editeze sau să salveze

  - **Data\_BytesAsynchronousWithWork –** numărul de byți (comprimat) fără care credem că putem deschide fișierul, dar care ar necesita investiții de cod semnificative pentru a funcționa

  - **Data\_BytesSynchronous –** numărul de byți (comprimat) de care avem nevoie înainte să putem deschide fișierul

  - **Data\_BytesUnknown –** numărul de byți din componentele de documente pe care nu ne așteptăm să le găsim

  - **Data\_DetachedDuration –** cât timp a fost activitatea detașată de fir

  - **Data\_Doc\_AccessMode –** documentul este doar în citire/editabil

  - **Data\_Doc\_AssistedReadingReasons –** set predefinit de valori privind motivul pentru care documentul a fost deschis în modul de citire asistată

  - **Data\_Doc\_ChunkingType -** unități utilizate pentru deschiderea incrementală a documentelor

  - **Data\_Doc\_EdpState -** setare de protecție a datelor electronice pentru document

  - **Data\_Doc\_Ext -** extensia documentului (docx/xlsb/pptx etc.)

  - **Data\_Doc\_FileFormat –** versiunea de protocol pentru formatul fișierului

  - **Data\_Doc\_Fqdn -** numele de domeniu OneDrive sau SharePoint Online

  - **Data\_Doc\_FqdnHash -** codul hash într-o singură direcție pentru numele de domeniu identificabil al clientului

  - **Data\_Doc\_IOFlags -** rapoarte privind semnalizările memorate în cache folosite pentru a seta opțiunile de deschidere a solicitărilor

  - **Data\_Doc\_IdentityTelemetryId -** codul hash într-o singură direcție pentru identitatea de utilizator folosită pentru deschidere

  - **Data\_DstDoc\_InitializationScenario -** înregistrează cum a fost deschis documentul

  - **Data\_Doc\_IrmRights -** acțiunile permise de politica de protejare a datelor electronice aplicată pentru document/utilizator

  - **Data\_Doc\_IsIncrementalOpen -** semnalizare care arată că documentul a fost deschis incremental

  - **Data\_Doc\_IsOcsSupported -** semnalizare care arată că documentul este acceptat în serviciul de colaborare

  - **Data\_Doc\_IsOpeningOfflineCopy -** semnalizare care arată că s-a deschis copia offline a unui document

  - **Data_Doc_IsRtcAlwaysOn -** true în cazul în care canalul în timp real (RTC) este întotdeauna activat pentru acest fișier.

  - **Data\_Doc\_IsSyncBacked –** marcaj care arată că pe computer există o copie sincronizată automat a documentului

  - **Data\_Doc\_Location –** arată ce serviciu a furnizat documentul (OneDrive, File Server, SharePoint etc.)

  - **Data\_Doc\_LocationDetails -** arată ce Folder cunoscut a furnizat un document stocat local

  - **Data\_Doc\_NumberCoAuthors -** numărul de alți utilizatori dintr-o sesiune de editare în colaborare

  - **Data\_Doc\_PasswordFlags -** arată semnalizările de parole pentru citire sau citire/scriere setate

  - **Data\_Doc\_ReadOnlyReasons –** motivele pentru care documentul a fost deschis doar în citire

  - **Data\_Doc\_ResourceIdHash –** un identificator de document anonimizat, folosit în diagnosticarea problemelor

  - **Data\_Doc\_ServerDocId –** un identificator de document anonimizat și imutabil, folosit în diagnosticarea problemelor

  - **Data\_Doc\_ServerProtocol –** versiunea de protocol folosită în comunicarea cu serviciul

  - **Data\_Doc\_ServerType –** tipul de server care oferă serviciul (SharePoint, OneDrive, WOPI etc.)

  - **Data\_Doc\_ServerVersion –** versiunea serverului care oferă serviciul

  - **Data\_Doc\_SessionId -** identifică o anumită sesiune de editare a documentului din sesiunea completă

  - **Data\_Doc\_SharePointServiceContext -** informații de diagnosticare din solicitările SharePoint Online

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

  - **Data\_Measurements –** șir codificat cu detalii de timp pentru diferitele părți ale deschiderii. Utilizat pentru a măsura performanța.

  - **Data\_MoveDisabledReason –** eroarea care dezactivează mutarea pentru document

  - **Data\_MoveFlightEnabled –** dacă ediția flight este activată pentru caracteristica de mutare

  - **Data\_PartsUnknown –** numărul de componente ale documentului pentru care nu am putut obține date

  - **Data\_RecoverableFailureInitiationLocationTag –** etichetă unică pentru site-ul de apelare a codului folosit pentru a identifica locul din cod în care încercăm să remediem fișierul înainte de a-l deschide

  - **Data\_RenameDisabledReason –** eroare care face redenumirea să fie dezactivată pentru acest document

  - **Data\_RenameFlightEnabled -** dacă este activată ediția flight pentru caracteristica de redenumire

  - **Data\_SecondaryTag –** etichetă unică pentru site-ul de apelare a codului folosit pentru a adăuga date suplimentare despre erori pentru deschidere

  - **Data\_TemplateFormat –** formatul de fișier al șablonului pe care se bazează documentul.

  - **Data\_UsesNormal –** indică dacă documentul deschis se bazează pe șablonul normal

#### <a name="officewordfileopenopenffileopenxstzcore"></a>Office.Word.FileOpen.OpenFFileOpenXstzCore

Acest eveniment indică faptul că Office Word deschide un document pe care a făcut dublu clic un utilizator. În plus, conține date esențiale despre performanța la deschiderea fișierelor și este un eveniment de pornire a aplicației din perspectiva utilizatorului. Evenimentul monitorizează dacă file-open-from-file-double-click funcționează așa cum vă așteptați. În plus, se folosește pentru a calcula utilizatorii/dispozitivele active lunar și măsurătorile de fiabilitate cloud.

Se colectează următoarele câmpuri:

  - **Data\_AddDocTelemRes –** raportează dacă am putut completa corect alte valori legate de telemetria documentelor din eveniment. Utilizat pentru diagnostice privind calitatea datelor

  - **Data\_BytesAsynchronous –** numărul de byți (comprimat) fără care credem că putem deschide fișierul dacă îi obținem înainte ca utilizatorul să vrea să editeze sau să salveze

  - **Data\_BytesAsynchronousWithWork –** numărul de byți (comprimat) fără care credem că putem deschide fișierul, dar care ar necesita investiții de cod semnificative pentru a funcționa

  - **Data\_BytesSynchronous –** numărul de byți (comprimat) de care avem nevoie înainte să putem deschide fișierul

  - **Data\_BytesUnknown –** numărul de byți din componentele de documente pe care nu ne așteptăm să le găsim

  - **Data\_DetachedDuration –** cât timp a fost activitatea detașată de fir

  - **Data\_Doc\_AccessMode –** documentul este doar în citire/editabil

  - **Data\_Doc\_AssistedReadingReasons –** set predefinit de valori privind motivul pentru care documentul a fost deschis în modul de citire asistată

  - **Data\_Doc\_ChunkingType -** unități utilizate pentru deschiderea incrementală a documentelor

  - **Data\_Doc\_EdpState -** setare de protecție a datelor electronice pentru document

  - **Data\_Doc\_Ext -** extensia documentului (docx/xlsb/pptx etc.)

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

  - **Data_Doc_IsRtcAlwaysOn -** true în cazul în care canalul în timp real (RTC) este întotdeauna activat pentru acest fișier.

  - **Data\_Doc\_IsSyncBacked -** semnalizare care arată că pe computer există o copie sincronizată automat a documentului

  - **Data\_Doc\_Location -** arată ce serviciu a furnizat documentul (OneDrive, File Server, SharePoint etc.)

  - **Data\_Doc\_LocationDetails -** arată ce Folder cunoscut a furnizat un document stocat local

  - **Data\_Doc\_NumberCoAuthors -** numărul de alți utilizatori dintr-o sesiune de editare în colaborare

  - **Data\_Doc\_PasswordFlags -** arată semnalizările de parole pentru citire sau citire/scriere setate

  - **Data\_Doc\_ReadOnlyReasons –** motivele pentru care documentul a fost deschis doar în citire

  - **Data\_Doc\_ResourceIdHash –** un identificator de document anonimizat, folosit în diagnosticarea problemelor

  - **Data\_Doc\_ServerDocId –** un identificator de document anonimizat și imutabil, folosit în diagnosticarea problemelor

  - **Data\_Doc\_ServerProtocol –** versiunea de protocol folosită în comunicarea cu serviciul

  - **Data\_Doc\_ServerType -** tipul de server care oferă serviciul (SharePoint, OneDrive, WOPI etc.)

  - **Data\_Doc\_ServerVersion –** versiunea serverului care oferă serviciul

  - **Data\_Doc\_SessionId –** versiunea serverului care oferă serviciul

  - **Data\_Doc\_SharePointServiceContext-**

  - **Data\_Doc\_SizeInBytes –** indicator privind dimensiunea documentului

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

  - **Data\_Measurements –** șir codificat cu detalii de timp pentru diferitele părți ale deschiderii. Utilizat pentru a măsura performanța.

  - **Data\_MoveDisabledReason –** eroarea care dezactivează mutarea pentru document

  - **Data\_MoveFlightEnabled –** dacă ediția flight este activată pentru caracteristica de mutare

  - **Data\_PartsUnknown –** numărul de componente ale documentului pentru care nu am putut obține date

  - **Data\_RecoverableFailureInitiationLocationTag –** etichetă unică pentru site-ul de apelare a codului folosit pentru a identifica locul din cod în care încercăm să remediem fișierul înainte de a-l deschide.

  - **Data\_RenameDisabledReason –** eroare care face redenumirea să fie dezactivată pentru acest document

  - **Data\_RenameFlightEnabled -** dacă este activată ediția flight pentru caracteristica de redenumire

  - **Data\_SecondaryTag –** etichetă unică pentru site-ul de apelare a codului folosit pentru a adăuga date suplimentare despre erori pentru deschidere.

  - **Data\_TemplateFormat –** formatul de fișier al șablonului pe care se bazează documentul.

  - **Data\_UsesNormal –** indică dacă documentul deschis se bazează pe șablonul normal


#### <a name="officewordfileopenopenifrinitargs"></a>Office.Word.FileOpen.OpenIfrInitArgs

Acest eveniment indică faptul că Office Word deschide un document prin activare COM sau linia de comandă. În plus, conține date esențiale despre performanța la deschiderea fișierelor și este un eveniment de pornire a aplicației din perspectiva utilizatorului. Evenimentul monitorizează dacă file-open-from-command-line funcționează așa cum vă așteptați. În plus, se folosește pentru a calcula utilizatorii/dispozitivele active lunar și măsurătorile de fiabilitate cloud.

Se colectează următoarele câmpuri:

  - **Data\_AddDocTelemRes -** raportează dacă am putut completa corect alte valori legate de telemetria documentelor din eveniment. Utilizat pentru diagnostice privind calitatea datelor.

  - **Data\_BytesAsynchronous –** numărul de byți (comprimat) fără care credem că putem deschide fișierul dacă îi obținem înainte ca utilizatorul să vrea să editeze sau să salveze.

  - **Data\_BytesAsynchronousWithWork –** numărul de byți (comprimat) fără care credem că putem deschide fișierul, dar care ar necesita investiții de cod semnificative pentru a funcționa

  - **Data\_BytesSynchronous –** numărul de byți (comprimat) de care avem nevoie înainte să putem deschide fișierul

  - **Data\_BytesUnknown –** numărul de byți din componentele de documente pe care nu ne așteptăm să le găsim.

  - **Data\_Doc\_AccessMode –** documentul este doar în citire/editabil

  - **Data\_Doc\_AssistedReadingReasons -** set predefinit de valori privind motivul pentru care documentul a fost deschis în modul de citire asistată

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

  - **Data_Doc_IsRtcAlwaysOn -** true în cazul în care canalul în timp real (RTC) este întotdeauna activat pentru acest fișier.

  - **Data\_Doc\_IsSyncBacked -** semnalizare care arată că pe computer există o copie sincronizată automat a documentului

  - **Data\_Doc\_Location –** arată ce serviciu a furnizat documentul (OneDrive, File Server, SharePoint)

  - **Data\_Doc\_LocationDetails –** arată ce Folder cunoscut a furnizat un document stocat local

  - **Data\_Doc\_NumberCoAuthors -** numărul de alți utilizatori dintr-o sesiune de editare în colaborare

  - **Data\_Doc\_PasswordFlags -** arată semnalizările de parole pentru citire sau citire/scriere setate

  - **Data\_Doc\_ReadOnlyReasons –** motivele pentru care documentul a fost deschis doar în citire

  - **Data\_Doc\_ResourceIdHash –** un identificator de document anonimizat, folosit în diagnosticarea problemelor

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

  - **Data\_PartsUnknown –** numărul de componente ale documentului pentru care nu am putut obține date

  - **Data\_RecoverableFailureInitiationLocationTag –** etichetă unică pentru site-ul de apelare a codului folosit pentru a identifica locul din cod în care încercăm să remediem fișierul înainte de a-l deschide

  - **Data\_RenameDisabledReason –** eroare care face redenumirea să fie dezactivată pentru acest document

  - **Data\_RenameFlightEnabled -** dacă este activată ediția flight pentru caracteristica de redenumire

  - **Data\_SecondaryTag –** etichetă unică pentru site-ul de apelare a codului folosit pentru a adăuga date suplimentare despre erori pentru deschidere.

  - **Data\_TemplateFormat –** formatul de fișier al șablonului pe care se bazează documentul.

  - **Data\_UsesNormal –** indică dacă documentul deschis se bazează pe șablonul normal.


#### <a name="officewordfileopenopenloadfile"></a>Office.Word.FileOpen.OpenLoadFile

Acest eveniment indică faptul că Office Word deschide un document prin caseta de dialog Deschidere. În plus, conține date esențiale despre performanța la deschiderea fișierelor și este un eveniment de pornire a aplicației din perspectiva utilizatorului. Evenimentul monitorizează dacă file-open-from-the-open-file-dialog funcționează așa cum vă așteptați. În plus, se folosește pentru a calcula utilizatorii/dispozitivele active lunar și măsurătorile de fiabilitate cloud.

Se colectează următoarele câmpuri:

  - **Data\_AddDocTelemRes -** raportează dacă am putut completa corect alte valori legate de telemetria documentelor din eveniment. Utilizat pentru diagnostice privind calitatea datelor.

  - **Data\_BytesAsynchronous –** numărul de byți (comprimat) fără care credem că putem deschide fișierul dacă îi obținem înainte ca utilizatorul să vrea să editeze sau să salveze

  - **Data\_BytesAsynchronousWithWork –** numărul de byți (comprimat) fără care credem că putem deschide fișierul, dar care ar necesita investiții de cod semnificative pentru a funcționa

  - **Data\_BytesSynchronous –** numărul de byți (comprimat) de care avem nevoie înainte să putem deschide fișierul

  - **Data\_BytesUnknown –** numărul de byți din componentele de documente pe care nu ne așteptăm să le găsim

  - **Data\_DetachedDuration –** cât timp a fost activitatea detașată de fir

  - **Data\_Doc\_AccessMode -** documentul este doar în citire/editabil

  - **Data\_Doc\_AssistedReadingReasons -** set predefinit de valori privind motivul pentru care documentul a fost deschis în modul de citire asistată

  - **Data\_Doc\_ChunkingType -** unități utilizate pentru deschiderea incrementală a documentelor

  - **Data\_Doc\_EdpState -** setare de protecție a datelor electronice pentru document

  - **Data\_Doc\_Ext -** extensia documentului (docx/xlsb/pptx etc.)

  - **Data\_Doc\_FileFormat –** versiunea de protocol pentru formatul fișierului

  - **Data\_Doc\_Fqdn -** numele de domeniu OneDrive sau SharePoint Online

  - **Data\_Doc\_FqdnHash –** codul hash într-o singură direcție pentru numele de domeniu identificabil al clientului

  - **Data\_Doc\_IdentityTelemetryId –** codul hash într-o singură direcție pentru identitatea de utilizator folosită pentru deschidere

  - **Data\_Doc\_InitializationScenario –** înregistrează cum a fost deschis documentul

  - **Data\_Doc\_IOFlags -** rapoarte privind semnalizările memorate în cache folosite pentru a seta opțiunile de deschidere a solicitărilor

  - **Data\_Doc\_IrmRights -** acțiunile permise de politica de protejare a datelor electronice aplicată pentru document/utilizator

  - **Data\_Doc\_IsIncrementalOpen -** semnalizare care arată că documentul a fost deschis incremental

  - **Data\_Doc\_IsOcsSupported -** semnalizare care arată că documentul este acceptat în serviciul de colaborare

  - **Data\_Doc\_IsOpeningOfflineCopy -** semnalizare care arată că s-a deschis copia offline a unui document

  - **Data_Doc_IsRtcAlwaysOn -** true în cazul în care canalul în timp real (RTC) este întotdeauna activat pentru acest fișier.

  - **Data\_Doc\_IsSyncBacked -** semnalizare care arată că pe computer există o copie sincronizată automat a documentului

  - **Data\_Doc\_Location -** arată ce serviciu a furnizat documentul (OneDrive, File Server, SharePoint etc.)

  - **Data\_Doc\_LocationDetails -** arată ce Folder cunoscut a furnizat un document stocat local

  - **Data\_Doc\_NumberCoAuthors -** numărul de alți utilizatori dintr-o sesiune de editare în colaborare

  - **Data\_Doc\_PasswordFlags -** arată semnalizările de parole pentru citire sau citire/scriere setate

  - **Data\_Doc\_ReadOnlyReasons –** motivele pentru care documentul a fost deschis doar în citire

  - **Data\_Doc\_ResourceIdHash –** un identificator de document anonimizat, folosit în diagnosticarea problemelor

  - **Data\_Doc\_ServerDocId –** un identificator de document anonimizat și imutabil, folosit în diagnosticarea problemelor

  - **Data\_Doc\_ServerProtocol –** versiunea de protocol folosită în comunicarea cu serviciul

  - **Data\_Doc\_ServerType –** tipul de server care oferă serviciul (SharePoint, OneDrive, WOPI etc.)

  - **Data\_Doc\_ServerVersion –** versiunea serverului care oferă serviciul

  - **Data\_Doc\_SessionId -** identifică o anumită sesiune de editare a documentului din sesiunea completă

  - **Data\_Doc\_SharePointServiceContext -** informații de diagnosticare din solicitările SharePoint Online

  - **Data\_Doc\_SizeInBytes -** indicator privind dimensiunea documentului

  - **Data\_Doc\_SpecialChars -** indicator privind caracterele speciale din calea sau adresa URL a documentului

  - **Data\_Doc\_StreamAvailability -** indicator care arată dacă șirul documentului este disponibil/dezactivat

  - **Data\_Doc\_SyncBackedType -** indicator privind tipul documentului (local sau bazat pe servicii)

  - **Data\_Doc\_UrlHash –** cod hash într-o singură direcție, pentru crearea unui identificator naiv de document

  - **Data\_EditorDisablingRename –** identificatorul primului editor care a provocat dezactivarea redenumirii

  - **Data\_EditorsCount –** numărul de editori din document

  - **Data\_ForceReadWriteReason –** valoare întreagă care reprezintă motivul pentru care fișierul a fost forțat în modul citire/scriere

  - **Data\_FSucceededAfterRecoverableFailure –** arată că deschiderea a reușit după repararea unei erori la deschiderea documentului

  - **Data\_LastLoggedTag –** etichetă unică pentru site-ul de apelare a codului folosit pentru a identifica momentele când nu reușim să încercăm salvarea de două ori (folosit pentru diagnosticarea calității datelor)

  - **Data\_LinkStyles –** indică dacă asociem stiluri de șabloane

  - **Data\_MainPdod –** Identificatorul documentului din procesul Office Word

  - **Data\_Measurements –** șir codificat cu detalii de timp pentru diferitele părți ale deschiderii. Utilizat pentru a măsura performanța.

  - **Data\_MoveDisabledReason –** eroarea care dezactivează mutarea pentru document

  - **Data\_MoveFlightEnabled –** dacă ediția flight este activată pentru caracteristica de mutare

  - **Data\_PartsUnknown –** numărul de componente ale documentului pentru care nu am putut obține date

  - **Data\_RecoverableFailureInitiationLocationTag –** etichetă unică pentru site-ul de apelare a codului folosit pentru a identifica locul din cod în care încercăm să remediem fișierul înainte de a-l deschide

  - **Data\_RenameDisabledReason –** eroare care face redenumirea să fie dezactivată pentru acest document

  - **Data\_RenameFlightEnabled -** dacă este activată ediția flight pentru caracteristica de redenumire

  - **Data\_SecondaryTag –** etichetă unică pentru site-ul de apelare a codului folosit pentru a adăuga date suplimentare despre erori pentru deschidere

  - **Data\_TemplateFormat –** formatul de fișier al șablonului pe care se bazează documentul

  - **Data\_UsesNormal** – indică dacă documentul deschis se bazează pe șablonul normal


### <a name="office-accessibility-configuration-subtype"></a>*Subtip de configurație accesibilitate Office*

Caracteristici de accesibilitate în Office

#### <a name="officeaccessibilityaccessibilitytoolsessionpresencewin32"></a>Office.Accessibility.AccessibilityToolSessionPresenceWin32

Ne permite să detectăm că utilizatorul are un instrument de tehnologie de asistare și numele său. Acest lucru ne permite să înțelegem dacă un utilizator Office se confruntă cu probleme cu un anumit instrument din Tehnologiile de asistare.

Se colectează următoarele câmpuri:

  - **Data\_Data\_Jaws –** indică dacă Jaws rula în timpul sesiunii**Data\_Data\_Magic –** indică dacă Magic rula în timpul sesiunii

  - **Data\_Data\_Magnify –** indică dacă Magnify rula în timpul sesiunii

  - **Data\_Data\_Narrator –** indică dacă Narrator rula în timpul sesiunii

  - **Data\_Data\_NVDA –** indică dacă NVDA rula în timpul sesiunii

  - **Data\_Data\_SA –** indică dacă SA rula în timpul sesiunii

  - **Data\_Data\_Supernova –** indică dacă Supernova rula în timpul sesiunii

  - **Data\_Data\_SuperNovaessSuite –** indică dacă SuperNovaAccessSuite rula în timpul sesiunii

  - **Data\_Data\_WinEyes –** indică dacă WinEyes rula în timpul sesiunii

  - **Data\_Data\_ZoomText –** indică dacă ZoomText rula în timpul sesiunii

#### <a name="officewordaccessibilitylearningtoolsreadaloudplayreadaloud"></a>Office.Word.Accessibility.LearningTools.ReadAloud.PlayReadAloud

Acest eveniment indică faptul că Office Word citește cu voce tare textul din document. Evenimentul este un mesaj repetat al caracteristicii de accesibilitate care permite ca Microsoft să evalueze starea de funcționare a caracteristicii textului citit cu voce tare.

Se colectează următoarele câmpuri:

  - **Data\_CharacterCount –** numărul de caractere al documentului

  - **Data\_CharactersWithSpaceCount –** numărul de caractere și spații al documentului

  - **Data\_IsPageCountInProgress –** numărul de pagini în curs

  - **Data\_LineCount –** numărul de linii al documentului

  - **Data\_PageCount –** numărul de pagini al documentului

  - **Data\_ParagraphCount –** numărul de paragrafe al documentului

  - **Data\_Play –** este prima dată când Word citește cu voce tare

  - **Data\_ViewKind –** tipul de vizualizare al documentului

  - **Data\_WordCount –** numărul de cuvinte al documentului

#### <a name="officewordaccessibilitylearningtoolsreadaloudstopreadaloud"></a>Office.Word.Accessibility.LearningTools.ReadAloud.StopReadAloud

Acest eveniment indică faptul că Office Word întrerupe citirea cu voce tare a textului din document. Evenimentul permite ca Microsoft să evalueze starea de funcționare a caracteristicii de citire cu voce tare a textului, măsurând durata de lucru.

Se colectează următoarele câmpuri:

  - Fără

## <a name="product-and-service-performance-data-events"></a>Evenimente privind datele despre performanța produselor și a serviciilor

Iată subtipurile de date din această categorie:
- [Ieșire neașteptată a aplicației (cădere)](#unexpected-application-exit-crash-subtype)
- [Performanța caracteristicii aplicației](#application-feature-performance-subtype)
- [Eroare de activitate a aplicației](#application-activity-error-subtype)

### <a name="unexpected-application-exit-crash-subtype"></a>*Subtip de ieșire neașteptată a aplicației (cădere)*

Ieșirile neașteptate ale aplicației și starea aplicației atunci când se întâmplă acest lucru.

#### <a name="officeappdomainunhandledexceptionhandlerfailed"></a>Office.AppDomain.UnhandledExceptionHandlerFailed

Colectează informații pentru orice excepții netratate, utilizând aplicația Data Streamer. Aceste date se utilizează pentru a monitoriza starea de funcționare a aplicației. Evenimentul este generat de Microsoft Data Streamer pentru programul de completare Excel.

Se colectează următoarele câmpuri:

- **Exception** – stiva de apeluri pentru excepție

- **Event name** – categoria evenimentului și eticheta acestuia.

#### <a name="officeextensibilitycomaddinunhandledexception"></a>Office.Extensibility.COMAddinUnhandledException

Eveniment generat atunci când se defectează programul de completare COM

Analiză desktop: aceasta este utilizată ca numărător în calculul stării de funcționare specifice pentru întreprindere a programelor de completare, utilizată pentru a deduce în timpul programului pilot dacă programul de completare este „gata de upgrade” în cercul de producție.  
Detalii globale: se utilizează pentru a calcula nivelul de pregătire global, specific întreprinderii, pentru un program de completare care este apoi publicat pe readyforwindows.com și alte instrumente, cum ar fi Readiness Toolkit

Se colectează următoarele câmpuri:

**ScopeId** – domeniul firului curent

**Method** – metoda Office unde a apărut excepția

**Interface** – interfața Office în care a apărut excepția

**AddinId** – ID-ul clasei programului de completare

**AddinProgId** – Identificator de program de completare

**AddinFriendlyName** – numele prietenos al programului de completare

**AddinTimeDateStamp** – marca de timp a programului de completare din metadatele DLL

**AddinVersion** – versiunea programului de completare

**AddinFileName** – numele de fișier al programului de completare, exclusiv calea fișierului

**VSTOAddIn** – dacă programul de completare este VSTO

**AddinConnectFlag** – comportamentul curent de încărcare

**LoadAttempts** – numărul de încercări pentru a încărca programul de completare

#### <a name="officeextensibilityvbatelemetrybreak"></a>Office.Extensibility.VbaTelemetryBreak

Eveniment generat atunci când un fișier activat pentru macrocomenzi întâmpină o eroare de compilare sau de rulare

Analiză desktop: aceasta este utilizată ca numărător în calculul stării de funcționare specifice pentru întreprindere a tipurilor de macrocomenzi (de exemplu, macrocomenzi Word, Excel etc.), utilizată pentru a deduce în timpul programului pilot dacă programul de completare este „gata de upgrade” în cercul de producție.

Se colectează următoarele câmpuri:

**TagId** – ID-ul etichetei de telemetrie

**BreakReason** – motivul întreruperii (rulare, compilare, altă eroare)

**SolutionType** – tipul soluției (document, șablon, program de completare pentru aplicație, program de completare COM)

**Data.ErrorCode** – codul de eroare raportat de motorul VBA

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

#### <a name="officepowerpointsession"></a>**Office.PowerPoint.Session**

Se colectează utilizarea caracteristicilor pentru fiecare sesiune PowerPoint. Aceste date se utilizează pentru a calcula raportul de închideri neplanificate PowerPoint la utilizarea unei caracteristici. Raportul de închideri neplanificate PowerPoint este un semnal cheie pentru a garanta că PowerPoint funcționează așa cum vă așteptați.

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

Se colectează caracteristica utilizată când sesiunea PowerPoint s-a închis pe neașteptate. Aceste informații sunt esențiale pentru a surprinde închiderile neașteptate PowerPoint. Microsoft utilizează aceste date pentru a diagnostica problema și a garanta că PowerPoint rulează așa cum vă așteptați.

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

#### <a name="officethisaddinstartupfailed"></a>Office.ThisAddIn.StartupFailed

Colectează informațiile pentru excepția care apare la pornirea aplicației Data Streamer. Aceste date se utilizează pentru a monitoriza starea de funcționare a aplicației. Evenimentul este generat de Microsoft Data Streamer pentru programul de completare Excel.

Se colectează următoarele câmpuri:

- **Exception** – stiva de apeluri pentru excepție

- **Event name** – categoria evenimentului și eticheta acestuia.


### <a name="application-feature-performance-subtype"></a>*Subtipul de performanță al caracteristicii aplicației*

Timpii de răspuns slabi sau performanțele scăzute pentru scenarii precum pornirea aplicației sau deschiderea unui fișier.

#### <a name="officemanageabilityserviceapplypolicy"></a>Office.Manageability.Service.ApplyPolicy

Telemetria critică pentru a urmări erorile\\Succesul de la aplicarea setărilor privind politica cloud în registry. LastError spune de ce și unde nu a reușit aplicarea politicii în registry.

Se colectează următoarele câmpuri:

  - **Data.ApplyLogMsg** – mesajul de excepție, dacă este cazul, în timp ce se aplica politica

  - **Data.Cid** – identificator de corelare generat dinamic și trimis la serviciu, atunci când apelarea serviciului s-a făcut pentru a prelua politica privind mediul cloud. Utilizat pentru a corela apelul care a provocat o problemă în timp ce se aplicau politicile în cloud.

  - **Data.Last Error** – una din cinci valori șir (enumeratori) pentru a înregistra în jurnal etapa de aplicare a politicii care se executa când a avut loc excepția

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

#### <a name="officeperformanceboot"></a>Office.Performance.Boot

Colectat atunci când o aplicație Office este inițializată. Include dacă inițializarea a fost inițiată prin deschiderea unui fișier sau lansarea prin meniul Start, dacă aceasta a fost prima inițializare a aplicației, cantitatea de memorie utilizată de aplicație și dacă a existat o IU de blocare afișată utilizatorului. Utilizat pentru a măsura cât de repede se încarcă aplicațiile Office și cantitatea de memorie utilizată atunci când pornesc, pentru a vă asigura că există o experiență de utilizator acceptabilă.

Se colectează următoarele câmpuri:

  - **ActivationKind** - dacă aplicația a fost pornită prin lansare din meniul Start, prin deschiderea unui fișier sau prin OLE Automation.

  - **FirstBoot** – dacă aceasta a fost prima pornire a aplicației.

  - **InitializationDuration** – durata necesară în microsecunde pentru a inițializa prima dată procesul Office.

  - **InterruptionMessageId** – dacă inițializarea a fost întreruptă de o casetă de dialog care solicită introducerea utilizatorului, ID-ul casetei de dialog.

  - **TotalWorkingSetMB** – volumul de memorie în megabaiți din setul de lucru al procesului.

  - **VirtualSetMB** – volumul de memorie în megabaiți din setul virtual al procesului. (Numai MacOS/iOS)

  - **WorkingSetPeakMB** – cel mai mare volum de memorie în megabaiți care a fost vreodată în setul de lucru al procesului până acum.

#### <a name="officeuxofficeinsidercanshowofficeinsiderslab"></a>Office.UX.OfficeInsider.CanShowOfficeInsiderSlab

Activitate prin care se urmărește dacă secțiunea Office Insider poate fi afișată utilizatorului de pe fila Cont din interfața cu utilizatorul Office Backstage.

Se colectează următoarele câmpuri:

  - **Data_CanShow** – indică dacă secțiunea Office Insider poate fi afișată utilizatorului de pe fila Cont din interfața cu utilizatorul Office Backstage.
  
  - **Data_Event** – neutilizat

  - **Data_EventInfo** – neutilizat

  - **Data_Reason** – neutilizat

#### <a name="officeuxofficeinsidershowofficeinsiderdlg"></a>Office.UX.OfficeInsider.ShowOfficeInsiderDlg

Activitate prin care se urmărește utilizarea și performanța casetei de dialog Office Insider.

Se colectează următoarele câmpuri:

  - **Data_AcceptedContactMeNew** – atunci când optează pentru un nivel Insider și atunci când alegerea utilizatorului a fost înregistrată cu succes, indică dacă utilizatorul a acceptat să fie contactat de Microsoft.

  - **Data_DialogChoice** = neutilizat
  
  - **Data_DialogId** = neutilizat
  
  - **Data_Event** – neutilizat
  
  - **Data_EventInfo** – neutilizat
  
  - **Data_InsiderLevel** – nivelul Insider când caseta de dialog este afișată pentru prima dată utilizatorului.
  
  - **Data_InsiderLevelNew** – nivelul nou Insider selectat de utilizator.
  
  - **Data_IsInternalUser** – indică dacă aplicația se execută sub acreditările unui cont @microsoft. com.
  
  - **Data_IsInternalUserInit** – indică dacă codul ar putea determina dacă aplicația se execută sub acreditările unui cont @microsoft.
  
  - **Data_OpenNewsletterWebpage** – atunci când este activată caracteristica de abonare la newsletter-ul Office Insider, iar utilizatorul comută la un nivel Insider din producție, indică dacă a fost declanșată navigarea în browser la linkul cu abonarea la newsletterul Office Insider.

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

### <a name="application-activity-error-subtype"></a>*Subtipul de eroare de activitate a aplicației*

Erorile în funcționalitatea unei caracteristici sau a unei experiențe de utilizator.

#### <a name="officeairspacebackendwin32graphicsdriversofthang"></a>Office.AirSpace.Backend.Win32.GraphicsDriverSoftHang 

Ajută Microsoft să separe blocările lungi ale driverului de placă video de cele scurte, pentru a lua decizii despre driverele de placă video care pot avea probleme. Driverul de placă video al utilizatorului a făcut Office să se blocheze, dar impactul blocării nu este cunoscut încă

Se colectează următoarele câmpuri:

  - **Data\_InDeviceCall** – metoda apelată pe placa video care a produs blocarea

  - **Data\_Timeout** – cât a durat blocarea

#### <a name="officegraphicsarcexceptions"></a>Office.Graphics.ARCExceptions 

Aceste informații de raportare a excepțiilor sunt importante pentru a evalua starea generală a stivei de elemente grafice și pentru a identifica părțile de cod în care apar erori cu o frecvență ridicată, pentru a stabili prioritatea investigațiilor. Aceste informații de raportare a excepțiilor sunt importante pentru a evalua starea generală a stivei de elemente grafice și pentru a identifica părțile de cod în care apar erori cu o frecvență ridicată. Acestea ajută inginerii să stabilească erorile de redare care afectează cei mai mulți utilizatori, permițându-ne să stabilim priorități pentru investigațiile noastre și să remediem problemele care vor aduce cele mai multe beneficii utilizatorilor.

Se colectează următoarele câmpuri:

  - **Data\_HResult** – codul de eroare returnat

  - **Data\_TagCount** – de căte ori a apărut fiecare eroare

  - **Data\_TagID** – identificatorul erorii care a apărut

#### <a name="officeoutlookdesktopcalendaracceptcalsharenavigatetosharedfoldererror"></a>Office.Outlook.Desktop.Calendar.AcceptCalShareNavigateToSharedFolder\_Error

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

  - **CountExceptionForward – numărul de excepții de întâlnire redirecționate**

  - **CountExceptionForwardAsiCal – numărul de excepții de întâlnire redirecționate ca iCal**

  - **CountExceptionForwardInSplit – numărul de excepții de întâlnire redirecționate din meniul Scindare din panglică**

  - **CountExceptionForwardWithAttach – numărul de excepții de întâlnire redirecționate ca atașare**

  - **CountRecurringForward – numărul de întâlniri recurente redirecționate**

  - **CountRecurringForwardAsiCal – numărul de întâlniri recurente redirecționate ca iCal**

  - **CountRecurringForwardInSplit** – numărul de întâlniri recurente redirecționate din meniul Scindare din panglică

  - **CountRecurringForwardWithAttach – numărul de întâlniri recurente redirecționate ca atașare**

  - **CountSingleForward – numărul de întâlniri unice redirecționate**

  - **CountSingleForwardAsiCal – numărul de întâlniri unice redirecționate ca iCal**

  - **CountSingleForwardInSplit – numărul de întâlniri unice redirecționate din meniul Scindare din panglică**

  - **CountSingleForwardWithAttach – numărul de întâlniri unice redirecționate ca atașare**

  - **HResult – ErrorCode**

  - **OlkViewName – indică vizualizarea Mail, Calendar sau Inspector**

#### <a name="officeoutlookdesktopoutlookcalendarusageerrmeetrcptreplyactionsruleo16"></a>Office.Outlook.Desktop.OutlookCalendarUsageErr.MeetRcpt.ReplyActions.Rule.O16

Colectează reușitele și nereușitele acțiunilor Răspuns, Răspuns tuturor, Răspuns cu mesaj instantaneu și Răspuns tuturor cu mesaj instantaneu pentru răspunsurile la întâlniri Unice, Recurente și Excepționale din vizualizarea Mail, Calendar și Inspector Outlook. Rata de nereușită a acțiunilor Răspuns, Răspuns tuturor, Răspuns cu mesaj instantaneu și Răspuns tuturor cu mesaj instantaneu este monitorizată activ pentru anomalii. Statisticile privind anomaliile indică o eroare în abilitatea Outlook de a efectua operațiuni de calendar de bază. Aceste date se utilizează, de asemenea, pentru a diagnostica alte probleme legate de Calendar care pot fi detectate.

Se colectează următoarele câmpuri:

  - **CountExceptionReply – numărul de excepții de Răspuns la întâlnire**

  - **CountExceptionReplyAll – numărul de excepții de Răspuns tuturor la întâlnire**

  - **CountExceptionReplyAllWithIM – numărul de excepții de Răspuns tuturor cu mesaj instantaneu la întâlnire**

  - **CountExceptionReplyWithIM – numărul de excepții de Răspuns cu mesaj instantaneu la întâlnire**

  - **CountRecurringReply – numărul de răspunsuri la întâlniri recurente**

  - **CountRecurringReplyAll – numărul de răspunsuri de tip Răspuns tuturor la întâlniri recurente**

  - **CountRecurringReplyAllWithIM – numărul de răspunsuri tuturor cu mesaj instantaneu la întâlniri recurente**

  - **CountRecurringReplyWithIM – numărul de răspunsuri cu mesaj instantaneu la întâlniri recurente**

  - **CountSingleReply – numărul de răspunsuri la întâlniri unice**

  - **CountSingleReplyAll – numărul de răspunsuri tuturor la întâlniri unice**

  - **CountSingleReplyAllWithIM – numărul de răspunsuri tuturor cu mesaj instantaneu la întâlniri unice**

  - **CountSingleReplyWithIM – numărul de răspunsuri cu mesaj instantaneu la întâlniri unice**

  - **HResult – ErrorCode**

  - **OlkViewName – indică vizualizarea Mail, Calendar sau Inspector**

#### <a name="officeoutlookdesktopoutlookprivsdlgsingleuserloadfail"></a>Office.Outlook.Desktop.OutlookPrivsDlgSingleUser.LoadFail

Această regulă colectează erorile de partajare a calendarelor atunci când se adaugă un utilizator nou (de tip EX sau SMTP) din agendă. Aceste date se utilizează pentru diagnosticarea și rezolvarea problemelor detectate în caseta de dialog Partajarea calendarelor

Se colectează următoarele câmpuri:

  - **CountAccountWizardEnd** – De câte ori s-a încheiat caseta de dialog pentru expertul moștenit

  - **CountCreatePIMAccount** – de câte ori utilizatorul a creat un profil PIM

#### <a name="officesystemsystemhealthasserts"></a>Office.System.SystemHealthAsserts

Erorile pe care le identifică acest eveniment ne ajută să înțelegem când experiența clienților se degradează. Multe dintre aceste ShipAsserts duc la căderi, iar aceste informații ne ajută să le remediem. Colectează ShipAsserts din cadrul produsului, pentru a identifica erorile.

Se colectează următoarele câmpuri:

Count – numărul fiecărei aserțiuni raportate

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

## <a name="device-connectivity-and-configuration-data-events"></a>Evenimente privind conectivitatea și datele de configurare ale dispozitivelor

Iată subtipurile de date din această categorie:

- [Conectivitatea și configurarea dispozitivelor](#device-connectivity-and-configuration-subtype)


### <a name="device-connectivity-and-configuration-subtype"></a>*Conectivitatea dispozitivelor și subtipul de configurare*

Starea conexiunii la rețea și setările dispozitivelor, cum ar fi memoria.

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
