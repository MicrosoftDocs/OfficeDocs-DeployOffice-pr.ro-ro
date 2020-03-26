---
title: Servicii esențiale pentru Office
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
description: Oferă administratorilor Office informații despre servicii esențiale în Office, cum ar fi Clic și Pornire și Licențiere, și asigură o listă de evenimente și câmpuri de date pentru aceste servicii esențiale.
hideEdit: true
ms.openlocfilehash: 2d285e2e0494b08e6d17a0a72bd8465e6c8edce7
ms.sourcegitcommit: 2b494bb428a3a1b837376c0ab9ef9c2357e3165f
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/24/2020
ms.locfileid: "42939774"
---
# <a name="essential-services-for-office"></a>Servicii esențiale pentru Office

> [!IMPORTANT]
> Informațiile din acest articol se aplică la versiunea 1904 sau o versiune mai recentă a următorului software client Office instalat pe un computer care rulează Windows:
> - Office 365 ProPlus și Office 365 Business
> - Office 365 Personal, Office 365 pentru acasă sau alte versiuni de Office, care fac parte dintr-un abonament Office 365.
> - Project și Visio care sunt oferite cu anumite planuri de abonament, cum ar fi planul Project Online Professional sau Visio Online Plan 2.
>
> Informațiile se aplică și la versiunea 16.28 sau la versiunile mai recente ale următoarelor aplicații Office pentru Mac: Excel, Outlook, OneNote, PowerPoint și Word.

Office constă din aplicațiile software client și experiențe conectate proiectate pentru a vă permite să creați, să comunicați și să colaborați mai eficient. Deși puteți controla multe dintre experiențele conectate care sunt la dispoziția dvs. sau a utilizatorilor dvs. în cazul în care sunteți administratorul organizației dvs., există un set de servicii care sunt esențiale pentru modul în care funcționează Office și care, prin urmare, nu pot fi dezactivate. De exemplu, serviciul de licențiere care confirmă că aveți licența corectă pentru a utiliza Office. Datele de serviciu necesare cu privire la aceste servicii sunt colectate și trimise la Microsoft, indiferent ce alte setări de politică privind confidențialitatea ați configurat. Puteți vedea aceste date utilizând Vizualizatorul de date de diagnosticare.

Pentru mai multe informații, consultați următoarele:

- [Date de serviciu obligatorii pentru Office](required-service-data.md)
- [Utilizarea Vizualizatorului de date de diagnosticare cu Office](https://support.office.com/article/cf761ce9-d805-4c60-a339-4e07f3182855)
- [Experiențe conectate în Office](connected-experiences.md)

Dacă sunteți administratorul organizației dvs., ați putea fi interesat și de următoarele:

- [Prezentare generală a controalelor de confidențialitate pentru Office 365 ProPlus](overview-privacy-controls.md)
- [Utilizați setările de politică pentru a gestiona controale de confidențialitate pentru Office 365 ProPlus](manage-privacy-controls.md)
- [Utilizați preferințele pentru a gestiona controalele de confidențialitate ale Office pentru Mac](mac-privacy-preferences.md)
- [Utilizați preferințele pentru a gestiona controalele de confidențialitate ale Office pe dispozitivele iOS.](ios-privacy-preferences.md)
- [Utilizați setările de politică pentru a gestiona controale de confidențialitate pentru Office pe dispozitivele Android](android-privacy-controls.md)

## <a name="list-of-essential-services-for-office"></a>Listă de servicii esențiale pentru Office 

Următorul tabel conține o listă a serviciilor esențiale pentru Office și o descriere a fiecărui serviciu.

| **Serviciu**  | **Descriere**  |
| ------ | ---- |
| [Autentificare](#authentication-events) | Autentificare este un serviciu multi-platformă care validează identitatea dvs. de utilizator Office.  Este necesar pentru a vă permite să vă conectați la Office, să vă activați licența de Office și să accesați fișierele stocate în cloud; oferă o experiență unitară la nivelul sesiunilor de Office și al dispozitivelor dvs.    |
| [Clic și Pornire](#click-to-run-events) | Clic și Pornire este tehnologia de instalare utilizată pentru a instala și a actualiza Office pe Windows. Aceasta caută noi versiuni de Office și, atunci când este disponibilă o nouă versiune, o descarcă și o instalează. Clic și Pornire va detecta dacă sunt necesare actualizări Office, inclusiv actualizări de securitate, le va descărca și le va instala.     |
| [Serviciul de configurație avansată (ECS)](#enhanced-configuration-service-ecs-events) | ECS oferă Microsoft capacitatea de a reconfigura instalările Office fără a fi nevoie să implementați din nou Office. Este utilizat pentru a controla implementarea treptată de caracteristici sau actualizări, în timp ce impactul implementării este monitorizat pe baza datelor de diagnosticare colectate. Este utilizat, de asemenea, pentru a atenua problemele de securitate sau de performanță cu o caracteristică sau actualizare. În plus, ECS acceptă modificările de configurare legate de datele de diagnosticare pentru a vă ajuta să vă asigurați că evenimentele corespunzătoare sunt colectate. |
| [Licențiere](#licensing-events)     | Licențiere este un serviciu bazat pe cloud care acceptă activarea Office pentru noile instalări și păstrează licența pe dispozitivele dvs. după ce Office a fost activat. Acesta înregistrează fiecare dintre dispozitivele dvs. și activează Office, verifică starea abonamentului Office și gestionează cheile de produs.    |
|[Microsoft AutoUpdate (MAU)](#microsoft-autoupdate-mau-events)|Microsoft AutoUpdate (MAU) este tehnologia utilizată pentru actualizarea aplicațiilor Microsoft produse pentru macOS, cum ar fi Office. MAU va detecta dacă sunt necesare actualizări ale aplicațiilor, inclusiv actualizări de securitate, le va descărca și le va instala.|
|[Sincronizare OneNote](#onenote-sync-events)|OneNote pentru Mac acceptă doar blocnotesurile stocate pe internet în OneDrive sau SharePoint Online. OneNote pentru Mac sincronizează continuu toate notele utilizatorului cu OneDrive sau SharePoint Online. Acest lucru le permite utilizatorilor să deschidă, să vizualizeze și să editeze blocnotesurile de pe toate dispozitivele, astfel încât blocnotesurile lor să fie întotdeauna actualizate.
 [Configurare servicii](#services-configuration-events)  | Configurare servicii oferă capacitatea de a efectua actualizări la setările de configurare Office pentru a activa sau a dezactiva caracteristici client. Este apelat de fiecare dată când pornește o aplicație Office și oferă detalii despre alte configurații și servicii Office. Configurare servicii controlează, de asemenea, ce servicii sunt desemnate ca servicii esențiale.  |
| [Telemetrie ](#telemetry-events)  | Serviciul de telemetrie este utilizat pentru a colecta date de diagnosticare din aplicațiile Office. Acesta permite colectarea datelor de diagnosticare generate de Office, atât datele de diagnosticare obligatorii, cât și cele opționale. De asemenea, este responsabil pentru colectarea porțiunii de date de diagnosticare a serviciului din datele de serviciu necesare pentru Office.  |

## <a name="events-and-data-fields-for-essential-services-for-office"></a>Evenimente și câmpuri de date pentru servicii esențiale pentru Office

Secțiunile următoare furnizează următoarele informații:

- O listă de evenimente pentru fiecare serviciu esențial
- O descriere a fiecărui eveniment
- O listă de câmpuri de date în fiecare eveniment
- O descriere a fiecărui câmp de date

Puteți vedea aceste evenimente utilizând Vizualizatorul de date de diagnosticare.



## <a name="authentication-events"></a>Evenimente de autentificare

Aceste evenimente cu date de diagnosticare sunt colectate atunci când Office încearcă să obțină un simbol de autentificare, fie în mod silențios, fie prin solicitare.

### <a name="officeandroidmsaguesttoaad"></a>Office.Android.MSAGuestToAAD

Acest eveniment vă ajută să înțelegeți câți utilizatori sunt notificați să furnizeze parolele conturilor personale când accesează resurse de lucru, atunci când contul personal poate fi un invitat valid al entității găzduite a contului de lucru.

Aceste date ne ajută să înțelegem câți utilizatori trec prin dificultatea de a li se solicita în mod repetat conectarea pentru a prioritiza în liniște achiziția simbolului AAD pe baza unei aserțiuni SAML (Security Assertion Markup Language) a contului Microsoft.

Se colectează următoarele câmpuri:

- **Tag** - indică faptul că un utilizator a primit o solicitare de conectare pentru contul personal în timp ce accesa o resursă a contului de la locul de muncă.


### <a name="officeidentityfbapromptwin32"></a>Office.Identity.FbaPromptWin32

Colectate atunci când Office prezintă utilizatorului o solicitare de conectare prin Autentificare bazată pe formulare.

Împreună cu achizițiile de simbol silențios, solicitările de autentificare sunt utilizate pentru a stabili dacă utilizatorul se află într-o stare de autentificare întreruptă, care, pentru utilizator, generează ceea ce este în esență o stare de client neconectat sau, în cel mai rău caz, autentificarea întreruptă poate să împiedice achiziționarea licenței, rezultatul fiind un client complet inutilizabil.

Solicitările de conectare Autentificare bazată pe formulare (FBA) sunt utilizate pentru unele scenarii de autentificare la nivel local și, de obicei, dorim să ne asigurăm că nu se întâmplă acest lucru, deoarece toată lumea ar trebui să utilizeze Autentificare modernă din cauza vulnerabilităților de securitate asociate cu FBA.

Se colectează următoarele câmpuri:

  - **AuthScheme** - schema de autentificare utilizată

  - **DocumentUrlHash** - o solicitare de URL criptat

  - **EndTag** - eticheta unde se termină formularul FBA

  - **Flags** - Depășit

  - **FlowTag** - eticheta unde începe formularul FBA

  - **LastError** - codul de eroare returnat

  - **PromptEndTime** - ora când s-a terminat solicitarea

  - **PromptStartTime** - ora când a început solicitarea

  - **Result** - dacă autentificarea a reușit

  - **SessionEndTime** - ora când s-a terminat sesiunea de eveniment

  - **Timeout** - ora când a expirat solicitarea

### <a name="officeidentitysignoutevent"></a>Office.Identity.SignOutEvent

Colectate atunci când un utilizator se deconectează din Office.

Cunoașterea faptului că utilizatorul este deconectat permite clasificarea altor evenimente, cum ar fi solicitările, potrivit așteptărilor, astfel încât evenimentele respective pot fi calculate în mod corect în măsurători de fiabilitate/pregătire pentru expediere; totodată, se evită alerta sau revenirea compilărilor pe premisa incorectă că utilizatorul primește solicitări de conectare neașteptate.

Se colectează următoarele câmpuri:

  - **FlowEndTime** - ora când s-a terminat acțiunea de deconectare

  - **FlowStartTime** - ora când a început acțiunea de deconectare

  - **IdentityErrorState** - orice stare de eroare de identitate în timpul deconectării

  - **IdentityHashedUniqueId** - ID-ul identității criptate care este deconectat

  - **IdentityProviderType** - furnizorul de identitate al identității care este deconectată

  - **IdentityUniqueID** - ID-ul identității care este deconectat

  - **SessionEndTime** - ora când s-a terminat sesiunea de eveniment

  - **SignOutUserAction** - indică faptul că utilizatorul inițiază acțiunea de deconectare

### <a name="officeidentitysspipromptwin32"></a>Office.Identity.SspiPromptWin32

Colectate atunci când Office prezintă utilizatorului o solicitare de conectare Windows SSPI. Împreună cu achizițiile de simbol silențios, solicitările de autentificare stabilesc dacă un utilizator se află într-o stare de autentificare întreruptă, care generează o stare de client neconectat. Autentificarea întreruptă poate să împiedice achiziționarea licenței, rezultatul fiind un client complet inutilizabil.

Solicitările Windows SSPI sunt utilizate pentru autentificarea cu Exchange (pentru sincronizarea corespondenței) atunci când resursa Exchange a utilizatorului nu a fost configurată pentru autentificare multi-factor.

Aceste evenimente, împreună cu evenimentele cu spațiu de nume Office.MATS, sunt utilizate în următoarele scopuri:

1\) Identificați dacă clienții pot obține cu succes un simbol de autentificare sau dacă au intrat într-o stare de autentificare întreruptă.

2\) Evaluați dacă modificările care au avut loc la nivelul clientului sau al serviciilor au dus la regresii critice ale fiabilității și experienței de autentificare a utilizatorului

3\) Atunci când apar erori, aceste semnale emit coduri de eroare importante de la componenta responsabilă (cod de client Office, biblioteci de autentificare sau servicii de autoritate) care pot fi utilizate pentru triere, diagnosticare și atenuare

4\) Aceste semnale alimentează diverse monitoare de pregătire pentru expediere și bună funcționare care declanșează avertizări pentru ca inginerii noștri să se implice rapid și să reducă timpul de atenuare a erorilor critice de blocare a utilizatorului

Se colectează următoarele câmpuri:

  - **AllowSavedCreds** - dacă noua acreditare este persistentă

  - **AuthScheme** - schema de autentificare utilizată

  - **CredsSaved** - dacă se salvează noua acreditare

  - **DocumentUrlHash** - solicitarea de URL criptat

  - **EndTag** - eticheta unde s-a terminat solicitarea

  - **NewIdentity**\_ErrorState - dacă noua identitate este validă

  - **NewIdentity\_HashedUniqueId** - ID-ul noii identități criptate după ce solicitarea este finalizată

  - **NewIdentity\_ProviderType** - furnizorul noii identități după ce solicitarea este finalizată

  - **NewIdentity\_UniqueID** - ID-ul noii identități după ce solicitarea este finalizată

  - **OutStatus** - dacă ieșirea solicitării este validă

  - **PromptEndTime** - ora când s-a terminat solicitarea

  - **PromptFailedTag** - eticheta care indică o solicitare SSPI nereușită

  - **PromptFlow** - eticheta care a invocat solicitarea SSPI

  - **PromptStartTime** - ora când a început solicitarea

  - **Proxy** - dacă se utilizează proxy

  - **ServerHash** - adresă server criptată

  - **SessionEndTime** - ora când s-a terminat sesiunea de eveniment

  - **Timeout** - ora când expiră solicitarea

  - **UiMessage** - mesajul UI din solicitare

  - **UserNameHash** - numele de utilizator criptat

### <a name="officeidentitywin32prompt"></a>Office.Identity.Win32Prompt

Colectate atunci când Office prezintă utilizatorului o solicitare de conectare prin autentificare multi-factor. Împreună cu achizițiile de simbol silențios, solicitările de autentificare stabilesc dacă un utilizator se află într-o stare de autentificare întreruptă, care generează o stare de client neconectat. Autentificarea întreruptă poate să împiedice achiziționarea licenței, rezultatul fiind un client complet inutilizabil.

Aceste evenimente, împreună cu evenimentele cu spațiu de nume Office.MATS, sunt utilizate în următoarele scopuri:

1\) Identificați dacă clienții pot obține cu succes un simbol de autentificare sau dacă au intrat într-o stare de autentificare întreruptă.

2\) Evaluați dacă modificările care au avut loc la nivelul clientului sau al serviciilor au dus la regresii critice ale fiabilității și experienței de autentificare a utilizatorului

3\) Atunci când apar erori, aceste semnale emit coduri de eroare importante de la componenta responsabilă (cod de client Office, biblioteci de autentificare sau servicii de autoritate) care pot fi utilizate pentru triere, diagnosticare și atenuare

4\) Aceste semnale alimentează diverse monitoare de pregătire pentru expediere și bună funcționare care declanșează avertizări pentru ca inginerii noștri să se implice rapid și să reducă timpul de atenuare a erorilor critice de blocare a utilizatorului.

Se colectează următoarele câmpuri:

  - **AdalWAMUsed** - eticheta care indică rezultatul dacă se utilizează ADAL-atop-WAM

  - **CallTag** - eticheta care indică apelantul UI de conectare

  - **Context** - contextul de conectare pentru solicitare

  - **EndTagIdentityProviderRequested** - eticheta unde se solicită furnizorul de identitate

  - **HrdShownTag** - eticheta unde se afișează caseta de dialog de conectare HRD

  - **IdentityProviderResulted** - tipul de furnizor de identitate pe care îl solicită

  - **IdPFlowTag** - eticheta care indică rezultatul solicitării de identitate

  - **LastLoginDelta** - delta timp de la ultima conectare reușită

  - **NewIdentity\_ErrorState** - dacă identitatea este validă după solicitare

  - **NewIdentity\_ProviderType** - tipul de furnizor al noii identități după solicitare

  - **NewIdentity\_UniqueID** - ID-ul noii identități returnat după solicitare

  - **PromptCorrelation** - ID-ul de corelare a solicitării în scopuri de diagnosticare

  - **PromptEndTime** - ora când s-a terminat solicitarea

  - **PromptStartTime** - ora când a început solicitarea

  - **SessionEndTime** - ora când s-a terminat sesiunea de eveniment

  - **ShowUIResult** - codul de rezultat returnat de interfața de utilizator pentru solicitare

  - **StartTag** - eticheta unde a început solicitarea Win32

  - **Timeout** - ora când expiră solicitarea

  - **WasIdentitySignedOut** - dacă utilizatorul este deconectat

### <a name="officematsactionofficewin32-officematsactionofficewinrt"></a>Office.MATS.actionofficewin32, Office.MATS.actionofficewinrt

Descrierea următoare se aplică atât pentru evenimente Win32, cât și WinRT (numele depinde de platformă.)

Microsoft Auth Telemetry System (MATS) este colectat atunci când Office încearcă să obțină un simbol de autentificare, fie în mod silențios, fie prin solicitare. Atunci când încercările de achiziționare eșuează, sunt incluse informații de eroare. Aceste evenimente ajută utilizatorii să nu intre în stări de autentificare întreruptă după cum urmează:

1\) Identifică dacă clienții pot obține cu succes un simbol de autentificare sau dacă au intrat într-o stare de autentificare întreruptă.

2\) Evaluează când anume au loc modificări la nivelul clientului sau al serviciilor, dacă acestea duc la regresii critice ale fiabilității și experienței de autentificare a utilizatorului

3\) Atunci când apar erori, aceste semnale emit coduri de eroare importante de la componenta responsabilă (cod de client Office, biblioteci de autentificare sau servicii de autoritate) care pot fi utilizate pentru triere, diagnosticare și atenuare

4\) Aceste semnale alimentează diverse monitoare de pregătire pentru expediere și bună funcționare care declanșează avertizări pentru ca inginerii noștri să se implice rapid și să reducă timpul de atenuare a erorilor critice.

Se colectează următoarele câmpuri:

  - **Actiontype** - ce bibliotecă de autentificare se utilizează

  - **Appaudience** - este versiunea de aplicație pentru uz intern sau extern

  - **Appforcedprompt** - a înlocuit aplicația memoria cache și a impus afișarea unei solicitări

  - **Appname** - numele aplicației care efectuează autentificarea

  - **Appver** - versiunea aplicației care efectuează autentificarea

  - **Askedforcreds** - i-a solicitat aplicația utilizatorului să introducă acreditări pentru această acțiune

  - **Authoutcome** - a reușit încercarea de autentificare, a eșuat sau a fost anulată

  - **Blockingprompt** - a lansat aplicația o solicitare care necesită interacțiune cu utilizatorul

  - **Correlationid** - GUID utilizat pentru asocierea cu datele serviciilor

  - **Count** - număr de evenimente în cazuri de agregare

  - **Data\_accounttype** - cont de consumator sau de organizație

  - **Devicenetworkstate** - a fost utilizatorul online

  - **Deviceprofiletelemetryid** - ID de dispozitiv anonim utilizat pentru a măsura experiența dispozitivului

  - **Duration** - cât a durat autentificarea

  - **Endtime** - când s-a terminat evenimentul de autentificare

  - **Error** - codul de eroare dacă autentificarea nu a reușit

  - **Errordescription** - scurtă descriere a erorii

  - **Errorsource** - a provenit eroarea de la serviciu, de la biblioteca de autentificare sau de la aplicație

  - **Identityservice** - a fost invocat serviciul Microsoft Service Account (MSA) sau Azure Active Directory (AAD)

  - **Interactiveauthcontainer** - ce tip de solicitare a fost afișată

  - **Issilent** - a fost afișată o solicitare

  - **Microsoft**\_**ADAL**\_**adal**\_**version** - versiune a Azure Active Directory Authentication Library (ADAL)

  - **Microsoft\_ADAL\_api\_error\_code** - cod de eroare emis de biblioteca de autentificare pentru această încercare de autentificare

  - **Microsoft\_ADAL\_api\_id** - API invocat pentru această încercare de autentificare

  - **Microsoft\_ADAL\_authority** - URL al autorității Azure Active Directory responsabil pentru autentificarea utilizatorului

  - **Microsoft\_ADAL\_authority\_type** - Acord de furnizare servicii pentru consumatori/Acordul de furnizare a serviciilor Microsoft (MSA) versus Azure Active Directory (AAD)/de organizație; în prezent întotdeauna AAD

  - **Microsoft\_ADAL\_authority\_validation\_status** - informează dacă autentificarea s-a finalizat pe partea serviciului

  - **Microsoft\_ADAL\_broker\_app** - informează dacă ADAL a utilizat un broker pentru autentificare

  - **Microsoft\_ADAL\_broker\_app\_used** - menționează numele brokerului (de ex., Windows Account Management)

  - **Microsoft\_ADAL\_broker\_version** - menționează versiunea brokerului în cazul în care s-a utilizat

  - **Microsoft\_ADAL\_cache\_event\_count** - numărul de evenimente aferente cache efectuate de ADAL efectuate în timpul regăsirii simbolului

  - **Microsoft\_ADAL\_cache\_event\_count\_max** - dacă acest semnal este agregat, numărul maxim de evenimente aferente cache ale oricăruia dintre evenimentele agregate.

  - **Microsoft\_ADAL\_cache\_event\_count\_min** - dacă acest semnal este agregat, numărul minim de evenimente aferente cache ale oricăruia dintre evenimentele agregate.

  - **Microsoft\_ADAL\_cache\_event\_count\_sum** - dacă acest semnal este agregat, suma evenimentelor aferente cache ale tuturor evenimentelor agregate.

  - **Microsoft\_ADAL\_cache\_read\_count** - de câte ori citește API din cache de pe disc. Prezent dacă a existat cel puțin o citire.

  - **Microsoft\_ADAL\_cache\_read\_error\_count** - de câte ori a eșuat citirea cache de pe disc. Este prezent dacă a existat cel puțin o nereușită.

  - **Microsoft\_ADAL\_cache\_read\_last\_error** - cod de eroare ADAL. Prezent dacă a existat cel puțin o citire nereușită.

  - **Microsoft\_ADAL\_cache\_read\_last\_system\_error** - cod de eroare sistem. Este prezent dacă a existat cel puțin o citire nereușită.

  - **Microsoft\_ADAL\_cache\_write\_count** - de câte ori a scris API în cache de pe disc. Prezent dacă a existat cel puțin o scriere.

  - **Microsoft\_ADAL\_cache\_write\_error\_count** - de câte ori a eșuat scrierea în cache de pe disc. Prezent dacă a existat cel puțin o nereușită.

  - **Microsoft\_ADAL\_cache\_write\_last\_error** - cod de eroare ADAL. Prezent dacă a existat cel puțin o scriere nereușită.

  - **Microsoft\_ADAL\_cache\_write\_last\_system\_error** - cod de eroare sistem. Prezent dacă a existat cel puțin o scriere nereușită.

  - **Microsoft\_ADAL\_client\_id** - ID de aplicație AAD codat hash.

  - **Microsoft\_ADAL\_extended\_expires\_on\_setting** - informare adevărată/falsă dacă simbolul are o durată de viață extinsă.

  - **Microsoft\_ADAL\_http\_event\_coun**t - numărul de apeluri HTTP efectuate de ADAL.

  - **Microsoft\_ADAL\_http\_event\_count\_max** - dacă acest semnal este agregat, numărul max. de apeluri HTTP efectuate de ADAL pentru orice eveniment agregat.

  - **Microsoft\_ADAL\_http\_event\_count\_min** - dacă acest semnal este agregat, numărul min. de apeluri HTTP efectuate de ADAL pentru orice eveniment agregat.

  - **Microsoft\_ADAL\_http\_event\_count\_sum** - dacă acest semnal este agregat, suma numărul apelurilor HTTP efectuate de ADAL pentru toate evenimentele agregate.

  - **Microsoft\_ADAL\_is\_silent\_ui** - informare adevărată/falsă dacă UI a fost afișată (solicitată) de ADAL.

  - **Microsoft\_ADAL\_is\_successful** - informare adevărată/falsă dacă ADAL API a reușit.

  - **Microsoft\_ADAL\_logging\_pii\_enabled** - informare adevărată/falsă dacă modul de înregistrare în jurnal completă ADAL este activat. Aceste date sunt înregistrate în jurnal doar local, fără să fie emise în telemetrie.

  - **Microsoft\_ADAL\_oauth\_error\_code** - codul de eroare al protocolului OAuth returnat de serviciu.

  - **Microsoft\_ADAL\_prompt\_behavior** - parametru HTTP de conectare sau niciunul transferat la serviciu pentru a specifica dacă interfața cu utilizatorul poate fi afișată.

  - **Microsoft\_ADAL\_request\_id** - GUID tranzacțional pentru solicitarea emisă de ADAL la serviciu.

  - **Microsoft\_ADAL\_response\_code** - cod răspuns HTTP de la serviciu.

  - **Microsoft\_ADAL\_response\_time** - cât timp a fost necesar serviciului pentru a reveni la ADAL.

  - **Microsoft\_ADAL\_response\_time\_max** - dacă semnalul este agregat, timpul max. care a fost necesar pentru ca ADAL să revină de la API printre oricare dintre evenimentele agregate.

  - **Microsoft\_ADAL\_response\_time\_min** - dacă semnalul este agregat, timpul min. care a fost necesar serviciului pentru a răspunde ADAL printre oricare dintre evenimentele agregate.

  - **Microsoft\_ADAL\_response\_time\_sum** - dacă semnalul este agregat, suma timpului necesar pentru ca ADAL să revină de la API printre toate evenimentele agregate.

  - **Microsoft\_ADAL\_rt\_age** - vârsta simbolului de reîmprospătare

  - **Microsoft\_ADAL\_server\_error\_code** - codul de eroare returnat de server

  - **Microsoft\_ADAL\_server\_sub\_error\_code** - subcod de eroare returnat de server pentru a contribui la clarificarea motivului pentru care solicitarea nu a reușit.

  - **Microsoft\_ADAL\_spe\_ring** - informare adevărată/falsă dacă utilizatorul utiliza cercul interior Secure Production Enterprise (numai angajații Microsoft).

  - **Microsoft\_ADAL\_start\_time** - ora la care a fost efectuat apelul ADAL API

  - **Microsoft\_ADAL\_stop\_time** - ora la care a fost returnat apelul ADAL API

  - **Microsoft\_ADAL\_telemetry\_pii\_enabled** - informare adevărată/falsă dacă modul de telemetrie completă ADAL este activat. Numele este un termen impropriu, deoarece nu sunt emise PII/EUII.

  - **Microsoft\_ADAL\_tenant\_id** - GUID de identificare a entității găzduite căreia îi aparține utilizatorul autentificat.

  - **Microsoft\_ADAL\_token\_acquisition\_from\_context** - descrie comportamentul ADAL pe baza simbolurilor din contextul de autentificare.

  - **Microsoft\_ADAL\_token\_type** - simbol de reîmprospătare (RT) sau simbol de reîmprospătare resurse multiple (MRRT).

  - **Microsoft\_ADAL\_ui\_event\_count** - numărul de solicitări afișate utilizatorului. Posibil să fi fost silențios.

  - **Microsoft\_ADAL\_user\_cancel** - adevărat/fals dacă fereastra interfeței cu utilizatorul a fost anulată.

  - **Microsoft\_ADAL\_x\_ms\_request\_id** - ID solicitare suplimentar furnizat în antetul HTTP la serviciu de către ADAL.

  - **Platform** - Win32/WinRT/Android/iOS/Mac

  - **Scenarioid** - GUID. Mai multe evenimente pot aparține unui singur scenariu, de ex., scenariul poate fi adăugarea unui cont nou, dar există mai multe solicitări care apar ca parte a scenariului respectiv. Acest ID permite corelarea.

  - **Sessionid** - GUID de identificare a sesiunii de pornire

  - **Skdver** - versiune de MATS client SDK utilizată pentru a produce aceste date

  - **Starttime** - ora la care a fost apelată Acțiunea de\*Începere MATS API

  - **Tenantid** - GUID de identificare a entității găzduite căreia îi aparține utilizatorul autentificat (în cazuri non-ADAL).

  - **Uploadid** - GUID unic pentru acest eveniment, utilizat pentru deduplicare

  - **Wamapi** - identifică ce WAM API este apelat

  - **Wamtelemetrybatch** - momentan neutilizat. În viitor, permite componentei WAM să expedieze informații suplimentare referitoare la evenimentul de autentificare.

### <a name="onenotesigninssoexternalappsaccountfound"></a>OneNote.SignIn.SSOExternalAppsAccountFound
 
Acest eveniment este înregistrat când un cont cu un simbol de reîmprospătare valid se găsește în lista de conturi furnizate de TokenSharingManager.  Acest scenariu este specific pentru Sign-on unic (SSO).
 
Se colectează următoarele câmpuri:
 
- **AccountType** - înregistrează tipul de cont

- **ProviderPackageID** - înregistrează ID-ul pachetului aplicației care a furnizat acest cont

### <a name="onenotesigninssoexternalappsinvalidaccount"></a>OneNote.SignIn.SSOExternalAppsInvalidAccount

Acest eveniment se înregistrează când a apărut o eroare atunci când s-a încercat obținerea unui simbol de reîmprospătare pentru un cont din lista de conturi furnizate de TokenSharingManager. Acest scenariu este specific pentru Sign-on unic (SSO)
 
Se colectează următoarele câmpuri:
 
- **RawError** - înregistrează eroarea brută obținută la încercarea de a obține un simbol de reîmprospătare cu contul dat

### <a name="onenotestickynotesfetchtokencompleted"></a>OneNote.StickyNotes.FetchTokenCompleted
 
Acest eveniment este înregistrat după autentificare, atunci când preluarea simbolului de reîmprospătare s-a încheiat.
 
Se colectează următoarele câmpuri:
 
- **ErrorMessage** - dacă preluarea simbolului nu a reușit, aici s-ar înregistra mesajul de eroare 

- **Result** - înregistrează rezultatul tentativei de preluare a simbolului

- **StickyNoteAccountType** - înregistrează tipul contului pentru care aplicația încerca să preia simbolul de reîmprospătare


## <a name="click-to-run-events"></a>Evenimente Clic și Pornire

### <a name="officeclicktorunbootstrapper"></a>Office.ClickToRun.Bootstrapper 

Date despre instalări și inventar Office colectate atunci când utilizatorul execută setup.exe Office pentru a modifica produsele Office instalate. Utilizat pentru a măsura succesul/eșecul unei instalări complete de Office inițiate de utilizator, inclusiv verificările cerinței preliminare.

Se colectează următoarele câmpuri:

  - **Data\_BootStrapperStateFailure\_ErrorCode** - codul de eroare cu care am eșuat

  - **Data\_BootStrapperStateFailure\_ErrorSource** - funcția în care am eșuat

  - **Data\_BootStrapperStateFailure\_FailingState** - partea în care am eșuat în boostrapperbootstrapper

  - **Data\_BootStrapperStateFailure\_OExceptionType** - tipul de excepție cu care am eșuat

  - **Data\_Culture** - cultura cu care rulăm acest exe, de ex. ro-ro

  - **Data\_HashedOLSToken** - un cod hash sha-256 al unui simbol pe care ni-l dă serviciul OLS

  - **Data\_Platform** - instalare x64 sau x86

  - **Data\_PrereqFailure\_Type** - eroarea de cerință preliminară pe care am întâmpinat-o, adică sistemul de operare nu este acceptat

  - **Data\_ProductReleaseId-** Produsul pe care îl instalăm, adică Office 365 ProPlus

### <a name="officeclicktoruncorruptioncheck"></a>Office.ClickToRun.CorruptionCheck

Date despre instalări și inventar Office colectate atunci când clientul Clic și Pornire rulează clientul rulează o verificare de deteriorare pentru a vă asigura că fișierele binare Office sunt corecte. Utilizat pentru a măsura deteriorarea fișierelor binare Office și ce fișiere binare sunt deteriorate.

Se colectează următoarele câmpuri:

  - **Data\_Active -** manifestul flux curent pe care îl verificăm pe disc

  - **Data\_ActivePackages -** ce pachete conține manifestul

  - **Data\_ActiveVersion -** versiunea de manifest

  - **Data\_AddFileCount -** câte fișiere adăugăm

  - **Data\_AddFileFiles -** un eșantion de fișiere pe care le adăugăm

  - **Data\_CompressionLevel -** cum sunt comprimate fișierele

  - **Data\_CorruptionCheckLevel -** cât de profund verificăm deteriorarea, etape

  - **Data\_CorruptSizeCount -** câte fișiere au dimensiunea deteriorată

  - **Data\_CorruptSizeFiles -** un eșantion de fișiere cu dimensiunea deteriorată

  - **Data\_CorruptVersionCount -** câte fișiere au o versiune deteriorată

  - **Data\_CorruptVersionFiles -** un eșantion de fișiere cu versiunea deteriorată

  - **Data\_FileBadDigestCount -** câte fișiere nu am reușit să deschidem

  - **Data\_FileBadDigestFiles -** un eșantion de fișiere pe care nu am putut să le deschidem

  - **Data\_FileNotSignedCount -** au multe fișiere nesemnate

  - **Data\_FileNotSignedFiles -** un eșantion de fișiere nesemnate

  - **Data\_FileNotTrustedCount -** câte fișiere nu sunt de încredere

  - **Data\_FileNotTrustedFiles -** un eșantion de fișiere în care nu avem încredere

  - **Data\_IncompleteFileCount -** câte fișiere par incomplete

  - **Data\_IncompleteFileFiles -** un eșantion de fișiere incomplete

  - **Data\_KeepFileCount -** asupra câtor fișiere nu intervenim

  - **Data\_KeepFileFiles -** un eșantion de fișiere pe care le păstrăm

  - **Data\_KeepIncompleteFileCount -** câte fișiere nu modificăm deși sunt incomplete

  - **Data\_KeepIncompleteFileFiles -** un eșantion de fișiere pe care le păstrăm și care sunt incomplete

  - **Data\_MismatchSizeCount -** câte fișiere au o dimensiune care nu corespunde manifestului nostru

  - **Data\_MismatchSizeFiles -** un eșantion de fișiere care nu corespund ca dimensiune

  - **Data\_MismatchVersionCount -** câte fișiere au o versiune diferită de manifestul nostru

  - **Data\_MismatchVersionFiles -** un eșantion de fișiere care au versiuni ce nu corespund

  - **Data\_MissingFileCount -** câte fișiere par să lipsească

  - **Data\_MissingFileFiles -** un eșantion de fișiere care lipsesc

  - **Data\_NotToBeStreamedFileCount -** câte fișiere nu redăm în flux

  - **Data\_RemoveFileCount -** câte fișiere eliminăm

  - **Data\_RemoveFileFiles -** un eșantion de fișiere pe care le eliminăm

  - **Data\_StreamUnitsMismatchCount -** câte fișiere au unități care nu corespund cu manifestul

  - **Data\_StreamUnitsMismatchFiles -** un eșantion de fișiere care au un flux cu unități care nu corespund

  - **Data\_TimeElapsed -** cât timp ne-a luat pentru a căuta deteriorări

  - **Data\_UpdateFileCount -** câte fișiere actualizăm

  - **Data\_UpdateFileFiles -** un eșantion de fișiere pe care le adăugăm

  - **Data\_Working -** noul manifest pe care îl verificăm

  - **Data\_WorkingVersion -** versiunea noului manifest

### <a name="officeclicktorunmachinemetadata"></a>Office.ClickToRun.MachineMetadata

Date despre instalări și inventar Office care oferă metadatele necesare pentru instalare și inventar și sunt utilizate pentru a stabili o bază de instalare precisă.

Se colectează următoarele câmpuri:

  - **Data\_C2RClientVer** - versiunea de OfficeClickToRun.exe pe computer

  - **Data\_OfficeBitness** - numărul de biți pe care este instalat Office, x86 sau x64

  - **Data\_OfficeVersion** - versiunea în care este instalat Office

  - **Data\_Sku** - SKU-ul instalat, adică Office 365 ProPlus.ro-ro

  - **Data\_SqmMachineID** - ID unic de computer utilizat de Date SQM Windows\_SusClientID- identificator actualizare Office computer

### <a name="officeclicktorunodt"></a>Office.ClickToRun.ODT

Date despre instalări și inventar Office colectate atunci când un administrator IT rulează Instrumentul de implementare Office Clic și Pornire setup.exe pentru a modifica produsele Office instalate ale utilizatorilor. Este utilizat pentru a măsura succesul/eșecul instalărilor complete de Office inițiate de administratorul IT, inclusiv verificările cerinței preliminare.

Se colectează următoarele câmpuri:

  - **Data\_BootStrapperStateFailure\_ErrorCode-** codul de eroare cu care am eșuat

  - **Data\_BootStrapperStateFailure\_ErrorSource-** funcția în care am eșuat

  - **Data\_BootStrapperStateFailure\_FailingState -** partea în care am eșuat în boostrapper

  - **Data\_BootStrapperStateFailure\_OExceptionType-** tipul de excepție cu care am eșuat

  - **Data\_ConfigurationHost-** gazda de unde provine configurație.xml

  - **Data\_ConfigurationId-** ID-ul pe care îl obținem de la un fișier configurație.xml

  - **Data\_ConfigurationSource-** de unde provine configurație.xml

  - **Data\_Culture-** cultura cu care rulăm acest exe, adică ro-ro

  - **Data\_HashedOLSToken-** un cod hash sha-256 al unui simbol pe care ni-l dă serviciul OLS

  - **Data\_MigrateArchRequest-** dacă migrăm utilizatorul de la x86 la x64 sau invers

  - **Data\_MigrateArchRequestValid-** dacă considerăm că solicitarea de migrare este validă

  - **Data\_Platform-** instalare x64 sau x86

  - **Data\_PlatformMigratedFrom-** pornire platformă, adică x86

  - **Data\_PlatformMigratedTo-** sfârșit platformă, adică x64

  - **Data\_PrereqFailure\_Type-** eroarea de cerință preliminară pe care am întâmpinat-o

  - **Data\_ProductReleaseId-** Produsul pe care îl instalăm, adică Office 365 ProPlus

### <a name="officeclicktorunrepomanlogger"></a>Office.ClickToRun.RepomanLogger

Raportează despre starea noului canal de actualizare Clic și Pornire („Repoman”) și dacă acesta descarcă și aplică actualizări Office cu succes.

Se colectează următoarele câmpuri:

  - **ApplySucceeded -** adevărat în cazul în care canalul a aplicat o actualizare Office cu succes, fals dacă nu.
  
  - **ApplySucceeded -** adevărat în cazul în care canalul a descărcat o actualizare Office cu succes, fals dacă nu.

  - **ErrorCode -** codul ultimei erori apărute în canalul Clic și Pornire Repoman.

  - **ErrorDetails -**  detaliile suplimentare ale erorii pentru ultima eroare apărută în canalul Clic și Pornire Repoman.
 
  - **ErrorMessage -** mesajul ultimei erori apărute în canalul Clic și Pornire Repoman.

  - **OpenStreamSessionSucceeded -** adevărat în cazul în care canalul creează cu succes o sesiune pentru redarea unei actualizări Office, fals dacă nu.

  - **RepomanErrorMessage -** mesajul de eroare primit de la repoman.dll.
 

### <a name="officeclicktorunscenarioinstalltaskconfigure"></a>Office.ClickToRun.Scenario.InstallTaskConfigure

Date despre instalări și inventar Office colectate atunci când programul de instalare Office plasează fișiere recent descărcate. Utilizat pentru a măsura succesul/eșecul unei instalări de Office.

Se colectează următoarele câmpuri:

  - **Data\_15\_SourceType -** unde se află sursa Office 15, adică CDN sau local 

  - **Data\_15\_UpdatesEnabled -** dacă sunt activate actualizările Office 15 

  - **Data\_15\_UpdateVersion -** la ce versiune Office 15 actualizăm 

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled -** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion-** ce versiune de Office 16 actualizați la 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** Produsele pe care le adăugăm 

  - **Data\_AddingProducts -** Ce produse ni s-a solicitat să adăugăm 

  - **Data\_CompletionState -** dacă am finalizat activitatea

  - **Data\_ErrorCode -** codul de eroare cu care am eșuat 

  - **Data\_ErrorDetails -** detalii suplimentare despre o eroare 

  - **Data\_ErrorMessage -** mesaj de eroare despre ce nu a funcționat bine 

  - **Data\_ErrorSource -** unde s-a produs eroarea 

  - **Data\_ExceptionType -** excepția cu care am eșuat 

  - **Data\_IsErrorCodeIgnorable -** dacă codul de eroare cu care am eșuat poate fi ignorat 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth -** dacă considerăm că codul de eroare poate fi ignorat 

  - **Data\_NewestPackageVersion -** cea mai nouă versiune de Office de pe computer 

  - **Data\_OldestPackageVersion -** cea mai veche versiune de Office de pe computer 

  - **Data\_ProductsToAdd -** Ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează. adică, instalare 

  - **Data\_ScenarioSubType -** Ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

  - **Data\_SourceType -** unde se află sursa noastră, adică CDN 

  - **Data\_SqmMachineID -** ID unic de computer utilizat de Windows SQM 

  - **Data\_SusClientID -** identificator de actualizare Office computer 

  - **Data\_TaskState -** care este starea activității, cum ar fi rulare sau anulat 

  - **Data\_TotalClientCabSize -** dimensiunea fișierului cab al clientului nostru 

  - **Data\_TriggeringUI -** ce a declanșat interfața cu utilizatorul 

  - **Data\_UpdatesEnabled -** dacă sunt activate actualizările Office 

  - **Data\_Version -** versiunea de Office 

### <a name="officeclicktorunscenarioinstalltaskconfigurelight"></a>Office.ClickToRun.Scenario.InstallTaskConfigurelight

Date despre instalări și inventar Office colectate atunci când programul de instalare Office stabilește ce fișiere trebuie descărcate. Utilizat pentru a măsura succesul/eșecul instalării Office.

Se colectează următoarele câmpuri:

  - **Data\_15\_SourceType -** unde se află sursa Office 15, adică CDN sau local 

  - **Data\_15\_UpdatesEnabled -** dacă sunt activate actualizările Office 15 

  - **Data\_15\_UpdateVersion -** la ce versiune Office 15 actualizăm 

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion-** ce versiune de Office 16 actualizați la 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** Produsele pe care le adăugăm 

  - **Data\_AddingProducts -** Ce produse ni s-a solicitat să adăugăm 

  - **Data\_CompletionState -** dacă am finalizat activitatea

  - **Data\_ErrorCode -** codul de eroare cu care am eșuat 

  - **Data\_ErrorDetails -** detalii suplimentare despre o eroare 

  - **Data\_ErrorMessage -** un mesaj de eroare despre ce nu a funcționat bine 

  - **Data\_ErrorSource -** unde s-a produs eroarea 

  - **Data\_ExceptionType -** excepția cu care am eșuat 

  - **Data\_IsErrorCodeIgnorable -** dacă codul de eroare cu care am eșuat poate fi ignorat 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth -** dacă considerăm că codul de eroare poate fi ignorat 

  - **Data\_NewestPackageVersion -** cea mai nouă versiune de Office de pe computer 

  - **Data\_OldestPackageVersion -** cea mai veche versiune de Office de pe computer 

  - **Data\_ProductsToAdd -** Ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează. adică, instalare 

  - **Data\_ScenarioSubType -** Ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

  - **Data\_SourceType -** unde se află sursa noastră, adică CDN 

  - **Data\_SqmMachineID -** ID unic de computer utilizat de Windows SQM 

  - **Data\_SusClientID-** identificator de actualizare Office computer 

  - **Data\_TaskState -** care este starea activității, cum ar fi rulare sau anulat 

  - **Data\_TotalClientCabSize -** dimensiunea fișierului cab al clientului nostru 

  - **Data\_TriggeringUI -** ce a declanșat interfața cu utilizatorul 

  - **Data\_UpdatesEnabled -** dacă sunt activate actualizările Office 

  - **Data\_Version -** versiunea de Office 

### <a name="officeclicktorunscenarioinstalltaskfinalintegrate"></a>Office.ClickToRun.Scenario.InstallTaskFinalintegrate

Date despre instalări și inventar Office colectate atunci când programul de instalare Office instalează setări de licențe și registry. Utilizat pentru a măsura succesul/eșecul instalării Office.

Se colectează următoarele câmpuri:

  - **Data\_15\_SourceType -** unde se află sursa Office 15, adică CDN sau local 

  - **Data\_15\_UpdatesEnabled -** dacă sunt activate actualizările Office 15 

  - **Data\_15\_UpdateVersion -** La ce versiune Office 15 actualizăm

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled -** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion  -** Ce versiune de Office 16 actualizăm 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** Produsele pe care le adăugăm 

  - **Data\_AddingProducts -** Ce produse ni s-a solicitat să adăugăm 

  - **Data\_CompletionState -** dacă am finalizat activitatea

  - **Data\_ErrorCode -** codul de eroare cu care am eșuat 

  - **Data\_ErrorDetails -** detalii suplimentare despre o eroare 

  - **Data\_ErrorMessage -** un mesaj de eroare despre ce nu a funcționat bine 

  - **Data\_ErrorSource -** unde s-a produs eroarea

  - **Data\_ExceptionType -** excepția cu care am eșuat 

  - **Data\_IsErrorCodeIgnorable -** dacă codul de eroare cu care am eșuat poate fi ignorat 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth -** dacă considerăm că codul de eroare poate fi ignorat 

  - **Data\_NewestPackageVersion -** cea mai nouă versiune de Office de pe computer 

  - **Data\_OldestPackageVersion -** cea mai veche versiune de Office de pe computer 

  - **Data\_ProductsToAdd -** Ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează. adică, instalare 

  - **Data\_ScenarioSubType -** Ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

  - **Data\_SourceType -** unde se află sursa noastră, adică CDN 

  - **Data\_SqmMachineID -** ID unic de computer utilizat de Windows SQM 

  - **Data\_SusClientID-** identificator de actualizare Office computer 

  - **Data\_TaskState -** care este starea activității, cum ar fi rulare sau anulat 

  - **Data\_TotalClientCabSize -** dimensiunea fișierului cab al clientului nostru 

  - **Data\_TriggeringUI -** ce a declanșat interfața cu utilizatorul 

  - **Data\_UpdatesEnabled -** dacă sunt activate actualizările Office 

  - **Data\_Version -** versiunea de Office 

### <a name="officeclicktorunscenarioinstalltaskfonts"></a>Office.ClickToRun.Scenario.InstallTaskFonts

Date despre instalări și inventar Office colectate atunci când programul de instalare Office instalează fonturi. Utilizat pentru a măsura succesul/eșecul instalării Office.

Se colectează următoarele câmpuri:

  - **Data\_15\_SourceType -** unde se află sursa Office 15, adică CDN sau local 

  - **Data\_15\_UpdatesEnabled -** dacă sunt activate actualizările Office 15 

  - **Data\_15\_UpdateVersion -** la ce versiune Office 15 actualizăm 

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion-** ce versiune de Office 16 actualizați la 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** Produsele pe care le adăugăm 

  - **Data\_AddingProducts -** Ce produse ni s-a solicitat să adăugăm 

  - **Data\_CompletionState -** dacă am finalizat activitatea

  - **Data\_ErrorCode -** codul de eroare cu care am eșuat 

  - **Data\_ErrorDetails -** detalii suplimentare despre o eroare 

  - **Data\_ErrorMessage -** un mesaj de eroare despre ce nu a funcționat bine 

  - **Data\_ErrorSource -** unde s-a produs eroarea 

  - **Data\_ExceptionType -** excepția cu care am eșuat 

  - **Data\_IsErrorCodeIgnorable -** dacă codul de eroare cu care am eșuat poate fi ignorat 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth -** dacă considerăm că codul de eroare poate fi ignorat 

  - **Data\_NewestPackageVersion -** cea mai nouă versiune de Office de pe computer 

  - **Data\_OldestPackageVersion -** cea mai veche versiune de Office de pe computer 

  - **Data\_ProductsToAdd -** Ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName  -** ce scenariu rulează. adică, instalare

  - **Data\_ScenarioSubType -** Ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

  - **Data\_SourceType -** unde se află sursa noastră, adică CDN 

  - **Data\_SqmMachineID   -** ID unic de computer utilizat de Windows SQM 

  - **Data\_SusClientID-** identificator de actualizare Office computer 

  - **Data\_TaskState -** care este starea activității, cum ar fi rulare sau anulat 

  - **Data\_TotalClientCabSize -** dimensiunea fișierului cab al clientului nostru 

  - **Data\_TriggeringUI -** ce a declanșat interfața cu utilizatorul 

  - **Data\_UpdatesEnabled -** dacă sunt activate actualizările Office 

  - **Data\_Version -** versiunea de Office 

### <a name="officeclicktorunscenarioinstalltaskinitupdates"></a>Office.ClickToRun.Scenario.InstallTaskInitupdates

Date despre instalări și inventar Office colectate atunci când programul de instalare Office creează setări pentru ca actualizările să funcționeze corespunzător. Utilizat pentru a măsura succesul/eșecul instalării Office.

Se colectează următoarele câmpuri:

  - **Data\_15\_SourceType -** unde se află sursa Office 15, adică CDN sau local 

  - **Data\_15\_UpdatesEnabled -** dacă sunt activate actualizările Office 15 

  - **Data\_15\_UpdateVersion -** la ce versiune Office 15 actualizăm 

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion-** ce versiune de Office 16 actualizați la 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** Produsele pe care le adăugăm 

  - **Data\_AddingProducts -** Ce produse ni s-a solicitat să adăugăm 

  - **Data\_CompletionState -** dacă am finalizat activitatea

  - **Data\_ErrorCode -** codul de eroare cu care am eșuat 

  - **Data\_ErrorDetails -** detalii suplimentare despre o eroare 

  - **Data\_ErrorMessage -** un mesaj de eroare despre ce nu a funcționat bine 

  - **Data\_ErrorSource -** unde s-a produs eroarea 

  - **Data\_ExceptionType -** excepția cu care am eșuat 

  - **Data\_IsErrorCodeIgnorable -** dacă codul de eroare cu care am eșuat poate fi ignorat 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth -** dacă considerăm că codul de eroare poate fi ignorat 

  - **Data\_NewestPackageVersion -** cea mai nouă versiune de Office de pe computer 

  - **Data\_OldestPackageVersion -** cea mai veche versiune de Office de pe computer 

  - **Data\_ProductsToAdd -** Ce produse Office adăugăm 

  - <bpt id="p1">**</bpt>Data<ph id="ph1">\_</ph>ProductsToRemove-<ept id="p1">**</ept><ph id="ph2"> </ph>what Office products we're removing 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează. adică, instalare

  - **Data\_ScenarioSubType -** Ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

  - **Data\_SourceType -** unde se află sursa noastră, adică CDN 

  - **Data\_SqmMachineID -**  ID unic de computer utilizat de Windows SQM 

  - **Data\_SusClientID-** identificator de actualizare Office computer 

  - **Data\_TaskState -** care este starea activității, cum ar fi rulare sau anulat 

  - **Data\_TotalClientCabSize -** dimensiunea fișierului cab al clientului nostru 

  - **Data\_TriggeringUI -** ce a declanșat interfața cu utilizatorul 

  - **Data\_UpdatesEnabled -** dacă sunt activate actualizările Office 

  - **Data\_Version -** versiunea de Office 

### <a name="officeclicktorunscenarioinstalltaskintegrateinstall"></a>Office.ClickToRun.Scenario.InstallTaskIntegrateinstall

Date despre instalări și inventar Office colectate atunci când programul de instalare Office creează intrări de registry pentru aplicațiile Office Utilizate pentru a măsura succesul/eșecul instalării Office. 

Se colectează următoarele câmpuri:

  - **Data\_15\_SourceType -** unde se află sursa Office 15, adică CDN sau local 

  - **Data\_15\_UpdatesEnabled -** dacă sunt activate actualizările Office 15 

  - **Data\_15\_UpdateVersion -** La ce versiune Office 15 actualizăm

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion-** ce versiune de Office 16 actualizați la 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** Produsele pe care le adăugăm 

  - **Data\_AddingProducts -** Ce produse ni s-a solicitat să adăugăm 

  - **Data\_CompletionState -** dacă am finalizat activitatea

  - **Data\_ErrorCode -** codul de eroare cu care am eșuat 

  - **Data\_ErrorDetails -** detalii suplimentare despre o eroare 

  - **Data\_ErrorMessage -** un mesaj de eroare despre ce nu a funcționat bine 

  - **Data\_ErrorSource -** unde s-a produs eroarea 

  - **Data\_ExceptionType -** excepția cu care am eșuat 

  - **Data\_IsErrorCodeIgnorable -** dacă codul de eroare cu care am eșuat poate fi ignorat 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth -** dacă considerăm că codul de eroare poate fi ignorat 

  - **Data\_NewestPackageVersion -** cea mai nouă versiune de Office de pe computer 

  - **Data\_OldestPackageVersion -** cea mai veche versiune de Office de pe computer 

  - **Data\_ProductsToAdd -** Ce produse Office adăugăm 

  - <bpt id="p1">**</bpt>Data<ph id="ph1">\_</ph>ProductsToRemove-<ept id="p1">**</ept><ph id="ph2"> </ph>what Office products we're removing 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName  -** ce scenariu rulează. adică, instalare 

  - **Data\_ScenarioSubType -** Ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

  - **Data\_SourceType -** unde se află sursa noastră, adică CDN 

  - **Data\_SqmMachineID  -** ID unic de computer utilizat de Windows SQM

  - **Data\_SusClientID-** identificator de actualizare Office computer 

  - **Data\_TaskState -** care este starea activității, cum ar fi rulare sau anulat 

  - **Data\_TotalClientCabSize -** dimensiunea fișierului cab al clientului nostru 

  - **Data\_TriggeringUI -** ce a declanșat interfața cu utilizatorul 

  - **Data\_UpdatesEnabled -** dacă sunt activate actualizările Office 

  - **Data\_Version -** versiunea de Office 

### <a name="officeclicktorunscenarioinstalltasklastrun"></a>Office.ClickToRun.Scenario.InstallTaskLastrun

Date despre instalări și inventar Office colectate atunci când programul de instalare Office finalizează instalarea, fixând comenzile rapide și creând setări de registry finale. Utilizat pentru a măsura succesul/eșecul instalării Office.

Se colectează următoarele câmpuri:

  - **Data\_15\_SourceType -** unde se află sursa Office 15, adică CDN sau local 

  - **Data\_15\_UpdatesEnabled -** dacă sunt activate actualizările Office 15 

  - **Data\_15\_UpdateVersion -** La ce versiune Office 15 actualizăm

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion-** ce versiune de Office 16 actualizați la 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** Produsele pe care le adăugăm 

  - **Data\_AddingProducts -** Ce produse ni s-a solicitat să adăugăm 

  - **Data\_CompletionState -** dacă am finalizat activitatea

  - **Data\_ErrorCode -** codul de eroare cu care am eșuat 

  - **Data\_ErrorDetails -** detalii suplimentare despre o eroare 

  - **Data\_ErrorMessage -** un mesaj de eroare despre ce nu a funcționat bine 

  - **Data\_ErrorSource -** unde s-a produs eroarea 

  - **Data\_ExceptionType -** excepția cu care am eșuat 

  - **Data\_IsErrorCodeIgnorable -** dacă codul de eroare cu care am eșuat poate fi ignorat 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth -** dacă considerăm că codul de eroare poate fi ignorat 

  - **Data\_NewestPackageVersion -** cea mai nouă versiune de Office de pe computer 

  - **Data\_OldestPackageVersion -** cea mai veche versiune de Office de pe computer 

  - **Data\_ProductsToAdd -** Ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName  -** ce scenariu rulează. adică, instalare

  - **Data\_ScenarioSubType -** Ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

  - **Data\_SourceType -** unde se află sursa noastră, adică CDN 

  - **Data\_SqmMachineID -** ID unic de computer utilizat de Windows SQM

  - **Data\_SusClientID-** identificator de actualizare Office computer 

  - **Data\_TaskState -** care este starea activității, cum ar fi rulare sau anulat 

  - **Data\_TotalClientCabSize -** dimensiunea fișierului cab al clientului nostru 

  - **Data\_TriggeringUI -** ce a declanșat interfața cu utilizatorul 

  - **Data\_UpdatesEnabled -** dacă sunt activate actualizările Office 

  - **Data\_Version -** versiunea de Office 

### <a name="officeclicktorunscenarioinstalltaskmigrate"></a>Office.ClickToRun.Scenario.InstallTaskMigrate

Date despre instalări și inventar Office colectate atunci când programul de instalare migrează setările de la versiunile mai vechi de Office. Utilizat pentru a măsura succesul/eșecul instalării Office.

Se colectează următoarele câmpuri:

  - **Data\_15\_SourceType -** unde se află sursa Office 15, adică CDN sau local 

  - **Data\_15\_UpdatesEnabled -** dacă sunt activate actualizările Office 15 

  - **Data\_15\_UpdateVersion -** La ce versiune Office 15 actualizăm

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion-** ce versiune de Office 16 actualizați la 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** Produsele pe care le adăugăm 

  - **Data\_AddingProducts -** Ce produse ni s-a solicitat să adăugăm 

  - **Data\_CompletionState -** dacă am finalizat activitatea

  - **Data\_ErrorCode -** codul de eroare cu care am eșuat 

  - **Data\_ErrorDetails -** detalii suplimentare despre o eroare 

  - **Data\_ErrorMessage -** un mesaj de eroare despre ce nu a funcționat bine 

  - **Data\_ErrorSource -** unde s-a produs eroarea

  - **Data\_ExceptionType -** excepția cu care am eșuat 

  - **Data\_IsErrorCodeIgnorable -** dacă codul de eroare cu care am eșuat poate fi ignorat 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth -** dacă considerăm că codul de eroare poate fi ignorat 

  - **Data\_NewestPackageVersion -** cea mai nouă versiune de Office de pe computer 

  - **Data\_OldestPackageVersion -** cea mai veche versiune de Office de pe computer 

  - **Data\_ProductsToAdd -** Ce produse Office adăugăm 

  - <bpt id="p1">**</bpt>Data<ph id="ph1">\_</ph>ProductsToRemove-<ept id="p1">**</ept><ph id="ph2"> </ph>what Office products we're removing 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName  -** ce scenariu rulează. adică, instalare

  - **Data\_ScenarioSubType -** Ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

  - **Data\_SourceType -** unde se află sursa noastră, adică CDN 

  - **Data\_SqmMachineID  -** ID unic de computer utilizat de Windows SQM

  - **Data\_SusClientID-**  identificator de actualizare Office computer

  - **Data\_TaskState -** care este starea activității, cum ar fi rulare sau anulat 

  - **Data\_TotalClientCabSize -** dimensiunea fișierului cab al clientului nostru 

  - **Data\_TriggeringUI -** ce a declanșat interfața cu utilizatorul 

  - **Data\_UpdatesEnabled -** dacă sunt activate actualizările Office 

  - **Data\_Version -** versiunea de Office 

### <a name="officeclicktorunscenarioinstalltaskpublishrsod"></a>Office.ClickToRun.Scenario.InstallTaskPublishrsod

Date despre instalări și inventar Office colectate atunci când programul de instalare publică registry virtual pentru nivelul de virtualizare AppV. Utilizat pentru a măsura succesul/eșecul instalării Office.

Se colectează următoarele câmpuri:

  - **Data\_15\_SourceType -** unde se află sursa Office 15, adică CDN sau local 

  - **Data\_15\_UpdatesEnabled -** dacă sunt activate actualizările Office 15 

  - **Data\_15\_UpdateVersion -** La ce versiune Office 15 actualizăm

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion-** ce versiune de Office 16 actualizați la 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** Produsele pe care le adăugăm 

  - **Data\_AddingProducts -** Ce produse ni s-a solicitat să adăugăm 

  - **Data\_CompletionState -** dacă am finalizat activitatea

  - **Data\_ErrorCode -** codul de eroare cu care am eșuat 

  - **Data\_ErrorDetails -** detalii suplimentare despre o eroare 

  - **Data\_ErrorMessage -** un mesaj de eroare despre ce nu a funcționat bine 

  - **Data\_ErrorSource -** unde s-a produs eroarea

  - **Data\_ExceptionType -** excepția cu care am eșuat 

  - **Data\_IsErrorCodeIgnorable -** dacă codul de eroare cu care am eșuat poate fi ignorat 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth -** dacă considerăm că codul de eroare poate fi ignorat 

  - **Data\_NewestPackageVersion -** cea mai nouă versiune de Office de pe computer 

  - **Data\_OldestPackageVersion -** cea mai veche versiune de Office de pe computer 

  - **Data\_ProductsToAdd -** Ce produse Office adăugăm 

  - <bpt id="p1">**</bpt>Data<ph id="ph1">\_</ph>ProductsToRemove-<ept id="p1">**</ept><ph id="ph2"> </ph>what Office products we're removing 

  - <bpt id="p1">**</bpt>Data<ph id="ph1">\_</ph>RemovingFixedProducts-<ept id="p1">**</ept> The products we're removing 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează, adică instalare 

  - **Data\_ScenarioSubType -** Ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

  - **Data\_SourceType -** unde se află sursa noastră, adică CDN 

  - **Data\_SqmMachineID -** ID unic de computer utilizat de Windows SQM

  - **Data\_SusClientID-** identificator de actualizare Office computer 

  - **Data\_TaskState -** care este starea activității, cum ar fi rulare sau anulat 

  - **Data\_TotalClientCabSize -** dimensiunea fișierului cab al clientului nostru 

  - **Data\_TriggeringUI -** ce a declanșat interfața cu utilizatorul 

  - **Data\_UpdatesEnabled -** dacă sunt activate actualizările Office 

  - **Data\_Version -** versiunea de Office 

### <a name="officeclicktorunscenarioinstalltaskremoveinstallation"></a>Office.ClickToRun.Scenario.InstallTaskRemoveinstallation

Date despre instalări și inventar Office colectate atunci când programul de dezinstalare Office elimină părți de Office de pe dispozitiv. Utilizat pentru a măsura succesul/eșecul instalării Office.

Se colectează următoarele câmpuri:

  - **Data\_15\_SourceType -** unde se află sursa Office 15, adică CDN sau local 

  - **Data\_15\_UpdatesEnabled -** dacă sunt activate actualizările Office 15 

  - **Data\_15\_UpdateVersion -** la ce versiune Office 15 actualizăm 

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion-** ce versiune de Office 16 actualizați la 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** Produsele pe care le adăugăm 

  - **Data\_AddingProducts -** Ce produse ni s-a solicitat să adăugăm 

  - **Data\_CompletionState -** dacă am finalizat activitatea

  - **Data\_ErrorCode -** codul de eroare cu care am eșuat 

  - **Data\_ErrorDetails -** detalii suplimentare despre o eroare 

  - **Data\_ErrorMessage -** un mesaj de eroare despre ce nu a funcționat bine 

  - **Data\_ErrorSource -** unde s-a produs eroarea 

  - **Data\_ExceptionType -** excepția cu care am eșuat 

  - **Data\_IsErrorCodeIgnorable -** dacă codul de eroare cu care am eșuat poate fi ignorat 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth -** dacă considerăm că codul de eroare poate fi ignorat 

  - **Data\_NewestPackageVersion -** cea mai nouă versiune de Office de pe computer 

  - **Data\_OldestPackageVersion -** cea mai veche versiune de Office de pe computer 

  - **Data\_ProductsToAdd -** Ce produse Office adăugăm 

  - <bpt id="p1">**</bpt>Data<ph id="ph1">\_</ph>ProductsToRemove-<ept id="p1">**</ept><ph id="ph2"> </ph>what Office products we're removing 

  - **Data\_RemovingFixedProducts-** Produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează. adică, instalare 

  - **Data\_ScenarioSubType -** Ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

  - **Data\_SourceType -** unde se află sursa noastră, adică CDN 

  - **Data\_SqmMachineID  -** ID unic de computer utilizat de Windows SQM

  - **Data\_SusClientID-** identificator de actualizare Office computer 

  - **Data\_TaskState -** care este starea activității, cum ar fi rulare sau anulat 

  - **Data\_TotalClientCabSize -** dimensiunea fișierului cab al clientului nostru 

  - **Data\_TriggeringUI -** ce a declanșat interfața cu utilizatorul 

  - **Data\_UpdatesEnabled -** dacă sunt activate actualizările Office 

  - **Data\_Version -** versiunea de Office 

### <a name="officeclicktorunscenarioinstalltaskstream"></a>Office.ClickToRun.Scenario.InstallTaskStream

Date despre instalări și inventar Office colectate atunci când programul de instalare Office descarcă fișiere noi pentru Office. Utilizat pentru a măsura succesul/eșecul instalării Office.

Se colectează următoarele câmpuri:

  - **Data\_15\_SourceType -** unde se află sursa Office 15, adică CDN sau local 

  - **Data\_15\_UpdatesEnabled -** dacă sunt activate actualizările Office 15 

  - **Data\_15\_UpdateVersion -** La ce versiune Office 15 actualizăm 

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType  -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled -** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion  -** Ce versiune de Office 16 actualizăm 

  - **Data\_16\_Version  -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** Produsele pe care le adăugăm 

  - **Data\_AddingProducts -** Ce produse ni s-a solicitat să adăugăm 

  - **Data\_CompletionState -** dacă am finalizat activitatea

  - **Data\_ErrorCode -** codul de eroare cu care am eșuat 

  - **Data\_ErrorDetails -** detalii suplimentare despre o eroare 

  - **Data\_ErrorMessage -** un mesaj de eroare despre ce nu a funcționat bine 

  - **Data\_ErrorSource -** unde s-a produs eroarea 

  - **Data\_ExceptionType -** excepția cu care am eșuat 

  - **Data\_IsErrorCodeIgnorable -** dacă codul de eroare cu care am eșuat poate fi ignorat 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth -** dacă considerăm că codul de eroare poate fi ignorat 

  - **Data\_NewestPackageVersion -** cea mai nouă versiune de Office de pe computer 

  - **Data\_OldestPackageVersion -** cea mai veche versiune de Office de pe computer 

  - **Data\_ProductsToAdd -** Ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - <bpt id="p1">**</bpt>Data<ph id="ph1">\_</ph>RemovingFixedProducts-<ept id="p1">**</ept> The products we're removing 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează. adică, instalare 

  - **Data\_ScenarioSubType -** Ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

  - **Data\_SourceType -** unde se află sursa noastră, adică CDN 

  - **Data\_SqmMachineID -**  ID unic de computer utilizat de Windows SQM 

  - **Data\_SusClientID -** identificator de actualizare Office computer 

  - **Data\_TaskState -** care este starea activității, cum ar fi rulare sau anulat 

  - **Data\_TotalClientCabSize -** dimensiunea fișierului cab al clientului nostru 

  - **Data\_TriggeringUI -** ce a declanșat interfața cu utilizatorul 

  - **Data\_UpdatesEnabled -** dacă sunt activate actualizările Office 

  - **Data\_Version -** versiunea de Office 

### <a name="officeclicktorunscenarioinstalltaskuninstallcentennial"></a>Office.ClickToRun.Scenario.InstallTaskUninstallcentennial

Date despre instalări și inventar Office colectate atunci când programul de instalare Office dezinstalează o versiune anterioară de Office din Store. Utilizat pentru a măsura succesul/eșecul instalării Office.

Se colectează următoarele câmpuri:

  - **Data\_15\_SourceType -** unde se află sursa Office 15, adică CDN sau local 

  - **Data\_15\_UpdatesEnabled -** dacă sunt activate actualizările Office 15 

  - **Data\_15\_UpdateVersion -** la ce versiune Office 15 actualizăm 

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion-** ce versiune de Office 16 actualizați la 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** Produsele pe care le adăugăm 

  - **Data\_AddingProducts -** Ce produse ni s-a solicitat să adăugăm 

  - **Data\_CompletionState -** dacă am finalizat activitatea

  - **Data\_ErrorCode -** codul de eroare cu care am eșuat 

  - **Data\_ErrorDetails -** detalii suplimentare despre o eroare 

  - **Data\_ErrorMessage -** un mesaj de eroare despre ce nu a funcționat bine 

  - **Data\_ErrorSource -** unde s-a produs eroarea 

  - **Data\_ExceptionType -** excepția cu care am eșuat 

  - **Data\_IsErrorCodeIgnorable -** dacă codul de eroare cu care am eșuat poate fi ignorat 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth -** dacă considerăm că codul de eroare poate fi ignorat 

  - **Data\_NewestPackageVersion -** cea mai nouă versiune de Office de pe computer 

  - **Data\_OldestPackageVersion -** cea mai veche versiune de Office de pe computer 

  - **Data\_ProductsToAdd -** Ce produse Office adăugăm 

  - <bpt id="p1">**</bpt>Data<ph id="ph1">\_</ph>ProductsToRemove-<ept id="p1">**</ept><ph id="ph2"> </ph>what Office products we're removing 

  - <bpt id="p1">**</bpt>Data<ph id="ph1">\_</ph>RemovingFixedProducts-<ept id="p1">**</ept> The products we're removing 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează. adică, instalare 

  - **Data\_ScenarioSubType -** Ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

  - **Data\_SourceType -** unde se află sursa noastră, adică CDN 

  - **Data\_SqmMachineID -**  ID unic de computer utilizat de Windows SQM

  - **Data\_SusClientID-** identificator de actualizare Office computer 

  - **Data\_TaskState -** care este starea activității, cum ar fi rulare sau anulat 

  - **Data\_TotalClientCabSize -** dimensiunea fișierului cab al clientului nostru 

  - **Data\_TriggeringUI -** ce a declanșat interfața cu utilizatorul 

  - **Data\_UpdatesEnabled -** dacă sunt activate actualizările Office 

  - **Data\_Version -** versiunea de Office 

### <a name="officeclicktorunscenariorepairtaskfinalintegrate"></a>Office.ClickToRun.Scenario.RepairTaskFinalintegrate

Date despre instalări și inventar Office colectate atunci când clientul de reparare Office publică din nou fișiere .msi și extensii Office. Utilizat pentru a măsura succesul/eșecul reparării Office.

Se colectează următoarele câmpuri:

  - **Data\_15\_SourceType -** unde se află sursa Office 15, adică CDN sau local 

  - **Data\_15\_UpdatesEnabled -** dacă sunt activate actualizările Office 15 

  - **Data\_15\_UpdateVersion -** la ce versiune Office 15 actualizăm 

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion-** ce versiune de Office 16 actualizați la 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** Produsele pe care le adăugăm 

  - **Data\_AddingProducts -** Ce produse ni s-a solicitat să adăugăm 

  - **Data\_CompletionState -** dacă am finalizat activitatea

  - **Data\_ErrorCode -** codul de eroare cu care am eșuat 

  - **Data\_ErrorDetails -** detalii suplimentare despre o eroare 

  - **Data\_ErrorMessage -** un mesaj de eroare despre ce nu a funcționat bine 

  - **Data\_ErrorSource -** unde s-a produs eroarea 

  - **Data\_ExceptionType -** excepția cu care am eșuat 

  - **Data\_IsErrorCodeIgnorable -** dacă codul de eroare cu care am eșuat poate fi ignorat 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth -** dacă considerăm că codul de eroare poate fi ignorat 

  - **Data\_NewestPackageVersion -** cea mai nouă versiune de Office de pe computer 

  - **Data\_OldestPackageVersion -** cea mai veche versiune de Office de pe computer 

  - **Data\_ProductsToAdd -** Ce produse Office adăugăm 

  - <bpt id="p1">**</bpt>Data<ph id="ph1">\_</ph>ProductsToRemove-<ept id="p1">**</ept><ph id="ph2"> </ph>what Office products we're removing 

  - <bpt id="p1">**</bpt>Data<ph id="ph1">\_</ph>RemovingFixedProducts-<ept id="p1">**</ept> The products we're removing 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează. adică, instalare 

  - **Data\_ScenarioSubType -** Ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

  - **Data\_SourceType -** unde se află sursa noastră, adică CDN 

  - **Data\_SqmMachineID -**  ID unic de computer utilizat de Windows SQM 

  - **Data\_SusClientID-** identificator de actualizare Office computer 

  - **Data\_TaskState -** care este starea activității, cum ar fi rulare sau anulat 

  - **Data\_TotalClientCabSize -** dimensiunea fișierului cab al clientului nostru 

  - **Data\_TriggeringUI -** ce a declanșat interfața cu utilizatorul 

  - **Data\_UpdatesEnabled -** dacă sunt activate actualizările Office 

  - **Data\_Version -** versiunea de Office 

### <a name="officeclicktorunscenariorepairtaskfullrepair"></a>Office.ClickToRun.Scenario.RepairTaskFullrepair

Date despre instalări și inventar Office colectate atunci când clientul de reparare Office descarcă cea mai recentă versiune a clientului Clic și Pornire pentru a pregăti computerul pentru dezinstalare și reinstalare. Utilizat pentru a măsura succesul/eșecul reparării Office.

Se colectează următoarele câmpuri:

  - **Data\_15\_SourceType -** unde se află sursa Office 15, adică CDN sau local 

  - **Data\_15\_UpdatesEnabled -** dacă sunt activate actualizările Office 15 

  - **Data\_15\_UpdateVersion -** la ce versiune Office 15 actualizăm 

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion-** ce versiune de Office 16 actualizați la 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** Produsele pe care le adăugăm 

  - **Data\_AddingProducts -** Ce produse ni s-a solicitat să adăugăm 

  - **Data\_CompletionState -** dacă am finalizat activitatea

  - **Data\_ErrorCode -** codul de eroare cu care am eșuat 

  - **Data\_ErrorDetails -** detalii suplimentare despre o eroare 

  - **Data\_ErrorMessage -** un mesaj de eroare despre ce nu a funcționat bine 

  - **Data\_ErrorSource -** unde s-a produs eroarea 

  - **Data\_ExceptionType -** excepția cu care am eșuat 

  - **Data\_IsErrorCodeIgnorable -** dacă codul de eroare cu care am eșuat poate fi ignorat 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth -** dacă considerăm că codul de eroare poate fi ignorat 

  - **Data\_NewestPackageVersion -** cea mai nouă versiune de Office de pe computer 

  - **Data\_OldestPackageVersion -** cea mai veche versiune de Office de pe computer 

  - **Data\_ProductsToAdd -** Ce produse Office adăugăm 

  - <bpt id="p1">**</bpt>Data<ph id="ph1">\_</ph>ProductsToRemove-<ept id="p1">**</ept><ph id="ph2"> </ph>what Office products we're removing 

  - <bpt id="p1">**</bpt>Data<ph id="ph1">\_</ph>RemovingFixedProducts-<ept id="p1">**</ept> The products we're removing 

  - <bpt id="p1">**</bpt>Data<ph id="ph1">\_</ph>RemovingProducts -<ept id="p1">**</ept> The products we're asked to remove 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează. adică, instalare 

  - **Data\_ScenarioSubType -** Ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

  - **Data\_SourceType -** unde se află sursa noastră, adică CDN 

  - **Data\_SqmMachineID -**  ID unic de computer utilizat de Windows SQM 

  - **Data\_SusClientID-** identificator de actualizare Office computer 

  - **Data\_TaskState -** care este starea activității, cum ar fi rulare sau anulat 

  - **Data\_TotalClientCabSize -** dimensiunea fișierului cab al clientului nostru 

  - **Data\_TriggeringUI -** ce a declanșat interfața cu utilizatorul 

  - **Data\_UpdatesEnabled -** dacă sunt activate actualizările Office 

  - **Data\_Version -** versiunea de Office 

### <a name="officeclicktorunscenariorepairtaskintegraterepair"></a>Office.ClickToRun.Scenario.RepairTaskIntegraterepair

Date despre instalări și inventar Office colectate atunci când clientul de reparare Office încearcă să repare unele intrări problematice de registry cunoscute. Utilizat pentru a măsura succesul/eșecul reparării Office.

Se colectează următoarele câmpuri:

  - **Data\_15\_SourceType -** unde se află sursa Office 15, adică CDN sau local 

  - **Data\_15\_UpdatesEnabled -** dacă sunt activate actualizările Office 15 

  - **Data\_15\_UpdateVersion -** la ce versiune Office 15 actualizăm 

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion-** ce versiune de Office 16 actualizați la 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** Produsele pe care le adăugăm 

  - **Data\_AddingProducts -** Ce produse ni s-a solicitat să adăugăm 

  - **Data\_CompletionState -** dacă am finalizat activitatea

  - **Data\_ErrorCode -** codul de eroare cu care am eșuat 

  - **Data\_ErrorDetails -** detalii suplimentare despre o eroare 

  - **Data\_ErrorMessage -** un mesaj de eroare despre ce nu a funcționat bine 

  - **Data\_ErrorSource -** unde s-a produs eroarea 

  - **Data\_ExceptionType -** excepția cu care am eșuat 

  - **Data\_IsErrorCodeIgnorable -** dacă codul de eroare cu care am eșuat poate fi ignorat 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth -** dacă considerăm că codul de eroare poate fi ignorat 

  - **Data\_NewestPackageVersion -** cea mai nouă versiune de Office de pe computer 

  - **Data\_OldestPackageVersion -** cea mai veche versiune de Office de pe computer 

  - **Data\_ProductsToAdd -** Ce produse Office adăugăm 

  - <bpt id="p1">**</bpt>Data<ph id="ph1">\_</ph>ProductsToRemove-<ept id="p1">**</ept><ph id="ph2"> </ph>what Office products we're removing 

  - <bpt id="p1">**</bpt>Data<ph id="ph1">\_</ph>RemovingFixedProducts-<ept id="p1">**</ept> The products we're removing 

  - <bpt id="p1">**</bpt>Data<ph id="ph1">\_</ph>RemovingProducts -<ept id="p1">**</ept> The products we're asked to remove 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează. adică, instalare 

  - **Data\_ScenarioSubType -** Ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

  - **Data\_SourceType -** unde se află sursa noastră, adică CDN 

  - **Data\_SqmMachineID -**  ID unic de computer utilizat de Windows SQM 

  - **Data\_SusClientID-** identificator de actualizare Office computer 

  - **Data\_TaskState -** care este starea activității, cum ar fi rulare sau anulat 

  - **Data\_TotalClientCabSize -** dimensiunea fișierului cab al clientului nostru 

  - **Data\_TriggeringUI -** ce a declanșat interfața cu utilizatorul 

  - **Data\_UpdatesEnabled -** dacă sunt activate actualizările Office 

  - **Data\_Version -** versiunea de Office 

### <a name="officeclicktorunscenariorepairtaskremoveinstallation"></a>Office.ClickToRun.Scenario.RepairTaskRemoveinstallation

Date despre instalări și inventar Office colectate atunci când clientul de reparare Office elimină Office de pe dispozitiv pentru a pregăti o reinstalare la reparare. Utilizat pentru a măsura succesul/eșecul reparării Office.

Se colectează următoarele câmpuri:

  - **Data\_15\_SourceType -** unde se află sursa Office 15, adică CDN sau local 

  - **Data\_15\_UpdatesEnabled -** dacă sunt activate actualizările Office 15 

  - **Data\_15\_UpdateVersion -** La ce versiune Office 15 actualizăm 

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion-** ce versiune de Office 16 actualizați la 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** Produsele pe care le adăugăm 

  - **Data\_AddingProducts -** Ce produse ni s-a solicitat să adăugăm 

  - **Data\_CompletionState -** dacă am finalizat activitatea

  - **Data\_ErrorCode -** codul de eroare cu care am eșuat 

  - **Data\_ErrorDetails -** detalii suplimentare despre o eroare 

  - **Data\_ErrorMessage -** un mesaj de eroare despre ce nu a funcționat bine 

  - **Data\_ErrorSource -** unde s-a produs eroarea 

  - **Data\_ExceptionType -** excepția cu care am eșuat 

  - **Data\_IsErrorCodeIgnorable -** dacă codul de eroare cu care am eșuat poate fi ignorat 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth -** dacă considerăm că codul de eroare poate fi ignorat 

  - **Data\_NewestPackageVersion -** cea mai nouă versiune de Office de pe computer 

  - **Data\_OldestPackageVersion -** cea mai veche versiune de Office de pe computer 

  - **Data\_ProductsToAdd -** Ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - <bpt id="p1">**</bpt>Data<ph id="ph1">\_</ph>RemovingFixedProducts-<ept id="p1">**</ept> The products we're removing 

  - <bpt id="p1">**</bpt>Data<ph id="ph1">\_</ph>RemovingProducts -<ept id="p1">**</ept> The products we're asked to remove 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează. adică, instalare 

  - **Data\_ScenarioSubType -** Ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

  - **Data\_SourceType -** unde se află sursa noastră, adică CDN 

  - **Data\_SqmMachineID -**  ID unic de computer utilizat de Windows SQM 

  - **Data\_SusClientID-** identificator de actualizare Office computer 

  - **Data\_TaskState -** care este starea activității, cum ar fi rulare sau anulat 

  - **Data\_TotalClientCabSize -** dimensiunea fișierului cab al clientului nostru 

  - **Data\_TriggeringUI -** ce a declanșat interfața cu utilizatorul 

  - **Data\_UpdatesEnabled -** dacă sunt activate actualizările Office 

  - **Data\_Version -** versiunea de Office 

### <a name="officeclicktorunscenarioupdatetaskintegrateupdate"></a>Office.ClickToRun.Scenario.UpdateTaskIntegrateupdate 

Date despre instalări și inventar Office colectate atunci când clientul Clic și Pornire actualizează licențe, dacă este necesar. Utilizat pentru a măsura succesul/eșecul actualizării Office.

Se colectează următoarele câmpuri:

  - **Data\_15\_SourceType -** unde se află sursa Office 15, adică CDN sau local 

  - **Data\_15\_UpdatesEnabled -** dacă sunt activate actualizările Office 15 

  - **Data\_15\_UpdateVersion -** la ce versiune Office 15 actualizăm 

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion-** ce versiune de Office 16 actualizați la 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** Produsele pe care le adăugăm 

  - **Data\_AddingProducts -** Ce produse ni s-a solicitat să adăugăm 

  - **Data\_CompletionState -** dacă am finalizat activitatea

  - **Data\_ErrorCode -** codul de eroare cu care am eșuat 

  - **Data\_ErrorDetails -** detalii suplimentare despre o eroare 

  - **Data\_ErrorMessage -** un mesaj de eroare despre ce nu a funcționat bine 

  - **Data\_ErrorSource -** unde s-a produs eroarea 

  - **Data\_ExceptionType -** excepția cu care am eșuat 

  - **Data\_IsErrorCodeIgnorable -** dacă codul de eroare cu care am eșuat poate fi ignorat 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth -** dacă considerăm că codul de eroare poate fi ignorat 

  - **Data\_NewestPackageVersion -** cea mai nouă versiune de Office de pe computer 

  - **Data\_OldestPackageVersion -** cea mai veche versiune de Office de pe computer 

  - **Data\_ProductsToAdd -** Ce produse Office adăugăm 

  - <bpt id="p1">**</bpt>Data<ph id="ph1">\_</ph>ProductsToRemove-<ept id="p1">**</ept><ph id="ph2"> </ph>what Office products we're removing 

  - <bpt id="p1">**</bpt>Data<ph id="ph1">\_</ph>RemovingFixedProducts-<ept id="p1">**</ept> The products we're removing 

  - <bpt id="p1">**</bpt>Data<ph id="ph1">\_</ph>RemovingProducts -<ept id="p1">**</ept> The products we're asked to remove 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează. adică, instalare 

  - **Data\_ScenarioSubType -** Ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

  - **Data\_SourceType -** unde se află sursa noastră, adică CDN 

  - **Data\_SqmMachineID -**  ID unic de computer utilizat de Windows SQM 

  - **Data\_SusClientID-** identificator de actualizare Office computer 

  - **Data\_TaskState -** care este starea activității, cum ar fi rulare sau anulat 

  - **Data\_TotalClientCabSize -** dimensiunea fișierului cab al clientului nostru 

  - **Data\_TriggeringUI -** ce a declanșat interfața cu utilizatorul 

  - **Data\_UpdatesEnabled -** dacă sunt activate actualizările Office 

  - **Data\_Version -** versiunea de Office 

### <a name="officeclicktorunscenarioupdatetaskpublishrsod"></a>Office.ClickToRun.Scenario.UpdateTaskPublishrsod

Date despre instalări și inventar Office colectate atunci când clientul Clic și Pornire actualizează setări de registry pentru fișiere binare noi. Utilizat pentru a măsura succesul/eșecul actualizării Office.

Se colectează următoarele câmpuri:

  - **Data\_15\_SourceType -** unde se află sursa Office 15, adică CDN sau local 

  - **Data\_15\_UpdatesEnabled -** dacă sunt activate actualizările Office 15 

  - **Data\_15\_UpdateVersion -** la ce versiune Office 15 actualizăm 

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion-** ce versiune de Office 16 actualizați la 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** Produsele pe care le adăugăm 

  - **Data\_AddingProducts -** Ce produse ni s-a solicitat să adăugăm 

  - **Data\_CompletionState -** dacă am finalizat activitatea

  - **Data\_ErrorCode -** codul de eroare cu care am eșuat 

  - **Data\_ErrorDetails -** detalii suplimentare despre o eroare 

  - **Data\_ErrorMessage -** un mesaj de eroare despre ce nu a funcționat bine 

  - **Data\_ErrorSource -** unde s-a produs eroarea 

  - **Data\_ExceptionType -** excepția cu care am eșuat 

  - **Data\_IsErrorCodeIgnorable -** dacă codul de eroare cu care am eșuat poate fi ignorat 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth -** dacă considerăm că codul de eroare poate fi ignorat 

  - **Data\_NewestPackageVersion -** cea mai nouă versiune de Office de pe computer 

  - **Data\_OldestPackageVersion -** cea mai veche versiune de Office de pe computer 

  - **Data\_ProductsToAdd -** Ce produse Office adăugăm 

  - <bpt id="p1">**</bpt>Data<ph id="ph1">\_</ph>ProductsToRemove-<ept id="p1">**</ept><ph id="ph2"> </ph>what Office products we're removing 

  - <bpt id="p1">**</bpt>Data<ph id="ph1">\_</ph>RemovingFixedProducts-<ept id="p1">**</ept> The products we're removing 

  - <bpt id="p1">**</bpt>Data<ph id="ph1">\_</ph>RemovingProducts -<ept id="p1">**</ept> The products we're asked to remove 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează. adică, instalare 

  - **Data\_ScenarioSubType -** Ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

  - **Data\_SourceType -** unde se află sursa noastră, adică CDN 

  - **Data\_SqmMachineID -**  ID unic de computer utilizat de Windows SQM 

  - **Data\_SusClientID-** identificator de actualizare Office computer 

  - **Data\_TaskState -** care este starea activității, cum ar fi rulare sau anulat 

  - **Data\_TotalClientCabSize -** dimensiunea fișierului cab al clientului nostru 

  - **Data\_TriggeringUI -** ce a declanșat interfața cu utilizatorul 

  - **Data\_UpdatesEnabled -** dacă sunt activate actualizările Office 

  - **Data\_Version -** versiunea de Office 

### <a name="officeclicktorunscenarioupdatetaskupdateapply"></a>Office.ClickToRun.Scenario.UpdateTaskUpdateapply

Date despre instalări și inventar Office colectate atunci când clientul Clic și Pornire închide aplicațiile care rulează, dacă este necesar, și instalează fișiere noi care au fost descărcate. Utilizat pentru a măsura succesul/eșecul actualizării Office.

Se colectează următoarele câmpuri:

  - **Data\_15\_SourceType -** unde se află sursa Office 15, adică CDN sau local 

  - **Data\_15\_UpdatesEnabled -** dacă sunt activate actualizările Office 15 

  - **Data\_15\_UpdateVersion -** la ce versiune Office 15 actualizăm 

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion-** ce versiune de Office 16 actualizați la 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** Produsele pe care le adăugăm 

  - **Data\_AddingProducts -** Ce produse ni s-a solicitat să adăugăm 

  - **Data\_AvailableVersion to-** ce versiune de Office este disponibilă pentru actualizare

  - **Data\_CompletedWithoutActionInfo-** De ce nu am finalizat scenariul, adică aplicațiile erau deschise

  - **Data\_CompletionState -** dacă am finalizat activitatea

  - **Data\_CorruptionChecksOnly -** În cazul în care doar căutăm deteriorări și nu actualizăm

  - **Data\_ErrorCode -** codul de eroare cu care am eșuat 

  - **Data\_ErrorDetails -** detalii suplimentare despre o eroare 

  - **Data\_ErrorMessage -** un mesaj de eroare despre ce nu a funcționat bine 

  - **Data\_ErrorSource -** unde s-a produs eroarea

  - **Data\_ExceptionType -** excepția cu care am eșuat 

  - **Data\_HardlinkingException -** excepția pe care am întâmpinat-o atunci când am încercat să creăm hardlinkuri

  - **Data\_IsErrorCodeIgnorable -** dacă codul de eroare cu care am eșuat poate fi ignorat 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth -** dacă considerăm că codul de eroare poate fi ignorat 

  - **Data\_NewestPackageVersion -** cea mai nouă versiune de Office de pe computer 

  - **Data\_OldestPackageVersion -** cea mai veche versiune de Office de pe computer 

  - **Data\_PackageOperationSuccessful -** adevărat dacă am finalizat cu succes activitatea noastră în pachetul Office

  - **Data\_ProductsToAdd -** Ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează. adică, instalare 

  - **Data\_ScenarioSubType -** Ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

  - **Data\_SourceType -** unde se află sursa noastră, adică CDN 

  - **Data\_SqmMachineID  -**  ID unic de computer utilizat de Windows SQM

  - **Data\_SusClientID-**  identificator de actualizare Office computer 

  - **Data\_TaskState -** care este starea activității, cum ar fi rulare sau anulat 

  - **Data\_TotalClientCabSize -** dimensiunea fișierului cab al clientului nostru 

  - **Data\_TriggeringUI -** ce a declanșat interfața cu utilizatorul 

  - **Data\_UpdatesEnabled -** dacă sunt activate actualizările Office 

  - **Data\_Version -** versiunea de Office 

  - **Data\_WorkstationLockState -** adevărat dacă credem că computerul este blocat

### <a name="officeclicktorunscenarioupdatetaskupdateclientdownload"></a>Office.ClickToRun.Scenario.UpdateTaskUpdateclientdownload

Date despre instalări și inventar Office colectate atunci când clientul Clic și Pornire descarcă o versiune mai nouă proprie. Utilizat pentru a măsura succesul/eșecul actualizării Office.

Se colectează următoarele câmpuri:

  - **Data\_15\_SourceType -** unde se află sursa Office 15, adică CDN sau local 

  - **Data\_15\_UpdatesEnabled -** dacă sunt activate actualizările Office 15 

  - **Data\_15\_UpdateVersion -** la ce versiune Office 15 actualizăm 

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion-** ce versiune de Office 16 actualizați la 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** Produsele pe care le adăugăm 

  - **Data\_AddingProducts -** Ce produse ni s-a solicitat să adăugăm 

  - **Data\_CompletionState -** dacă am finalizat activitatea

  - **Data\_ErrorCode -** codul de eroare cu care am eșuat 

  - **Data\_ErrorDetails -** detalii suplimentare despre o eroare 

  - **Data\_ErrorMessage -** un mesaj de eroare despre ce nu a funcționat bine 

  - **Data\_ErrorSource -** unde s-a produs eroarea 

  - **Data\_ExceptionType -** excepția cu care am eșuat 

  - **Data\_IsErrorCodeIgnorable -** dacă codul de eroare cu care am eșuat poate fi ignorat 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth -** dacă considerăm că codul de eroare poate fi ignorat 

  - **Data\_NewestPackageVersion -** cea mai nouă versiune de Office de pe computer 

  - **Data\_OldestPackageVersion -** cea mai veche versiune de Office de pe computer 

  - **Data\_ProductsToAdd -** Ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName-** ce scenariu rulează. adică, instalare 

  - **Data\_ScenarioSubType -** Ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

  - **Data\_SourceType -** unde se află sursa noastră, adică CDN 

  - **Data\_SqmMachineID  -** ID unic de computer utilizat de Windows SQM

  - **Data\_SusClientID-** identificator de actualizare Office computer 

  - **Data\_TaskState -** care este starea activității, cum ar fi rulare sau anulat 

  - **Data\_TotalClientCabSize -** dimensiunea fișierului cab al clientului nostru 

  - **Data\_TriggeringUI -** ce a declanșat interfața cu utilizatorul 

  - **Data\_UpdatesEnabled -** dacă sunt activate actualizările Office 

  - **Data\_Version -** versiunea de Office 

### <a name="officeclicktorunscenarioupdatetaskupdatedetection"></a>Office.ClickToRun.Scenario.UpdateTaskUpdatedetection

Date despre instalări și inventar Office colectate atunci când clientul Clic și Pornire verifică dacă este disponibilă o nouă actualizare. Utilizat pentru a măsura succesul/eșecul actualizării Office.

Se colectează următoarele câmpuri:

  - **Data\_15\_SourceType -** unde se află sursa Office 15, adică CDN sau local 

  - **Data\_15\_UpdatesEnabled -** dacă sunt activate actualizările Office 15 

  - **Data\_15\_UpdateVersion -** la ce versiune Office 15 actualizăm 

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion-** ce versiune de Office 16 actualizați la 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** Produsele pe care le adăugăm 

  - **Data\_AddingProducts -** Ce produse ni s-a solicitat să adăugăm 

  - **Data\_AvailableVersion -** ce versiune de Office este disponibilă pentru actualizare

  - **Data\_ComAction -** O int care reprezintă o acțiune com pe care o efectuăm

  - **Data\_CompletedWithoutActionInfo-** De ce nu am finalizat scenariul, adică aplicațiile erau deschise

  - **Data\_CompletionState -** dacă am finalizat activitatea

  - **Data\_ErrorCode -** codul de eroare cu care am eșuat 

  - **Data\_ErrorDetails -** detalii suplimentare despre o eroare 

  - **Data\_ErrorMessage -** un mesaj de eroare despre ce nu a funcționat bine 

  - **Data\_ErrorSource  -** unde s-a produs eroarea

  - **Data\_ExceptionType -** excepția cu care am eșuat 

  - **Data\_IsErrorCodeIgnorable -** dacă codul de eroare cu care am eșuat poate fi ignorat 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth -** dacă considerăm că codul de eroare poate fi ignorat 

  - **Data\_NewestPackageVersion -** cea mai nouă versiune de Office de pe computer 

  - **Data\_OldestPackageVersion -** cea mai veche versiune de Office de pe computer 

  - **Data\_PackageUpdateAvailable -** adevărat dacă avem o nouă versiune de Office disponibilă

  - **Data\_ProductsToAdd -** Ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează. adică, instalare

  - **Data\_ScenarioSubType -** Ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

  - **Data\_SourceType -** unde se află sursa noastră, adică CDN 

  - **Data\_SqmMachineID -**  ID unic de computer utilizat de Windows SQM 

  - **Data\_SusClientID-**  identificator de actualizare Office computer 

  - **Data\_TaskState -** care este starea activității, cum ar fi rulare sau anulat 

  - **Data\_TotalClientCabSize -** dimensiunea fișierului cab al clientului nostru 

  - **Data\_TriggeringUI -** ce a declanșat interfața cu utilizatorul 

  - **Data\_UpdatesEnabled -** dacă sunt activate actualizările Office 

  - **Data\_Version -** versiunea de Office 

### <a name="officeclicktorunscenarioupdatetaskupdatedownload"></a>Office.ClickToRun.Scenario.UpdateTaskUpdatedownload

Date despre instalări și inventar Office colectate atunci când clientul Clic și Pornire descarcă o actualizare nouă. Utilizat pentru a măsura succesul/eșecul actualizării Office.

Se colectează următoarele câmpuri:

  - **Data\_15\_SourceType -** unde se află sursa Office 15, adică CDN sau local 

  - **Data\_15\_UpdatesEnabled -** dacă sunt activate actualizările Office 15 

  - **Data\_15\_UpdateVersion -** La ce versiune Office 15 actualizăm 

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion-** ce versiune de Office 16 actualizați la 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** Produsele pe care le adăugăm 

  - **Data\_AddingProducts -** Ce produse ni s-a solicitat să adăugăm 

  - **Data\_AvailableVersion -** ce versiune de Office este disponibilă pentru actualizare

  - **Data\_CompletedWithoutActionInfo-** De ce nu am finalizat scenariul, adică aplicațiile erau deschise

  - **Data\_CompletionState -** dacă am finalizat activitatea

  - **Data\_CorruptionChecksOnly -** În cazul în care doar căutăm deteriorări și nu actualizăm

  - **Data\_ErrorCode -** codul de eroare cu care am eșuat 

  - **Data\_ErrorDetails -** detalii suplimentare despre o eroare 

  - **Data\_ErrorMessage -** un mesaj de eroare despre ce nu a funcționat bine 

  - **Data\_ErrorSource -** unde s-a produs eroarea

  - **Data\_ExceptionType -** excepția cu care am eșuat 

  - **Data\_FoundCorruptFiles -** adevărat dacă am găsit fișiere deteriorate

  - **Data\_IsErrorCodeIgnorable -** dacă codul de eroare cu care am eșuat poate fi ignorat 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth -** dacă considerăm că codul de eroare poate fi ignorat 

  - **Data\_NewestPackageVersion -** cea mai nouă versiune de Office de pe computer 

  - **Data\_OldestPackageVersion -** cea mai veche versiune de Office de pe computer 

  - **Data\_PackageOperationSuccessful -** adevărat dacă am finalizat cu succes activitatea noastră în pachetul Office

  - **Data\_PipelineExitCode -** codul de ieșire returnat de canalul de fișier 

  - **Data\_ProductsToAdd -** Ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează. adică, instalare 

  - **Data\_ScenarioSubType -** Ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

  - **Data\_SourceType -** unde se află sursa noastră, adică CDN 

  - **Data\_SqmMachineID -** ID unic de computer utilizat de Windows SQM 

  - **Data\_SusClientID-** identificator de actualizare Office computer 

  - **Data\_TaskState -** care este starea activității, cum ar fi rulare sau anulat 

  - **Data\_TotalClientCabSize -** dimensiunea fișierului cab al clientului nostru 

  - **Data\_TriggeringUI -** ce a declanșat interfața cu utilizatorul 

  - **Data\_UpdatesEnabled -** dacă sunt activate actualizările Office 

  - **Data\_Version -** versiunea de Office 

### <a name="officeclicktorunscenarioupdatetaskupdatefinalize"></a>Office.ClickToRun.Scenario.UpdateTaskUpdatefinalize

Date despre instalări și inventar Office colectate atunci când clientul Clic și Pornire este în curs de curățare de la actualizare și restaurează aplicații care au fost deschise anterior. Utilizat pentru a măsura succesul sau eșecul actualizării Office.

Se colectează următoarele câmpuri:

  - **Data\_15\_SourceType -** unde se află sursa Office 15, adică CDN sau local 

  - **Data\_15\_UpdatesEnabled -** dacă sunt activate actualizările Office 15 

  - **Data\_15\_UpdateVersion -** la ce versiune Office 15 actualizăm 

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion-** ce versiune de Office 16 actualizați la 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** Produsele pe care le adăugăm 

  - **Data\_AddingProducts -** Ce produse ni s-a solicitat să adăugăm 

  - **Data\_CompletionState -** dacă am finalizat activitatea

  - **Data\_ErrorCode -** codul de eroare cu care am eșuat 

  - **Data\_ErrorDetails -** detalii suplimentare despre o eroare 

  - **Data\_ErrorMessage -** un mesaj de eroare despre ce nu a funcționat bine 

  - **Data\_ErrorSource -** unde s-a produs eroarea 

  - **Data\_ExceptionType -** excepția cu care am eșuat 

  - **Data\_IsErrorCodeIgnorable -** dacă codul de eroare cu care am eșuat poate fi ignorat 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth -** dacă considerăm că codul de eroare poate fi ignorat 

  - **Data\_NewestPackageVersion -** cea mai nouă versiune de Office de pe computer 

  - **Data\_OldestPackageVersion -** cea mai veche versiune de Office de pe computer 

  - **Data\_ProductsToAdd -** Ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează. adică, instalare 

  - **Data\_ScenarioSubType -** Ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

  - **Data\_SourceType -** unde se află sursa noastră, adică CDN 

  - **Data\_SqmMachineID -**  ID unic de computer utilizat de Windows SQM 

  - **Data\_SusClientID -** identificator de actualizare Office computer 

  - **Data\_TaskState -** care este starea activității, cum ar fi rulare sau anulat 

  - **Data\_TotalClientCabSize -** dimensiunea fișierului cab al clientului nostru 

  - **Data\_TriggeringUI -** ce a declanșat interfața cu utilizatorul 

  - **Data\_UpdatesEnabled -** dacă sunt activate actualizările Office 

  - **Data\_Version -** versiunea de Office 

### <a name="officeclicktoruntransport"></a>Office.ClickToRun.Transport

Raportează acțiunile de descărcare a fișierelor pentru a determina succesul operațiunii, tipul de descărcare efectuată și informațiile de diagnostic.


- **BytesFromGroupPeers -** octeți de la colegi de grup, doar pentru descărcări care utilizează Optimizarea livrărilor

- **BytesFromHttp -** Octeți de la http, doar pentru descărcări care utilizează Optimizarea livrărilor

- **BytesFromInternetPeers -** Octeți de la colegi de internet, doar pentru descărcări care utilizează Optimizarea livrărilor 

- **BytesFromLanPeers -** octeți de la colegi de Lan, doar pentru descărcări care utilizează Optimizarea livrărilor 

- **canceledJobs -**     numărul solicitărilor anulate din sesiune

- **Conectat-** Indiferent dacă este conectat la sursă

- **ErrorCode -** Codul ultimei erori

- **ErrorDetails -**     detaliile ultimei erori

- **ErrorMessage -**    mesajul ultimei erori 

- **ErrorSource-** Sursa ultimei erori, de exemplu, Connection, LoadFile sau LoadRange

- **FailedJob-** numărul de solicitări nereușite din sesiune

- **FileSize -**    dimensiunea resursei

- **SourcePathNoFilePath-** calea sursă a resursei. Doar sursa http este raportată, calea fișierului local sau calea UNC sunt filtrate

- **SucceededJobs -** Numărul solicitărilor reușite din sesiune

- **TotalJobs -**    Numărul total de solicitări din sesiune

- **TotalRequestedBytes-** Numărul total de octeți din sesiune

- **TotalTransferTime -**   Timpul total de transfer din sesiune

- **TransferredBytes -** Număr total de octeți transferați în sesiune

- **TransportType -** Tip de transport, de exemplu (în optimizarea livrării memoriei, HTTP, serviciu de transfer inteligent de fundal)



### <a name="officeclicktoruntransportexperimentaltransportpipelinecreatetransport"></a>Office.ClickToRun.Transport.ExperimentalTransport.PipelineCreateTransport

Date despre instalări și inventar Office colectate atunci când clientul Clic și Pornire creează un flux de transport pentru a descărca fișiere Office. Utilizat pentru a stabili starea de funcționare a diferitelor tehnologii de transport (de ex., HTTP, BITS, DO) care este de importanță critică la descărcarea corespunzătoare a Office pentru instalare și actualizări.

Se colectează următoarele câmpuri:

  - **Data\_IsForeGroundStreaming** – Dacă redăm în flux în prim plan sau în fundal

  - **Data\_IsInstallMode**-1 dacă instalăm și descărcăm fișiere, 0 dacă nu

  - **Data\_SourceProtocol-** Dacă descărcăm dintr-o rețea de date de conținut, CDN, computerul pe care instalăm, local sau de la o resursă de pe rețeaua locală,

  - **Data\_Status** - succes sau eșec 

### <a name="officeclicktorunupdatestatus"></a>Office.ClickToRun.UpdateStatus

Date despre instalări și inventar Office colectate atunci când clientul Clic și Pornire finalizează o stare de actualizare

Se colectează următoarele câmpuri:

  - **Data\_build** - versiunea de Office instalată momentan

  - **Data\_channel** - canalul în care se află utilizatorul

  - **Data\_errorCode** - cod întreg care specifică tipul de eroare care a apărut, dacă este cazul

  - **Data\_errorMessage** - un șir care descrie eroarea care a apărut, dacă este cazul

  - **Data\_status** - o scurtă stare despre ceea ce s-a întâmplat în timpul actualizării, cum ar fi Reușit sau Descărcat

  - **Data\_targetBuild -** versiunea de Office la care încercăm să actualizăm


### <a name="officeclicktorununiversalbootstrapperapplication"></a>Office.ClickToRun.UniversalBootstrapper.Application

Raportează rezultatul încercării de instalare completă

 - **ErrorCode -** Valoarea întreagă asociată cu o excepție netratată

 - **ErrorDetails -** șir care descrie locația locului în care s-a produs o excepție netratată (funcție, fișier, număr linie, parametri suplimentari setați de lansator)

 - **ErrorMessage -** șir definit în punctul în care a fost lansată o excepție netratată, descriind natura erorii

 - **ErrorType-** Șir care descrie categoria unei excepții netratate

 - **ExitCode -** Valoarea întreagă asociată cu rezultatul rulării aplicației de pregătire, indicând succesul comparativ cu anumite tipuri de erori

### <a name="officeclicktorununiversalbootstrappercalculateparameters"></a>Office.ClickToRun.UniversalBootstrapper.CalculateParameters

Raportează acțiunea care stabilește intrarea colectată utilizând CollectParameters

- **BitField -** valoarea întreagă a argumentului BitField, care ne spune dacă s-a solicitat un canal de instalare/actualizare explicit (lunar, utilizatori Insider lent, utilizatori Insider rapid, semi-anual, vizat semi-anual)

- **ChannelID -** Număr întreg reprezentând valoarea de enumerare a canalului de actualizare/instalare selectat (lunar, utilizatori Insider lent, utilizatori Insider rapid, semi-anual, țintă semi-anual, nevalid)

- **CMDMode -** Șirul prietenos care corespunde comutatorului de mod general care a fost detectat în argumentele cmd transmise către exe.

- **C2RClientUICulture -** Cultura clientului C2R pentru instalare

- **ErrorCode -** Valoarea întreagă asociată cu o excepție netratată

- **ErrorDetails -** șir care descrie locația locului în care s-a produs o excepție netratată (funcție, fișier, număr linie, parametri suplimentari setați de lansator)

- **ErrorMessage -** șir definit în punctul în care a fost lansată o excepție netratată, descriind natura erorii

- **ErrorType-** Șir care descrie categoria unei excepții netratate

- **ExcludedApps -** șir care listează numele aplicațiilor Office individuale solicitate pentru a fi excluse din suitele Office instalate

- **InstalledCabVersion -** Versiunea „16.0.xxxxx.yyyyy” a unui client Office C2R deja instalat

- **InstalledProductVersion -** Versiunea „16.0.xxxxx.yyyyy” a unui produs Office C2R deja instalat

- **IsC2RServiceRunning -** Semnalizarea booleană care indică dacă serviciul unui computer local al unui client C2R modern funcționează pe dispozitiv

- **IsElevatedFlagSet -** semnalizarea booleană care indică dacă aplicația de pregătire a încercat deja să obțină elevarea de administrare

- **IsFireFlyInstalled -** Semnalizarea booleană care indică dacă clientul Office 2013 RTM C2R este instalat în prezent

- **IsFireflyServiceRunning -** Semnalizarea booleană care indică dacă serviciul unui computer local al unui client 2013 RTM C2R funcționează pe dispozitiv

- **IsOfficeInstalled -** Semnalizarea booleană care indică dacă un client Office modern este deja instalat

- **OfficeCultures -** Lista serializată a culturilor Office de instalat

- **OfficeSourceType-** șir prietenos asociat cu valoarea de enumerare a sursei de instalare (CDN, HTTP, UNC, CMBITS, DVD, LOCAL)

- **Origin -** Valoarea șirului care ne informează care dintre originile suportate (Puerto Rico [PR], Singapore [SG], Dublin [DB]) trebuie utilizate pentru fluxul de instalare inițial

- **PlatformFromLink -** șir care indică numărul implicit de biți x86|x64| Office solicitat prin serviciul de configurare C2R

- **PlatformOfExistingInstallation -** Șir care indică dacă Office x86 sau x64 a fost deja instalat pe dispozitiv

- **PlatformToInstall -** Șir care indică decizia finală privind instalarea Office x86 sau x64. Posibilitățile sunt: autorun, configurare, consumator, descărcare, ajutor, arhivator

- **PRID –**    valoarea șirului care reprezintă ID-ul de lansare a produsului solicitat într-un scenariu de instalare de către consumator (de exemplu, „O365ProPlusRetail”)

- **PridsToMigrateFromCentennial-** șir de produse Office pentru migrare de la instalări Magazin la Clic și Pornire

- **ProductsToAdd –**   Șirul serializat care instruiește clientul C2R despre combinațiile de produse/culturi pe care ar trebui să le instaleze

- **ProductsToMigrateFromO15C2R -**  șir de produse și culturi Office pentru migrare de la o instalare Office 2013 Clic și Pornire

- **ProductsToRemove -** șirul serializat care instruiește clientul C2R despre combinațiile de produse/culturi pe care ar trebui să le dezinstaleze

- **SharedComputerLicensing -** Boolean care indică dacă un administrator IT a solicitat configurarea pentru a activa caracteristica „SharedComputerLicensing”

- **ShouldActivate -** Boolean care indică dacă un administrator IT a solicitat o încercare de activare automată a licențelor în configuration.xml

- **ShouldUninstallCentennial -** semnalizare booleană care indică dacă produsele Office de la Magazin ar trebui dezinstalate

- **VersionToInstall -** valoarea șirului din versiunea Office „16.0.xxxxx.yyyyy” care este instalată
 

### <a name="officeclicktorununiversalbootstrappercollectembeddedsignature"></a>Office.ClickToRun.UniversalBootstrapper.CollectEmbeddedSignature

Raportează acțiunea care citește intrarea etichetată din semnătura încorporată exe.  Acesta este un concept nedovedit pentru faptul că iterația anterioară a programului setup.exe nu a fost implementată și este lucrul pe care ne bazăm pentru a transmite opțiunile de produs/limbă/număr de biți ale utilizatorului de la pagina web la procesarea din setup.exe.
 
- **ErrorCode -** Numărul întreg asociat cu o excepție netratată

- **ErrorDetails -** șir care descrie locația locului în care s-a produs o excepție netratată (funcție, fișier, număr linie, parametri suplimentari setați de lansator)

- **ErrorMessage -** șir definit în punctul în care a fost lansată o excepție netratată, descriind natura erorii

- **ErrorType-** Șir care descrie categoria unei excepții netratate

### <a name="officeclicktorununiversalbootstrappercollectparameters"></a>Office.ClickToRun.UniversalBootstrapper.CollectParameters

Raportează parametrii utilizați pentru instalarea Office

- **BitField -** valoarea întreagă a argumentului BitField, care ne spune dacă s-a solicitat un canal de instalare/actualizare explicit (lunar, utilizatori Insider lent, utilizatori Insider rapid, semi-anual, vizat semi-anual)

- **ChannelID -** Număr întreg reprezentând valoarea de enumerare a canalului de actualizare/instalare selectat (lunar, utilizatori Insider lent, utilizatori Insider rapid, semi-anual, țintă semi-anual, nevalid)

- **CMDMode -** Șirul prietenos care corespunde comutatorului de mod general care a fost detectat în argumentele cmd transmise către exe. Posibilitățile sunt: autorun, configurare, consumator, descărcare, ajutor, arhivator

- **C2RClientUICulture -** Cultura clientului C2R pentru instalare

- **ErrorCode -** Valoarea întreagă asociată cu o excepție netratată

- **ErrorDetails -** șir care descrie locația locului în care s-a produs o excepție netratată (funcție, fișier, număr linie, parametri suplimentari setați de lansator)

- **ErrorMessage -** șir definit în punctul în care a fost lansată o excepție netratată, descriind natura erorii

- **ErrorType-** Șir care descrie categoria unei excepții netratate

- **ExcludedApps -** șir care listează numele aplicațiilor Office individuale solicitate pentru a fi excluse din suitele Office instalate

- **InstalledCabVersion -** Versiunea „16.0.xxxxx.yyyyy” a unui client Office C2R deja instalat

- **InstalledProductVersion -** Versiunea „16.0.xxxxx.yyyyy” a unui produs Office C2R deja instalat

- **IsC2RServiceRunning -** Semnalizarea booleană care indică dacă serviciul unui computer local al unui client C2R modern funcționează pe dispozitiv

- **IsElevatedFlagSet -** semnalizarea booleană care indică dacă aplicația de pregătire a încercat deja să obțină elevarea de administrare

- **IsFireFlyInstalled -** Semnalizarea booleană care indică dacă clientul Office 2013 RTM C2R este instalat în prezent

- **IsFireflyServiceRunning -** Semnalizarea booleană care indică dacă serviciul unui computer local al unui client 2013 RTM C2R funcționează pe dispozitiv

- **IsOfficeInstalled -** Semnalizarea booleană care indică dacă un client Office modern este deja instalat

- **OfficeCultures -** Lista serializată a culturilor Office de instalat

- **OfficeSourceType-** șir prietenos asociat cu valoarea de enumerare a sursei de instalare (CDN, HTTP, UNC, CMBITS, DVD, LOCAL)

- **Origin -** Valoarea șirului care ne informează care dintre originile suportate (Puerto Rico [PR], Singapore [SG], Dublin [DB]) trebuie utilizate pentru fluxul de instalare inițial

- **PlatformFromLink -** șir care indică numărul implicit de biți x86|x64| Office solicitat prin serviciul de configurare C2R

- **PlatformOfExistingInstallation -** Șir care indică dacă Office x86 sau x64 a fost deja instalat pe dispozitiv

- **PlatformToInstall -** Șir care indică decizia finală privind instalarea Office x86 sau x64.

- **PRID –**    valoarea șirului care reprezintă ID-ul de lansare a produsului solicitat într-un scenariu de instalare de către consumator (de exemplu, „O365ProPlusRetail”)

- **PridsToMigrateFromCentennial-** șir de produse Office pentru migrare de la instalări Magazin la Clic și Pornire

- **ProductsToAdd –**   Șirul serializat care instruiește clientul C2R despre combinațiile de produse/culturi pe care ar trebui să le instaleze

- **ProductsToMigrateFromO15C2R -** șir de produse și culturi Office pentru migrare de la o instalare Office 2013 Clic și Pornire

- **ProductsToRemove -** șirul serializat care instruiește clientul C2R despre combinațiile de produse/culturi pe care ar trebui să le dezinstaleze

- **SharedComputerLicensing -** Boolean care indică dacă un administrator IT a solicitat configurarea pentru a activa caracteristica „SharedComputerLicensing”

- **ShouldActivate -** Boolean care indică dacă un administrator IT a solicitat o încercare de activare automată a licențelor în configuration.xml

- **ShouldUninstallCentennial -** semnalizare booleană care indică dacă produsele Office de la Magazin ar trebui dezinstalate

- **VersionToInstall -** Valoarea șirului din versiunea Office „16.0.xxxxx.yyyyy” care este instalată

### <a name="officeclicktorununiversalbootstrapperexecute"></a>Office.ClickToRun.UniversalBootstrapper.Execute

Raportează acțiunile cu impact realizate de computer, așa cum sunt determinate de datele argumentate din „CalculateParameters”

- **AvailableClientVersionText -** Valoarea șirului din versiunea client C2R „16.0.xxxxx.yyyyy” găsită în Descriptorul de versiuni XML, care este utilizată pentru a determina dacă un client C2R instalat în prezent ar trebui să fie actualizat

- **CleanFireflyAction -** „adevărat” dacă activitatea CleanFireflyAction este programată să ruleze în timpul acestei instalări

- **CleanO15Action -**  „adevărat” dacă activitatea CleanO15Action este programată să ruleze în timpul acestei instalări

- **CMDMode -** Șirul prietenos care corespunde comutatorului de mod general care a fost detectat în argumentele cmd transmise către exe. Posibilitățile sunt: autorun, configurare, consumator, descărcare, ajutor, arhivator

- **DeliveryMechanism -** Ghid-ul „FFNRoot” extras din Descriptorul de versiune XML (ștampilat de RDX), care ne informează de la ce audiență/canal a venit sursa de compilare

- **DownloadC2RClientAction -** „adevărat” dacă activitatea DownloadC2RClientAction este programată să ruleze în timpul acestei instalări

- **ErrorCode -** Valoarea întreagă asociată cu o excepție netratată

- **ErrorDetails -** șir care descrie locația locului în care s-a produs o excepție netratată (funcție, fișier, număr linie, parametri suplimentari setați de lansator)

- **ErrorMessage -** șir definit în punctul în care a fost lansată o excepție netratată, descriind natura erorii

- **ErrorType-** Șir care descrie categoria unei excepții netratate

- **ExitCode -** valoarea întreagă asociată cu rezultatul rulării fazei de executare a aplicației de pregătire, indicând succesul comparativ cu anumite tipuri de erori

- **LaunchAction -**  „adevărat” dacă activitatea LaunchAction este programată să ruleze în timpul acestei instalări

- **LaunchUpdateAction -**  „adevărat” dacă activitatea LaunchUpdateAction este programată să ruleze în timpul acestei instalări

- **PreReqResult -** valoarea de enumerare întreagă a rezultatului atunci când s-au efectuat verificări PreReq (acceptare/respingere/rerulare)

- **UnexpectedAction -** „adevărat” dacă activitatea UnexpectedAction (un caz de eroare) este programată să ruleze în timpul acestei instalări

- **VersionToInstall -** valoarea șirului din versiunea Office „16.0.xxxxx.yyyyy” care este instalată

### <a name="officeserviceabilitymanagerinventoryaddonheartbeat"></a>Office.ServiceabilityManager.InventoryAddon.Heartbeat

*[Acest eveniment a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

Acest eveniment este utilizat pentru obținerea metadatelor standard la fiecare rulare a programului de completare Inventar, care este parte a Office Serviceability Manager și este utilizat pentru informații de inventar Office pe computerele pentru care a optat un administrator IT. Metadatele de interes specific aici sunt ID-ul sesiunii și sunt folosite pentru legarea cu alte date stocate într-un serviciu cloud pentru fiecare entitate găzduită.

Acest eveniment nu conține câmpuri suplimentare fiindcă numai metadatele sunt relevante.

### <a name="officeserviceabilitymanagerinventoryaddonresults"></a>Office.ServiceabilityManager.InventoryAddon.Results

Acest eveniment este înregistrat când apelul către webservice efectuat în cadrul programului de completare Clic și Pornire Serviceability Manager Inventory se termină, indiferent dacă reușește sau nu. Aceasta este, în esență, ultima operațiune din programul de completare care urmărește starea generală a operațiunii.

Se colectează următoarele câmpuri:

-  **WebCallSource** - o valoare de enumerare (specificată ca un număr întreg) care indică programul de completare Serviceability Manager care a fost sursa apelului:
   - Inventar: 0
   - Configurație inventar: 1
   - Politică inventar: 2
   - Stare rețea inventar: 3

- **Result** - semnalizări numerice ale codurilor de eroare returnate de apelurile API ale Office webservice.

### <a name="officeserviceabilitymanagerwebservicefailure"></a>Office.ServiceabilityManager.WebserviceFailure

De fiecare dată când un apel la un WebService dintr-un program de completare Office Service Manager nu reușește, se înregistrează această instrucțiune. Erorile pot fi cauzate de erori interne sau de incapacitatea de a vă conecta la WebService.

Se colectează următoarele câmpuri:

- **Add-on** - programul de completare Clic și Pornire Serviceability Manager din care a fost efectuat apelul webservice. Acesta poate avea valori, cum ar fi inventar, gestionare etc. codificate ca valoare numerică.

- **Correlation ID** - un GUID generat aleatoriu specific pentru instanța curentă, care este trimis la webservice pentru a corela apelurile între client și server.

- **ErrorInfo** - informații numerice ale codurilor de eroare returnate de apelurile API ale Office webservice.

- **ErrorMessage**- Un mesaj care furnizează detalii suplimentare despre eșec. Fiecare tip de eroare are Hărți la un șir de hardcoded, cu unele tipuri de erori de cartografiere la mai multe șiruri, în funcție de natura specifică a erorii.

- **Function** - funcția din cod de la care a avut loc apelul curent.

- **Status** - codul de stare HTTP returnat de apelul către webservice, de exemplu, 404, 500 etc.


## <a name="enhanced-configuration-service-ecs-events"></a>Evenimente Serviciu de configurație avansată (ECS)

### <a name="officeexperimentationfeaturequerybatched"></a>Office.Experimentation.FeatureQueryBatched

Colectează informații despre Porți de caracteristici/Modificare porți interogate prin codul executat.

Se colectează următoarele câmpuri:

  - **Count** - număr de porți de caracteristici interogate în acest eveniment inclus în set

  - **Features** - informații despre poarta interogată.

  - **Sequence** - ordinea în care a fost interogată FeatureGate

### <a name="officeexperimentationflightnumberline"></a>Office.Experimentation.FlightNumberLine

Colectează lista de configurații primită de client de la ECS

Se colectează următoarele câmpuri:

  - **ECSConfigs** - listă de Configurări ECS cu separator virgulă

  - **LockType** - tip de blocare FlightManager.

  - **TasFlightingVersion** - Număr de versiune

  - **TimeToLock** - timp dintre inițierea liblet și blocarea FlightManager

  - **UnmergedConfigs** -listă de configurații care nu s-au îmbinat

### <a name="officeexperimentationtriggeranalysis"></a>Office.Experimentation.TriggerAnalysis

Acest eveniment contribuie la analiza domeniului de aplicare al utilizării și al indicatorilor de performanță ale produselor (cum ar fi căderile, blocările etc.) pentru subsetul de utilizatori sau de dispozitive eligibile pentru utilizarea caracteristicii, contribuind astfel la asigurarea funcționării corecte a produsului.

Se colectează următoarele câmpuri:

  - **FeatureGate -** identifică setul de caracteristici la care se aplică analiza trigger.

### <a name="onenoteflightdefault"></a>OneNote.FlightDefault
 
Acest eveniment este înregistrat când OneNote solicită serverului ECS valorile edițiilor flight.  Acest lucru este utilizat pentru a activa caracteristicile experimentale pentru utilizatorii care au optat pentru primirea edițiilor flight de acest tip.
 
Se colectează următoarele câmpuri:
 
- **ConfigParam** - configurarea pentru care este accesată valoarea

## <a name="licensing-events"></a>Evenimente de licențiere

### <a name="officelicensingaccepteulaforcurrentlicense"></a>Office.Licensing.AcceptEulaForCurrentLicense 

Se colectează atunci când utilizatorul obține licența și acceptă Termenii licenței pentru licența curentă

Este utilizat pentru a detecta dacă utilizatorul se află sau nu în stare bună, pentru sănătatea sistemului și în scopuri de diagnosticare dacă un utilizator raportează o problemă cu computerul

Se colectează următoarele câmpuri:

  - **ACID** - identificator GUID care reprezintă produsul Office pentru care are licență utilizatorul

  - **DwEulaId** - identificator numeric al tipului de Termeni ai licenței care tocmai au fost acceptați de către utilizator

### <a name="officelicensingactivation"></a>Office.Licensing.Activation 

După configurarea licenței pe computer, încercăm să activăm licența prin apelarea serviciului AVS. Acesta raportează rezultatul apelului de activare

Este de importanță critică în a detecta câți utilizatori întâmpină probleme de activare. Dispunem de o detectare a anomaliilor pentru a detecta orice regresie. Acest lucru este de importanța critică absolută deoarece avem o dependență externă de AVS iar acest semnal indică dacă partenerii noștri externi sunt sănătoși. Este utilizat, de asemenea, în scopuri de diagnosticare și sănătate a sistemului dacă un utilizator raportează o problemă cu computerul

Se colectează următoarele câmpuri:

  - **Acid** - identificator GUID care reprezintă produsul Office pentru care are licență utilizatorul

  - **ReferralData** - identificator al OEM care a instalat Office pe computer

### <a name="officelicensingactivationwizard"></a>Office.Licensing.ActivationWizard 

Dacă nu putem activa automat licența dintr-un motiv sau altul, afișăm utilizatorului un expert de activare. Acesta raportează faptul că expertul i se afișează utilizatorului. Este de importanță critică pentru a detecta dacă utilizatorul se află în stare bună, fără să îi lipsească funcționalități, este utilizat pentru sănătatea sistemului și în scopuri de diagnosticare dacă un utilizator raportează o problemă cu computerul

Acest eveniment nu colectează niciun câmp.

### <a name="officelicensingenforcesigninqualified"></a>Office.Licensing.EnforceSignInQualified 

Acesta este semnalul care ne informează dacă experimentul pe care îl efectuăm pentru a impune semnătura utilizatorului ca parte a licențierii este reușit. Acest lucru este de importanță critică în a detecta succesul sau eșecul experimentului care impune utilizatorilor să se conecteze, ceea ce reprezintă un pas obligatoriu pentru stiva de licențiere modernă. Dacă nu se conectează, utilizatorii nu vor putea utiliza aplicația.

Se colectează următoarele câmpuri:

  - **Qualified** – identifică dacă utilizatorul este calificat pentru impunerea conectării

### <a name="officelicensingexpirationdialogshown"></a>Office.Licensing.ExpirationDialogShown

Se colectează când afișăm utilizatorului caseta de dialog de expirare care spune că licența a expirat. Este de importanță critică pentru a detecta dacă utilizatorul se află în stare bună, fără să îi lipsească funcționalități, este utilizat pentru sănătatea sistemului și în scopuri de diagnosticare dacă un utilizator raportează o problemă cu computerul

Se colectează următoarele câmpuri:

  - **LicNotificationState** – un enumerator care ne informează ce fel de notificare se afișează pentru utilizator

### <a name="officelicensingfullvalidation"></a>Office.Licensing.FullValidation 

Se colectează la fiecare sesiune care raportează starea de licențiere a computerului și erorile vizualizate de utilizator din cauza cărora nu poate să utilizeze aplicația. Acest eveniment indică dacă computerul utilizatorului este în bună stare de funcționare sau nu. Avem configurată o detectare a anomaliilor pentru acest eveniment pentru a indica dacă o regresie provoacă un comportament inadecvat al utilizatorului. Și acesta este de importanță critică la diagnosticarea problemelor utilizatorului și pentru monitorizarea sănătății sistemului

Se colectează următoarele câmpuri:

  - **Acid** - identificator GUID care reprezintă produsul Office pentru care are licență utilizatorul 

  - **IsSessionLicensing** - indiferent dacă momentan rulează sau nu în modul de activare computer partajat 

  - **LicenseCategory** - categoria de licență Office pe care o folosește utilizatorul 

  - **Licenses** - lista de nume a tuturor licențelor de Office prezente pe calculator 

  - **LicenseStatuses** - starea tuturor licențelor de Office prezente pe calculator 

### <a name="officelicensinggetentitlement"></a>Office.Licensing.GetEntitlement 

Colectăm acest lucru atunci când utilizatorul configurează un dispozitiv și apelăm serviciul nostru de licențiere pentru a detecta dacă utilizatorul autentificat are drepturi de Office sau nu. Acesta raportează rezultatul apelului respectiv. Este de importanță critică pentru a detecta dacă utilizatorul se află în stare bună și dacă îi lipsesc funcționalități, este utilizat pentru sănătatea sistemului și în scopuri de diagnosticare dacă un utilizator raportează o problemă cu computerul

Se colectează următoarele câmpuri:

- **EntitlementCount** - numărul de drepturi pe care le are utilizatorul


### <a name="officelicensingheartbeat"></a>Office.Licensing.Heartbeat 

La fiecare sesiune verificăm dacă au trecut 72 de ore de la ultima reînnoire de licență și încercăm să extindem valabilitatea licenței curente. Acest eveniment raportează succesul sau eșecul apelului pe care îl efectuăm pentru a ne asigura că putem extinde valabilitatea licenței și să păstrăm funcțională instalarea Office a utilizatorului. Este de importanță critică în diagnosticarea problemelor legate de abonament și serviciu pentru utilizator și în detectarea regresiilor pentru utilizatorii care dețin deja un abonament activat.

Se colectează următoarele câmpuri:

  - **Mode** - o reprezentare cu enumerator a stivei de licențiere Office care este utilizată la acest computer

### <a name="officelicensinginclientpinredemptioncallpinredemptionapi"></a>Office.Licensing.InClientPinRedemption.CallPinRedemptionAPI

Această telemetrie urmărește rezultatele apelului de serviciu de valorificare a pinului Office.

Se colectează următoarele câmpuri:

- **ClientTransactionId** - Identificator unic pentru apelul de serviciu.

- **ErrorCategory** - Fiecare tip de eroare poate aparține unei categorii mai generale, cum ar fi „reîncercare”.

- **ErrorType** - Motivul erorii, cum ar fi "AlreadyRedeemedByOther".

- **InAFOFlow** - Valoare booleană care indică dacă ne aflăm în fluxul de valorificare AFO.

- **StatusCode** - Rezultat de un cuvânt al apelului de serviciu, cum ar fi „Creat”.

- **StatusMessage** - Detalii despre codul de stare, cum ar fi „Aprovizionat cu succes”.

- **UsingNulApi** - valoare booleană care indică dacă utilizăm noua stivă de licențiere.

### <a name="officelicensinginrfm"></a>Office.Licensing.InRFM 

Dacă dispozitivul intră în modul de funcționalitate redusă, trimitem acest semnal pentru a indica faptul că computerul nu este într-o stare bună de funcționare. Este de importanță critică pentru a detecta dacă utilizatorul se află în stare bună și dacă îi lipsesc funcționalități, este utilizat pentru sănătatea sistemului și în scopuri de diagnosticare dacă un utilizator raportează o problemă cu computerul

Se colectează următoarele câmpuri:

  - **ACID** - identificator GUID care reprezintă produsul Office pentru care are licență utilizatorul

  - **DaysRemaining** - numărul de zile rămase până la expirarea licenței Office curente

  - **Mode** - o reprezentare cu enumerator a stivei de licențiere Office care este utilizată la acest computer

  - **ProductName** - numele produsului utilizat în prezent de utilizator

  - **Reason** - Codul de eroare care indică motivul stării curente a licenței

### <a name="officelicensinginstallkey"></a>Office.Licensing.InstallKey

Se colectează atunci când încercăm să instalăm o cheie la dispozitiv pentru a licenția computerul. Raportează dacă instalarea a reușit și, dacă nu a reușit, raportează apoi codul de eroare. Este de importanță critică pentru a detecta dacă utilizatorul se află în stare bună, fără să îi lipsească funcționalități, este utilizat pentru sănătatea sistemului și în scopuri de diagnosticare dacă un utilizator raportează o problemă cu computerul

Se colectează următoarele câmpuri:

  - **Prid** - numele grupului de produse pentru care este instalată o cheie

  - **SkuId** - identificator GUID care reprezintă produsul Office pentru care este instalată o cheie 

### <a name="officelicensinginvokelicensewizard"></a>Office.Licensing.InvokeLicenseWizard

În cazul în care observăm probleme cu fluxul de lucru de Activare, declanșăm un expert de licențe și trimitem acest semnal pentru a indica același lucru Este de importanță critică pentru a detecta dacă utilizatorul se află în stare bună, fără să îi lipsească funcționalități, este utilizat pentru sănătatea sistemului și în scopuri de diagnosticare dacă un utilizator raportează o problemă cu computerul

Se colectează următoarele câmpuri:

  - **Acid** - identificator GUID care reprezintă produsul Office pentru care are licență utilizatorul

  - **LicenseStatus** - starea licenței Office pe care o folosește utilizatorul

  - **MachineKey** - identificator alfanumeric al cheii de licență care a fost emise pentru utilizator

### <a name="officelicensinglicensingbar"></a>Office.Licensing.LicensingBar

Dacă dispozitivul întâmpină probleme de licențiere și în final afișăm utilizatorului o bară, trimitem acest semnal care raportează, de asemenea, tipul de bară afișată utilizatorului. Este de importanță critică pentru a detecta dacă utilizatorul se află în stare bună, fără să îi lipsească funcționalități, este utilizat pentru sănătatea sistemului și în scopuri de diagnosticare dacă un utilizator raportează o problemă cu computerul.

Se colectează următoarele câmpuri:

  - **SuppressNotification** - indică dacă am eliminat bara de licențiere

  - **Title** - titlul barei de licențiere care a fost afișată utilizatorului

  - **Type** - tipul de bară de licențiere care a fost afișată utilizatorului

### <a name="officelicensinglicexitofficeprocess"></a>Office.Licensing.LicExitOfficeProcess 

Dacă în final Office se închide/cade din cauza unei probleme de licențiere, trimitem acest semnal pentru a indica problema. Este de importanță critică pentru a detecta dacă utilizatorul se află în stare bună, fără să îi lipsească funcționalități, este utilizat pentru sănătatea sistemului și în scopuri de diagnosticare dacă un utilizator raportează o problemă cu computerul.

Se colectează următoarele câmpuri:

  - **ExitCode** - codul intern care a cauzat ieșirea din aplicație

### <a name="officelicensingloadidentityticket"></a>Office.Licensing.LoadIdentityTicket

În cadrul procesului în care se încearcă licențierea dispozitivului, aplicația încearcă să încarce identitatea utilizatorului pentru a vedea dacă utilizatorul are drepturi de Office sau nu. Acest eveniment raportează succesul sau eșecul în aceeași situație împreună cu codul de eroare Este de importanță critică pentru a detecta dacă utilizatorul se află în stare bună, fără să îi lipsească funcționalități, este utilizat pentru sănătatea sistemului și în scopuri de diagnosticare dacă un utilizator raportează o problemă cu computerul.

Se colectează următoarele câmpuri:

  - **FederationProvider** - un șir care identifică furnizorul de federație pentru utilizatorul conectat în prezent

  - **IdentityProvider** – un șir care identifică furnizorul de identitate pentru utilizatorul conectat în prezent

### <a name="officelicensinglvuxeulaexplicitcrash"></a>Office.Licensing.LVUX.EULAExplicitCrash 

Se colectează dacă am prezentat utilizatorului Termenii licenței, iar utilizatorul a decis să nu îi accepte, ceea ce ne-a determinat să blocăm/închidem aplicația. Este de importanță critică pentru a detecta dacă utilizatorul se află în stare bună, fără să îi lipsească funcționalități, este utilizat pentru sănătatea sistemului și în scopuri de diagnosticare dacă un utilizator raportează o problemă cu computerul.

Se colectează următoarele câmpuri:

  - **Acid** - identificator GUID care reprezintă produsul Office pentru care are licență utilizatorul

  - **OptInShown** - indică dacă s-a afișat deja caseta de dialog de optare pentru înscriere la prima pornire a aplicației

### <a name="officelicensingnextuserlicensingeligible"></a>Office.Licensing.NextUserLicensingEligible 

Acest semnal ne informează dacă un utilizator este calificat să treacă la noua noastră stivă de licențiere. Este de importanță critică pentru a cuantifica impactul asupra utilizatorilor existenți pe măsură ce implementăm noua noastră stivă de licențiere și ne asigurăm că utilizatorii nu pierd funcționalitatea.

Acest eveniment nu colectează niciun câmp.

### <a name="officelicensingnulfetcherfetchmodelfromols"></a>Office.Licensing.Nul.Fetcher.FetchModelFromOls

Atunci când dispozitivul este pe stiva de licențiere modernă, încercăm să obținem un fișier de licență direct de la serviciu. Acest eveniment raportează succesul sau eșecul împreună cu codul de eroare al respectivului apel de serviciu. Este de importanță critică pentru a detecta dacă utilizatorul se află în stare bună pe stiva de licențiere modernă, este utilizat pentru sănătatea sistemului și în scopuri de diagnosticare dacă un utilizator raportează o problemă cu computerul.

Se colectează următoarele câmpuri:

  - **MetadataValidationResult** - rezultatul validării metadatelor licenței pentru a verifica faptul că nu a fost falsificată

  - **SignatureValidationResult** – rezultatul validării semnăturii licenței pentru a verifica faptul că nu a fost falsificată

### <a name="officelicensingnulvalidationfullvalidation"></a>Office.Licensing.Nul.Validation.FullValidation 

Se colectează la fiecare sesiune a unui dispozitiv care rulează pe stiva de licențiere modernă. Raportează starea de licențiere a computerului și erorile vizualizate de utilizator din cauza cărora nu poate să utilizeze aplicația. Acest eveniment indică dacă computerul utilizatorului este în bună stare de funcționare pe stiva de licențiere modernă. Avem configurată o detectare a anomaliilor pentru acest eveniment pentru a indica dacă o regresie provoacă un comportament inadecvat al utilizatorului. Și acesta este de importanță critică la diagnosticarea problemelor utilizatorului și pentru monitorizarea sănătății sistemului.

Se colectează următoarele câmpuri:

  - **Acid** - identificator GUID care reprezintă produsul Office pentru care are licență utilizatorul 

  - **AllAcids** – listă cu toate GUID-urile produsului pentru care utilizatorul deține în prezent licență 

  - **Category** - categoria de licență Office folosită de utilizator 

  - **DaysRemaining** - numărul de zile rămase până la expirarea licenței Office curente 

  - **LicenseId** - identificator alfanumeric al licenței care a fost emise pentru utilizator 

  - **LicenseType** - tipul de licență Office folosită de utilizator 

### <a name="officelicensingofficeclientlicensingdolicensevalidation"></a>Office.Licensing.OfficeClientLicensing.DoLicenseValidation 

Este vorba despre metadatele de licențiere colectate de pe dispozitiv la fiecare pornire care raportează indicatorul acid al licenței, starea licenței, tipul de licență și alte proprietăți ale acesteia care sunt esențiale în identificarea caracteristicilor puse la dispoziția utilizatorului. Este de importanță critică în a identifica setul de caracteristici puse la dispoziția utilizatorului, precum și dacă utilizatorului îi lipsește o anumită funcționalitate. Este utilizat, de asemenea, pentru calculele Utilizatorilor activi zilnic/lunar și pentru diferite alte rapoarte ale unor echipe la nivelul Office deoarece precizează produsul tip folosit de utilizator, indiferent că este un produs cu abonament sau că utilizatorului îi lipsește o funcționalitate de importanță critică.

Se colectează următoarele câmpuri:

  - **FullValidationMode** – mod care indică faptul că suntem în curs de verificare completă a validării licenței 

  - **IsRFM** - indică dacă utilizatorul se află în modul de funcționalitate redusă sau nu 

  - **IsSCA** - indică dacă rulăm în modul de activare am rulează în modul de activare computer partajat 

  - **IsSubscription** - indică dacă utilizatorul utilizează o licență de abonament sau nu 

  - **IsvNext** - indică dacă utilizăm noua stivă de licențiere modernă sau nu 

  - **LicenseCategory** - categoria de licență Office pe care o folosește utilizatorul 

  - **LicenseStatus** - starea licenței Office pe care o folosește utilizatorul 

  - **LicenseType** - tipul de licență Office folosită de utilizator 

  - **LicensingACID** - identificator GUID care reprezintă produsul Office pentru care are licență utilizatorul 

  - **OlsLicenseId** - identificator alfanumeric al licenței care a fost emise pentru utilizator 

  - **SkuIdIsNull** – Indică dacă am întâmpinat o eroare și nu cunoaștem produsul pe care rulează utilizatorul 

  - **SlapiIsNull** – indică dacă am întâmpinat o problemă la popularea unuia dintre obiectele de licențiere 

### <a name="officelicensingonlinerepair"></a>Office.Licensing.OnlineRepair 

Dacă dintr-un motiv sau altul nu putem activa un utilizator și trebuie să îi afișăm o casetă de dialog care îi solicită să intre online și să încerce să parcurgă pașii de reparare, se declanșează acest eveniment. Este de importanță critică pentru a detecta dacă utilizatorul se află în stare bună, fără să îi lipsească funcționalități, este utilizat pentru sănătatea sistemului și în scopuri de diagnosticare dacă un utilizator raportează o problemă cu computerul

Acest eveniment nu colectează niciun câmp.

### <a name="officelicensingoobetrybuychoice"></a>Office.Licensing.OOBE.TryBuyChoice

Utilizatorilor cu Office preinstalat pe noile dispozitive care nu au drepturi Office li se afișează o casetă de dialog prin care pot să încerce, să cumpere sau să introducă o cheie de produs pentru a obține licența. Acest eveniment capturează acțiunea utilizatorului din caseta de dialog. Acest eveniment este utilizat pentru a urmări acțiunea utilizatorului întreprinsă în caseta de dialog afișată pentru utilizatorii fără drepturi Office, când Office a fost preinstalat pe computer și ajută să determinăm dacă utilizatorul este licențiat sau nelicențiat în mod implicit.

Se colectează următoarele câmpuri:

- **Buy** - spune dacă utilizatorul a făcut clic sau nu pe butonul cumpărați

- **ForceAutoActivate** - spune dacă activarea în cadrul aplicației ar trebui să fie încercată sau nu

- **GoBackToSignIn** - spune dacă utilizatorul a dorit să se conecteze din nou (eventual cu alt cont)

- **IsPin** - spune dacă utilizatorul a introdus un cod PIN

- **ProductKey** - spune dacă utilizatorul a încercat să introducă o cheie de produs

- **Try** - spune dacă utilizatorul a făcut clic sau nu pe butonul încercați

- **UserDismissed** - Indică dacă utilizatorul a respins caseta de dialog și, prin urmare, este în perioada de grație sau în modul de funcționalitate redusă, deoarece nu a ales să cumpere Office sau să obțină o versiune de încercare

### <a name="officelicensingpurchase"></a>Office.Licensing.Purchase 

Avem un experiment care oferă utilizatorului opțiunea de a încerca și a configura plata automată pentru Office direct din aplicație, fără să iasă din contextul aplicației. Acesta raportează succesul sau eșecul experimentului respectiv împreună cu codul de eroare Este de importanță critică pentru a detecta dacă utilizatorul se află în stare bună, fără să îi lipsească funcționalități, este utilizat pentru sănătatea sistemului și în scopuri de diagnosticare dacă un utilizator raportează o problemă cu computerul.

Se colectează următoarele câmpuri:

  - **StorePurchaseStatus** - reprezintă codul de eroare/codul de succes al apelului de achiziție care a fost efectuat prin Microsoft Store

### <a name="officelicensingsearchforsessiontoken"></a>Office.Licensing.SearchForSessionToken

Dacă utilizatorul rulează în modul de activare computer partajat, încercăm să căutăm un simbol de sesiune pe computer care permite utilizatorului să folosească aplicația. Acest eveniment raportează succesul sau eșecul scenariului împreună cu codul de eroare Este de importanță critică pentru a detecta dacă utilizatorul se află în stare bună, fără să îi lipsească funcționalități, este utilizat pentru sănătatea sistemului și în scopuri de diagnosticare dacă un utilizator raportează o problemă cu computerul.

Se colectează următoarele câmpuri:

  - **LoadLicenseResult** - reprezintă codul de eroare/codul de succes al operației noastre de încărcare a licențelor pentru utilizatorul curent

  - **OpportunisticTokenRenewalAttempted** - Indică dacă am încercat să reînnoim simbolul de sesiune al utilizatorului în mod oportunist

  - **SetAcidResult** - reprezintă codul de eroare/codul de succes al operației noastre de setare a indicatorului acid la valoarea prevăzută

### <a name="officelicensingshownewdeviceactivationdialog"></a>Office.Licensing.ShowNewDeviceActivationDialog

La prima pornire a unei aplicații Office, vom încerca să afișăm o casetă de dialog de conectare prepopulată cu acreditările utilizatorului folosite la descărcarea Office. Apoi, utilizatorul poate continua să se conecteze cu acreditările respective, să utilizeze alte acreditări sau să dezactiveze caseta de dialog. Acest eveniment raportează acțiunea întreprinsă de utilizator atunci când îi apare această casetă de dialog. Este de importanță critică pentru a detecta dacă un utilizator se află în stare bună pe stiva de licențiere modernă, este utilizat pentru sănătatea sistemului și în scopuri de diagnosticare dacă un utilizator raportează o problemă cu computerul

Se colectează următoarele câmpuri:

  - **UserAction** - identificator pentru acțiunea întreprinsă de utilizator atunci când îi apare această casetă de dialog.

### <a name="officelicensingskutoskuconversion"></a>Office.Licensing.SkuToSkuConversion

Ca parte a licențierii utilizatorului, dacă trebuie să modificăm unitatea SKU a utilizatorului de la o unitate SKU la alta, trimitem acest semnal împreună cu codul de succes sau de eroare. Este de importanță critică pentru a detecta dacă utilizatorul se află în stare bună și dacă îi lipsesc funcționalități, este utilizat pentru sănătatea sistemului și în scopuri de diagnosticare dacă un utilizator raportează o problemă cu computerul.

Se colectează următoarele câmpuri:

  - **DestinationSku** - numele unității SKU la care trebuie convertit produsul instalat în prezent

  - **PendingAcid** - ID-ul produsului pentru care este în așteptare o conversie SKU

  - **SourceSku** -numele unității SKU originale care a fost instalată pe computer

  - **UninstallProduct** - indică dacă produsul vechi va fi dezinstalat ca parte a conversiei

### <a name="officelicensingtelemetryflowolsresults"></a>Office.Licensing.TelemetryFlow.OLSResults

Atunci când un utilizatorul nu este licențiat, efectuăm mai multe apeluri de serviciu pentru a-l aduce pe utilizator în stare de licențiere și pentru a-și activa produsul Office.  Acest eveniment este declanșat la apelarea Serviciului de licențiere Office pentru a verifica dacă utilizatorul are drepturi.  Acest eveniment va fi utilizat pentru a urmări starea de licențiere a utilizatorului după apelarea Serviciului de licențiere Office și starea clientului Office după încercarea de activare a Office.

Se colectează următoarele câmpuri:

- **EntitlementPickerShown** - spune dacă utilizatorul a avut mai multe drepturi și dacă utilizatorul a trebuit să aleagă manual între acestea pentru a obține licența

- **GetAuthResult** - comunică diverse situații în care poate fi clientul cum ar fi dacă au primit o cheie de produs necompletată de la Serviciul de licențiere Office sau dacă au aveau dreptul să primească alt produs, iar Office trebuie să fie schimbat cu un produs nou

- **GetEntitlementsCount** - indică numărul de drepturi pe care le are utilizatorul

- **GetEntitlementsSucceeded** - indică dacă apelul către un API pentru Serviciul de licențiere Office pentru a regăsi drepturile utilizatorului a reușit sau nu

- **GetKeySucceeded** - indică dacă apelul către un API pentru Serviciul de licențiere Office pentru a regăsi o cheie a reușit

- **GetNextUserLicenseResult** - spune dacă stiva de licențiere modernă a putut funcționa și dacă utilizatorul a fost licențiat sau nu

- **InstallKeyResult** - indică diverse motive pentru care utilizatorul poate fi într-o stare nepotrivită, cum ar fi dacă activarea nu a reușit sau dacă instalarea cheii nu a reușit

- **NotInitializedBeforeWhileAdding** - este doar informativ și indică dacă evenimentul a fost adăugat la o hartă a managerului de telemetrie fără să se înregistreze explicit pentru aceasta

- **NotInitializedBeforeWhileSending** - este doar informativ și indică dacă s-a încercat trimiterea evenimentului fără să fie înregistrat dinainte în mod explicit în harta managerului de telemetrie

- **SentOnDestruction** - Este doar informativ și indică dacă evenimentul a fost adăugat la o hartă a managerului de telemetrie și nu a fost trimis în mod explicit

- **Tag** - utilizat pentru a indica de unde din cod a fost trimis evenimentul

- **VerifyEntitlementsResult** - indică diverse stări în care poate fi utilizatorul după validarea drepturilor regăsite la Serviciul de licențiere Office

### <a name="officelicensingtelemetryflowsearchforbindingresult"></a>Office.Licensing.TelemetryFlow.SearchForBindingResult

Computere OEM care sunt dotate cu Office (abonamente pe un an sau permanente).  Aceste produse Office sunt plătite când clientul își cumpără computerul. Computerele care sunt setate cu un anumit regkey (OOBEMode: OEMTA) pot avea o legătură Office asociată.  Atunci când încărcăm Office pe astfel de computere, efectuăm verificări de serviciu pentru a vedea dacă este găsită o legătură Office care corespunde calculatorului.

Această activitate de telemetrie urmărește punctele de succes și eșec în căutarea unei legături, astfel încât să ne asigurăm că mașinile care au o legătură o pot prelua cu succes și că serviciile noastre sunt funcționale.  Această activitate nu urmărește calculatoarele care nu au legături asociate cu acestea după ce verificăm serviciile noastre.

Se colectează următoarele câmpuri:

- **GenuineTicketFailure** - Ne indică HRESULT eșec atunci când se încearcă obținerea tichetului/cheii de produs (WPK) originale Windows a computerului.

- **PinValidationFailure** - ne spune de ce procesul de validare a codului PIN nu a reușit. Erori posibile:
    - GeoBlocked
    - InvalidFormat
    - InvalidPin
    - InvalidState
    - InvalidVersion
    - Unknown
    - Used

- **PinValidationResult** - ne indică rezultatul validării codului PIN pentru un PIN pe care nu am reușit să-l descifrăm.

- **Pkpn** - intervalul pkpn căruia îi aparține codul PIN.

- **Success** - indică faptul că am preluat cu succes o legătură Office (PIN) validă pentru calculator.

- **Tag** - ne spune la ce pas am oprit căutarea unei legături. Etichete posibile:
  - 0x03113809  Eroare lipsă conexiune la internet/serviciu în timpul validării codului PIN
   - 0x0311380a Eroare de validare a codului PIN, trimis cu câmpul PinValidationFailure
  - 0x0310410f Succes, trimis cu câmpul Success
  - 0x0311380d  Erori de reîncercare (probleme de internet, erori necunoscute)
  - 0x0311380e  Erori care nu pot fi reîncercate (oferta de legătură a expirat)
  - 0x0311380f  Alte erori (nu se poate licenția)
  - 0x03104111  Nereușită la descifrarea codului PIN Office, trimis cu câmpul PinValidationResult

- **WpkBindingFailure** - Ne spune codul de eroare la legarea dintre codul PIN Office și WPK pentru computer.

### <a name="officelicensingtelemetryflowshowafodialogs"></a>Office.Licensing.TelemetryFlow.ShowAFODialogs

După obținerea cu succes a unui cod PIN Office valid legat la un calculator cu Office preinstalat, îi afișăm utilizatorului o casetă de dialog de conectare sau o casetă de dialog de valorificare.  După ce codul PIN a fost valorificat, afișăm caseta de dialog EULA.  Ca parte din caracteristica noastră AFO modernizată, am reîmprospătat cele două casete de dialog pentru a transmite mai multe informații despre produsul Office care este livrat cu calculatorul.  Această telemetrie este utilizată pentru a urmări dacă caracteristica noastră reduce cu succes dezacordurile cu utilizatorul la valorificarea produsului său, urmărind fluxul și punctele de ieșire ale procesului de valorificare (ce casetă de dialog a fost respinsă).

Se colectează următoarele câmpuri:

- **ActionCreateAccount** - utilizatorul a ales să creeze un cont.

- **ActionSignIn** - utilizatorul a ales să se conecteze.

- **DialogRedemption** - afișarea dialogului de valorificare AFO.

- **DialogSignIn** - afișarea dialogului de conectare AFO.

- **OExDetails** - Detaliile erorii pe care o primim când dialogul de conectare pentru identitate a fost respins.

- **OExType** - tipul erorii pe care o primim când dialogul de conectare pentru identitate a fost respins.

- **Tag** - ne spune la ce pas părăsește utilizatorul procesul de valorificare AFO. Etichete posibile:
    - 0x0311380b    Utilizatorul a respins dialogul de conectare a identității din dialogul de valorificare
    - 0x0311380c    Nu a reușit să încarce automat un mesaj de conectare la identitatea utilizatorului din caseta de dialog de valorificare
    - 0x03113810    Nu a reușit să încarce informațiile demografice ale contului (cod de țară, limbă, monedă, oferta de încercare și preferințele de marketing)
    - 0x03113805    Utilizatorul a respins dialogul de conectare a identității din dialogul de conectare
    - 0x03113806    nu a reușit să încarce automat un mesaj de conectare la identitatea utilizatorului din dialogul de conectare
    - 0x03113807    nu a reușit să încarce automat o identitate
    - 0x03113811    utilizatorul a închis dialogul de conectare/valorificare
    - 0x03113812    utilizatorul a închis dialogul de acceptare EULA
    - 0x03113808    utilizatorul a acceptat EULA

- **UseInAppRedemption** - Ne spune dacă menținem utilizatorii în aplicație pentru valorificare sau îi trimitem pe web pentru a-și valorifica pinul preluat (pre populat).

- **UseModernAFO** - Ne spune dacă utilizăm noua sau vechea experiență AFO.

### <a name="officelicensingtelemetryflowshowtrybuydialogforoobe"></a>Office.Licensing.TelemetryFlow.ShowTryBuyDialogForOOBE

Atunci când calculatoarele noi au Office preinstalat și utilizatorul nu are drepturi, vom afișa un dialog care îi oferă utilizatorului opțiunea de a încerca, a cumpăra sau a introduce o cheie de produs, astfel încât utilizatorul să poată fi licențiat și acest eveniment urmărește dacă dialogul a fost afișat. Acest eveniment ne ajută să știm dacă dialogul i-a fost afișat utilizatorului pentru a încerca, a cumpăra sau a introduce cheia de produs și, prin urmare, ne va ajuta să aflăm dacă utilizatorul a avut oportunitatea de a obține licența.

Se colectează următoarele câmpuri: 

- **ActiveView** - indică ID-ul dialogului care i-a fost afișat utilizatorului

- **CurrentOOBEMode** - indică modul de pre-instalare (modul OOBE, cum ar fi AFO, OEM etc.)

- **NotInitializedBeforeWhileAdding** - este doar informativ și indică dacă evenimentul a fost adăugat la o hartă a managerului de telemetrie fără să se înregistreze explicit pentru aceasta

- **SentOnDestruction** - Este doar informativ și indică dacă evenimentul a fost adăugat la o hartă a managerului de telemetrie și nu a fost trimis în mod explicit

- **ShowTryButton** - indică dacă butonul Try i-a fost afișat utilizatorului în dialog sau nu

- **Tag** - utilizat pentru a indica de unde din cod a fost trimis evenimentul

### <a name="officelicensingtelemetryflowtrialflow"></a>Office.Licensing.TelemetryFlow.TrialFlow

Atunci când un utilizator nelicențiat de Office preinstalat pe un computer încearcă să obțină o versiune de încercare, se declanșează acest eveniment.  Este utilizat pentru a vedea ce cale va urma utilizatorul pentru a obține o versiune de încercare și dacă au existat erori în timpul obținerii versiunii de încercare prin achizițiile în cadrul aplicațiilor.  În funcție de acțiunea utilizatorului și de rezultatul achiziției în cadrul aplicației, utilizatorul poate deveni nelicențiat.

Se colectează următoarele câmpuri:

- **HasConnectivity** - Indică dacă utilizatorul are conexiune la internet și, în caz că nu, utilizatorul ar putea să trebuiască să utilizeze o licență de grație de cinci zile sau ar putea fi în modul de funcționalitate redusă

- **InAppTrialPurchase** - indică dacă ediția flight este activată pentru lansarea SDK de achiziție în Magazin pentru a captura PI și a achiziționa o versiune de încercare în cadrul aplicației

- **IsRS1OrGreater** - indică dacă versiunea sistemului de operare este mai mare decât RS1 sau nu, deoarece SDK de achiziție în Magazin ar trebui să fie utilizat doar dacă versiunea sistemului de operare este mai mare decât RS1

- **NotInitializedBeforeWhileAdding**: este doar informativ și indică dacă evenimentul a fost adăugat la o hartă a managerului de telemetrie fără să se înregistreze explicit pentru aceasta

- **OEMSendToWebForTrial** - indică dacă ediția flight este activată pentru a trimite utilizatorii pe web pentru a valorifica o versiune de încercare

- **StoreErrorConditions** - indică diversele condiții sub care poate să fi eșuat SDK de achiziție în Magazin.

- **StoreErrorHResult** - indică codul de eroare returnat de SDK de achiziție în Magazin

- **StorePurchaseStatusResult** - spune rezultatul apelării SDK de achiziție în Magazin și dacă utilizatorul a făcut sau nu o achiziție, ceea ce ne ajută să determinăm dacă utilizatorul trebuie să primească licență pentru a utiliza Office

- **Tag** - utilizat pentru a indica de unde din cod a fost trimis evenimentul

- **UserSignedInExplicitly** - spune dacă utilizatorul s-a conectat în mod explicit, iar în acest caz am redirecționa utilizatorii către web pentru versiunea de încercare

### <a name="officelicensingusegracekey"></a>Office.Licensing.UseGraceKey

Dintr-un motiv sau altul, nu putem să licențiem utilizatorul; instalăm o cheie de grație și trimitem acest semnal cu semnificație. Este de importanță critică pentru a detecta dacă utilizatorul se află în stare bună și dacă îi lipsesc funcționalități, este utilizat pentru sănătatea sistemului și în scopuri de diagnosticare dacă un utilizator raportează o problemă cu computerul

Se colectează următoarele câmpuri:

  - **OpportunisticTokenRenewalAttempted** - indică dacă am încercat o reînnoire oportunistă pentru utilizator în modul de activare computer partajat

  - **ReArmResult** - indică rezultatul reactivării perioadei de probă a cheii instalate, ceea ce poate extinde valabilitatea licenței curente

### <a name="onenoteenrollmentresult"></a>OneNote.EnrollmentResult
 
Acest eveniment înregistrează starea la înscrierea în Intune.  Acest scenariu este specific conturilor activate pentru Intune.
 
Se colectează următoarele câmpuri:
 
- **EnrollmentResult** - rezultatul înscrierii în Intune

## <a name="microsoft-autoupdate-mau-events"></a>Evenimente Microsoft AutoUpdate (MAU)

### <a name="appdelegate_launch"></a>appdelegate_launch

Acest eveniment indică faptul că s-a produs o încercare de lansare a aplicației. Vom înregistra rezultatul (eșecul sau succesul). Vom utiliza acest eveniment pentru a identifica cazurile în care MAU nu reușește să fie lansat

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul
    
- **AppInfo_Language** - limba în care rulează aplicația

- **AppversionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

 - **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - un set de text static care indică starea lansării.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="appdelegate_terminate"></a>appdelegate_terminate

Acest eveniment indică faptul că a avut loc o ieșire elegantă din aplicație. Vom utiliza acest eveniment pentru a distinge ieșirile elegante din aplicație de cele neelegante.

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public
    
- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului
    
- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text static care indică finalizarea Microsoft Autoupdate.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="appinstall_connecttoxpc"></a>appinstall_connecttoxpc

Acest eveniment indică faptul că s-au produs erori la conectarea la MAU Helper (o componentă care efectuează instalarea aplicației).  Acest eveniment indică o potențială corupție a aplicației MAU. Dispozitivul nu va putea instala actualizări.

Se colectează următoarele câmpuri:    

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține informații despre erori legate de problema de conexiune.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="appregistry_info"></a>appregistry_info

Acest eveniment indică faptul că aplicația a fost lansată. Vom utiliza acest eveniment pentru a lista aplicațiile pentru care MAU poate controla actualizările, numărul de copii disponibile, precum și versiunea acestora și locația de instalare (implicită sau altele).

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține informații despre lista de identificatori utilizați de aplicație pentru înregistrarea serviciilor Microsoft Autoupdate și numărul de instalări înregistrate pentru aplicație.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="appregistry_remove"></a>appregistry_remove

Acest eveniment indică faptul că a avut loc o încercare de eliminare a unei aplicații din lista de aplicații gestionate de MAU. Vom utiliza acest eveniment pentru a confirma faptul că doar aplicațiile lansate de MAU sunt gestionate prin MAU (aici nu ar trebui să apară aplicații AppStore).

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - numele și identificatorul aplicației eliminate, dacă aplicația încă există în locația înregistrată și dacă aceasta a fost instalată din AppStore.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="catalog_errorsignature"></a>catalog_errorsignature

Acest eveniment indică faptul că s-a produs o eroare în timpul validării semnăturii codului pentru un fișier de actualizare colateral.  Orice verificare colaterală nereușită a semnăturii codului trebuie să fie considerată nevalidă.

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține numele fișierului catalog cu semnătura nevalidă. Textul static diferit descrie condiții de eroare diferite.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="cloningtask_helpertoolconnection"></a>cloningtask_helpertoolconnection

Acest eveniment înregistrează probleme cu instalarea pe clonă (de exemplu, dacă nu reușim să ne conectăm la ajutor pentru a aplica o actualizare sau ne conectăm, dar ajutorul nu poate aplica actualizarea). Dacă primim vreodată o înregistrare raportată, acest lucru înseamnă că instalarea pe clonă nu a reușit și acum va trebui să revenim la o actualizare locală.

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține un ID pentru identificarea unei activități de actualizare singulare și eroarea proxy raportată în timpul procesului de clonare.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="configuration_channel"></a>configuration_channel

Acest eveniment înregistrează încercările de comutare a canalelor (grup de public) în MAU.  Utilizăm acest lucru pentru a înregistra încercările și rezultatele acestora (succes sau eșec).

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține numele canalului selectat.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="configuration_metadata"></a>configuration_metadata

Acest eveniment este înregistrat de fiecare dată când se inițializează MAU. Acesta este un tip de eveniment MAU cu mesaje repetate

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text static care indică dacă se inițializează metadatele individuale sau configurația.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune.


### <a name="controller_alertmanager_reinstallresponse"></a>controller_alertmanager_reinstallresponse

Acest eveniment indică faptul că MAU a intrat într-o stare inutilizabilă/irecuperabilă și trebuie reinstalat. Acest eveniment indică o eroare irecuperabilă și necesitatea intervenției utilizatorilor.

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința verificării actualizărilor

- **Payload** - conține selecția enumerată de utilizator.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

    
### <a name="controller_alertmanager_tmpdiskfull"></a>controller_alertmanager_tmpdiskfull

Acest eveniment indică faptul că a fost detectat insuficient spațiu pe disc. Nu vom putea instala actualizări din cauza spațiului insuficient pe disc.

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text static. 

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="controller_alertmanager_tmpdiskfullretry"></a>controller_alertmanager_tmpdiskfullretry

Acest eveniment indică faptul că a fost inițiată o reîncercare de instalare a unei actualizări după detectarea spațiului insuficient pe disc. Încercăm din nou instalarea după ce nu am putut să instalăm actualizări din cauza spațiului insuficient pe disc.

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text static. 

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune
    

### <a name="controller_alertmanager_tmpdiskfullretrycancel"></a>controller_alertmanager_tmpdiskfullretrycancel

Acest eveniment indică faptul că a fost detectată o anulare a unei reîncercări de instalare după detectarea spațiului insuficient pe disc. Vom utiliza acest eveniment pentru a determina dacă mecanismul nostru de rezervă a fost suficient pentru a ghida utilizatorul prin procesul de actualizare atunci când s-a detectat insuficient spațiu pe disc.

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)
    
- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor
    
- **Payload** - text static. 

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

    
### <a name="controller_checkwindow_noupdatefoundok"></a>controller_checkwindow_noupdatefoundok

Acest eveniment indică faptul că în urma unei verificări a actualizărilor nu au fost găsite actualizări. Utilizăm acest eveniment pentru a ne asigura că actualizările sunt oferite corect, pentru a optimiza încărcarea serviciilor și pentru a defini frecvența de verificare a actualizărilor. De asemenea, dorim să optimizăm cadență noastră de lansare pe baza așteptărilor utilizatorilor față de actualizări.

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text static. 

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

    

### <a name="controller_checkwindow_updatecheck"></a>controller_checkwindow_updatecheck

Acest eveniment indică faptul că a fost efectuată o verificare a actualizărilor. Utilizăm acest eveniment pentru a ne asigura că actualizările sunt oferite corect, pentru a optimiza încărcarea serviciilor și pentru a defini frecvența de verificare a actualizărilor. De asemenea, dorim să optimizăm cadență noastră de lansare pe baza așteptărilor utilizatorilor față de actualizări.

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului
    
- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text static. 

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="controller_checkwindow_updatecheckcancel"></a>controller_checkwindow_updatecheckcancel

Acest eveniment indică faptul că procesul de verificare a actualizărilor a fost anulat (de către utilizator sau de către sistem). Utilizăm acest eveniment pentru a ne asigura că actualizările sunt oferite corect, pentru a optimiza încărcarea serviciilor și pentru a defini frecvența de verificare a actualizărilor. De asemenea, dorim să optimizăm cadență noastră de lansare pe baza așteptărilor utilizatorilor față de actualizări.

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text static. 

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

    
### <a name="controller_checkwindow_updatecheckcanceluser"></a>controller_checkwindow_updatecheckcanceluser

Acest eveniment indică faptul că procesul de verificare a actualizărilor a fost anulat de către utilizator.  Utilizăm acest eveniment pentru a ne asigura că actualizările sunt oferite corect, pentru a optimiza încărcarea serviciilor și pentru a defini frecvența de verificare a actualizărilor. De asemenea, dorim să optimizăm cadență noastră de lansare pe baza așteptărilor utilizatorilor față de actualizări.

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației
    
- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text static. 

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

    
### <a name="controller_checkwindow_updatesfound"></a>controller_checkwindow_updatesfound

Acest eveniment indică faptul că în urma procesului de verificare a actualizărilor nu au fost găsite actualizări.  Utilizăm acest eveniment pentru a ne asigura că actualizările sunt oferite corect.

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text static. 

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

    
### <a name="controller_checkwindow_uptodate"></a>controller_checkwindow_uptodate

Acest eveniment indică faptul că în urma procesului de verificare a actualizărilor nu au fost găsite actualizări din cauză că aplicațiile din dispozitiv sunt actualizate.  Utilizăm acest eveniment pentru a ne asigura că actualizările sunt oferite corect.

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text static. 

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="controller_downloadwindow_applaunchwithpendingupdate"></a>controller_downloadwindow_applaunchwithpendingupdate

Acest eveniment indică faptul că a fost lansată o aplicație care este în curs de instalare a actualizărilor. Utilizăm acest eveniment pentru a ne asigura că actualizările sunt oferite corect. Ar trebui să prevenim instalarea actualizărilor pentru aplicațiile deschise. Aplicațiile trebuie să fie închise înainte de actualizare.

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text static. 

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP
    
- **SessionId** - identificatorul pentru sesiune

    
### <a name="controller_downloadwindow_closeapplicationdialog"></a>controller_downloadwindow_closeapplicationdialog

Acest eveniment indică faptul că a fost lansată o aplicație care este în curs de instalare a actualizărilor. Utilizăm acest eveniment pentru a ne asigura că actualizările sunt oferite corect. Ar trebui să prevenim instalarea actualizărilor pentru aplicațiile deschise. Aplicațiile trebuie să fie închise înainte de actualizare.

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text static. 

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

    
### <a name="controller_downloadwindow_curtasknull"></a>controller_downloadwindow_curtasknull

Acest eveniment indică faptul că s-a produs o eroare neașteptată în timpul încercării de aplicare a unei actualizări. Utilizăm acest eveniment pentru a ne asigura că actualizările sunt oferite corect.

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text static. 

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

    
### <a name="controller_downloadwindow_downloadcancel"></a>controller_downloadwindow_downloadcancel

Acest eveniment indică faptul că procesul de descărcare a fost anulat de către utilizator.  Utilizăm acest eveniment pentru a ne asigura că actualizările sunt oferite corect.

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text static. 

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

    
### <a name="controller_downloadwindow_downloadfailed"></a>controller_downloadwindow_downloadfailed

Acest eveniment indică faptul că s-a produs o eroare în timpul descărcării unei actualizări. Utilizăm acest eveniment pentru a ne asigura că actualizările sunt oferite și descărcate corect.

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

    
### <a name="controller_downloadwindow_downloadfailedok"></a>controller_downloadwindow_downloadfailedok

Acest eveniment indică faptul că s-a produs o eroare în timpul descărcării unei actualizări și că utilizatorul a fost notificat. Utilizăm acest eveniment pentru a ne asigura că actualizările sunt oferite și descărcate corect și că, în cazul unei erori, utilizatorul va primi o notificare.

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="controller_downloadwindow_downloadpathmissing"></a>controller_downloadwindow_downloadpathmissing

Acest eveniment indică faptul că s-a produs o eroare în timpul descărcării unei actualizări. Utilizăm acest eveniment pentru a ne asigura că actualizările sunt oferite și descărcate corect. Acest eveniment indică faptul că lipsește un URL de descărcare.

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="controller_downloadwindow_downloadtasknull"></a>controller_downloadwindow_downloadtasknull

Acest eveniment indică faptul că s-a produs o eroare în timpul descărcării unei actualizări. Utilizăm acest eveniment pentru a ne asigura că actualizările sunt oferite și descărcate corect. Acest eveniment indică faptul că aplicația Microsoft Autoupdate a fost solicitată să întrerupă/reia o descărcare, dar nu a putut găsi managerul de descărcare corespunzător.

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="controller_downloadwindow_filesignaturenotverified"></a>controller_downloadwindow_filesignaturenotverified

Acest eveniment indică faptul că s-a produs o eroare în timpul descărcării unei actualizări. Acest eveniment indică faptul că Microsoft Autoupdate nu a reușit să verifice dacă această actualizare a fost publicată de Microsoft. Utilizăm acest eveniment pentru a ne asigura că actualizările sunt oferite și descărcate corect. 

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care conține URL-ul de descărcare. Aceasta este o locație de descărcare Microsoft, cu excepția cazului în care canalul este setat pe Particularizat. Pentru canalul particularizat, această valoare este setată pe „locație particularizată”.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="controller_downloadwindow_installcomplete"></a>controller_downloadwindow_installcomplete

Acest eveniment indică faptul că instalarea tuturor actualizărilor oferite de Microsoft Autoupdate a fost finalizată. Utilizăm acest eveniment pentru a ne asigura că actualizările sunt oferite și descărcate corect. 

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația
    
- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="controller_downloadwindow_networkunavailablealert"></a>controller_downloadwindow_networkunavailablealert

Acest eveniment indică faptul că conectivitatea la rețea a fost pierdută în timpul descărcării actualizărilor.  Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

    
### <a name="controller_downloadwindow_networkunavailablealertok"></a>controller_downloadwindow_networkunavailablealertok

Acest eveniment indică faptul că conectivitatea la rețea a fost pierdută în timpul descărcării actualizărilor. De asemenea, indică faptul că utilizatorul a fost notificat de această eroare. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

    
### <a name="controller_downloadwindow_noconnectionok"></a>controller_downloadwindow_noconnectionok

Acest eveniment indică faptul că conectivitatea la rețea a fost pierdută în timpul descărcării actualizărilor. De asemenea, indică faptul că utilizatorul a fost notificat de această eroare. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="controller_downloadwindow_repairrequired"></a>controller_downloadwindow_repairrequired

Acest eveniment indică faptul că procesul de actualizare nu a reușit. De asemenea, indică faptul că s-a finalizat o actualizare, însă Microsoft Autoupdate a găsit o problemă cu aplicația actualizată și este necesară repararea. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)
    
- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului
    
- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

### <a name="controller_downloadwindow_updateaborted"></a>controller_downloadwindow_updateaborted

Acest eveniment indică faptul că procesul de actualizare a fost anulat. De asemenea, indică faptul că o actualizare era deja în curs prin Daemon și că utilizatorul a făcut clic pe OK pentru a anula descărcarea. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="controller_downloadwindow_updatefailed"></a>controller_downloadwindow_updatefailed

Acest eveniment indică faptul că una sau mai multe actualizări din lotul actual nu au reușit. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.
    
- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="controller_downloadwindow_updatesuccessful"></a>controller_downloadwindow_updatesuccessful

Acest eveniment indică faptul că toate actualizările din lotul actual au fost efectuate cu succes. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="controller_downloadwindow_userpaused"></a>controller_downloadwindow_userpaused

Acest eveniment indică faptul că toate actualizările din lotul actual au fost efectuate cu succes. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="controller_downloadwindow_userresumed"></a>controller_downloadwindow_userresumed

Acest eveniment indică faptul că procesul de descărcare a actualizărilor a fost reluat cu succes după întrerupere. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul
    
- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="controller_mainwindow_setautomaticdownloadinstall"></a>controller_mainwindow_setautomaticdownloadinstall

Acest eveniment indică faptul că dispozitivul a fost înscris în modul de Actualizare automată. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

    
### <a name="controller_mainwindow_setmanualchecking"></a>controller_mainwindow_setmanualchecking

Acest eveniment indică faptul că dispozitivul a fost înscris în modul de Actualizare manuală. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

    
### <a name="controller_templateawindow_cancel"></a>controller_templateawindow_cancel

Acest eveniment indică faptul că utilizatorul a ales să anuleze sau să ignore un mesaj de avertizare furnizat. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

    
### <a name="controller_templateawindow_enroll"></a>controller_templateawindow_enroll

Acest eveniment indică faptul că utilizatorul a ales să urmeze o recomandare de avertizare furnizată. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor
    
- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune



### <a name="controller_templateawindow_install"></a>controller_templateawindow_install

Acest eveniment indică faptul că utilizatorul a ales să urmeze o recomandare de avertizare furnizată legată de inițierea unei acțiuni de instalare de software. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="controller_updatewindow_begindownloadingapps"></a>controller_updatewindow_begindownloadingapps

Acest eveniment indică faptul că descărcarea actualizărilor a fost începută prin fereastra Actualizare. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține un dicționar cu pachete de actualizări disponibile și o indicație care afișează dacă utilizatorul a selectat instalarea acelei intrări.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

    
### <a name="controller_updatewindow_networkretry"></a>controller_updatewindow_networkretry

Acest eveniment indică faptul că a fost declanșată o reîncercare în Foaia de actualizări din cauza unei erori de rețea. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

    
### <a name="controller_updatewindow_networkretrycancel"></a>controller_updatewindow_networkretrycancel

Acest eveniment indică faptul că nu a putut fi declanșată o reîncercare în Foaia de actualizări din cauza unei erori de rețea. Acest eveniment indică faptul că utilizatorul a ales să anuleze actualizările după ce a fost alertat că rețeaua va fi indisponibilă. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="controller_updatewindow_networkunavailable"></a>controller_updatewindow_networkunavailable

Acest eveniment indică faptul că conectivitatea la rețea a fost pierdută brusc. Acest eveniment indică faptul că serverul nu este accesibil atunci când se încearcă descărcarea unui pachet de actualizare. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="controller_updatewindow_noupdateavailable"></a>controller_updatewindow_noupdateavailable

Acest eveniment indică faptul că a existat o căutare de actualizări în urma căreia nu a fost găsită nicio actualizare disponibilă. Acest eveniment indică faptul că nu s-au găsit actualizări disponibile de către Microsoft Autoupdate. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="controller_updatewindow_noupdatestoselect"></a>controller_updatewindow_noupdatestoselect

Acest eveniment indică faptul că s-a produs o eroare, rezultând o listă de actualizări necompletată. Acest eveniment indică faptul că Microsoft Autoupdate afișează o foaie de actualizări necompletată. Acest lucru nu ar trebui să se întâmple. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="controller_updatewindow_updateavailable"></a>Controller_UpdateWindow_UpdateAvailable

Acest eveniment indică faptul că a existat o căutare de actualizări în urma căreia au fost găsite actualizări. Utilizăm acest eveniment pentru a determina dacă actualizările sunt oferite pentru a fi vizualizate de către utilizator, dacă sunt afișate actualizările corespunzătoare sau dacă blocarea actualizărilor funcționează în mod corect. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține un dicționar cu pachete de actualizări disponibile și starea selecției utilizatorului pentru fiecare.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

    
### <a name="controller_updatewindow_updateavailablecancel"></a>controller_updatewindow_updateavailablecancel

Acest eveniment indică faptul că un utilizator a anulat actualizarea după ce am afișat foaia de actualizări cu actualizările. Utilizăm acest eveniment pentru a explica motivele pentru care nu se realizează actualizarea (adică, utilizatorul anulează de bună voie). Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="downloadactor_pause"></a>downloadactor_pause

Acest eveniment indică faptul că utilizatorul a emis o solicitare de întrerupere a descărcării. Utilizăm acest eveniment pentru a explica motivele pentru care actualizările par că nu sunt finalizate. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="downloadactor_redirect"></a>downloadactor_redirect

Acest eveniment indică faptul că agentul de descărcare este îndreptat către un punct final care emite o redirecționare URL pentru solicitarea de descărcare. Utilizăm acest eveniment pentru a explica motivele erorilor de descărcare și diagnosticarea problemelor proxy. De asemenea, ne poate ajuta la diagnosticarea motivelor pentru care se observă că utilizatorii instalează compilări mai vechi. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține URL-ul redirecționat. Aceasta este locația de descărcare Microsoft, cu excepția cazului în care canalul este setat pe Particularizat. Pentru canalul particularizat, această valoare este setată pe „locație particularizată”.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

    
### <a name="downloadactor_resume"></a>downloadactor_resume

Acest eveniment indică faptul că utilizatorul a emis o solicitare de reluare a unei descărcări întrerupte. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="downloadactor_resumeerror"></a>downloadactor_resumeerror

Acest eveniment indică faptul că utilizatorul a emis o solicitare de reluare a unei descărcări întrerupte. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține calea URL de descărcare. Aceasta este locația de descărcare Microsoft, cu excepția cazului în care canalul este setat pe Particularizat. Pentru canalul particularizat, această valoare este setată pe „locație particularizată”.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

    
### <a name="downloadactor_status"></a>downloadactor_status

Acest eveniment înregistrează faptul că există încercări de preluare a fișierelor colaterale și rezultatul acestora (succes sau eșec). Dorim să știm care sunt fișierele colaterale și pachetele preluate. Un fișier incorect preluat poate indica o problemă de compilare/colaterală. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține URL-ul de descărcare și un cod de eroare, în cazul unei erori. URL-ul de descărcare este locația de descărcare Microsoft, cu excepția cazului în care canalul este setat pe Particularizat. Pentru canalul particularizat, această valoare este setată pe „locație particularizată”.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="downloadmanifest_downloadcatalogfail"></a>downloadmanifest_downloadcatalogfail

Acest eveniment indică faptul că a avut loc o eroare de descărcare. Fișierul care nu s-a descărcat este înregistrat. Dorim să știm care sunt fișierele colaterale și pachetele preluate. O eroare de descărcare a unui manifest poate indica o eroare de generare colaterală a compilării, o eroare de configurare CDN, o eroare de configurare a clientului, o eroare de rețea. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține codul de eroare de descărcare și un URL pentru fișierul descărcat. Aceasta este locația de descărcare Microsoft, cu excepția cazului în care canalul este setat pe Particularizat. Pentru canalul particularizat, această valoare este setată pe „locație particularizată”.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

    
### <a name="downloadmanifest_downloadcatalogsuccess"></a>downloadmanifest_downloadcatalogsuccess

Acest eveniment indică faptul că un fișier a fost descărcat cu succes. O eroare de descărcare a unui manifest poate indica o eroare de generare colaterală a compilării, o eroare de configurare CDN, o eroare de configurare a clientului, o eroare de rețea. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul
    
- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține codul de eroare de descărcare și un URL pentru fișierul descărcat. Aceasta este locația de descărcare Microsoft, cu excepția cazului în care canalul este setat pe Particularizat. Pentru canalul particularizat, această valoare este setată pe „locație particularizată”.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="downloadmanifest_downloadfail"></a>downloadmanifest_downloadfail

Acest eveniment indică faptul că s-a produs o eroare de descărcare. Fișierul cu manifestul sau pachetul care nu a reușit să fie descărcat, precum și detaliile erorii, sunt înregistrate. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține codul de eroare de descărcare și un URL pentru fișierul descărcat. Aceasta este locația de descărcare Microsoft, cu excepția cazului în care canalul este setat pe Particularizat. Pentru canalul particularizat, această valoare este setată pe „locație particularizată”.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="downloadmanifest_downloadfromurl"></a>downloadmanifest_downloadfromurl

Acest eveniment indică faptul că a început descărcarea unui fișier catalog. Înregistrăm adresa URL de la care se descarcă fișierul catalog. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține codul de eroare de descărcare și un URL pentru fișierul descărcat. Aceasta este locația de descărcare Microsoft, cu excepția cazului în care canalul este setat pe Particularizat. Pentru canalul particularizat, această valoare este setată pe „locație particularizată”.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="downloadmanifest_downloading"></a>downloadmanifest_downloading

Acest eveniment indică faptul că a început descărcarea unui fișier catalog. Înregistrăm adresa URL de la care se descarcă fișierul catalog. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține codul de eroare de descărcare și un URL pentru fișierul descărcat. Aceasta este locația de descărcare Microsoft, cu excepția cazului în care canalul este setat pe Particularizat. Pentru canalul particularizat, această valoare este setată pe „locație particularizată”.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="downloadmanifest_downloadsuccess"></a>downloadmanifest_downloadsuccess

Acest eveniment indică faptul că descărcarea unui fișier XML și de pachet a reușit. Înregistrăm adresa URL de la care se descarcă fișierul. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține codul de eroare de descărcare și un URL pentru fișierul descărcat. Aceasta este locația de descărcare Microsoft, cu excepția cazului în care canalul este setat pe Particularizat. Pentru canalul particularizat, această valoare este setată pe „locație particularizată”.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

    
### <a name="downloadmanifest_downloadurl"></a>downloadmanifest_downloadurl

Acest eveniment indică faptul că s-a produs o solicitare de descărcare a unui fișier. Înregistrăm adresa URL de la care se descarcă fișierul. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul
    
- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține codul de eroare de descărcare și un URL pentru fișierul descărcat. Aceasta este locația de descărcare Microsoft, cu excepția cazului în care canalul este setat pe Particularizat. Pentru canalul particularizat, această valoare este setată pe „locație particularizată”.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="downloadmanifest_filenameerror"></a>downloadmanifest_filenameerror

Acest eveniment indică faptul că s-a produs o eroare neașteptată. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="downloadmanifest_invalidhash"></a>downloadmanifest_invalidhash

Acest eveniment indică faptul că validarea securității fișierelor noastre nu a reușit. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține numele fișierului de descărcare cu valoarea hash nevalidă.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="downloadmanifest_missingdaemon"></a>downloadmanifest_missingdaemon

Acest eveniment indică faptul că un utilizator a încercat să caute actualizări și am descoperit că aplicației MAU îi lipsește o componentă de bază (Daemon). Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="downloadmanifest_signatureerror"></a>downloadmanifest_signatureerror

Acest eveniment indică faptul că verificarea semnăturii codului nu a reușit pentru un pachet. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține un nume al fișierului de descărcare cu valoarea hash nevalidă.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="downloadmanifest_status"></a>downloadmanifest_status

Acest eveniment înregistrează o agregare rezumativă a încercărilor/eșecurilor din timpul procesului de descărcare pentru fișiere manifest și pachet. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține informații care includ adresa URL (adresa Microsoft), prefixul fișierului care este descărcat, orice erori întâmpinate, etc.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="downloadmgr_downloadend"></a>downloadmgr_downloadend

Acest eveniment înregistrează un marcator care indică procesul de descărcare finalizat pe cont propriu. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține informații care includ adresa URL (adresa Microsoft), prefixul fișierului care este descărcat, orice erori întâmpinate, etc.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="downloadmgr_downloadstart"></a>downloadmgr_downloadstart

Acest eveniment înregistrează actualizarea care urmează să fie descărcată. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține numele actualizării care este descărcată.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="downloadtask_downloadfailure"></a>downloadtask_downloadfailure

Acest eveniment înregistrează faptul că s-a produs o eroare la descărcarea unui fișier pachet. Înregistrăm calea actualizării și eroarea. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține numele actualizării care este descărcată și eroarea observată.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="downloadtask_downloadsuccess"></a>downloadtask_downloadsuccess

Descărcarea cu succes a unui fișier pachet. Înregistrăm calea actualizării utilizate. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține calea actualizării pentru descărcarea cu succes.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="fba_checkforupdate"></a>fba_checkforupdate

Acest eveniment indică faptul că un proces de fundal caută actualizări. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="fba_checkforupdateskip"></a>fba_checkforupdateskip

Acest eveniment indică faptul că un proces de fundal a ignorat actualizarea din cauza faptului că MAU GUI este deschis. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="fba_launchstatus"></a>fba_launchstatus

Acest eveniment înregistrează erorile Daemon ale MAU în timpul încercării de lansare. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține OSStatus (codul de stare Apple) care reflectă starea lansării.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="fba_silentupdateoptin"></a>fba_silentupdateoptin

Acest eveniment indică faptul că utilizatorul optează pentru actualizările silențioase. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="fba_skipforcedupdate"></a>fba_skipforcedupdate

Acest eveniment indică faptul că verificatorul de actualizări forțate este ignorat din cauza aplicațiilor deschise. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="fba_startforcedupdate"></a>fba_startforcedupdate

Acest eveniment indică faptul că s-a produs o încercare de aplicare a unei actualizări forțate. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="fba_terminate"></a>fba_terminate

Acest eveniment indică faptul că Daemon MAU s-a oprit normal. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="fba_updatefound"></a>fba_updatefound

Acest eveniment indică faptul că Daemon MAU a găsit actualizări disponibile oferite. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține numărul de actualizări disponibile găsite.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

    
### <a name="fba_updatetimer"></a>fba_updatetimer

Acest eveniment indică faptul că procesul Daemon Microsoft Autoupdate a devenit activ pentru a căuta actualizări după ce a fost inactiv pentru o perioadă de timp setată. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține informațiile actuale de spre dată și oră.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="fbasilentupdate_allappsclosed"></a>fbasilentupdate_allappsclosed

Acest eveniment înregistrează dacă toate aplicațiile au fost închise înaintea unei instalări. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public
    
- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="fbasilentupdate_applaunchafterupdate"></a>fbasilentupdate_applaunchafterupdate

Acest eveniment înregistrează o încercare de a relansa aplicația după o actualizare silențioasă și modul de actualizare (clonă sau nu). Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține un identificator utilizat pentru urmărirea unei activități de actualizare și numele aplicației care urmează să fie lansată.
    
- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)
    
- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="fbasilentupdate_applaunchwileinstalling"></a>fbasilentupdate_applaunchwileinstalling

Înregistrăm când s-a efectuat o lansare de aplicație în timpul instalării unei actualizări. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține un identificator utilizat pentru urmărirea unei activități de actualizare.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="fbasilentupdate_appneedtoclose"></a>fbasilentupdate_appneedtoclose

Înregistrăm când s-a lansat un proces de actualizare și descoperim că aplicația care trebuie actualizată a fost deschisă. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține un identificator utilizat pentru urmărirea unei activități de actualizare, numele unei actualizări și ID-ul pachetului aplicației.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="fbasilentupdate_appterminationeventreceived"></a>fbasilentupdate_appterminationeventreceived

Acest eveniment indică faptul că Microsoft Autoupdate a primit un eveniment Apple care informează că aplicația a fost oprită. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține un identificator utilizat pentru urmărirea unei activități de actualizare și ID-ul pachetului aplicației. Acesta poate conține și un șir de erori dacă Microsoft Autoupdate determină că aplicația încă rulează, chiar dacă a fost primit un eveniment de oprire.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="fbasilentupdate_codesignfailure"></a>fbasilentupdate_codesignfailure

Acest eveniment înregistrează rezultatul verificării semnăturii codului după aplicarea unei actualizări. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține rezultatul operațiunii de verificare a semnăturii codului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="fbasilentupdate_download"></a>fbasilentupdate_download

Acest eveniment indică faptul că se descarcă o actualizare. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține un identificator utilizat pentru urmărirea unei activități de actualizare și numele unei actualizări.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="fbasilentupdate_downloadfailed"></a>fbasilentupdate_downloadfailed

Acest eveniment indică faptul că s-a produs o eroare în timpul descărcării unei actualizări. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține un identificator utilizat pentru urmărirea unei activități de actualizare și numele unei actualizări.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="fbasilentupdate_downloadinbackground"></a>fbasilentupdate_downloadinbackground

Acest eveniment indică faptul că începem descărcarea unui set de actualizări pe fundal (înregistrăm numărul de actualizări descărcate concomitent). Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține numărul de actualizări puse în așteptare.

    - **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="fbasilentupdate_downloadingrepairupdate"></a>fbasilentupdate_downloadingrepairupdate

Acest eveniment indică faptul că am inițiat o încercare de descărcare a unui fișier de reparare pentru o actualizare eșuată. Înregistrăm versiunea și actualizarea. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține un identificator utilizat pentru urmărirea unei activități de actualizare și numele unei actualizări.
    
- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="fbasilentupdate_duplicatedownloadattempted"></a>fbasilentupdate_duplicatedownloadattempted

Acest eveniment indică faptul că s-a produs o eroare. Ar trebui să descărcăm pe rând fiecare actualizare pentru o anumită aplicație. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="fbasilentupdate_installattemptfailed"></a>fbasilentupdate_installattemptfailed

Acest eveniment indică faptul că o încercare de instalare a unei actualizări (versiuni) nu a reușit. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="fbasilentupdate_installcomplete"></a>fbasilentupdate_installcomplete

Acest eveniment indică faptul că toate actualizările din grup au fost instalate. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="fbasilentupdate_installed"></a>fbasilentupdate_installed

Acest eveniment indică faptul că o actualizare individuală a fost instalată cu succes. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului. Conține identificatorul actualizării.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

    
### <a name="fbasilentupdate_installing"></a>fbasilentupdate_installing

Acest eveniment indică faptul că a fost inițiată o actualizare individuală. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține un identificator utilizat pentru urmărirea unei activități de actualizare, numele unei actualizări și numele pachetului de actualizare.
    
- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="fbasilentupdate_notificationremoved"></a>fbasilentupdate_notificationremoved

Acest eveniment indică faptul că o actualizare care a fost blocată nu mai este blocată. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține un ID de aplicație (identificatorul aplicației utilizat pentru înregistrarea în serviciul Microsoft Autoupdate) pentru aplicația blocată anterior
    
- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="fbasilentupdate_queueinstall"></a>fbasilentupdate_queueinstall

Acest eveniment indică faptul că o actualizare va fi pusă în coada de așteptare pentru instalarea silențioasă. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține un identificator utilizat pentru urmărirea unei activități de actualizare și numele actualizării.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="fbasilentupdate_requiredappsclosed"></a>fbasilentupdate_requiredappsclosed

Înregistrăm când o aplicație care are o actualizare în așteptare a fost închisă. Acest lucru indică momentul în care se poate continua instalarea propriu-zisă. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține un identificator utilizat pentru urmărirea unei activități de actualizare și ID-ul pachetului aplicației.
    
- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="fbasilentupdate_updateavailablenotification"></a>fbasilentupdate_updateavailablenotification

Acest eveniment indică faptul că este declanșată o notificare de actualizare disponibilă. Trebuie să ne asigurăm că fluxul de solicitare a actualizărilor se declanșează atunci când este detectată o actualizare. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="fbasilentupdate_userclicknotification"></a>fbasilentupdate_userclicknotification

Acest eveniment indică faptul că utilizatorul a făcut clic pe secțiunea de conținut a notificării de actualizare disponibilă și aplicația Microsoft Autoupdate GUI este lansată. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="fbasilentupdate_userselectinstalllater"></a>fbasilentupdate_userselectinstalllater

Acest eveniment indică faptul că utilizatorul a optat pentru instalarea ulterioară după ce a fost afișată notificarea de actualizare disponibilă. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="fbasilentupdate_userselectinstallnow"></a>fbasilentupdate_userselectinstallnow

Acest eveniment indică faptul că utilizatorul a optat pentru instalarea în momentul de față după ce a fost afișată notificarea de actualizare disponibilă. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="installdata_checkrunning"></a>installdata_checkrunning

Acest eveniment înregistrează rezultatul unei verificări între aplicațiile care vor fi instalate și dacă încercarea de instalare va continua în funcție de aplicația care este deschisă. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

    
### <a name="installdata_cleanup"></a>installdata_cleanup

Fișierele pachet trebuie eliminate după instalare. Acest eveniment înregistrează instanțele în care nu reușim să le eliminăm. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține numele fișierului descărcat și detaliile erorii.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="installedapp_invalidbundle"></a>installedapp_invalidbundle

Acest eveniment indică faptul că Microsoft Autoupdate nu a putut recupera informațiile despre pachet pentru aplicația înregistrată în calea dată. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține numele aplicației.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

    
### <a name="installedapp_invalidpreference"></a>installedapp_invalidpreference

Acest eveniment înregistrează cazurile în care preferința utilizatorului conține o intrare de aplicație nevalidă. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința verificării actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

    
### <a name="installedapp_nilbundleid"></a>installedapp_nilbundleid

Acest eveniment înregistrează cazurile în care ID-ul pachetului lipsește pentru o aplicație. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține numele aplicației.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="installedapp_nilbundlename"></a>installedapp_nilbundlename

Acest eveniment înregistrează cazurile în care numele pachetului lipsește pentru o aplicație. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține numele aplicației.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

    
### <a name="installstatus_codesign"></a>installstatus_codesign

Acest eveniment înregistrează starea binară a semnăturii codului pentru sistemul de operare. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul
    
- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="installstatus_daemon"></a>installstatus_daemon

Acest eveniment înregistrează starea aplicației Daemon Microsoft Autoupdate. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține o indicație privind existența componentei Daemon în locația așteptată și dacă codul acesteia este semnat.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="installstatus_helper"></a>installstatus_helper

Acest eveniment înregistrează starea instrumentului de asistență al aplicației Daemon Microsoft Autoupdate. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține o indicație privind existența componentei PrivilegedHelperTool în locația așteptată și dacă codul acesteia este semnat.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

    
### <a name="installupdatestask_applaunched"></a>installupdatestask_applaunched

Acest eveniment indică faptul că Microsoft Autoupdate a detectat aplicația lansare pentru o actualizare blocată, dar nu a putut găsi programul de instalare potrivit. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține numele aplicației lansate.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

    
### <a name="installupdatestask_applaunchwithpendingupdate"></a>installupdatestask_applaunchwithpendingupdate

Acest eveniment indică faptul că Microsoft Autoupdate a detectat aplicația lansare pentru o aplicație cu o actualizare în așteptare. Aplicația lansată va fi oprită. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

    
### <a name="installupdatestask_codesignverificationfail"></a>installupdatestask_codesignverificationfail

Acest eveniment indică faptul că verificarea CodeSign nu a reușit pentru o actualizare de aplicație. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține un identificator utilizat pentru urmărirea unei activități de actualizare, numele aplicației actualizate și codul de eroare.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="installupdatestask_codesignverificationstart"></a>installupdatestask_codesignverificationstart

Acest eveniment indică faptul că verificarea CodeSign a început pentru o actualizare de aplicație. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține un identificator utilizat pentru urmărirea unei activități de actualizare și numele aplicației actualizate.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="installupdatestask_codesignverificationsuccess"></a>installupdatestask_codesignverificationsuccess

Acest eveniment indică faptul că verificarea CodeSign a reușit pentru o actualizare de aplicație. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține un identificator utilizat pentru urmărirea unei activități de actualizare și numele aplicației actualizate.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="installupdatestask_failsilentinstall"></a>installupdatestask_failsilentinstall

Acest eveniment înregistrează erorile din timpul aplicării actualizărilor silențioase și dacă aceasta a fost o instalare clonată sau obișnuită. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 
    
- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține un identificator utilizat pentru urmărirea unei activități de actualizare și tipul actualizării.
    
- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

    
### <a name="installupdatestask_multiplerelocatablepackage"></a>installupdatestask_multiplerelocatablepackage

Acest eveniment indică faptul că Microsoft Autoupdate a găsit mai multe instanțe de intrare de aplicație pentru un pachet de actualizare dat din manifestul descărcat. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține un identificator utilizat pentru urmărirea unei activități de actualizare și numele actualizării

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

    
### <a name="installupdatestask_removeclone"></a>installupdatestask_removeclone

Acest eveniment indică faptul că o clonă a fost eliminată. Eliminăm o clonă când procesul de Instalare pe clonă s-a finalizat sau atunci când începe un proces nou și pe computer se găsește o versiune mai veche clonată. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține un identificator utilizat pentru urmărirea unei activități de actualizare, numele pachetului de actualizare, starea eliminării clonei/detaliile erorii.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="installupdatestask_retryfail"></a>installupdatestask_retryfail

Acest eveniment indică faptul că au fost întâmpinate erori în timpul procesului de reîncercare a instalării. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține un identificator utilizat pentru urmărirea unei activități de actualizare, numele actualizării și dacă instalarea trebuie realizată prin Instalarea pe clonă

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="installupdatestask_retryproxyerror"></a>installupdatestask_retryproxyerror

Acest eveniment înregistrează erorile de comunicare din proces (comunicarea cu instrumentul de asistență MAU). Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține un identificator utilizat pentru urmărirea unei activități de actualizare, numele actualizării și detaliile despre eroarea proxy raportată.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

    
### <a name="installupdatestask_retryproxyerror"></a>installupdatestask_retryproxyerror

Acest eveniment înregistrează erorile de comunicare din proces (comunicarea cu instrumentul de asistență MAU). Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține un identificator utilizat pentru urmărirea unei activități de actualizare, numele actualizării și detaliile despre eroarea proxy raportată.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

    

### <a name="installupdatestask_retryresponse"></a>installupdatestask_retryresponse

Acest eveniment înregistrează faptul că o reîncercare nu a funcționat. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține un identificator utilizat pentru urmărirea unei activități de actualizare, numele actualizării, versiunea aplicației, numele pachetului de actualizare și indică dacă Instalarea pe clonă a fost activată, dacă instalarea a avut succes și dacă au fost raportate erori în cazul în care instalarea nu a reușit.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="installupdatestask_retrysuccess"></a>installupdatestask_retrysuccess

Acest eveniment înregistrează o instalare de actualizare reușită după o reîncercare. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține un identificator utilizat pentru urmărirea unei activități de actualizare, numele actualizării, versiunea aplicației, numele pachetului de actualizare și indică dacă Instalarea pe clonă a fost activată.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="installupdatestask_setreopengui"></a>installupdatestask_setreopengui

Acest eveniment indică dacă setarea preferinței de redeschidere a interfeței GUI după instalare a reușit. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică succesul operațiunii.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="msupdate_cli_eventhandler_applyupdates_appids"></a>msupdate_cli_eventhandler_applyupdates_appids

Acest eveniment indică faptul că a fost emisă o comandă CLI (interfață client-linie) pentru aplicarea unei actualizări. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține lista cu ID-urile aplicației care trebuie actualizate.
    
- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="msupdate_cli_eventhandler_config"></a>msupdate_cli_eventhandler_config

Acest eveniment indică faptul că modulul de interfață pentru linia de comandă Microsoft Autoupdate a primit un eveniment Apple pentru configurare. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="msupdate_cli_eventhandler_updates"></a>msupdate_cli_eventhandler_updates

Acest eveniment indică faptul că modulul de interfață pentru linia de comandă Microsoft Autoupdate a primit un eveniment Apple pentru afișarea de actualizări. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

    
### <a name="msupdate_monitor_progress_downloaded"></a>msupdate_monitor_progress_downloaded

Acest eveniment indică faptul că s-au descărcat actualizări. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține listele cu actualizările descărcate

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="msupdate_monitor_progress_failure"></a>msupdate_monitor_progress_failure

Acest eveniment înregistrează o listă de actualizări în așteptare care nu au reușit să fie aplicate. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține listele cu actualizări.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

    
### <a name="msupdate_monitor_progress_finished"></a>msupdate_monitor_progress_finished

Acest eveniment înregistrează o listă de actualizări în așteptare care au fost instalate. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține listele cu actualizări.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="msupdate_monitor_progress_queued"></a>msupdate_monitor_progress_queued

Acest eveniment înregistrează o listă de actualizări în așteptare. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține listele cu actualizări.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="optinnotificationaction"></a>Optinnotificationaction

Acest eveniment înregistrează răspunsul utilizatorului la caseta de dialog de optare pentru înscrierea în actualizări silențioase. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține text static ce reprezintă alegerea utilizatorului legată de optarea pentru Descărcarea și instalarea automată.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="sauupdateinfoprovider"></a>sauupdateinfoprovider

Acest eveniment înregistrează fiecare moment în care o cheie de manifest lipsește dintr-un fișier colateral. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține șirul utilizat pentru căutarea locației sau dimensiunii actualizării.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="updatecore_appregistration"></a>updatecore_appregistration

Acest eveniment înregistrează încercările de înregistrare a unei aplicații și rezultatul/motivul. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține un identificator utilizat pentru urmărirea unei activități de actualizare, indică dacă preferința este disponibilă, dacă aceasta este o reînregistrare și dacă înregistrarea este necesară.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="updatecore_loadinglaunchagent"></a>updatecore_loadinglaunchagent

Acest eveniment indică faptul că Agentul de lansare este încărcat. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="updatecore_server_connectionfail"></a>updatecore_server_connectionfail

Acest eveniment înregistrează erorile întâmpinate în timp ce contactați CDN. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține informații despre numele serverului, care server este disponibil și dacă serverul poate fi contactat.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="updatefilterhelper_cannotretrievebuilddate"></a>updatefilterhelper_cannotretrievebuilddate

Putem filtra actualizările prin serviciul MAU doar când actualizarea oferită nu este mai veche decât un anumit număr zile. Aici înregistrăm faptul că nu am putut recupera datele din metadatele aplicației. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține ID-ul aplicației.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="updatefilterhelper_invalidresponsefromupdatefiltering"></a>updatefilterhelper_invalidresponsefromupdatefiltering

Putem filtra actualizările prin serviciul MAU doar când actualizarea oferită nu este mai veche decât un anumit număr zile. Aici înregistrăm faptul că data lipsește din metadatele aplicației. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 
    
- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține ID-ul aplicației.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="updatefilterhelper_missingbuilddate"></a>updatefilterhelper_missingbuilddate

Putem filtra actualizările prin serviciul MAU doar când actualizarea oferită nu este mai veche decât un anumit număr zile. Aici înregistrăm faptul că data lipsește din metadatele aplicației. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține ID-ul aplicației.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="updatefilterhelper_updatebypassedoldage"></a>updatefilterhelper_updatebypassedoldage

Putem filtra actualizările prin serviciul MAU doar când actualizarea oferită nu este mai veche decât un anumit număr zile. Aici înregistrăm faptul că serviciul este ignorat din cauza datei de actualizare vechi. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține ID-ul aplicației.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="updatefinder_check_start"></a>updatefinder_check_start

Acest eveniment înregistrează fiecare moment în care inițiem o operațiune de verificare a actualizărilor. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul
    
- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține informații despre actualizările oferite, aplicațiile înregistrate și locația temporară în care vor fi salvate fișierele descărcate.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="updatefinder_check_status"></a>updatefinder_check_status

Acest eveniment colectează starea operațiunilor de verificare a actualizărilor (pâlnia de la căutare până la descărcare). Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține informații despre actualizările oferite, aplicațiile înregistrate și locația temporară în care vor fi salvate fișierele descărcate.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="updatefinder_check_updatefound"></a>updatefinder_check_updatefound

Înregistrăm fiecare moment în care în cadrul unei verificări a actualizărilor nu sunt găsite actualizări. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="updatefinder_check_updatenotfound"></a>updatefinder_check_updatenotfound

Înregistrăm fiecare moment în care în cadrul unei verificări a actualizărilor nu este oferită nicio actualizare din cauză că nu a fost găsită nicio actualizare. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="updatefinder_check_uptodate"></a>updatefinder_check_uptodate

Înregistrăm fiecare moment în care în cadrul unei verificări a actualizărilor nu este oferită nicio actualizare din cauză că toate aplicațiile sunt deja actualizate. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="updatefinder_offerupdates_minoscheckfail"></a>updatefinder_offerupdates_minoscheckfail

Înregistrăm fiecare moment în care am blocat o actualizare din cauză că aceasta nu a îndeplinit cerințele sistemului de operare. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține versiunea minimă necesară a sistemului de operare, specificată în manifestul descărcat.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="updatefinder_offerupdates_nullbundleforappid"></a>updatefinder_offerupdates_nullbundleforappid

Acest eveniment indică faptul că Microsoft Autoupdate nu a putut încărca informațiile despre pachet pentru ID-ul de aplicație specificat în fișierul manifest descărcat. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține ID-ul aplicației.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="updatefinder_offerupdates_updaterulematched"></a>updatefinder_offerupdates_updaterulematched

Acest eveniment indică faptul că a fost găsită o actualizare pentru o aplicație și o linie de bază. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține ID-ul aplicației și informații despre versiunea pachetului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

    
### <a name="updatefinder_registeredapps"></a>updatefinder_registeredapps

Înregistrăm aplicațiile instalate/înregistrate/controlate de MAU. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține ID-ul aplicației și informații despre versiunea pachetului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

    
### <a name="updatefinder_suite_missingcollateral"></a>updatefinder_suite_missingcollateral

Suite Update - înregistrăm fiecare moment în care o actualizare a suitei nu este aplicabilă din cauza lipsei fișierului colateral. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="updatefinder_suite_staleversion"></a>updatefinder_suite_staleversion

Suite Update - înregistrăm fiecare moment în care o actualizare a suitei nu este aplicabilă din cauză că versiunea de bază este prea veche. Înregistrăm versiunea de bază și suita AppId. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține numele suitei.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="updatefinder_suite_updateapplicable"></a>updatefinder_suite_updateapplicable

Suite Update - înregistrăm fiecare moment în care o actualizare a suitei este aplicabilă. Înregistrăm versiunea de bază și suita AppId. Înregistrăm versiunea de bază și suita AppId. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține numele, linia de bază și versiunea actualizării suitei.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="updatefinder_suite_updatenotapplicabledefaultpath"></a>updatefinder_suite_updatenotapplicabledefaultpath

Suite Update - înregistrăm fiecare moment în care o actualizare a suitei nu este oferită din cauză că nu toate aplicațiile suitei sunt instalate în calea implicită. Înregistrăm versiunea de bază și suita AppId. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține numele, linia de bază și versiunea actualizării suitei.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

    
### <a name="updatefinder_suite_updatenotapplicableversion"></a>updatefinder_suite_updatenotapplicableversion

Suite Update - înregistrăm fiecare moment în care o actualizare a suitei nu este oferită din cauză că nu toate aplicațiile suitei au aceeași versiune de bază. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține numele, linia de bază și versiunea actualizării suitei.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="updatefinder_suite_updatenotoffered"></a>updatefinder_suite_updatenotoffered

Suite Update - înregistrăm fiecare moment în care o actualizare a suitei nu este oferită din cauză că dimensiunea suitei este mai mare decât actualizările individuale. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține numele suitei.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="updatefinder_suite_updateoffered"></a>updatefinder_suite_updateoffered

Suite Update - înregistrăm fiecare moment în care este oferită o actualizare a suitei. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține numele, linia de bază și versiunea actualizării suitei.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="updatemanager_checkupdate"></a>updatemanager_checkupdate

Acest eveniment înregistrează numărul de actualizări găsite de Microsoft Autoupdate în timpul căutării de actualizări disponibile. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține numărul de actualizări disponibile găsite.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

    
### <a name="updatemanager_updatespending"></a>updatemanager_updatespending

Acest eveniment indică faptul că s-au găsit actualizări și instalarea este în așteptare. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - indică dacă activitatea rulează pe firul principal și numărul de actualizări în așteptare.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

    
### <a name="webservices_checkforsilentupdates"></a>webservices_checkforsilentupdates

Acest eveniment indică faptul că au fost găsiți candidați pentru actualizarea silențioasă. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține numărul de actualizări găsite și ID-ul aplicației.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="webservices_deltaupdater"></a>webservices_deltaupdater

Acest eveniment înregistrează interacțiunile dintre codul clientului și poarta de caracteristică care verifică dacă clientul ar trebui să permită actualizări Delta. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține răspunsul de la serviciile web și tipul de instrument de actualizare care trebuie aplicat.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="webservices_serviceaction"></a>webservices_serviceaction

Înregistrăm orice erori rezultate dintr-un răspuns webservice neașteptat. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține detaliile acțiunii realizate de serviciile web.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="webservices_serviceaction"></a>webservices_serviceaction

Înregistrăm orice erori rezultate dintr-un răspuns webservice neașteptat. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține detaliile acțiunii realizate de serviciile web.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="webservices_serviceresponse"></a>webservices_serviceresponse

Acest eveniment înregistrează solicitările către serviciul MAU, timpii de răspuns și erorile. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține ID-ul solicitării, numele aplicației, tipul de răspuns și/sau codul de stare.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

    
### <a name="webservices_silentupdate"></a>webservices_silentupdate

Înregistrăm solicitările de verificare a regulilor de aplicabilitate a „actualizării forțate”, adică, trebuie să mutăm un utilizator din compilarea N în compilarea N+1 din cauza unei probleme majore. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține ID-ul solicitării, numele aplicației, tipul de răspuns și/sau codul de stare.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune



### <a name="webservices_webcontent"></a>webservices_webcontent

Înregistrăm solicitările și răspunsurile primite prin webservices. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține ID-ul apelantului la serviciul web

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

## <a name="onenote-sync-events"></a>Evenimente de sincronizare OneNote

### <a name="officeonenotestoragenotebooksyncresult"></a>Office.OneNote.Storage.NotebookSyncResult
 
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

### <a name="officeonenotestoragerealtimewebsocketsessioninfo"></a>Office.OneNote.Storage.RealTime.WebSocketSessionInfo
 
Acest eveniment înregistrează rezultatul sincronizării WebSocket atât pentru sincronizarea conținutului paginii moderne OneNote, cât și pentru sincronizarea ierarhiei moderne. Acesta este utilizat pentru a afla de câte ținte de sincronizare unice este nevoie pentru calcularea scorului de sincronizare OneNote. De asemenea, acesta este utilizat pentru tabloul de bord pentru performanța sincronizării moderne OneNote.
 
Se colectează următoarele câmpuri:
 
- **CloseReason** - motivul închiderii WebSocket, de exemplu, închiderea anormală, etc.

- **DataIsFreshCount** - numărul de solicitări de extragere reușite în sesiunea WebSocket

- **DeviceSessionId** - ID-ul sesiunii dispozitivului

- **DownloadCount** - numărul de descărcări din sesiunea WebSocket

- **Eroare** - este, practic, Exception_Type + Exception_Description + Exception_Code + Exception_Tag

- **Exception_Code** - un cod numerotat sau alfanumeric utilizat pentru a determina natura unei erori și/sau motivul pentru care aceasta s-a produs

- **Exception_Description** - o descriere a erorii

- **Exception_Tag** - indică unde în cod se generează eroarea

- **Exception_Type** - tipul erorii, de exemplu, Win32Error, etc.

- **FirstUpdateSize** - lungimea mesajului pentru prima actualizare

- **HasError** - indică dacă există o eroare în timpul sesiunii WebSocket 

- **IsEducationNotebook** - blocnotesul curent este un blocnotes de educație sau nu

- **IsHierarchyResource** - resursa curentă este o pagină sau o secțiune

- **NotebookId** - ID-ul blocnotesului OneNote

- **OperationWithError** - în ce operațiune s-a întâmplat eroarea, de exemplu, WebSocket.Close, WebSocket.Open, etc.

- **ResourceId** - ID-ul resursei paginii sau secțiunii OneNote

- **SectionId** - ID-ul secțiunii OneNote

- **ServerSessionId** - ID-ul sesiunii utilizat pentru corelarea solicitării WebSocket către onenote.com

- **SessionDurationInMs** - durata sesiunii WebSocket în milisecunde

- **TenantId** - ID-ul entității găzduite SharePoint

- **TimeToFirstUpdateInMs** - timpul necesar, în milisecunde, pentru primirea primei actualizări de la server după ce s-a stabilit sesiunea WebSocket

- **UploadAckCount** - numărul de acceptări pentru încărcare în sesiunea WebSocket

- **WebUrl** - adresa URL web pentru PII 

### <a name="officeonenotestoragesectionsyncresult"></a>Office.OneNote.Storage.SectionSyncResult
 
Acest eveniment înregistrează rezultatul sincronizării secțiunii. Este utilizat pentru a afla câte ținte de sincronizare unice există atunci când se calculează scorul de sincronizare OneNote. De asemenea, acesta este utilizat pentru tabloul de bord pentru performanța sincronizării moderne OneNote.
 
Se colectează următoarele câmpuri

- **Error_Code** - un cod numerotat sau alfanumeric utilizat pentru a determina natura unei erori și/sau motivul pentru care aceasta s-a produs

- **Error_Description** - o descriere a erorii

- **Error_Tag** - indică unde în cod se generează eroarea

- **Error_Type** - tipul erorii, de exemplu, Win32Error, etc.

- **ErrorLast** - codul de eroare al ultimei erori observate 

- **ExecutionTime** - timpul necesar pentru reproducerea secțiunii, în milisecunde

- **InitialReplicationInSession** - dacă această reproducere este sau nu prima reproducere a blocnotesului după deschidere

- **IsAttachedViaShortcut** - secțiunea este atașată prin comandă rapidă sau nu

- **IsBackgroundSync** - aceasta este o sincronizare de fundal sau nu

- **IsEncrypted** - secțiunea este criptată sau nu

- **IsErrorSuppressed** - această eroare este suprimată sau nu 

- **IsErrorTransient** - această eroare este tranzitorie sau nu

- **IsErrorUnexpected** - această eroare este neașteptată sau nu

- **IsUsingRealtimeSync** - sincronizarea secțiunii utilizează sincronizarea modernă a conținutului paginilor sau nu

- **NotebookId** - ID blocnotes

- **NotebookPath** - adresa URL blocnotes pentru PII

- **SectionPath** - adresa URL a secțiunii pentru PII

- **SectionReplicatingIsOutbound** - această reproducere este o reproducere de ieșire sau nu

- **SectionReplicatingIsSameIdentity** - această reproducere este bazată pe aceeași identitate de fișier sau nu

- **SectionResourceId** - ID-ul resursei secțiunii OneNote

- **Success** - secțiunea a fost sincronizată cu succes sau nu

- **SyncDestinationType** - tipul destinației de sincronizare, adică OneDrive sau SharePoint Online

- **SyncId** - un număr unic pentru fiecare sincronizare de secțiune

- **SyncWasFirstInSession** - este acestă sincronizare prima sincronizare din sesiunea curentă

- **SyncWasUserInitiated** - este această sincronizare inițiată de utilizator sau nu

- **TenantId** - ID-ul entității găzduite SharePoint

- **UnmappedGosid** - ID-ul de secțiune înainte de aplicarea GUID de mapare


### <a name="officeonenotestoragesyncscore"></a>Office.OneNote.Storage.SyncScore
 
Acest eveniment înregistrează toți factorii negativi din experiența de sincronizare care sunt vizibili pentru utilizatori. Acesta este utilizat pentru calcularea scorului de sincronizare OneNote, care este o măsurătoare critică pentru evaluarea experienței de sincronizare a utilizatorilor OneNote.
 
Se colectează următoarele câmpuri

- **AutoShowSyncStatus** - indică dacă starea de sincronizare este afișată automat sau nu

- **Cause** - ce a cauza mutarea paginilor/secțiunilor OneNote la secțiuni amplasate incorect

- **Context** - o enumerare care clasifică ce încearcă să facă utilizatorul, de exemplu, să redenumească o secțiune, să redeschidă un blocnotes, etc.

- **Error_Code** - un cod numerotat sau alfanumeric utilizat pentru a determina natura unei erori și/sau motivul pentru care aceasta s-a produs

- **Error_Description** - o descriere a erorii

- **Error_Tag** - indică unde în cod se generează eroarea

- **Error_Type** - tipul erorii, de exemplu, Win32Error, etc.

- **ErrorText** - textul erorii afișat în UI

- **Explanation** - explică ce tip de modificări de ieșire în așteptare trebuie mutate la secțiuni amplasate incorect

- **fishbowlType** - tipul de acvariu, de exemplu, acvariu de pagină, acvariu de secțiune, etc.

- **IDS** - un identificator întreg pentru textul afișat în UI

- **idsFishbowl** - un identificator întreg pentru eroarea de acvariu afișată în UI

- **IsUsingRealtimeHierarchySync** - utilizează sincronizarea ierarhiei moderne sau nu

- **NotebookId** - ID blocnotes

- **PageSyncUIState** - șirul de stare pentru sincronizarea paginii, de exemplu, UpToDate, Syncing, SaveOffline, SyncError, etc. 

- **ServerGosid** - ID-ul resursei pentru noua pagină de conflict creată

- **Source** - o enumerare care indică ce eveniment a declanșat UI, adică, crearea unei noi imagini redx, o eroare de sincronizare în sincronizarea UI, afișarea unui dialog de eroare, etc.

### <a name="onenoteappprovisioningmovelocalnotebooktoonlinenotebookfailed"></a>OneNote.App.Provisioning.MoveLocalNotebookToOnlineNotebookFailed
 
Acest eveniment este înregistrat când nu reușește mutarea blocnotesului local pe drive.  Acest scenariu este specific pentru utilizatorii cu conectare întârziată Atunci când utilizatorul se conectează, blocnotesul său local este transferat în spațiul de stocare OneDrive. 
 
Se colectează următoarele câmpuri:
 
- **ErrorMsg** - mesajul de eroare corespunzător.

### <a name="onenotesynccreatenotebookfailed"></a>OneNote.Sync.CreateNotebookFailed
 
Acest eveniment este înregistrat când nu reușește crearea unui blocnotes.  
 
Se colectează următoarele câmpuri:
 
- **NetworkConnection** - înregistrează tipul de conexiune pe care îl are dispozitivul în prezent, de exemplu, Wi-Fi, offline, 3G 

- **ServerType** - înregistrează tipul de server în care trebuia să fie creat blocnotesul.

### <a name="onenotesyncfirstrunerror"></a>OneNote.Sync.FirstRunError
 
Acest eveniment este înregistrat când sincronizarea Notelor rapide nu a reușit pentru un utilizator în timpul primei experiențe de rulare pe un dispozitiv.  Acest lucru este specific pentru scenariul de primă rulare.
 
Se colectează următoarele câmpuri:
 
- **NetworkConnection** - înregistrează tipul de conexiune pe care îl are dispozitivul în prezent, de exemplu, Wi-Fi, offline, 3G

- **ServerType** - înregistrează tipul de server în care trebuia să fie creat blocnotesul Note rapide

## <a name="services-configuration-events"></a>Evenimente de configurare servicii

Configurare servicii nu colectează niciun eveniment cu date necesare de diagnosticare a serviciului.

## <a name="telemetry-events"></a>Evenimente de telemetrie

### <a name="office_firstrun_apple_telemetryoptin"></a>Office_FirstRun_Apple_TelemetryOptIn

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Evenimentul este utilizat pentru a monitoriza starea de funcționare a fluxului nostru de optare pentru telemetrie în prima experiență de rulare. Culegem un cod care denotă ce tip de opțiune de colectare a datelor de diagnostic a fost selectată de către utilizator.

Se colectează următoarele câmpuri:

 - **Data_EventId** - un cod care indică preferința de colectare a datelor de diagnostic selectată de utilizator.


### <a name="officesystemidentitychanged"></a>Office.System.IdentityChanged

Informații privind identitatea utilizatorului necesare pentru îndeplinirea solicitărilor persoanei vizate.

Se colectează următoarele câmpuri:

  - **IdentityChanged** - întotdeauna adevărată. Identitatea s-a modificat.

  - **TimerDetectedChange** - dacă modificarea a fost detectată prin metoda ping cu temporizare regulată.

### <a name="officesystemprivacyfallbacktosettingsstore"></a>Office.System.PrivacyFallbackToSettingsStore

Utilizat pentru a determina dacă există erori la citirea setărilor de confidențialitate ale utilizatorului din depozitul Roaming.

Se colectează următoarele câmpuri:

  - **Eticheta-** eticheta de cod care indică ce setare a revenit la depozitul de setări.

### <a name="officesystemsessiondatao365"></a>Office.System.SessionDataO365

Metadatele necesare pentru a izola reproducerea unui erori.

Se colectează următoarele câmpuri:

  - **AppId -** identificator pentru aplicația Office la care se referă aceste date.

  - **ApplicationArchitecture -** pentru ce arhitectură de procesor este construit Office.

  - **AppVersionBuild -** versiunea compilată a aplicației Office.

  - **AppVersionMajor -** versiunea majoră a aplicației Office.

  - **AppVersionMinor -** versiunea minoră a aplicației Office.

  - **AppVersionUpdate -** revizuirea compilată a aplicației Office.

  - **CollectorVersion -** identificator de versiune pentru logica de colecție a clientului.

  - **DeviceHash -** cod hash unidirecțional al identificatorului de dispozitiv cu sistem de operare.

  - **DeviceName -** numele dispozitivului pe care rulează Office.

  - **Domain -** domeniul dispozitivului pe care rulează Office.

  - **IsCeip -** dacă instalarea Office a fost înscrisă în fostul Program de îmbunătățire a experienței clienților.

  - **IsDebug -** dacă aceasta este o versiune de depanare a Office.

  - **IsImmersive -** dacă aplicația Office este o aplicație Universal Windows sau Immersive.

  - **IsLaptop -** dacă dispozitivul pe care rulează Office este un laptop.

  - **IsMicrosoftInternal -** dacă utilizatorul Windows care rulează Office este angajat Microsoft.

  - **IsO365 -** dacă instalarea Office face parte din fostul program Outlook 365.

  - **IsTablet -** dacă dispozitivul pe care rulează Office este o tabletă.

  - **IsTerminalServer -** adevărat/fals este client server terminal

  - **MaxMemory -** volumul maxim al memoriei cu acces aleator disponibile pentru dispozitivul pe care rulează Office.

  - **OsArchitecture -** arhitectura CPU pentru care este construit sistemul de operare pe care rulează Office.

  - **OsVersionBuild -** versiunea compilată a sistemului de operare.

  - **OsVersionMajor -** versiunea majoră a sistemului de operare.

  - **OsVersionMinor-** versiunea minoră a sistemului de operare.

  - **OsVersionUpdate -** revizuire compilare SO

  - **ProcessFileName -** Numele de executabil al aplicației care rulează

  - **ProcessorArchitecture -** pe ce arhitectură de procesor rulează Office.

  - **ProcessorFrequency -** viteza procesorului la dispozitivele pe care rulează Office în megahertzi.

  - **SessionStart -** ora la care a început procesul de rulare Office.

  - **UserName -** numele contului pe care rulează Office.

### <a name="officesystemsystemhealthcoremetadata"></a>Office.System.SystemHealthCoreMetadata

Metadatele necesare pentru a izola reproducerea unui erori.

Se colectează următoarele câmpuri:

  - **AppBuild -** versiunea compilată a aplicației Office.

  - **AppBuildRevision -** revizuirea compilată a aplicației Office.

  - **AppMajorVer -** versiunea majoră a aplicației Office.

  - **AppMinorVer -** versiunea minoră a aplicației Office.

  - **CID -** identitate a utilizatorului pseudonimizată

  - **CollectibleClassifications -** setul de clasificări de date care pot fi colectate.

  - **CollectionTime -** ora la care au fost colectate metadatele.

  - **DeviceManufacturer -** producătorul dispozitivului pe care rulează Office.

  - **DeviceModel -** modelul de dispozitiv pe care rulează Office.

  - **FirstRunTime -** prima dată când a fost rulată o aplicație Office.

  - **IsClickToRunInstall -** dacă aplicația Office a fost instalată cu ajutorul Clic și Pornire

  - **IsDebug -** dacă aceasta este o versiune de depanare a Office.

  - **IsLabMachine -** dacă Office rulează într-un laborator Microsoft.

  - **IsLaptop -** dacă dispozitivul pe care rulează Office este un laptop.

  - **IsMsftInternal -** dacă utilizatorul Windows care rulează Office este angajat Microsoft.

  - **IsSubscription -** dacă aplicația Office este instalată sub o licență de abonament.

  - **IsTablet -** dacă dispozitivul pe care rulează Office este o tabletă.

  - **IsTerminalServer -** dacă Office rulează pe un server terminal.

  - **MsoAppId -** identificator pentru aplicația Office la care se referă aceste date.

  - **OfficeArchitectureText -** pentru ce arhitectură de procesor este construit Office.

  - **OsBuild -** versiunea compilată a sistemului de operare.

  - **OsBuildRevision -** revizuire compilare SO

  - **OSEnvironment -** identificator pentru mediul în care rulează Office.

  - **OsMajorVer -** versiunea majoră a sistemului de operare.

  - **OsMinorVer-** versiunea minoră a sistemului de operare.

  - **OSVersionString -** versiunea sistemului de operare ca șir.

  - **ProcessorArchitecture -** pe ce arhitectură de procesor rulează Office.

  - **ProcessorCount -** numărul de procesoare de la dispozitivul pe care rulează Office.

  - **ProcSpeedMHz -** viteza procesorului la dispozitivele pe care rulează Office în megahertzi.

  - **RamMB -** volumul de RAM disponibil în dispozitivul pe care rulează Office.

  - **SqmUserId -** identificator aleatoriu pentru instalarea Office.

### <a name="officesystemsystemhealthdesktopsessionlifecycleandheartbeat"></a>Office.System.SystemHealthDesktopSessionLifecycleAndHeartbeat

Oferă informații despre măsurătorile stării de funcționare a sistemului.

Se colectează următoarele câmpuri:

  - **InstallMethod** - dacă pentru versiunea de compilare curentă a Office s-a efectuat upgrade, dacă s-a revenit la ea sau dacă este o instalare nouă.

  - **PreviousBuild** - versiunea de Office la care s-a efectuat upgrade pentru această compilare sau de la care s-a revenit.

  - **State** - starea la care s-a modificat sesiunea.

  - **Time** - ora la care s-a modificat starea sesiunii.

### <a name="officesystemsystemhealthessentialidentitycount"></a>Office.System.SystemHealthEssentialIdentityCount

Colectează numărul de identități de utilizatori conectați

Se colectează următoarele câmpuri:

  - **AllIdentityCount** - numărul total de identități

  - **ValidIdentityCount** - numărul de identități validate

### <a name="officesystemsystemhealthessentialmetadataallidentities"></a>Office.System.SystemHealthEssentialMetadataAllIdentities

Monitorizează starea conturilor recunoscute de Office în această sesiune. Utilizat pentru a izola o eroare la un tip de conectare la cont dacă eroarea este specifică unui tip.

Se colectează următoarele câmpuri:

  - **CollectionTime** - ora la care au fost colectate informațiile de identitate.

  - **IdentityType** - tipul de autentificare sau cont

  - **IdentityUniqueId** - identificator de identitate pseudonimizată

  - **IdentityUniqueIdHashed** - cod hash unidirecțional al ID-ului de identitate unic

### <a name="officesystemsystemhealthmetadataapplicationadditional"></a>Office.System.SystemHealthMetadataApplicationAdditional

Metadatele necesare pentru a izola reproducerea unui erori.

Se colectează următoarele câmpuri:

  - **Alias -** dacă utilizatorul care rulează Office este angajat Microsoft, alias din interiorul firmei.

  - **AppBuild -** versiunea compilată a aplicației Office.

  - **AppBuildRevision -** revizuirea compilată a aplicației Office.

  - **AppMajorVer -** versiunea majoră a aplicației Office.

  - **AppMinorVer -** versiunea minoră a aplicației Office.

  - **CID -** identitate a utilizatorului pseudonimizată

  - **CollectibleClassifications -** setul de clasificări de date care pot fi colectate.

  - **DeviceManufacturer -** producătorul dispozitivului pe care rulează Office.

  - **DeviceModel -** modelul de dispozitiv pe care rulează Office.

  - **DeviceProcessorModel -** modelul de procesor al dispozitivului pe care rulează Office.

  - **DigitizerInfo -** informații despre digitizorul atașat la dispozitivul pe care rulează Office.

  - **DomainName -** numele domeniului la care este asociat computerul pe care rulează Office (dacă este cazul).

  - **FirstRunTime -** prima dată când a fost rulată o aplicație Office.

  - **HorizontalResolution -** rezoluția orizontală a ecranului

  - **IsDebug -** dacă aceasta este o versiune de depanare a Office.

  - **IsImmersive -** dacă aplicația Office este o aplicație Universal Windows sau Immersive.

  - **IsJoinedToDomain -** dacă dispozitivul pe care rulează Office este asociat la domeniu.

  - **IsLabMachine -** dacă Office rulează într-un laborator Microsoft.

  - **IsLaptop -** dacă dispozitivul pe care rulează Office este un laptop.

  - **IsMsftInternal -** dacă utilizatorul Windows care rulează Office este angajat Microsoft.

  - **IsOEMInstalled -** dacă aplicația care rulează Office a fost instalată de un OEM.

  - **IsRunAsAdmin -** dacă aplicația Office rulează ca Administrator.

  - **IsSubscription -** dacă aplicația Office este instalată sub o licență de abonament.

  - **MsoAppId -** identificator pentru aplicația Office la care se referă aceste date.

  - **NumProcPhysCores -** numărul de nuclee fizice din procesor.

  - **OfficeBuild -** versiunea compilată a bibliotecilor partajate Office.

  - **OfficeBuildRevision -** versiune de revizuire compilată a bibliotecilor partajate Office.

  - **OfficeMajorVer -** versiune majoră a bibliotecilor partajate Office.

  - **OfficeMajorVer -** versiune minoră a bibliotecilor partajate Office.

  - **OsBuild -** versiunea compilată a sistemului de operare.

  - **OsBuildRevision -** revizuire compilare SO

  - **OsMajorVer -** versiunea majoră a sistemului de operare.

  - **OsMinorVer-** versiunea minoră a sistemului de operare.

  - **PowerPlatformRole -** Identificator rol computer preferat OEM al dispozitivului pe care rulează Office.

  - **ProcessFileName -** Numele de executabil al aplicației care rulează

  - **ProcessorCount -** numărul de procesoare de la dispozitivul pe care rulează Office.

  - **RamMB -** volumul de RAM disponibil în dispozitivul pe care rulează Office.

  - **SqmUserId -** identificator aleatoriu pentru instalarea Office.

  - **StudyId -** identificator studiu măsurători de calitate software.

  - **VerticalResolution -** rezoluția verticală a ecranului

  - **WinUserActType -** dacă utilizatorul Windows ce rulează Office este un administrator local, utilizator puternic sau utilizator normal.

### <a name="officesystemsystemhealthmetadataapplicationandlanguage"></a>Office.System.SystemHealthMetadataApplicationAndLanguage

Metadatele sunt obligatorii pentru a izola reproducerea unei erori.

Se colectează următoarele câmpuri:

  - **AppBuild -** versiunea compilată a aplicației Office.

  - **AppBuildRevision -** revizuirea compilată a aplicației Office.

  - **AppMajorVer -** versiunea majoră a aplicației Office.

  - **AppMinorVer -** versiunea minoră a aplicației Office.

  - **AppState -** identificator pentru starea în care se află aplicația Office.

  - **Click2RunPackageVersionBuild -** versiune compilată a pachetului cu programul de instalare Clic și Pornire.

  - **Click2RunPackageVersionMajor -** versiune majoră a pachetului cu programul de instalare Clic și Pornire.

  - **Click2RunPackageVersionMinor -** versiune minoră a pachetului cu programul de instalare Clic și Pornire.

  - **Click2RunPackageVersionRevision -** revizuire compilare a pachetului cu programul de instalare Clic și Pornire.

  - **DistributionChannel -** canalul prin care Office a fost distribuit.

  - **InstallType -** identificator pentru metoda prin care a fost instalat Office.

  - **IsClickToRunInstall -** dacă aplicația Office a fost instalată utilizând Clic și Pornire

  - **IsDebug -** dacă aceasta este o versiune de depanare a Office.

  - **IsImmersive -** dacă aplicația Office este o aplicație Universal Windows sau Immersive.

  - **IsMsftInternal -** dacă utilizatorul Windows care rulează Office este angajat Microsoft.

  - **IsOEMInstalled -** dacă aplicația care rulează Office a fost instalată de un OEM.

  - **IsRunAsAdmin -** dacă aplicația Office rulează ca Administrator.

  - **IsSubscription -** dacă aplicația Office este instalată sub o licență de abonament.

  - **MsoAppId -** identificator pentru aplicația Office la care se referă aceste date.

  - **OfficeArchitectureText -** pentru ce arhitectură de procesor este construit Office.

  - **OfficeBuild -** versiunea compilată a bibliotecilor partajate Office.

  - **OfficeBuildRevision -** versiune de revizuire compilată a bibliotecilor partajate Office.

  - **OfficeMajorVer -** versiune majoră a bibliotecilor partajate Office.

  - **OfficeMajorVer -** versiune minoră a bibliotecilor partajate Office.

  - **OfficeMuiCount -** numărul de pachetele lingvistice Office instalate.

  - **OfficeSkuLanguage -** limba SKU instalată.

  - **OfficeSkuLanguageTag -** limba SKU instalată.

  - **OfficeUiLang -** limba interfeței cu utilizatorul pentru aplicația Office.

  - **OfficeUiLangTag -** limba interfeței cu utilizatorul pentru aplicația Office.

  - **ProcessFileName -** Numele de executabil al aplicației care rulează

  - **SqmAppId -** identificator pentru aplicația de Office la care se referă aceste date.

### <a name="officesystemsystemhealthmetadatadelayedlogin"></a>Office.System.SystemHealthMetadataDelayedLogin

Informații privind identitatea utilizatorului necesare pentru îndeplinirea solicitărilor persoanei vizate.

Se colectează următoarele câmpuri:

  - **CID** - identitatea utilizatorului pseudonimizată

### <a name="officesystemsystemhealthmetadatadevice"></a>Office.System.SystemHealthMetadataDevice

Metadatele necesare pentru a izola reproducerea unui erori.

Se colectează următoarele câmpuri:

  - **CollectionTime -** ora la care au fost colectate metadatele.

  - **ComputerSystemProductUuidHash -** cod hash unidirecțional UUID placă de bază.

  - **DeviceClass -** identificator pentru tipul de dispozitiv pe care rulează Office.

  - **DeviceMake -** identificator al familiei sistemului hardware al dispozitivului pe care rulează Office.

  - **DeviceManufacturer -** producătorul dispozitivul pe care rulează Office.

  - **DeviceModel -** modelul de dispozitiv pe care rulează Office.

  - **DigitizerInfo -** informații despre digitizorul atașat la dispozitivul pe care rulează Office.

  - **IsLaptop -** dacă dispozitivul pe care rulează Office este un laptop.

  - **IsTablet -** dacă dispozitivul pe care rulează Office este o tabletă.

  - **LicensingACID -** identificator de licențiere pentru instalarea Office.

  - **MachineName -** numele dispozitivului pe care rulează Office.

  - **NumProcPhysCores -** numărul de nuclee fizice din procesor.

  - **NumProcShareSingleCache -** numărul de procesoare care partajează un cache unic pe dispozitivul pe care rulează Office.

  - **NumProcShareSingleCore -** numărul de procesoare per nucleu fizic la dispozitivul pe care rulează Office.

  - **OlsLicenseId -** identificator al serviciului de licențiere pentru instalarea Office.

  - **Platform -** identificator al mediului în care rulează Office.

  - **PowerPlatformRole -** Identificator rol computer preferat OEM al dispozitivului pe care rulează Office.

  - **ProcessorCount -** numărul de procesoare de la dispozitivul pe care rulează Office.

  - **ProcSpeedMHz -** viteza procesorului la dispozitivul pe care rulează Office în megahertzi.

  - **ProcType -** arhitectura procesorului.

  - **ProcTypeText -** tipul de procesor de la dispozitivul pe care rulează Office.

  - **RamMB -** volumul de RAM disponibil în dispozitivul pe care rulează Office.

  - **SusClientId -** ID-ul Windows Update al dispozitivului pe care rulează Office.

  - **SystemFamily -** identificator al familiei sistemului hardware al dispozitivului pe care rulează Office.

  - **SystemSKU -** identificator al SKU al sistemului hardware al dispozitivului pe care rulează Office.

  - **SysVolFreeSpaceMB -** spațiul liber disponibil din volumul sistemului în MB.

  - **SysVolSizeMB -** spațiul disponibil din volumul sistemului în MB.

  - **WindowsErrorReportingMachineId -** identificator computer atribuit Tehnologie Windows de raportare a erorilor al dispozitivului pe care rulează Office.

  - **WindowsSqmMachineId -** identificator computer atribuit Windows al dispozitivului pe care rulează Office.

### <a name="officesystemsystemhealthmetadatadeviceconsolidated"></a>Office.System.SystemHealthMetadataDeviceConsolidated

Metadatele necesare pentru a izola reproducerea unui erori.

Se colectează următoarele câmpuri:

  - **BootDiskType -** unitate disc sau SSD

  - **ComputerSystemProductUuidHash -** cod hash unidirecțional UUID placă de bază.

  - **DeviceClass -** identificator pentru tipul de dispozitiv pe care rulează Office.

  - **DeviceManufacturer -** producătorul dispozitivul pe care rulează Office.

  - **DeviceModel -** modelul de dispozitiv pe care rulează Office.

  - **DeviceProcessorModel -** modelul de procesor al dispozitivului pe care rulează Office.

  - **DigitizerInfo -** informații despre digitizorul atașat la dispozitivul pe care rulează Office.

  - **HasSpectreFix -** dacă procesorul dispozitivului pe care rulează Office are o remediere Spectre.

  - **IsLaptop -** dacă dispozitivul pe care rulează Office este un laptop.

  - **IsTablet -** dacă dispozitivul pe care rulează Office este o tabletă.

  - **MachineName -** numele dispozitivului pe care rulează Office.

  - **NumProcPhysCores -** numărul de nuclee fizice din procesor.

  - **NumProcShareSingleCache -** numărul de procesoare care partajează un cache unic pe dispozitivul pe care rulează Office.

  - **NumProcShareSingleCore -** numărul de procesoare per nucleu fizic la dispozitivul pe care rulează Office.

  - **Platform -** identificator al mediului în care rulează Office.

  - **PowerPlatformRole -** Identificator rol computer preferat OEM al dispozitivului pe care rulează Office.

  - **powerPlatformRole -** Identificator rol computer preferat OEM al dispozitivului pe care rulează Office.

  - **ProcessorCount -** numărul de procesoare de la dispozitivul pe care rulează Office.

  - **ProcSpeedMHz -** viteza procesorului la dispozitivul pe care rulează Office în megahertzi.

  - **ProcType -** arhitectura procesorului.

  - **ProcTypeText -** tipul de procesor de la dispozitivul pe care rulează Office.

  - **RamMB -** volumul de RAM disponibil în dispozitivul pe care rulează Office.

  - **SusClientId -** ID-ul Windows Update al dispozitivului pe care rulează Office.

  - **SysVolFreeSpaceMB -** spațiul liber disponibil din volumul sistemului în MB.

  - **SysVolSizeMB -** spațiul disponibil din volumul sistemului în MB.

  - **sysVolSizeMB -** spațiul disponibil din volumul sistemului în MB.

  - **WindowsErrorReportingMachineId** - identificator computer atribuit Tehnologie Windows de raportare a erorilor al dispozitivului pe care rulează Office.

  - **WindowsSqmMachineId** - identificator computer atribuit Windows al dispozitivului pe care rulează Office.

### <a name="officesystemsystemhealthmetadataoperatingsystem"></a>Office.System.SystemHealthMetadataOperatingSystem

Metadatele necesare pentru a izola reproducerea unui erori.

Se colectează următoarele câmpuri:

  - **CollectionTime** - ora la care acest eveniment a fost atașat la coadă pentru încărcare

  - **IsTerminalServer** - adevărat/fals este client server terminal

  - **OsBuild** - versiunea compilată a sistemului de operare.

  - **OsBuildRevision** - revizuire compilare SO

  - **OSEnvironment** - Windows, iOS, Mac, Android etc.

  - **OsMajorVer** - versiunea majoră a sistemului de operare.

  - **OsMinorVer** - versiunea minoră a sistemului de operare.

  - **OSSDKVersionCode** - identificator de versiune pentru SDK al sistemului de operare.

  - **OsSku** - SKU SO

  - **OsSuite2** - identificator suită sistem de operare.

  - **OSVersionString** - identificator versiune sistem de operare.

  - **ServicePackMajorVer** - versiune majoră pachet Service Pack SO

  - **ServicePackMinorVer** - versiune minoră pachet Service Pack SO

### <a name="officesystemsystemhealthmetadataoperatingsystemdevice"></a>Office.System.SystemHealthMetadataOperatingSystemDevice

Metadatele necesare pentru a izola reproducerea unui erori.

Se colectează următoarele câmpuri:

  - **CollectionTime -** ora la care acest eveniment a fost atașat la coadă pentru încărcare

  - **DeviceClass -** identificator pentru tipul de dispozitiv pe care rulează Office.

  - **DeviceManufacturer -** producătorul dispozitivul pe care rulează Office.

  - **DeviceModel -** modelul de dispozitiv pe care rulează Office.

  - **DigitizerInfo -** informații despre digitizorul atașat la dispozitivul pe care rulează Office.

  - **IsLaptop -** dacă dispozitivul pe care rulează Office este un laptop.

  - **IsTablet -** dacă dispozitivul pe care rulează Office este o tabletă.

  - **IsTerminalServer -** adevărat/fals este client server terminal

  - **MachineName -** numele dispozitivului pe care rulează Office.

  - **NumProcPhysCores -** numărul de nuclee fizice din procesor.

  - **NumProcShareSingleCache -** numărul de procesoare care partajează un cache unic pe dispozitivul pe care rulează Office.

  - **NumProcShareSingleCore -** numărul de procesoare per nucleu fizic la dispozitivul pe care rulează Office.

  - **OsBuild -** versiunea compilată a sistemului de operare.

  - **OsBuildRevision -** revizuire compilare SO

  - **OSEnvironment -** Windows, iOS, Mac, Android etc.

  - **OsMajorVer -** versiunea majoră a sistemului de operare.

  - **OsMinorVer-** versiunea minoră a sistemului de operare.

  - **OSSDKVersionCode -** identificator de versiune pentru SDK al sistemului de operare.

  - **OsSku -** SKU SO

  - **OsSuite2 -** identificator suită sistem de operare.

  - **OSVersionString -** identificator versiune sistem de operare.

  - **Platform -** identificator al mediului în care rulează Office.

  - **PowerPlatformRole -** Identificator rol computer preferat OEM al dispozitivului pe care rulează Office.

  - **ProcessorCount -** numărul de procesoare de la dispozitivul pe care rulează Office.

  - **ProcSpeedMHz -** viteza procesorului la dispozitivul pe care rulează Office în megahertzi.

  - **ProcTypeText -** tip de procesor

  - **RamMB -** volumul de RAM disponibil în dispozitivul pe care rulează Office.

  - **ServicePackMajorVer -** versiune majoră pachet Service Pack SO

  - **ServicePackMinorVer -** versiune minoră pachet Service Pack SO

  - **SysVolFreeSpaceMB -** spațiul liber disponibil din volumul sistemului în MB.

  - **SysVolSizeMB -** spațiul disponibil din volumul sistemului în MB.

### <a name="officesystemsystemhealthmetadataos"></a>Office.System.SystemHealthMetadataOS

Metadatele necesare pentru a izola reproducerea unui erori.

Se colectează următoarele câmpuri:

  - **CountryRegion -** setare sistem de operare identificator țară/regiune.

  - **HorizontalResolution -** rezoluția orizontală a ecranului

  - **IsTerminalServer -** adevărat/fals este client server terminal

  - **KeyboardLanguage -** identificator de limbă a tastaturii dispozitivului

  - **KeyboardLanguageTag -** identificator de limbă a tastaturii dispozitivului

  - **OfficeWvd -** identifică starea în care se află Desktop virtual Windows.

  - **OsBuild -** versiunea compilată a sistemului de operare.

  - **OsBuildRevision -** revizuire compilare SO

  - **OSEnvironment -** Windows, iOS, Mac, Android etc.

  - **OsLocale -** identificator setări regionale sistem de operare.

  - **OsLocaleTag -** identificator setări regionale sistem de operare.

  - **OsMajorVer -** versiunea majoră a sistemului de operare.

  - **OsMinorVer-** versiunea minoră a sistemului de operare.

  - **OSSDKVersionCode -** identificator versiune SDK sistem de operare.

  - **OsSku -** identificator SKU sistem de operare.

  - **OsSuite2 -** identificator suită sistem de operare.

  - **OsUiLang -** limba interfeței cu utilizatorul a sistemului de operare.

  - **OSVersionString -** identificator versiune sistem de operare.

  - **ScreenDepth -** adâncime ecran

  - **ScreenDepth -** dpi ecran

  - **ServicePackMajorVer -** versiune majoră pachet Service Pack SO

  - **ServicePackMinorVer -** versiune minoră pachet Service Pack SO

  - **SystemLocale -** setările regionale implicite ale sistemului de operare

  - **SystemLocaleTag -** setările regionale implicite ale sistemului de operare

  - **TimeZoneBiasInMinutes -** diferența în minute între ora locală și UTC.

  - **VerticalResolution -** rezoluția verticală a ecranului

### <a name="officesystemsystemhealthmetadatascreencultureusersqmid"></a>Office.System.SystemHealthMetadataScreenCultureUserSqmId

Metadatele necesare pentru a izola reproducerea unui erori.

Se colectează următoarele câmpuri:

  - **Alias -** angajat Microsoft sau alias utilizator automat

  - **CID -** identitate a utilizatorului pseudonimizată

  - **CollectibleClassifications -** clasificări de date care pot fi colectate în conformitate cu setările de confidențialitate ale clientului

  - **CollectionTime -** ora la care acest eveniment a fost atașat la coadă pentru încărcare

  - **CountryRegion -** setare sistem de operare identificator țară/regiune.

  - **DomainName -** numele de domeniu al domeniului Microsoft

  - **HorizontalResolution -** rezoluția orizontală a ecranului

  - **IntegratedScreenSize -** dimensiunea ecranului integrat.

  - **IsJoinedToDomain -** adevărat/fals este clientul asociat la domeniu

  - **IsLabMachine -** este computer din laboratorul de testare Microsoft

  - **IsMsftInternal -** adevărat/fals este computerul din domeniul de corporație Microsoft

  - **IsSubscription -** dacă aplicația Office este instalată sub o licență de abonament.

  - **KeyboardLanguage -** identificator de limbă a tastaturii dispozitivului

  - **KeyboardLanguageTag -** identificator de limbă a tastaturii dispozitivului

  - **OsLocale -** identificator setări regionale sistem de operare.

  - **OsLocaleTag -** identificator setări regionale sistem de operare.

  - **OsUiLang -** limba interfeței cu utilizatorul a sistemului de operare.

  - **ScreenDepth -** adâncime ecran

  - **ScreenDepth -** dpi ecran

  - **ScreenXDpi -** DPI ecran X

  - **ScreenYDpi -** DPI ecran Y

  - **SqmUserId -** identificator aleatoriu pentru instalarea Office.

  - **StudyId -** identificator studiu măsurători de calitate software.

  - **SystemLocale -** setările regionale implicite ale sistemului de operare

  - **SystemLocaleTag -** setările regionale implicite ale sistemului de operare

  - **TimeZoneBiasInMinutes -** diferența în minute între ora locală și UTC.

  - **VerticalResolution -** rezoluția verticală a ecranului

  - **WinUserActType -** dacă utilizatorul Windows ce rulează Office este un administrator local, utilizator puternic sau utilizator normal.

### <a name="officesystemsystemhealthofficelensidentity"></a>Office.System.SystemHealthOfficeLensIdentity

Informații privind identitatea utilizatorului necesare pentru îndeplinirea solicitărilor persoanei vizate.

Se colectează următoarele câmpuri:

  - **CID** - identitatea utilizatorului pseudonimizată

### <a name="officesystemsystemhealthrollbacksessionmetadata"></a>Office.System.SystemHealthRollbackSessionMetadata

Metadatele necesare pentru a izola reproducerea unui erori.

Se colectează următoarele câmpuri:

  - **InstallMethod** - instalare nouă, actualizare sau revenire

  - **IsSubscription** - dacă aplicația Office este instalată sub o licență de abonament.

  - **PreviousBuild** - versiune compilată instalată anterior

### <a name="officesystemsystemhealthsessionlifecycleandheartbeat"></a>Office.System.SystemHealthSessionLifecycleAndHeartbeat

Oferă informații despre măsurătorile stării de funcționare a sistemului.

Se colectează următoarele câmpuri:

  - **InstallMethod** - dacă pentru instalarea curentă a Office s-a efectuat upgrade, dacă s-a revenit la ea sau dacă este o instalare nouă.

  - **InteractionSessionID** - identificator sesiune.

  - **PreviousBuild** - versiunea de Office la care s-a efectuat upgrade pentru această compilare sau de la care s-a revenit.

  - **State** - starea la care s-a modificat sesiunea.

  - **Time** - punct în care s-a modificat starea sesiunii.

### <a name="officesystemsystemhealthsessionstarttime"></a>Office.System.SystemHealthSessionStartTime

Utilizat cu date de cădere pentru a separa primele căderi de cele de mai târziu (adică stabiliți dacă utilizatorul a folosit aplicația o anumită perioadă înaintea de cădere)

Se colectează următoarele câmpuri:

  - **SessionStart** - ora la care telemetria pornește datele de procesare.

### <a name="officesystemsystemhealthungracefulappexitdesktop"></a>Office.System.SystemHealthUngracefulAppExitDesktop

Utilizat pentru a captura măsurători privind căderea.

Se colectează următoarele câmpuri:

  - **AffectedProcessAppBuild -** identificator versiune compilată pentru procesul afectat.

  - **AffectedProcessAppBuildRevision -** identificator revizuire compilare pentru procesul afectat.

  - **AffectedProcessAppMinorVer -** identificator versiune minoră pentru procesul afectat.

  - **AffectedProcessAppName -** numele procesului afectat.

  - **AffectedProcessExeBuildVersion -** numărul versiunii compilate a procesului afectat.

  - **AffectedProcessExeMajorVersion -** numărul versiunii majore a procesului afectat.

  - **AffectedProcessExeMinorVersion -** numărul versiunii minore a procesului afectat.

  - **AffectedProcessExeRevisionVersion -** numărul versiunii compilate a procesului afectat.

  - **AffectedProcessIsDebug -** dacă procesul afectat este o compilare de depanare.

  - **AffectedProcessIsLabMachine -** dacă procesul afectat este într-un laborator Microsoft.

  - **AffectedProcessOsEnvironment -** identificator de sistem de operare pentru procesul afectat.

  - **AppName -** numele aplicației afectate.

  - **CrashedAssignedFlights -** Ediții flight atribuite procesului care a suferit o cădere.

  - **CrashedConfigIds -** configurația atribuită procesului care a suferit o cădere.

  - **CrashedEcsETag -** Identificator de experiment pentru procesul care a suferit o cădere.

  - **CrashedImpressionId -** identificatorul de impresie al procesului care a suferit o cădere.

  - **CrashedProcessSessionID -** identificator unic al procesului care a suferit o cădere.

  - **CrashedProcessSessionInitTime -** ora la care a început procesul afectat.

  - **CrashType -** identificator de bucket pentru tipul de cădere.

  - **DetectionTime -** ora la care s-a detectat ieșirea neprevăzută.

  - **ErrorString -** descrierea erorii.

  - **ExceptionAddress -** adresa din programul unde a apărut eroarea.

  - **ExceptionCode -** identificator de bucket pentru excepție.

  - **FaultAppName -** numele aplicației defecte.

  - **InstallMethod -** dacă pentru versiunea de compilare curentă a Office s-a efectuat upgrade, dacă s-a revenit la ea sau dacă este o instalare nouă.

  - **InstallType -** identificator pentru metoda prin care a fost instalat Office.

  - **InstallTypeName -** identificator pentru metoda prin care a fost instalat Office

  - **IsLabMachine -** dacă Office rulează într-un laborator Microsoft.

  - **IsMsftInternal -** dacă utilizatorul Windows care rulează Office este angajat Microsoft.

  - **ModuleBaseAddress -** adresa de bază a modulului cu erori.

  - **ModuleBuildVersion -** numărul versiunii compilate a modulului cu erori.

  - **ModuleMajorVersion -** numărul versiunii majore a modulului cu erori.

  - **ModuleMinorVersion -** numărul versiunii minore a modulului cu erori.

  - **ModuleName -** numele modulului cu erori.

  - **ModuleOffset -** deplasare în octeți de la adresa de bază unde a apărut eroarea.

  - **ModuleRevisionVersion -** numărul versiunii de revizuire compilate a modulului cu erori.

  - **ModuleSize -** dimensiunea modulului cu erori în octeți.

  - **OSEnvironment -** identificator pentru mediul în care rulează Office.

  - **PreviousBuild -** versiune compilată instalată anterior

  - **UAETypeName -** identificator de bucket privind modul brusc în care s-a închis aplicația.

  - **VerifyElseCrashTag -** identificator unic al locului unde a căzut aplicația.

### <a name="officesystemsystemhealthungracefulappexitimmersive"></a>Office.System.SystemHealthUngracefulAppExitImmersive

Utilizat pentru a captura măsurători privind căderea.

Se colectează următoarele câmpuri:

  - **AffectedProcessAppBuild -** identificator versiune compilată pentru procesul afectat.

  - **AffectedProcessAppBuildRevision -** identificator revizuire compilare pentru procesul afectat.

  - **AffectedProcessAppMajorVer -** identificator versiune majoră pentru procesul afectat.

  - **AffectedProcessAppMinorVer -** identificator versiune minoră pentru procesul afectat.

  - **AffectedProcessAppName -** numele procesului afectat.

  - **AffectedProcessExeBuildVersion -** numărul versiunii compilate a procesului afectat.

  - **AffectedProcessExeMajorVersion -** numărul versiunii majore a procesului afectat.

  - **AffectedProcessExeMinorVersion -** numărul versiunii minore a procesului afectat.

  - **AffectedProcessExeRevisionVersion -** numărul versiunii compilate a procesului afectat.

  - **AffectedProcessIsDebug -** dacă procesul afectat este o compilare de depanare.

  - **AffectedProcessIsLabMachine -** dacă procesul afectat este într-un laborator Microsoft.

  - **AffectedProcessOsEnvironment -** identificator de sistem de operare pentru procesul afectat.

  - **AppName -** numele aplicației afectate.

  - **CrashedAssignedFlights -** Ediții flight atribuite procesului care a suferit o cădere.

  - **CrashedConfigIds -** configurația atribuită procesului care a suferit o cădere.

  - **CrashedImpressionId -** identificatorul de impresie al procesului care a suferit o cădere.

  - **CrashedInteractionSessionID -** identificator sesiune de interacțiune pentru procesul afectat.

  - **CrashedInteractionSessionTime -** ora la care s-a putut interacționa cu procesul afectat.

  - **CrashedProcessSessionID -** identificator unic al procesului care a suferit o cădere.

  - **CrashedProcessSessionInitTime -** ora la care a început procesul afectat.

  - **DetectionTime -** ora la care s-a detectat ieșirea neprevăzută.

  - **IsLabMachine -** dacă Office rulează într-un laborator Microsoft.

  - **IsMsftInternal -** dacă utilizatorul Windows care rulează Office este angajat Microsoft.

  - **OSEnvironment -** identificator pentru mediul în care rulează Office.

  - **PreviousLifecycleState -** starea procesului afectat când a suferit o cădere.

  - **UAETypeName -** identificator de bucket privind modul brusc în care s-a închis aplicația.

### <a name="officesystemsystemhealthungracefulapplicationexitwin32"></a>Office.System.SystemHealthUngracefulApplicationExitWin32

Evenimentul este declanșat de o întrerupere anormală a aplicației (de exemplu, anularea managerului de activități, suspendarea aplicației etc.) pentru aplicațiile client Office, cum ar fi, dar fără a se limita la, Word, Excel, PowerPoint și Outlook. Utilizăm măsurători ale ieșirilor neelegante din aplicație pentru a măsura starea de funcționare a produselor client Office. Acesta este un semnal esențial pentru activitate utilizat de către inginerii Office pentru a deduce stabilitatea produselor.

Se colectează următoarele câmpuri:

  - **BootCompleted-** A fost boot Office finalizată la momentul căderii.

  - **CrashedAppBuild -** identificator versiune compilată pentru procesul afectat.

  - **CrashedAppMajor -** identificator versiune majoră pentru procesul afectat.

  - **CrashedAppMinor -** identificator versiune minoră pentru procesul afectat.

  - **CrashedAppRevision -** identificator versiune compilată pentru procesul afectat.

  - **CrashedEcsETag -** identificator de experiment pentru procesul care a suferit o cădere.

  - **CrashedModuleName -** numele modulului cu erori.

  - **CrashedSessionId -** identificator unic al procesului care a suferit o cădere.

  - **CrashedSessionInitTime -** ora la care a început procesul afectat.

  - **CrashTime –** Momentelor în care se menționează că clientul s-a terminat negrațios.

  - **CrashType -** identificator de bucket pentru tipul de cădere.

  - **DetectionTime -** ora la care s-a detectat ieșirea neprevăzută.

  - **ExceptionAddress -** adresa din programul unde a apărut eroarea.

  - **ExceptionCode -** identificator de bucket pentru excepție.

  - **Refacerea –** A creat utilizatorul și a înmânat procesul Office într-o nouă sesiune.

  - **HasEdit-** A fost utilizatorul care a editat un document în clientul prăbușit.

  - **HasOpen-** A fost un document deschis în clientul prăbușit.

  - **HexCrashTag -**  identificatorul unic pentru codul căderii.

  - **HexExceptionAddress -** adresa în hexazecimale din programul unde a apărut eroarea.

  - **HexExceptionCode -** identificator de bucket în hexazecimale pentru excepție.

  - **HexModuleBaseAddress -** adresa de bază în hexazecimale a modulului cu erori.

  - **HexModuleOffset -** deplasare în octeți (în hexazecimale) de la adresa de bază unde a apărut eroarea.

  - **HexModuleSize -** dimensiune modul cu erori în octeți în hexazecimale.

  - **HexVerifyElseCrashTag -** identificator unic în hexazecimale al locului unde a căzut aplicația

  - **InstallMethod -** dacă pentru versiunea de compilare curentă a Office s-a efectuat upgrade, dacă s-a revenit la ea sau dacă este o instalare nouă.

  - **IsLabMachine -** dacă Office rulează într-un laborator Microsoft.

  - **ModuleBaseAddress -** adresa de bază a modulului cu erori.

  - **ModuleOffset -** deplasare în octeți de la adresa de bază unde a apărut eroarea.

  - **ModuleSize -** dimensiunea modulului cu erori în octeți.

  - **OpenUILang -** Limba interfeței cu utilizatorul pentru aplicația Office.

  - **PreviousBuild -** Versiune compilată instalată anterior

  - **SafeMode-** A fost sesiunea pornită în modul de siguranță.

  - **UAEOSEnvironment -** identificator de mediu pentru sistemul de operare.

  - **UninitLibletId –** identificatorul unic pentru componenta cu erori a căderii.

  - **VerifyElseCrashTag -** identificator unic al locului unde a căzut aplicația. *[Acest eveniment a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

### <a name="officesystemungracefulapplicationexitdesktopappexit"></a>Office.System.UngracefulApplicationExit.DesktopAppExit

Utilizat pentru a captura măsurători privind căderea.

Se colectează următoarele câmpuri:

  - **AppBuildVersion -** identificator versiune compilată pentru procesul afectat.

  - **AppMajorVersion -** numărul versiunii majore a procesului afectat.

  - **AppMinorVersion -** identificator versiune minoră pentru procesul afectat.

  - **AppName -** numele aplicației afectate.

  - **AppRevisionVersion -** identificator versiune compilată pentru procesul afectat.

  - **CrashedAssignedFlights -** Ediții flight atribuite procesului care a suferit o cădere.

  - **CrashedConfigIds -** configurația atribuită procesului care a suferit o cădere.

  - **CrashedImpressionId -** identificatorul de impresie al procesului care a suferit o cădere.

  - **CrashedInteractionSessionId -** identificator sesiune de interacțiune a procesului care a suferit o cădere.

  - **CrashedProcessSessionId -** identificator unic al procesului care a suferit o cădere.

  - **CrashType -** identificator de bucket pentru tipul de cădere.

  - **ErrorString -** descrierea erorii.

  - **ExceptionAddress -** adresa din programul unde a apărut eroarea.

  - **ExceptionCode -** identificator de bucket pentru excepție.

  - **FaultAppName -** numele aplicației defecte.

  - **InstallMethod -** dacă pentru versiunea de compilare curentă a Office s-a efectuat upgrade, dacă s-a revenit la ea sau dacă este o instalare nouă.

  - **InstallType -** identificator pentru metoda prin care a fost instalat Office.

  - **IsDebug -** dacă aceasta este o versiune de depanare a Office.

  - **IsHandledCrash -** dacă rutina de tratare a căderii a fost invocată în sesiunea de cădere.

  - **IsLabMachine -** dacă Office rulează într-un laborator Microsoft.

  - **ModuleBaseAddress -** adresa de bază a modulului cu erori.

  - **ModuleName -** numele modulului cu erori.

  - **ModuleOffset -** deplasare în octeți de la adresa de bază unde a apărut eroarea.

  - **ModuleSize -** dimensiunea modulului cu erori în octeți.

  - **OSEnvironment -** identificator pentru mediul în care rulează Office.

  - **PreviousBuild -** versiune compilată instalată anterior

  - **PreviousInteractionSessionTime -** ora la care a început sesiunea de interacțiune anterioară.

  - **PreviousLifecycleState -** identificator stare ciclu de viață sesiune anterioară.

  - **PreviousSessionInitTime -** ora la care a început sesiunea anterioară.

  - **StackHash -** identificator care indică unde anume în cod a căzut procesul afectat.

  - **VerifyElseCrashTag -** identificator unic al locului unde a căzut aplicația.

### <a name="officesystemuserchangeddiagnosticlevel"></a>Office.System.UserChangedDiagnosticLevel

Informații obligatorii pentru a garanta faptul că opțiunile privind politica de confidențialitate a utilizatorului sunt impuse.

Se colectează următoarele câmpuri:

  - **DiagnosticLevelChanged**: indică faptul că utilizatorul a modificat nivelul de diagnosticare.

  - **NewDiagnosticLevel**: nivelul după modificarea utilizatorului.

  - **OldDiagnosticLevel**: nivelul la care se afla utilizatorul înainte de modificare.

### <a name="officetelemetryariaeventsinkhandlemsadevicetokenresponse"></a>Office.Telemetry.AriaEventSink.HandleMsaDeviceTokenResponse

Semnal ale unei indisponibilități a serviciului cont Microsoft.

Se colectează următoarele câmpuri:

  - **RetryCount** - numărul de reîncercări de conectare la serviciul MSA.

### <a name="officetelemetryariaeventsinkrequestmsadevicetoken"></a>Office.Telemetry.AriaEventSink.RequestMsaDeviceToken

Semnal ale unei indisponibilități a serviciului cont Microsoft.

Se colectează următoarele câmpuri:

  - **RetryCount** - numărul de reîncercări de conectare la serviciul cont Microsoft.

### <a name="officetelemetryclientsamplingoverridden"></a>Office.Telemetry.ClientSamplingOverridden

Obligatoriu pentru a obține rate de reproducere corespunzătoare. În mod normal nu se aplică la grupul de public Producție.

Se colectează următoarele câmpuri:

  - **OverriddenMeasureEnabled** - este clientul configurat să trimită mai mult decât evenimente neeșantionate

  - **OverriddenNumberlinePosition** - noua poziție a liniei numărului pentru eșantionare

  - **OverriddenReportedSampleRate** - noua rată de eșantionare raportată

  - **OverriddenSampleRate** - noua rată de eșantionare

  - **PreviousNumberlinePosition** - poziția liniei numărului pentru eșantionare.

  - **PreviousSampleRate** - rata de eșantionare înainte de a fi înlocuită.

  - **WasMeasureEnabled** - a fost clientul configurat să trimită mai mult decât evenimente neeșantionate

### <a name="officetelemetrycomplianceeventnotinbasicallowlist"></a>Office.Telemetry.Compliance.EventNotInBasicAllowList

Raportează implementări de telemetrie nevalide

Se colectează următoarele câmpuri:

  - **EventName** - numele evenimentului care nu se află în listă

### <a name="officetelemetrycompliancemissingdatacategory"></a>Office.Telemetry.Compliance.MissingDataCategory

Raportează implementări de telemetrie nevalide

Se colectează următoarele câmpuri:

  - **EventName** - numele evenimentului din care lipsește o categorie

  - **IsFromRule** - dacă evenimentul provine dintr-o regulă de telemetrie

### <a name="officetelemetrycompliancemissingdatacategoryinrule"></a>Office.Telemetry.Compliance.MissingDataCategoryInRule

Raportează implementări de telemetrie nevalide

Se colectează următoarele câmpuri:

  - **RuleId** - ID-ul regulii din care lipsește o categorie de date

  - **RuleVersion** - ID-ul regulii din care lipsește o categorie de date

### <a name="officetelemetrydiagnosticdataviewerstatechanged"></a>Office.Telemetry.DiagnosticDataViewerStateChanged

Validează faptul că consumatorii pot vizualiza datele pe măsură ce ies din computer utilizând Vizualizatorul datelor diagnosticare.

Se colectează următoarele câmpuri:

  - **Dialogcanceled** - a fost anulată caseta de dialog a Vizualizatorului datelor de diagnosticare

  - **NewState** - noua stare a Vizualizatorului datelor de diagnosticare

  - **WasDialogUsed** - a fost utilizată caseta de dialog a Vizualizatorului datelor de diagnosticare 

### <a name="officetelemetrydynamicconfigfetchconfigs"></a>Office.Telemetry.DynamicConfig.FetchConfigs

Datele necesare pentru a măsura starea de funcționare a Serviciului de configurare telemetrie.

Se colectează următoarele câmpuri:

  - **ParsedConfigCount** - numărul de configurări dinamice analizate

  - **ParsedConfigs** - numărul de configurări dinamice analizate

  - **RejectedConfigCount** - numărul de configurări respinse

  - **RejectedConfigs** - numărul de configurări respinse

  - **RejectedConfigsList** - listă de configurări respinse cu separator virgulă.

### <a name="officetelemetrydynamicconfigparsejsonconfig"></a>Office.Telemetry.DynamicConfig.ParseJsonConfig

Datele necesare pentru a măsura starea de funcționare a Serviciului de configurare telemetrie

Se colectează următoarele câmpuri:

  - **ErrorMessage** - mesaj de eroare de analizare 

  - **NodeName** - nodul care nu a reușit să analizeze

### <a name="officetelemetrydynamicconfigpopulatedrequestignored"></a>Office.Telemetry.DynamicConfig.PopulatedRequestIgnored

Acest eveniment este generat atunci când nu reușim să configurăm canalul de configurare a telemetriei.

Acest eveniment nu colectează niciun câmp.

### <a name="officetelemetrydynamicconfigpopulatetreecalledagain"></a>Office.Telemetry.DynamicConfig.PopulateTreeCalledAgain

Datele necesare pentru a măsura starea de funcționare a Serviciului de configurare telemetrie.

Acest eveniment nu colectează niciun câmp.

### <a name="officetelemetryeventquarantined"></a>Office.Telemetry.EventQuarantined

Utilizat pentru a verifica dacă alte evenimente NSD funcționează corect.

Se colectează următoarele câmpuri:

  - **EventName** - nume eveniment în carantină

  - **Motivul** - motivul carantinei

### <a name="officetelemetryflusheventbuffer"></a>Office.Telemetry.FlushEventBuffer 

Raportează dimensiunea zonei tampon a evenimentului și poate indica erorile de telemetrie aferente utilizării unei zone tampon mari.

Se colectează următoarele câmpuri:

  - **EventCount** - numărul de evenimente din zona tampon

  - **FirstPassCount** - numărul primei treceri de evenimente

  - **SecondPassCount** - numărul celei de a doua treceri de evenimente

### <a name="officetelemetrygetfilteredpayloadsfromdisk"></a>Office.Telemetry.GetFilteredPayloadsFromDisk

Verifică anumite părți ale canalului de telemetrie moștenit funcționează pe platforme care încă îl utilizează.

Acest eveniment nu colectează niciun câmp.

### <a name="officetelemetryinvaliddatacontractname"></a>Office.Telemetry.InvalidDataContractName

Raportează implementări de telemetrie nevalide

Se colectează următoarele câmpuri:

  - **DataContractName** - numele contractului de date de telemetrie

  - **EventName** - numele evenimentului cu contract de date nevalid

  - **IsRuleEvent** - adevărat/fals a fost acest eveniment implementat printr-o regulă de telemetrie

### <a name="officetelemetryinvaliddatafieldname"></a>Office.Telemetry.InvalidDataFieldName 

Raportează implementări de telemetrie nevalide

Se colectează următoarele câmpuri:

  - **DataFieldName** - numele câmpului de date de telemetrie

  - **EventName** - numele evenimentului cu câmpul nevalid

  - **IsRuleEvent** - adevărat/fals a fost acest eveniment implementat printr-o regulă de telemetrie.

### <a name="officetelemetryinvalideventcontractname"></a>Office.Telemetry.InvalidEventContractName 

Raportează implementări de telemetrie nevalide

Se colectează următoarele câmpuri:

  - **EventContractName** - numele contractului de telemetrie nevalid

  - **EventName** - numele evenimentului cu numele de contract nevalid

  - **IsRuleEvent** - adevărat/fals a fost acest eveniment implementat printr-o regulă de telemetrie

### <a name="officetelemetryloadxmlrules"></a>Office.Telemetry.LoadXmlRules

Raportează dacă regulile de telemetrie de analiză au reușit

Se colectează următoarele câmpuri:

  - **DetachedDuration** - durata detașată în microsecunde

### <a name="officetelemetrymissingfielddetails"></a>Office.Telemetry.MissingFieldDetails

Raportează informațiile din câmpul lipsă pentru a diagnostica greșeli de ortografie din configurația telemetriei.

Se colectează următoarele câmpuri:

  - **ErrorRuleId** - ID-ul regulii de telemetrie care a solicitat câmpul lipsă

  - **ErrorRuleVersion** - versiunea regulii de telemetrie care a solicitat câmpul lipsă

  - **EtwEventGuid** - GUID-ul ETW al câmpului solicitat

  - **EtwEventId** - ID-ul de eveniment ETW al câmpului solicitat

  - **MissingFieldName** - numele câmpului solicitat

  - **UlsTagId** - eticheta de cod a câmpului lipsă

### <a name="officetelemetryprocessidlequeuejob"></a>Office.Telemetry.ProcessIdleQueueJob

Raportează faptul că procesarea inactivă a telemetriei a început conform așteptărilor.

Se colectează următoarele câmpuri:

  - **DetachedDuration** - durata detașată în microsecunde

  - **FailureDiagnostic** - operația nereușită

### <a name="officetelemetryredstoneinboxsampling"></a>Office.Telemetry.RedstoneInboxSampling

Starea de eșantionare a clientului obligatorie pentru a interpreta corect alte măsurători.

Se colectează următoarele câmpuri:

  - **MeasuresEnabled** - sunt măsurile activate în această sesiune?

  - **SamplingClientIdValue** - valoare de eșantionare pentru acest client

  - **SamplingKey** - cheie de eșantionare pentru acest client

  - **SamplingMethod** - metodă de eșantionare pentru acest client

### <a name="officetelemetryredstoneinboxsamplingcritical"></a>Office.Telemetry.RedstoneInboxSamplingCritical

Starea de eșantionare a clientului poate fi necesară pentru a interpreta corect alte măsurători.

Se colectează următoarele câmpuri:

  - **MeasuresEnabled** - sunt măsurile activate în această sesiune?

  - **SamplingClientIdValue** - valoare de eșantionare pentru acest client

  - **SamplingKey** - cheie de eșantionare pentru acest client

  - **SamplingMethod** - metodă de eșantionare pentru acest client

### <a name="officetelemetryruleerrorsaggregated"></a>Office.Telemetry.RuleErrorsAggregated

Raportarea erorilor privind starea de funcționare a telemetriei. Obligatoriu pentru a valida alte date (inclusiv NSD).

Se colectează următoarele câmpuri:

  - **ErrorCount** - numărarea acestei erori în fereastra de timp de agregare

  - **ErrorInfo** - numărul de informații de diagnosticare a erorii

  - **ErrorRuleId** - ID-ul regulii de telemetrie care a cauzat eroarea

  - **ErrorRuleVersion** - versiunea regulii de telemetrie care a cauzat eroarea

  - **WarningInfo** - număr informații de diagnosticare avertisment

<!-- end list -->

  - **QueueFlushCount** - numărul de goliri ale cozii de așteptare

  - **QueueFlushDueToSizeLimit** - dimensiunea la care telemetria golește coada de așteptare

  - **QueueFlushesDueToSize** - numărul de goliri ale cozii de așteptare cauzate de dimensiunea zonei tampon

  - **QueueHardLimit** - limită de închidere telemetrie

  - **QueueLimitHitTime** - când s-a atins limita de închidere

  - **ResultTime** - ora acestui eveniment

### <a name="officetelemetryrulesenginediskthrottled"></a>Office.Telemetry.RulesEngineDiskThrottled

Limitare măsurători DQ. Este obligatoriu pentru a avea încredere în toate celelalte date.

Se colectează următoarele câmpuri:

  - **DiskWriteLimit** - limita dimensiunii pe disc pentru datele de telemetrie

  - **DiskWriteTotal** - total scriere pe disc pentru datele de telemetrie

  - **SessionDiskWriteTotal** - total scriere pe disc sesiune pentru datele de telemetrie

  - **ThrottlingTimestamp** - ora la care a fost limitată sesiunea

### <a name="officetelemetryrulesenginemediumcostthrottled"></a>Office.Telemetry.RulesEngineMediumCostThrottled

Limitare măsurători DQ. Este obligatoriu pentru a avea încredere în toate celelalte date.

Acest eveniment nu colectează niciun câmp.

### <a name="officetelemetryrulesenginespikethrottled"></a>Office.Telemetry.RulesEngineSpikeThrottled

Limitare măsurători DQ. Este obligatoriu pentru a avea încredere în toate celelalte date.

Se colectează următoarele câmpuri:

  - **CurrentLimit** - limită efect tranzitoriu curent

  - **Duration** - durată efect tranzitoriu

  - **Factor** - factor efect tranzitoriu

  - **HighestImpactingRuleBytes** - cea mai mare cantitate de octeți înregistrată printr-o regulă de telemetrie

  - **HighestImpactingRuleId** -ID-ul regulii care a înregistrat cei mai mulți octeți

  - **HighestImpactingRuleVersion** - versiunea regulii care a înregistrat cei mai mulți octeți

  - **MaxLimit** - limita maximă

  - **ThrottlingTimestamp** - când a fost limitată telemetria

### <a name="officetelemetryrulesenginethrottled"></a>Office.Telemetry.RulesEngineThrottled

Limitare măsurători DQ. Este obligatoriu pentru a avea încredere în toate celelalte date.

Se colectează următoarele câmpuri:

  - **ThrottlingTimestamp** - când a fost limitată telemetria

### <a name="officetelemetryrulesengineulsqueuesizebackgroundprocessinglevelreached"></a>Office.Telemetry.RulesEngineUlsQueueSizeBackgroundProcessingLevelReached

Raportează faptul că există prea multe evenimente în coada de așteptare pentru a procesa în perioada de inactivitate a aplicației.

Se colectează următoarele câmpuri:

  - **BackgroundProcessingLevelInBytes** - dimensiunea cozii de așteptare pentru pornirea procesării în fundal.

  - **CurrentQueueSize** - numărul de evenimente din coada de așteptare nULS.

  - **CurrentQueueSizeInBytes** - dimensiunea cozii de așteptare nULS în octeți.

  - **ReachedTimestamp** - ora la care a început procesarea în fundal.

### <a name="officetelemetryrulesresultuploadlatencyrule"></a>Office.Telemetry.RulesResultUploadLatencyRule

Latență de încărcare medie, minimă și maximă a regulii duce la încărcarea sarcinii în fiecare oră

Se colectează următoarele câmpuri:

  - **AverageLatency** - latență medie de încărcare.

  - **CollectionTime** - ora la care au fost colectate datele privind încărcarea regulii.

  - **LatencyGE201LE400** - numărul de încărcări cu o latență mai mare sau egală cu 201ms și mai mică sau egală cu 400ms

  - **LatencyGE3001** - numărul de încărcări cu o latență mai mare sau egală cu 3001ms.

  - **LatencyGE401LE600** - numărul de încărcări cu o latență mai mare sau egală cu 401ms și mai mică sau egală cu 600ms

  - **LatencyGE601LE800** - numărul de încărcări cu o latență mai mare sau egală cu 601ms și mai mică sau egală cu 800ms

  - **LatencyLE200** - numărul de încărcări cu o latență mai mică de 200 milisecunde.

  - **MaxLatency** - cea mai mare latență observată.

  - **MinLatency** - cea mai mică latență observată.

### <a name="officetelemetrysamplingpolicy"></a>Office.Telemetry.SamplingPolicy

Starea de eșantionare a clientului obligatorie pentru a interpreta corect alte măsurători.

Se colectează următoarele câmpuri:

  - **MeasuresEnabled** - sunt măsurile activate în această sesiune?

  - **SamplingClientIdValue** - valoare de eșantionare pentru acest client

  - **SamplingKey** - cheie de eșantionare pentru acest client

  - **SamplingMethod** - metodă de eșantionare pentru acest client

### <a name="officetelemetrysamplingpolicyeventtrigger"></a>Office.Telemetry.SamplingPolicyEventTrigger

Starea de eșantionare a clientului obligatorie pentru a interpreta corect alte măsurători.

Se colectează următoarele câmpuri:

  - **MeasuresEnabled** - sunt măsurile activate în această sesiune?

  - **SamplingKey** - cheie de eșantionare pentru acest client

  - **SamplingMethod** - metodă de eșantionare pentru acest client

### <a name="officetelemetrysessiontelemetryruleschanged"></a>Office.Telemetry.SessionTelemetryRulesChanged

Raportează faptul că setul de reguli de telemetrie s-a modificat

Se colectează următoarele câmpuri:

  - **ChangedRuleId** - ID-ul regulii de telemetrie care s-a modificat în actualizarea curentă

  - **ChangedRuleVersion** - Versiunea regulii de telemetrie care s-a modificat în actualizarea curentă

  - **OperationType** - adăugarea sau eliminarea eticheta de operații

### <a name="officetelemetrysessiontelemetryrulescount"></a>Office.Telemetry.SessionTelemetryRulesCount

Raportează numărul de reguli de telemetrie încărcate

Se colectează următoarele câmpuri:

  - **CountOfLoadedRules** - câte reguli de telemetrie sunt încărcate

  - **HadRuleFileAtBoot** - dacă a existat un fișier cu reguli de telemetrie la pornirea aplicației

### <a name="officetelemetrysessiontelemetryrulesinitialstate"></a>Office.Telemetry.SessionTelemetryRulesInitialState

Raportează regulile de telemetrie care au fost încărcate la pornirea sesiunii

Se colectează următoarele câmpuri:

  - **HadRuleFileAtBoot** - dacă a existat un fișier cu reguli de telemetrie la pornirea aplicației

  - **LoadedRulesCount** - câte reguli de telemetrie sunt încărcate

  - **LoadedRulesList** - lista de reguli de telemetrie încărcate

### <a name="officetelemetrysystemhealthmetadatanetworkcost"></a>Office.Telemetry.SystemHealthMetadataNetworkCost

Costul rețelei arată capacitatea noastră de a obține sau nu date.

Se colectează următoarele câmpuri:

  - **NetworkCost** - noul cost contorizat sau necontorizat al rețelei

  - **OldNetworkCost** - costul anterior contorizat sau necontorizat al rețelei

  - **Tag** - eticheta codului-sursă care a detectat modificarea

### <a name="officetelemetrysystemhealthmetadatanetworkcostchange"></a>Office.Telemetry.SystemHealthMetadataNetworkCostChange

Costul rețelei arată capacitatea noastră de a obține sau nu date.

Se colectează următoarele câmpuri:

  - **NewNetworkCost** - noul cost contorizat sau necontorizat al rețelei

  - **OldNetworkCost** - costul anterior contorizat sau necontorizat al rețelei

  - **Tag** - eticheta codului-sursă care a detectat modificarea

### <a name="officetelemetrytelemetryactivityaggregationwindowstatistics"></a>Office.Telemetry.TelemetryActivityAggregationWindowStatistics

Raportează numărul grupurilor de activitate agregate și de instanțe din fiecare activitate care este încărcat.

Se colectează următoarele câmpuri:

  - **GroupCount** - numărul de activități agregate care trimit date.

  - **InstancesToSend** - numărul de instanțe ale activităților agregate care trimit date.

### <a name="officetelemetrytelemetryulsqueueusage"></a>Office.Telemetry.TelemetryUlsQueueUsage

Raportarea erorilor privind starea de funcționare a telemetriei. Obligatoriu pentru a valida alte date (inclusiv NSD).

Se colectează următoarele câmpuri:

  - **AverageEventCount** - număr mediu de evenimente în coada de așteptare

  - **AverageQueueCB** - dimensiunea medie a memoriei cozii de așteptare

  - **PeakEventCount** - număr maxim de evenimente în coada de așteptare

  - **PeakQueueCB** - dimensiunea maximă a memoriei cozii de așteptare

  - **QueueDisableRuleLimit** - limită la care regulile de telemetrie se dezactivează

### <a name="officetelemetryulsqueuetopthrottlingtags"></a>Office.Telemetry.UlsQueueTopThrottlingTags

Raportează etichetele de nivel superior care au contribuit la închiderea cozii de așteptare ULS.

Se colectează următoarele câmpuri:

  - **Tag0 -** eticheta care a consumat cea mai mare parte a cozii de așteptare

  - **Tag0Percent -** procentul din coada de așteptare utilizat de tag0

  - **Tag1 -** eticheta care a consumat a 2-a cea mai mare parte din coada de așteptare

  - **Tag10 -** eticheta care a consumat a 11-a cea mai mare parte din coada de așteptare

  - **Tag10Percent -** procentul din coada de așteptare utilizat de tag10

  - **Tag11 -** eticheta care a consumat a 12-a cea mai mare parte din coada de așteptare

  - **Tag11Percent -** procentul din coada de așteptare utilizat de tag11

  - **Tag12 -** eticheta care a consumat a 13-a cea mai mare parte din coada de așteptare

  - **Tag12Percent -** procentul din coada de așteptare utilizat de tag12

  - **Tag13 -** eticheta care a consumat a 14-a cea mai mare parte din coada de așteptare

  - **Tag13Percent -** procentul din coada de așteptare utilizat de tag13

  - **Tag14 -** eticheta care a consumat a 15-a cea mai mare parte din coada de așteptare

  - **Tag14Percent -** procentul din coada de așteptare utilizat de tag14

  - **Tag1Percent -** procentul din coada de așteptare utilizat de tag1

  - **Tag2 -** eticheta care a consumat a 3-a cea mai mare parte din coada de așteptare

  - **Tag2Percent -** procentul din coada de așteptare utilizat de tag2

  - **Tag3 -** eticheta care a consumat a 4-a cea mai mare parte din coada de așteptare

  - **Tag3Percent -** procentul din coada de așteptare utilizat de tag3

  - **Tag4 -** eticheta care a consumat a 5-a cea mai mare parte din coada de așteptare

  - **Tag4Percent -** procentul din coada de așteptare utilizat de tag4

  - **Tag5 -** eticheta care a consumat a 6-a cea mai mare parte din coada de așteptare

  - **Tag5Percent -** procentul din coada de așteptare utilizat de tag5

  - **Tag6 -** eticheta care a consumat a 7-a cea mai mare parte din coada de așteptare

  - **Tag6Percent -** procentul din coada de așteptare utilizat de tag6

  - **Tag7 -** eticheta care a consumat a 8-a cea mai mare parte din coada de așteptare

  - **Tag7Percent -** procentul din coada de așteptare utilizat de tag7

  - **Tag8 -** eticheta care a consumat a 9-a cea mai mare parte din coada de așteptare

  - **Tag8Percent -** procentul din coada de așteptare utilizat de tag8

  - **Tag9 -** eticheta care a consumat a 10-a cea mai mare parte din coada de așteptare

  - **Tag9Percent -** procentul din coada de așteptare utilizat de tag9

### <a name="officetelemetryvolumetrackingdata"></a>Office.Telemetry.VolumeTrackingData

Măsurători de urmărire a volumului evenimentului pentru evenimentele de telemetrie

Se colectează următoarele câmpuri:

  - **EventThreshold** - numărul maxim de instanțe ale unui eveniment unic, care pot fi trimise într-o fereastră de timp.

  - **HighestEventCount** - cel mai mare număr de instanțe ale unui eveniment unic trimise în această fereastră.

  - **HighestEventName** - numele evenimentului cu cel mai mare număr de instanțe din această fereastră.

  - **TimeWindowInSeconds** - durata ferestrei în secunde.

  - **TotalEvents** - numărul total de evenimente trimise în timpul acestei ferestre.

  - **UniqueEvents** - numărul de evenimente unice trimise în timpul unei ferestre.

### <a name="officetelemetrywritepayloadstodisk"></a>Office.Telemetry.WritePayloadsToDisk

Verifică dacă anumite părți ale canalului moștenit funcționează pe platforme care încă îl utilizează.

Se colectează următoarele câmpuri:

  - **DetachedDuration** - durata detașată în microsecunde
