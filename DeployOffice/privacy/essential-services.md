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
ms.openlocfilehash: 6dede4fdc57074aa5a9daaf28a20a736c813d626
ms.sourcegitcommit: 0e2ec395ca334719883a7a48b5313a72217f2eab
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/11/2021
ms.locfileid: "52907366"
---
# <a name="essential-services-for-office"></a>Servicii esențiale pentru Office

> [!NOTE]
> Pentru o listă de produse Office care sunt reglementate de aceste informații despre confidențialitate, consultați [Controale de confidențialitate disponibile pentru produsele Office](products-versions-privacy-controls.md).

Office constă din aplicațiile software client și experiențe conectate proiectate pentru a vă permite să creați, să comunicați și să colaborați mai eficient. Deși puteți controla multe dintre experiențele conectate care sunt la dispoziția dvs. sau a utilizatorilor dvs. în cazul în care sunteți administratorul organizației dvs., există un set de servicii care sunt esențiale pentru modul în care funcționează Office și care, prin urmare, nu pot fi dezactivate. De exemplu, serviciul de licențiere care confirmă că aveți licența corectă pentru a utiliza Office. Datele de serviciu necesare cu privire la aceste servicii sunt colectate și trimise la Microsoft, indiferent ce alte setări de politică privind confidențialitatea ați configurat.

Pentru mai multe informații, consultați articolele de mai jos:

- [Date de serviciu obligatorii pentru Office](required-service-data.md)
- [Experiențe conectate în Office](connected-experiences.md)

Dacă sunteți administratorul organizației dvs., v-ar putea interesa și următoarele articole:

- [Prezentare generală a controalelor de confidențialitate pentru Aplicații Microsoft 365 pentru întreprindere](overview-privacy-controls.md)
- [Utilizați setările de politică pentru a gestiona controale de confidențialitate pentru Aplicații Microsoft 365 pentru întreprindere](manage-privacy-controls.md)
- [Utilizați preferințele pentru a gestiona controalele de confidențialitate ale Office pentru Mac](mac-privacy-preferences.md)
- [Utilizați preferințele pentru a gestiona controalele de confidențialitate ale Office pe dispozitivele iOS.](ios-privacy-preferences.md)
- [Utilizați setările de politică pentru a gestiona controale de confidențialitate pentru Office pe dispozitivele Android](android-privacy-controls.md)
- [Utilizarea setărilor de politică pentru a gestiona controalele de confidențialitate pentru Office pentru aplicațiile web](office-web-privacy-controls.md)

## <a name="list-of-essential-services-for-office"></a>Listă de servicii esențiale pentru Office 

Următorul tabel conține o listă a serviciilor esențiale pentru Office și o descriere a fiecărui serviciu.

| **Serviciu**  | **Descriere**  |
| ------ | ---- |
| [Autentificare](#authentication-events) | Autentificare este un serviciu multi-platformă care validează identitatea dvs. de utilizator Office. Acesta este necesar pentru a vă permite să vă conectați la Office, să vă activați licența de Office și să vă accesați fișierele stocate în cloud; oferă o experiență unitară la nivelul sesiunilor de Office și al dispozitivelor dvs.    |
| [Clic și Pornire](#click-to-run-events) | Clic și Pornire este tehnologia de instalare utilizată pentru a instala și a actualiza Office pe Windows. Aceasta caută noi versiuni de Office și, atunci când este disponibilă o nouă versiune, o descarcă și o instalează.  Clic și Pornire va detecta dacă sunt necesare actualizări Office, inclusiv actualizări de securitate, le va descărca și le va instala.     |
| [Serviciul de configurație avansată (ECS)](#enhanced-configuration-service-ecs-events) | ECS oferă Microsoft capacitatea de a reconfigura instalările Office fără a fi nevoie să implementați din nou Office. Este utilizat pentru a controla implementarea treptată de caracteristici sau actualizări, în timp ce impactul implementării este monitorizat pe baza datelor de diagnosticare colectate. Este utilizat, de asemenea, pentru a atenua problemele de securitate sau de performanță cu o caracteristică sau actualizare. În plus, ECS acceptă modificările de configurare legate de datele de diagnosticare pentru a vă ajuta să vă asigurați că evenimentele corespunzătoare sunt colectate. |
| [Licențiere](#licensing-events)     | Licențiere este un serviciu bazat pe cloud care acceptă activarea Office pentru noile instalări și păstrează licența pe dispozitivele dvs. după ce Office a fost activat. Acesta înregistrează fiecare dintre dispozitivele dvs. și activează Office, verifică starea abonamentului Office și gestionează cheile de produs.    |
|[Microsoft AutoUpdate (MAU)](#microsoft-autoupdate-mau-events)|Microsoft AutoUpdate (MAU) este tehnologia utilizată pentru actualizarea aplicațiilor Microsoft produse pentru macOS, cum ar fi Office. MAU va detecta dacă sunt necesare actualizări ale aplicațiilor, inclusiv actualizări de securitate, le va descărca și le va instala.|
|[Sincronizare OneNote](#onenote-sync-events)|OneNote pentru Mac acceptă doar blocnotesurile stocate pe internet în OneDrive sau SharePoint Online. OneNote pentru Mac sincronizează continuu toate notele utilizatorului cu OneDrive sau SharePoint Online. Acest lucru le permite utilizatorilor să deschidă, să vizualizeze și să editeze blocnotesurile de pe toate dispozitivele, astfel încât blocnotesurile lor să fie întotdeauna actualizate.
 [Configurare servicii](#services-configuration-events)  | Configurare servicii oferă capacitatea de a efectua actualizări la setările de configurare Office pentru a activa sau a dezactiva caracteristici client. Este apelat de fiecare dată când pornește o aplicație Office și oferă detalii despre alte configurații și servicii Office. Configurare servicii controlează, de asemenea, ce servicii sunt desemnate ca servicii esențiale.  |
| [Telemetrie ](#telemetry-events)  | Serviciul de telemetrie este utilizat pentru a colecta date de diagnosticare din aplicațiile Office. Acesta permite colectarea datelor de diagnosticare generate de Office, atât datele de diagnosticare obligatorii, cât și cele opționale. De asemenea, este responsabil pentru colectarea unor date de serviciu necesare pentru Office.  |

## <a name="events-and-data-fields-for-essential-services-for-office"></a>Evenimente și câmpuri de date pentru servicii esențiale pentru Office

Secțiunile următoare furnizează următoarele informații:

- O listă de evenimente pentru fiecare serviciu esențial
- O descriere a fiecărui eveniment
- O listă de câmpuri de date în fiecare eveniment
- O descriere a fiecărui câmp de date


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

  - **Duration_Max** - dacă acest semnal este agregat, durata maximă a oricărui eveniment agregat.

  - **Duration_Min** - dacă acest semnal este agregat, durata minimă a oricărui eveniment agregat.

  - **Duration_Sum** - dacă acest semnal este agregat, suma duratelor tuturor evenimentelor agregate.

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

  - **Microsoft\_ADAL\_broker\_app\_used** - menționează numele brokerului (de exemplu, Windows Account Management)

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

  - **Microsoft\_ADAL\_http\_event\_coun** t - numărul de apeluri HTTP efectuate de ADAL.

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

  - **Microsoft_ADAL_was_request_throttled** – adevărat/fals indicând dacă acest eveniment a fost accelerat de ADAL din cauza prea multor solicitări.
 
  - **Microsoft\_ADAL\_x\_ms\_request\_id** - ID solicitare suplimentar furnizat în antetul HTTP la serviciu de către ADAL.

  - **Platform** - Win32/WinRT/Android/iOS/Mac

  - **Promptreasoncorrelationid** – pentru solicitări, acesta este ID-ul de corelare a unui alt eveniment, care explică de ce utilizatorul poate vedea o solicitare de autentificare.

  - **Resource** – resursa pentru care utilizatorul solicită un simbol, cum ar fi Exchange sau SharePoint.

  - **Scenarioid** - GUID. Mai multe evenimente pot aparține unui singur scenariu, de exemplu, scenariul poate fi adăugarea unui cont nou, dar există mai multe solicitări care apar ca parte a scenariului respectiv. Acest ID permite corelarea.

  - **Scenarioname** – numele scenariului căruia îi aparține acest eveniment de autentificare.

  - **Sessionid** - GUID de identificare a sesiunii de pornire

  - **Skdver** - versiune de MATS client SDK utilizată pentru a produce aceste date

  - **Starttime** - ora la care a fost apelată Acțiunea de\*Începere MATS API

  - **Tenantid** - GUID de identificare a entității găzduite căreia îi aparține utilizatorul autentificat (în cazuri non-ADAL).

  - **Uploadid** - GUID unic pentru acest eveniment, utilizat pentru deduplicare

  - **Wamapi** - identifică ce WAM API este apelat

  - **Wamtelemetrybatch** - momentan neutilizat. În viitor, permite componentei WAM să expedieze informații suplimentare referitoare la evenimentul de autentificare.


### <a name="officematsoneauthactionmicrosoftofficewin32"></a>Office.MATS.OneAuth.ActionMicrosoftOfficeWin32

Microsoft Auth Telemetry System (MATS) este colectat atunci când Office încearcă să obțină un simbol de autentificare, fie în mod silențios, fie prin solicitare. Atunci când încercările de achiziționare eșuează, sunt incluse informații de eroare. Aceste evenimente ajută utilizatorii să nu intre în stări de autentificare întreruptă după cum urmează:

1) Identifică dacă clienții pot obține cu succes un simbol de autentificare din serviciu sau dacă au intrat într-o stare de autentificare întreruptă.

2) Evaluați când anume au loc modificări la nivelul clientului sau al serviciilor, dacă acestea duc la regresii critice ale fiabilității și experienței de autentificare a utilizatorului

3) Atunci când apar erori, aceste semnale emit coduri de eroare importante de la componenta responsabilă (cod de client Office, biblioteci de autentificare sau servicii de autoritate) care pot fi utilizate pentru triere, diagnosticare și atenuare

4) Aceste semnale alimentează diverse monitoare de pregătire pentru expediere și bună funcționare care declanșează avertizări pentru ca inginerii noștri să se implice rapid și să reducă timpul de atenuare a erorilor critice.

Se colectează următoarele câmpuri:

- **Accounttype** - tipul contului utilizat pentru acest eveniment de autentificare, de exemplu, consumator sau organizație.

- **Actionname** - numele prietenos pentru acest eveniment, dacă s-a furnizat unul.

- **Actiontype** - specifică tipul bibliotecii de autentificare în uz.

- **Appaudience** - este versiunea de aplicație pentru uz intern sau extern

- **Appforcedprompt** - a înlocuit aplicația memoria cache și a impus afișarea unei solicitări

- **Appname** - numele aplicației care efectuează autentificarea

- **Appver** - versiunea aplicației care efectuează autentificarea

- **Askedforcreds** - i-a solicitat aplicația utilizatorului să introducă acreditări pentru această acțiune

- **Authoutcome** - a reușit încercarea de autentificare, a eșuat sau a fost anulată

- **Blockingprompt** - a lansat aplicația o solicitare care necesită interacțiune cu utilizatorul

- **Correlationid** - identificatorul utilizat pentru a asocia informațiile despre acest eveniment individual cu datele de servicii

- **Count** - numărul total de acțiuni agregate care au fost raportate în acest eveniment de date.

- **Devicenetworkstate** - este dispozitivul conectat la internet.

- **Deviceprofiletelemetryid** - ID-ul de dispozitiv anonim, utilizat pentru a măsura experiența de autentificare și fiabilitatea la nivelul dispozitivului.

- **Duration** - cât a durat autentificarea

- **duration_max** - durata maximă a oricăruia dintre evenimentele agregate

- **duration_min** - durata minimă a oricăruia dintre evenimentele agregate

- **duration_sum** - suma duratei tuturor evenimentelor agregate

- **endtime** - când s-a terminat evenimentul de autentificare

- **error** - codul de eroare dacă autentificarea nu a reușit

- **errordescription** - scurtă descriere a erorii

- **errorsource** - a provenit eroarea de la serviciu, de la biblioteca de autentificare sau de la aplicație

- **eventtype** - este un eveniment care raportează un punct de date de autentificare sau un eveniment de eroare de calitate a datelor. Utilizat pentru a măsura calitatea datelor.

- **from_cache** - boolean care reprezintă dacă înregistrarea este din memoria cache de bază WAM sau din plugin

- **hasadaltelemetry** - indică dacă biblioteca de autentificare Azure Active Directory (ADAL) a furnizat telemetrie pentru acest eveniment.

- **Identityservice** - a fost invocat serviciul Microsoft Service Account (MSA) sau Azure Active Directory (AAD)

- **Interactiveauthcontainer** - ce tip de solicitare a fost afișată

- **Issilent** - a fost o solicitare afișată sau a fost un eveniment de autentificare silențioasă (în fundal)

- **Microsoft_ADAL_adal_version** - versiunea bibliotecii de autentificare Azure Active Directory (ADAL)

- **Microsoft_ADAL_api_error_code** - codul de eroare emis de biblioteca de autentificare pentru această încercare de autentificare

- **Microsoft_ADAL_api_id** - API invocat pentru această încercare de autentificare

- **Microsoft_ADAL_application_name** - numele aplicației / procesului care utilizează ADAL.

- **Microsoft_ADAL_application_version** - versiunea aplicației care utilizează ADAL.

- **Microsoft_ADAL_authority** - URL-ul autorității Azure Active Directory responsabil pentru autentificarea utilizatorului

- **Microsoft_ADAL_authority_type** - acordul de furnizare a serviciilor pentru consumator / Microsoft (MSA) vs Azure Active Directory (AAD) / de organizație; în prezent întotdeauna AAD

- **Microsoft_ADAL_authority_validation_status** - specifică dacă autentificarea a fost finalizată pe partea serviciului

- **Microsoft_ADAL_broker_app** - specifică dacă ADAL a utilizat un broker pentru autentificare

- **Microsoft_ADAL_broker_app_used** - specifică numele brokerului (de exemplu, Windows Account Management)

- **Microsoft_ADAL_broker_version** - specifică versiunea brokerului, dacă este utilizat

- **Microsoft_ADAL_cache_event_count** - numărul de evenimente cache efectuate de ADAL în timpul regăsirii simbolului

- **Microsoft_ADAL_cache_event_count_max** - dacă acest semnal este agregat, numărul maxim de evenimente cache ale oricăruia dintre evenimentele agregate

- **Microsoft_ADAL_cache_event_count_min** - dacă acest semnal este agregat, numărul minim de evenimente cache ale oricăruia dintre evenimentele agregate

- **Microsoft_ADAL_cache_event_count_sum** - dacă acest semnal este agregat, suma evenimentelor cache ale tuturor evenimentelor agregate

- **Microsoft_ADAL_cache_read_count** - de câte ori a citit API din cache-ul de pe disc. Prezent dacă a existat cel puțin o citire

- **Microsoft_ADAL_cache_read_error_count** - de câte ori a eșuat citirea cache de pe disc. Este prezent dacă a existat cel puțin o nereușită

- **Microsoft_ADAL_cache_read_last_error** - codul de eroare ADAL. Prezent dacă a existat cel puțin o citire nereușită

- **Microsoft_ADAL_cache_read_last_system_error** - codul de eroare de sistem.  Este prezent dacă a existat cel puțin o citire nereușită

- **Microsoft_ADAL_cache_write_count** - de câte ori a scris API în cache-ul de pe disc. Prezent dacă a existat cel puțin o scriere

- **Microsoft_ADAL_cache_write_error_count** - de câte ori a eșuat scrierea în cache-ul de pe disc. Prezent dacă a existat cel puțin o nereușită

- **Microsoft_ADAL_cache_write_last_error** - codul de eroare ADAL. Prezent dacă a existat cel puțin o scriere nereușită

- **Microsoft_ADAL_cache_write_last_system_error** - codul de eroare de sistem. Prezent dacă a existat cel puțin o scriere nereușită

- **Microsoft_ADAL_client_id** - ID aplicație Azure Active Directory hash

- **Microsoft_ADAL_device_id** - ID dispozitiv local generat de ADAL.

- **Microsoft_ADAL_error_domain** - domeniul/componenta care a generat codul de eroare.

- **Microsoft_ADAL_error_protocol_code** - codul de eroare de protocol OAuth returnat de serviciu, înregistrat de ADAL.

- **Microsoft_ADAL_extended_expires_on_setting** - specificarea adevărat/fals dacă simbolul are o durată de viață extinsă

- **Microsoft_ADAL_http_event_count** - numărul solicitărilor HTTP generate de ADAL.

- **Microsoft_ADAL_idp** - Furnizorul de identitate (idp) utilizat de ADAL.

- **Microsoft_ADAL_network_event_count** - contorizarea apelurilor de rețea efectuate de ADAL.

- **Microsoft_ADAL_http_event_count_max** - dacă acest semnal este agregat, numărul maxim de apeluri http efectuate de ADAL

- **Microsoft_ADAL_http_event_count_min** - dacă acest semnal este agregat, numărul minim de apeluri http efectuate de ADAL

- **Microsoft_ADAL_http_event_count_sum** - dacă semnalul este agregat, suma apelurilor http efectuate de ADAL

- **Microsoft_ADAL_network_event_count_max** - dacă acest semnal este agregat, numărul maxim de apeluri de rețea efectuate de ADAL din orice eveniment agregat

- **Microsoft_ADAL_network_event_count_min** - dacă acest semnal este agregat, numărul minim de apeluri de rețea efectuate de ADAL din orice eveniment agregat

- **Microsoft_ADAL_network_event_count_sum** - dacă acest semnal este agregat, suma apelurilor de rețea efectuate de ADAL din toate evenimentele agregate

- **Microsoft_ADAL_is_silent_ui** - specificarea adevărat/fals dacă UI a fost afișată (solicitare) de ADAL

- **Microsoft_ADAL_is_successfull** - specificarea adevărat/fals dacă ADAL API a reușit (macOS)

- **Microsoft_ADAL_is_successful** - specificarea adevărat/fals dacă ADAL API a reușit 

- **Microsoft_ADAL_logging_pii_enabled** - specificarea adevărat/fals dacă modul înregistrare în jurnal completă ADAL este activat. Aceste date sunt înregistrate în jurnal doar local, fără să fie emise în telemetrie

- **Microsoft_ADAL_ntlm** - specificarea adevărat/fals dacă ADAL a utilizat autentificarea de bază (NTLM).

- **Microsoft_ADAL_oauth_error_code** - codul de eroare de protocol OAuth returnată de serviciu

- **Microsoft_ADAL_prompt_behavior** - parametru de conectare sau niciunul transferat la serviciu pentru a specifica dacă interfața cu utilizatorul poate fi afișată

- **Microsoft_ADAL_request_id** - GUID tranzacțional pentru solicitarea emisă de ADAL pentru serviciu

- **Microsoft_ADAL_response_code** - codul de răspuns de rețea de la serviciu

- **Microsoft_ADAL_response_time** - cât timp a fost necesar serviciului pentru a reveni la ADAL

- **Microsoft_ADAL_response_time_max** - dacă semnalul este agregat, timpul maxim necesar pentru ca ADAL să revină de la API printre oricare dintre evenimentele agregate

- **Microsoft_ADAL_response_time_min** - dacă semnalul este agregat, timpul minim necesar serviciului pentru a răspunde la ADAL printre oricare dintre evenimentele agregate

- **Microsoft_ADAL_response_time_sum** - dacă semnalul este agregat, suma timpului necesar pentru ca ADAL să revină de la API printre toate evenimentele agregate

- **Microsoft_ADAL_rt_age** - vârsta simbolului de reîmprospătare

- **Microsoft_ADAL_server_error_code** - codul de eroare returnat de server

- **Microsoft_ADAL_server_sub_error_code** - subcodul de eroare returnată de server pentru a contribui la clarificarea motivului pentru care solicitarea nu a reușit

- **Microsoft_ADAL_spe_info** - specificarea adevărat/fals dacă utilizatorul a utilizat cercul interior Secure Production Enterprise (numai angajații Microsoft)

- **Microsoft_ADAL_spe_ring** - specificarea adevărat/fals dacă utilizatorul a utilizat cercul interior Secure Production Enterprise (numai angajații Microsoft)

- **Microsoft_ADAL_start_time** - ora la care a fost efectuat apelul ADAL API

- **Microsoft_ADAL_status** - starea de succes/eroare în invocația generală ADAL

- **Microsoft_ADAL_stop_time** - ora la care apelul ADAL API a fost returnat

- **Microsoft_ADAL_telemetry_pii_enabled** - specificarea adevărat/fals dacă modul de telemetrie completă ADAL este activat. Numele este un termen impropriu, deoarece nu sunt emise PII/EUII

- **Microsoft_ADAL_tenant_id** - un GUID care identifică entitatea găzduită căreia îi aparține utilizatorul autentificat

- **Microsoft_ADAL_token_acquisition_from_context** - descrie comportamentul ADAL pe baza simbolurilor din contextul de autentificare

- **Microsoft_ADAL_token_frt_status** - starea simbolului de reîmprospătare: dacă a fost încercat, nu este necesar, nu a fost găsit sau a fost șters.

- **Microsoft_ADAL_token_mrrt_status** - starea MultiResourceRefreshToken: dacă a fost încercat, nu este necesar, nu a fost găsit sau a fost șters.

- **Microsoft_ADAL_token_rt_status** - starea simbolului de reîmprospătare: dacă a fost încercat, nu este necesar, nu a fost găsit sau a fost șters.

- **Microsoft_ADAL_token_type** - simbolul de reîmprospătare (RT) sau simbolul de reîmprospătare cu resurse multiple (MRRT)

- **Microsoft_ADAL_ui_event_count** - numărul de solicitări afișate utilizatorului. Posibil să fi fost silențios

- **Microsoft_ADAL_user_cancel** - adevărat/fals dacă fereastra interfeței cu utilizatorul a fost anulată

- **Microsoft_ADAL_x_ms_request_id** - ID de solicitare suplimentară furnizat în antetul de rețea la serviciu de ADAL

- **Microsoft_ADAL_x_client_cpu** - informații despre arhitectura CPU a dispozitivului

- **Microsoft_ADAL_x_client_os** - versiunea sistemului de operare al dispozitivului.

- **Microsoft_ADAL_x_client_sku** - numele SKU pentru sistemul de operare al dispozitivului.

- **Microsoft_ADAL_x_client_ver** - versiunea bibliotecii ADAL.

- **MSAL_all_error_tags** - toate etichetele de eroare întâlnite de biblioteca de autentificare Microsoft (MSAL) în timpul fluxului de autentificare.

- **MSAL_api_error_code** - dacă MSAL întâlnește o eroare din sistemul de operare, codurile de eroare ale platformei sunt stocate aici.

- **MSAL_api_error_context** - șir ce conține detalii suplimentare ce poate fi citit de oameni despre ultima eroare MSAL întâlnită. 

- **MSAL_api_error_tag** - șir unic pentru locul în cod unde s-a produs eroarea.

- **MSAL_api_name** - numele API-ului de nivel superior MSAL, apelat pentru a porni acest flux de autentificare.

- **MSAL_api_status_code** - starea codului MSAL returnat pentru acest rezultat al fluxului de autentificare.

- **MSAL_auth_flow** - pașii MSAL încercați în timpul acestui flux de autentificare (AT, PRT, LRT, FRT, ART, IRT). Separat prin simbolul bară verticală „|” pentru analiză simplă.

- **MSAL_auth_flow_last_error** - codul de eroare primit de la server pe penultimul element din AuthFLow. (De exemplu: dacă AuthFlow = "PRT|LRT", eroarea PRT ar fi în AuthFlowLastError).

- **MSAL_authority_type** - a fost această solicitare pentru un utilizator: AAD, Federativ sau MSA.

- **MSAL_broker_app_used** - a fost folosită o aplicație broker în acest flux de autentificare.

- **MSAL_client_id** - ID-ul de client al aplicației de apelare

- **MSAL_correlation_id** - GUID unic pentru acest eveniment, utilizat pentru a asocia acțiunile din jurnalele de client, de server și de aplicații.

- **MSAL_delete_token** - lista simbolurilor care au fost șterse din memoria cache în timpul fluxului de autentificare.

- **MSAL_http_call_count** - numărul apelurilor HTTP efectuate de MSAL în timpul fluxului de autentificare.

- **MSAL_is_successful** - a fost fluxul de autentificare reușit.

- **MSAL_last_http_response_code** - dacă MSAL a efectuat unul sau mai multe apeluri HTTP, acesta este ultimul cod de răspuns HTTP primit.

- **MSAL_msal_version** - șir versiune MSAL, format X.X.X+(„OneAuth”, „local” sau un hash de comitere). 

- **MSAL_read_token** - simboluri citite din cache (AT, ART, FRT, LRT, IRT, PRT, EAT [EAT = AT-ul expirat a fost citit, dar a fost eliminat]).

- **MSAL_read_token_last_error** - dacă MSAL a întâlnit o eroare la citirea din cache, vom stoca informațiile aici. (De exemplu: eroare de citire disc din SO, eroare Portchei în macOS).

- **MSAL_request_duration** - cât a durat solicitarea de când s-a apelat API-ul de nivel superior MSAL, până când v-am returnat un rezultat.

- **MSAL_request_id** - ID-ul de solicitare pentru ultimul apel efectuat către serviciul de simbol de securitate Microsoft.

- **MSAL_server_error_code** - codul specific de eroare numeric al serviciului de simbol de securitate Microsoft, dacă am primit unul.

- **MSAL_server_spe_ring** - informațiile cercului Secure Production Enterprise al serviciului de simbol de securitate Microsoft, dacă le-am primit.

- **MSAL_server_suberror_code** - șir de cod specific de suberoare al serviciului de simbol de securitate Microsoft, dacă am primit unul.

- **MSAL_start_time** - ora la care a fost începută solicitarea MSAL la API-ul public de nivel superior.

- **MSAL_stop_time** - ora la care s-a finalizat procesarea solicitării și s-a returnat rezultatul apelantului.

- **MSAL_tenant_id** - GUID Microsoft care identifică entitatea găzduită în care există utilizatorul.

- **MSAL_ui_event_count** - numărul solicitărilor IU pe care le-a afișat MSAL pe ecran.

- **MSAL_wam_telemetry** - conține un lot de date de telemetrie WAM într-un șir JSON care va fi analizat și convertit la câmpurile din acest document care provin din WAM.

- **MSAL_was_request_throttled** - adevărat dacă MSAL a reglat această solicitare și a împiedicat-o să lovească rețeaua. Dacă acest lucru este vreodată adevărat, este cel mai probabil că există o buclă în aplicația de apelare.

- **MSAL_write_token** - simbolurile care au fost scrise în cache  (AT, ART, FRT, LRT, IRT, PRT, EAT [EAT = AT-ul expirat a fost citit, dar a fost eliminat]).

- **MSAL_write_token_last_error** - dacă MSAL a întâlnit o eroare la scrierea în cache, vom stoca informațiile aici. (De exemplu: eroare de citire disc din SO, eroare Portchei în macOS).

- **oneauth_api** - OneAuth API invocat pentru această încercare de autentificare.

- **oneauth_transactionuploadid** - GUID care specifică un apel individual către OneAuth API.

- **oneauth_version** - versiunea OneAuth SDK.

- **Platform** - Platforma sistemului de operare (0: Windows desktop, 1: Android, 2: iOS, 3: macOS, 4: UWP)

- **Promptreasoncorrelationid** - un identificator de corelare care poate fi utilizat pentru a căuta un eveniment de autentificare anterior, care este utilizat pentru a explica de ce i s-a solicitat utilizatorului să se autentifice.

- **Resource** - resursa pentru care se solicită un simbol.

- **Scenarioid** - mai multe evenimente pot aparține unui singur scenariu, de exemplu, scenariul poate fi adăugarea unui cont nou, dar există mai multe solicitări care apar ca parte a scenariului respectiv. Acest identificator activează corelarea acelor evenimente conexe.

- **Scenarioname** - numele scenariului de aplicație în care se solicită autentificarea, de exemplu, prima inițializare, verificarea licenței, etc.

- **Scope** - domeniul pentru care se solicită un simbol.

- **Sdkver** - versiunea bibliotecii de sisteme de telemetrie de autentificare Microsoft utilizată pentru a produce aceste date

- **Sessionid** - identificatorul pentru sesiunea de boot

- **Starttime** - ora la care a început evenimentul de autentificare.

- **Tenantid** - GUID de identificare a entității găzduite căreia îi aparține utilizatorul autentificat (în cazuri non-ADAL)

- **Uploadid** - GUID unic pentru acest eveniment, utilizat pentru deduplicare

- **wamapi** - identifică care API Web Account Management (WAM) este denumit

- **wamtelemetrybatch** - momentan neutilizat. În viitor, permite componentei WAM să expedieze informații suplimentare referitoare la evenimentul de autentificare

- **WAM_account_join_on_end** - starea asocierii contului la sfârșitul unei operațiuni WAM.  Valori posibile: „principal”, „secundar”, „not_joined”

- **WAM_account_join_on_start** - starea asocierii contului la începutul unei operațiuni WAM.  Valori posibile: „principal”, „secundar”, „not_joined”

- **WAM_api_error_code** - dacă a venit un răspuns de eroare de la pluginul AAD WAM, acest câmp va exista și va conține codul de eroare

- **WAM_authority** - șir ce conține URL-ul de autoritate—acesta ar trebui să fie punctul final login.windows.net utilizat

- **WAM_broker_version** - prezent, dacă a fost utilizat WAM, acesta este șirul de versiune de broker

- **WAM_cache_event_count** - numărul evenimentelor cache WAM în cadrul operațiunii

- **WAM_client_id** - identificator pentru asocierea la date de servicii, acest lucru identifică aplicația client.

- **WAM_correlation_id** - Identificator de asociere a evenimentelor cu datele serviciilor

- **WAM_device_join** - starea asocierii dispozitivului; valorile posibile sunt „aadj”, „haadj”

- **WAM_network_event_count** - prezent, dacă a avut loc cel puțin un apel de rețea; numărul apelurilor de rețea către serviciul pentru operațiunea WAM

- **WAM_network_status** - prezent, dacă a avut loc cel puțin un apel de rețea, conține un cod de eroare HTTP, dacă solicitarea de rețea nu a reușit.

- **WAM_idp** - specifică dacă a fost utilizat consumatorul WAM sau pluginul de autentificare de organizație.

- **WAM_is_cached** - specifică dacă răspunsul furnizat de WAM a fost preluat din cache.

- **WAM_oauth_error_code** - conține codul de eroare returnată de serviciu ca parte din protocolul OAuth.

- **WAM_prompt_behavior** - specifică dacă această solicitare este forțată de aplicație, sau, dacă această solicitare poate omite solicitarea dacă realizează autentificarea în mod silențios.

- **WAM_provider_id** - specifică punctul final Microsoft pentru autoritatea utilizată în scenariul de autentificare.

- **WAM_redirect_uri** - URL-ul de redirecționare înregistrat pentru aplicația în Azure Active Directory.

- **WAM_resource**  - resursa pentru care se solicită un simbol.

- **WAM_server_error_code** - codul de eroare returnată de serviciu către WAM.

- **WAM_server_sub_code** - un cod de eroare suplimentar utilizat pentru a descompune și mai mult cauzele erorii, returnat de serviciu.

- **WAM_silent_code** - codul de eroare întâmpinat de încercarea internă silențioasă WAM, înainte de a solicita utilizatorului.

- **WAM_silent_mats** - neutilizat.

- **WAM_silent_message** - mesajul de eroare asociat cu încercarea internă silențioasă efectuată de WAM, înainte de a solicita utilizatorului.

- **WAM_silent_status** - starea de succes/eroare pentru încercarea internă silențioasă efectuată de WAM, înainte de a solicita utilizatorului.

- **WAM_tenant_id** - un identificator pentru entitatea găzduită căreia îi aparține utilizatorul AAD autentificat, dacă este returnat de serviciu

- **WAM_ui_visible** - prezent dacă cel puțin o fereastră IU a fost afișată utilizatorului, fie „adevărat” sau „fals”

- **WAM_x_ms_clitelem** - prezent dacă serviciul returnează „x-ms-clitelem”


### <a name="officematsoneauthtransactionmicrosoftofficewin32"></a>Office.MATS.OneAuth.TransactionMicrosoftOfficeWin32

Microsoft Auth Telemetry System (MATS) este colectat atunci când Office încearcă să obțină un simbol de autentificare, fie în mod silențios, fie prin solicitare. Acest eveniment este părintele unuia sau a mai multor evenimente, permițând evenimentele conexe să fie grupate împreună. Aceste evenimente ajută utilizatorii să nu intre în stări de autentificare întreruptă după cum urmează:

1) Identifică dacă clienții pot obține cu succes un simbol de autentificare din serviciu sau dacă au intrat într-o stare de autentificare întreruptă.

2) Evaluați când anume au loc modificări la nivelul clientului sau al serviciilor, dacă acestea duc la regresii critice ale fiabilității și experienței de autentificare a utilizatorului

3) Atunci când apar erori, aceste semnale emit coduri de eroare importante de la componenta responsabilă (cod de client Office, biblioteci de autentificare sau servicii de autoritate) care pot fi utilizate pentru triere, diagnosticare și atenuare

4) Aceste semnale alimentează diverse monitoare de pregătire pentru expediere și bună funcționare care declanșează avertizări pentru ca inginerii noștri să se implice rapid și să reducă timpul de atenuare a erorilor critice.

Se colectează următoarele câmpuri:

- **Actiontype** - singura valoare este „oneauthtransaction”.

- **Appaudience** - public aplicație (automatizare, pre-producție sau producție)

- **Appname** - numele aplicației

- **Appver** - versiunea aplicației

- **Authoutcome** - a reușit încercarea de autentificare, a eșuat sau a fost anulată

- **Correlationid** - identificatorul utilizat pentru a asocia informațiile despre acest eveniment individual cu datele de servicii

- **Count** - de câte ori s-a produs eroarea

- **Devicenetworkstate** - starea de rețea a dispozitivului

- **Deviceprofiletelemetryid** - ID-ul de telemetrie a profilului pentru dispozitiv (șir utilizat de MATS pentru a identifica un anumit dispozitiv)

- **duration_max** - durata minimă, în milisecunde, a tranzacțiilor agregate pe acest semnal.

- **duration_min** - durata maximă, în milisecunde, a tranzacțiilor agregate pe acest semnal.

- **duration_sum** - suma duratei, în milisecunde, a tranzacțiilor agregate pe acest semnal.

- **Endtime** - ora la care s-a terminat tranzacția OneAuth.

- **Error** - codul stării OneAuth.

- **Eventtype** - tipul evenimentului

- **Issilent** - fals, dacă a fost afișat IU; adevărat, dacă a fost un eveniment de fundal.

- **oneauth_api** - specifică API-ul public de OneAuth care a fost invocat.

- **oneauth_Domain** - dacă apelul API a dus la o eroare, acesta este domeniul de sistem al acelei erori.

- **oneauth_ErrorCode** - codul de eroare care reprezintă starea de eroare internă pentru OneAuth. Înlocuiește câmpul vechi oneauth_errortag.

- **oneauth_errortag** - identificatorul numeric pentru o linie de cod, responsabilă pentru generarea unei erori.

- **oneauth_ExecutionFlow** - o serie de etichete care identifică calea de cod a invocației API.

- **oneauth_internalerror** - codul de eroare care reprezintă starea de eroare internă pentru OneAuth.

- **oneauth_ServerErrorCode** - eroare de server returnată la OneAuth la încheierea acestui apel API, dacă aceasta a avut loc.

- **oneauth_SystemErrorCode** - eroarea de sistem returnată la OneAuth la încheierea acestui apel API, dacă aceasta a avut loc.

- **oneauth_Tag** - eticheta OneAuth care desemnează locul final din cod, atins la încheierea acestui apel API.

- **oneauth_transactionuploadid** - specifică GUID-ul intern generat aleatoriu care mapează invocația specifică a unui API OneAuth.

- **oneauth_version** - versiunea OneAuth SDK.

- **Platform** - platforma SO (0: Win32, 1: Android, 2: iOS, 3: macOS, 4: WinRT

- **Scenarioname** - numele scenariului pentru care autentificarea este necesară, specificat de aplicația de apelare.

- **Schemaver** - versiunea schemei

- **Sdkver** - versiunea de MATS sdk

- **Sessionid** - ID-ul sesiunii

- **severityError** - severitatea

- **starttime** - ora la care a început tranzacția OneAuth.

- **Timestamp** - marca de timp

- **Type** - tipul erorii

- **Uploaded** - identificator unic pentru acest eveniment, pentru scopuri de duplicare.


### <a name="onenotesigninssoexternalappsaccountfound"></a>OneNote.SignIn.SSOExternalAppsAccountFound
 
Acest eveniment este înregistrat când un cont cu un simbol de reîmprospătare valid se află în lista de conturi furnizate de TokenSharingManager.  Acest scenariu este specific pentru Sign-on unic (SSO)
 
Se colectează următoarele câmpuri:
 
- **AccountType** - înregistrează tipul de cont

- **ProviderPackageID** - înregistrează ID-ul pachetului aplicației care a furnizat acest cont

### <a name="onenotesigninssoexternalappsinvalidaccount"></a>OneNote.SignIn.SSOExternalAppsInvalidAccount

Acest eveniment este înregistrat când a apărut o eroare în cazul unei tentative de obținere a simbolului de reîmprospătare pentru un cont din lista de conturi furnizată de TokenSharingManager. Acest scenariu este specific pentru Sign-on unic (SSO)
 
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

  - **Data\_ProductReleaseId** - produsul pe care îl instalăm, adică Aplicații Microsoft 365 pentru întreprindere

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

  - **Data\_Sku** - SKU-ul instalat, adică Aplicații Microsoft 365 pentru întreprindere

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

  - **Data\_ProductReleaseId** - produsul pe care îl instalăm, adică Aplicații Microsoft 365 pentru întreprindere

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

Datele despre instalare și inventar Office colectate atunci când programul de instalare Office plasează fișierele recent descărcate. Se utilizează pentru a măsura succesul/eșecul unei instalări Office.

Se colectează următoarele câmpuri:

  - **Data\_15\_SourceType -** unde se află sursa Office 15, adică CDN sau local 

  - **Data\_15\_UpdatesEnabled -** dacă sunt activate actualizările Office 15 

  - **Data\_15\_UpdateVersion -** la ce versiune Office 15 actualizăm 

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled -** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion-** ce versiune de Office 16 actualizați la 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** produsele pe care le adăugăm 

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

  - **Data\_ProductsToAdd -** ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează, adică instalare 

  - **Data\_ScenarioSubType -** Ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

  - **Data\_SourceType -** unde se află sursa noastră, adică CDN 

  - **Data\_SqmMachineID -** ID unic de computer utilizat de Windows SQM 

  - **Data\_SusClientID -** identificator de actualizare Office computer 

  - **Data\_TaskState -** care este starea activității, cum ar fi rulare sau anulat 

  - **Data\_TotalClientCabSize -** dimensiunea fișierului cab al clientului nostru 

  - **Data\_TriggeringUI -** ce a declanșat interfața cu utilizatorul 

  - **Data\_UpdatesEnabled -** dacă sunt activate actualizările Office 

  - **Data\_Version -** versiunea de Office 

### <a name="officeclicktorunscenarioinstalltaskconfigurelight"></a>Office.ClickToRun.Scenario.InstallTaskConfigurelight

Date despre instalări și inventar Office colectate atunci când programul de instalare Office stabilește ce fișiere trebuie descărcate. Utilizat pentru a măsura succesul/eșecul instalării Office.

Se colectează următoarele câmpuri:

  - **Data\_15\_SourceType -** unde se află sursa Office 15, adică CDN sau local 

  - **Data\_15\_UpdatesEnabled -** dacă sunt activate actualizările Office 15 

  - **Data\_15\_UpdateVersion -** la ce versiune Office 15 actualizăm 

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion-** ce versiune de Office 16 actualizați la 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** produsele pe care le adăugăm 

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

  - **Data\_ProductsToAdd -** ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName-** ce scenariu rulează. adică, instalare 

  - **Data\_ScenarioSubType -** Ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

  - **Data\_SourceType -** unde se află sursa noastră, adică CDN 

  - **Data\_SqmMachineID -** ID unic de computer utilizat de Windows SQM 

  - **Data\_SusClientID-** identificator de actualizare Office computer 

  - **Data\_TaskState -** care este starea activității, cum ar fi rulare sau anulat 

  - **Data\_TotalClientCabSize -** dimensiunea fișierului cab al clientului nostru 

  - **Data\_TriggeringUI -** ce a declanșat interfața cu utilizatorul 

  - **Data\_UpdatesEnabled -** dacă sunt activate actualizările Office 

  - **Data\_Version -** versiunea de Office 

### <a name="officeclicktorunscenarioinstalltaskfinalintegrate"></a>Office.ClickToRun.Scenario.InstallTaskFinalintegrate

Date despre instalări și inventar Office colectate atunci când programul de instalare Office instalează licențe și setări de registry. Utilizate pentru a măsura succesul/eșecul instalării Office.

Se colectează următoarele câmpuri:

  - **Data\_15\_SourceType -** unde se află sursa Office 15, adică CDN sau local 

  - **Data\_15\_UpdatesEnabled -** dacă sunt activate actualizările Office 15 

  - **Data\_15\_UpdateVersion -** la ce versiune Office 15 actualizăm

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled -** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion-** ce versiune de Office 16 actualizați la 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** produsele pe care le adăugăm 

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

  - **Data\_ProductsToAdd -** ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează, adică instalare 

  - **Data\_ScenarioSubType -** Ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

  - **Data\_SourceType -** unde se află sursa noastră, adică CDN 

  - **Data\_SqmMachineID -** ID unic de computer utilizat de Windows SQM 

  - **Data\_SusClientID-** identificator de actualizare Office computer 

  - **Data\_TaskState -** care este starea activității, cum ar fi rulare sau anulat 

  - **Data\_TotalClientCabSize -** dimensiunea fișierului cab al clientului nostru 

  - **Data\_TriggeringUI -** ce a declanșat interfața cu utilizatorul 

  - **Data\_UpdatesEnabled -** dacă sunt activate actualizările Office 

  - **Data\_Version -** versiunea de Office 

### <a name="officeclicktorunscenarioinstalltaskfonts"></a>Office.ClickToRun.Scenario.InstallTaskFonts

Date despre instalări și inventar Office colectate atunci când programul de instalare Office instalează fonturi. Utilizate pentru a măsura succesul/eșecul instalării Office.

Se colectează următoarele câmpuri:

  - **Data\_15\_SourceType -** unde se află sursa Office 15, adică CDN sau local 

  - **Data\_15\_UpdatesEnabled -** dacă sunt activate actualizările Office 15 

  - **Data\_15\_UpdateVersion -** la ce versiune Office 15 actualizăm 

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion-** ce versiune de Office 16 actualizați la 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** produsele pe care le adăugăm 

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

  - **Data\_ProductsToAdd -** ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează. adică, instalare

  - **Data\_ScenarioSubType -** Ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

  - **Data\_SourceType -** unde se află sursa noastră, adică CDN 

  - **Data\_SqmMachineID -** ID unic de computer utilizat de Windows SQM 

  - **Data\_SusClientID-** identificator de actualizare Office computer 

  - **Data\_TaskState -** care este starea activității, cum ar fi rulare sau anulat 

  - **Data\_TotalClientCabSize -** dimensiunea fișierului cab al clientului nostru 

  - **Data\_TriggeringUI -** ce a declanșat interfața cu utilizatorul 

  - **Data\_UpdatesEnabled -** dacă sunt activate actualizările Office 

  - **Data\_Version -** versiunea de Office 

### <a name="officeclicktorunscenarioinstalltaskinitupdates"></a>Office.ClickToRun.Scenario.InstallTaskInitupdates

Date despre instalări și inventar Office colectate atunci când programul de instalare Office creează setări pentru funcționarea corectă a actualizărilor. Utilizate pentru a măsura succesul/eșecul instalării Office. 

Se colectează următoarele câmpuri:

  - **Data\_15\_SourceType -** unde se află sursa Office 15, adică CDN sau local 

  - **Data\_15\_UpdatesEnabled -** dacă sunt activate actualizările Office 15 

  - **Data\_15\_UpdateVersion -** la ce versiune Office 15 actualizăm 

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion-** ce versiune de Office 16 actualizați la 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** produsele pe care le adăugăm 

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

  - **Data\_ProductsToAdd -** ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează, adică instalare

  - **Data\_ScenarioSubType -** Ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

  - **Data\_SourceType -** unde se află sursa noastră, adică CDN 

  - **Data\_SqmMachineID -** ID unic de computer utilizat de Windows SQM 

  - **Data\_SusClientID-** identificator de actualizare Office computer 

  - **Data\_TaskState -** care este starea activității, cum ar fi rulare sau anulat 

  - **Data\_TotalClientCabSize -** dimensiunea fișierului cab al clientului nostru 

  - **Data\_TriggeringUI -** ce a declanșat interfața cu utilizatorul 

  - **Data\_UpdatesEnabled -** dacă sunt activate actualizările Office 

  - **Data\_Version -** versiunea de Office 

### <a name="officeclicktorunscenarioinstalltaskintegrateinstall"></a>Office.ClickToRun.Scenario.InstallTaskIntegrateinstall

Date despre instalări și inventar Office colectate atunci când programul de instalare Office creează intrări de registry pentru aplicațiile Office Utilizate pentru a măsura succesul/eșecul instalării Office. 

Se colectează următoarele câmpuri:

  - **Data\_15\_SourceType -** unde se află sursa Office 15, adică CDN sau local 

  - **Data\_15\_UpdatesEnabled -** dacă sunt activate actualizările Office 15 

  - **Data\_15\_UpdateVersion -** la ce versiune Office 15 actualizăm

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion-** ce versiune de Office 16 actualizați la 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** produsele pe care le adăugăm 

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

  - **Data\_ProductsToAdd -** ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează, adică instalare 

  - **Data\_ScenarioSubType -** Ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

  - **Data\_SourceType -** unde se află sursa noastră, adică CDN 

  - **Data\_SqmMachineID -** ID unic de computer utilizat de Windows SQM

  - **Data\_SusClientID-** identificator de actualizare Office computer 

  - **Data\_TaskState -** care este starea activității, cum ar fi rulare sau anulat 

  - **Data\_TotalClientCabSize -** dimensiunea fișierului cab al clientului nostru 

  - **Data\_TriggeringUI -** ce a declanșat interfața cu utilizatorul 

  - **Data\_UpdatesEnabled -** dacă sunt activate actualizările Office 

  - **Data\_Version -** versiunea de Office 

### <a name="officeclicktorunscenarioinstalltasklastrun"></a>Office.ClickToRun.Scenario.InstallTaskLastrun

Date despre instalări și inventar Office colectate atunci când programul de instalare Office finalizează instalarea, fixează comenzi rapide și creează setări de registry finale. Utilizate pentru a măsura succesul/eșecul instalării Office. 

Se colectează următoarele câmpuri:

  - **Data\_15\_SourceType -** unde se află sursa Office 15, adică CDN sau local 

  - **Data\_15\_UpdatesEnabled -** dacă sunt activate actualizările Office 15 

  - **Data\_15\_UpdateVersion -** la ce versiune Office 15 actualizăm

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion-** ce versiune de Office 16 actualizați la 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** produsele pe care le adăugăm 

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

  - **Data\_ProductsToAdd -** ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează, adică instalare

  - **Data\_ScenarioSubType -** Ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

  - **Data\_SourceType -** unde se află sursa noastră, adică CDN 

  - **Data\_SqmMachineID -** ID unic de computer utilizat de Windows SQM

  - **Data\_SusClientID-** identificator de actualizare Office computer 

  - **Data\_TaskState -** care este starea activității, cum ar fi rulare sau anulat 

  - **Data\_TotalClientCabSize -** dimensiunea fișierului cab al clientului nostru 

  - **Data\_TriggeringUI -** ce a declanșat interfața cu utilizatorul 

  - **Data\_UpdatesEnabled -** dacă sunt activate actualizările Office 

  - **Data\_Version -** versiunea de Office 

### <a name="officeclicktorunscenarioinstalltaskmigrate"></a>Office.ClickToRun.Scenario.InstallTaskMigrate

Datele despre instalare și inventar Office colectate atunci când Office Installer migrează setări din versiuni mai vechi de Office. Se utilizează pentru a măsura succesul/eșecul instalării Office.

Se colectează următoarele câmpuri:

  - **Data\_15\_SourceType -** unde se află sursa Office 15, adică CDN sau local 

  - **Data\_15\_UpdatesEnabled -** dacă sunt activate actualizările Office 15 

  - **Data\_15\_UpdateVersion -** la ce versiune Office 15 actualizăm

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion-** ce versiune de Office 16 actualizați la 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** produsele pe care le adăugăm 

  - **Data\_AddingProducts -** Ce produse ni s-a solicitat să adăugăm 

  - **Data\_CompletionState -** dacă am finalizat activitatea

  - **Data\_ErrorCode -** codul de eroare cu care am eșuat 

  - **Data\_ErrorDetails -** detalii suplimentare despre o eroare 

  - **Data\_ErrorMessage -** mesaj de eroare despre ce nu a funcționat bine 

  - **Data\_ErrorSource – -** unde s-a produs eroarea

  - **Data\_ExceptionType -** excepția cu care am eșuat 

  - **Data\_IsErrorCodeIgnorable -** dacă codul de eroare cu care am eșuat poate fi ignorat 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth -** dacă considerăm că codul de eroare poate fi ignorat 

  - **Data\_NewestPackageVersion -** cea mai nouă versiune de Office de pe computer 

  - **Data\_OldestPackageVersion -** cea mai veche versiune de Office de pe computer 

  - **Data\_ProductsToAdd -** ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează, adică instalare

  - **Data\_ScenarioSubType -** Ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

  - **Data\_SourceType -** unde se află sursa noastră, adică CDN 

  - **Data\_SqmMachineID -** ID unic de computer utilizat de Windows SQM

  - **Data\_SusClientID -** identificator de actualizare Office computer

  - **Data\_TaskState -** care este starea activității, cum ar fi rulare sau anulat 

  - **Data\_TotalClientCabSize -** dimensiunea fișierului cab al clientului nostru 

  - **Data\_TriggeringUI -** ce a declanșat interfața cu utilizatorul 

  - **Data\_UpdatesEnabled -** dacă sunt activate actualizările Office 

  - **Data\_Version -** versiunea de Office 

### <a name="officeclicktorunscenarioinstalltaskpublishrsod"></a>Office.ClickToRun.Scenario.InstallTaskPublishrsod

Date despre instalări și inventar Office colectate atunci când programul de instalare Office publică registry virtual pentru nivelul de virtualizare AppV. Utilizate pentru a măsura succesul/eșecul instalării Office. 

Se colectează următoarele câmpuri:

  - **Data\_15\_SourceType -** unde se află sursa Office 15, adică CDN sau local 

  - **Data\_15\_UpdatesEnabled -** dacă sunt activate actualizările Office 15 

  - **Data\_15\_UpdateVersion -** la ce versiune Office 15 actualizăm

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion-** ce versiune de Office 16 actualizați la 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** produsele pe care le adăugăm 

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

  - **Data\_ProductsToAdd -** ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează, adică instalare 

  - **Data\_ScenarioSubType -** Ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

  - **Data\_SourceType -** unde se află sursa noastră, adică CDN 

  - **Data\_SqmMachineID -** ID unic de computer utilizat de Windows SQM

  - **Data\_SusClientID-** identificator de actualizare Office computer 

  - **Data\_TaskState -** care este starea activității, cum ar fi rulare sau anulat 

  - **Data\_TotalClientCabSize -** dimensiunea fișierului cab al clientului nostru 

  - **Data\_TriggeringUI -** ce a declanșat interfața cu utilizatorul 

  - **Data\_UpdatesEnabled -** dacă sunt activate actualizările Office 

  - **Data\_Version -** versiunea de Office 

### <a name="officeclicktorunscenarioinstalltaskremoveinstallation"></a>Office.ClickToRun.Scenario.InstallTaskRemoveinstallation

Date despre instalări și inventar Office colectate atunci când programul de dezinstalare Office elimină părți de Office de pe dispozitiv. Utilizat pentru a măsura succesul/eșecul instalării Office.

Se colectează următoarele câmpuri:

  - **Data\_15\_SourceType -** unde se află sursa Office 15, adică CDN sau local 

  - **Data\_15\_UpdatesEnabled -** dacă sunt activate actualizările Office 15 

  - **Data\_15\_UpdateVersion -** la ce versiune Office 15 actualizăm 

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion-** ce versiune de Office 16 actualizați la 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** produsele pe care le adăugăm 

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

  - **Data\_ProductsToAdd -** ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează, adică instalare 

  - **Data\_ScenarioSubType -** Ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

  - **Data\_SourceType -** unde se află sursa noastră, adică CDN 

  - **Data\_SqmMachineID -** ID unic de computer utilizat de Windows SQM

  - **Data\_SusClientID-** identificator de actualizare Office computer 

  - **Data\_TaskState -** care este starea activității, cum ar fi rulare sau anulat 

  - **Data\_TotalClientCabSize -** dimensiunea fișierului cab al clientului nostru 

  - **Data\_TriggeringUI -** ce a declanșat interfața cu utilizatorul 

  - **Data\_UpdatesEnabled -** dacă sunt activate actualizările Office 

  - **Data\_Version -** versiunea de Office 

### <a name="officeclicktorunscenarioinstalltaskstream"></a>Office.ClickToRun.Scenario.InstallTaskStream

Date despre instalări și inventar Office colectate atunci când programul de instalare Office cdescarcă noi fișiere pentru Office. Utilizate pentru a măsura succesul/eșecul instalării Office. 

Se colectează următoarele câmpuri:

  - **Data\_15\_SourceType -** unde se află sursa Office 15, adică CDN sau local 

  - **Data\_15\_UpdatesEnabled -** dacă sunt activate actualizările Office 15 

  - **Data\_15\_UpdateVersion -**  la ce versiune Office 15 actualizăm 

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled -** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion-** ce versiune de Office 16 actualizați la 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** produsele pe care le adăugăm 

  - **Data\_AddingProducts -** ce produse ni s-a solicitat să adăugăm 

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

  - **Data\_ProductsToAdd -** ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează, adică instalare 

  - **Data\_ScenarioSubType -** Ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

  - **Data\_SourceType -** unde se află sursa noastră, adică CDN 

  - **Data\_SqmMachineID -** ID unic de computer utilizat de Windows SQM 

  - **Data\_SusClientID -** identificator de actualizare Office computer 

  - **Data\_TaskState -** care este starea activității, cum ar fi rulare sau anulat 

  - **Data\_TotalClientCabSize -** dimensiunea fișierului cab al clientului nostru 

  - **Data\_TriggeringUI -** ce a declanșat interfața cu utilizatorul 

  - **Data\_UpdatesEnabled -** dacă sunt activate actualizările Office 

  - **Data\_Version -** versiunea de Office 

### <a name="officeclicktorunscenarioinstalltaskuninstallcentennial"></a>Office.ClickToRun.Scenario.InstallTaskUninstallcentennial

Date despre instalări și inventar Office colectate atunci când programul de instalare Office dezinstalează o versiune anterioară de Office din Store. Utilizate pentru a măsura succesul/eșecul instalării Office.

Se colectează următoarele câmpuri:

  - **Data\_15\_SourceType -** unde se află sursa Office 15, adică CDN sau local 

  - **Data\_15\_UpdatesEnabled -** dacă sunt activate actualizările Office 15 

  - **Data\_15\_UpdateVersion -** la ce versiune Office 15 actualizăm 

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion-** ce versiune de Office 16 actualizați la 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** produsele pe care le adăugăm 

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

  - **Data\_ProductsToAdd -** ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează, adică instalare 

  - **Data\_ScenarioSubType -** Ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

  - **Data\_SourceType -** unde se află sursa noastră, adică CDN 

  - **Data\_SqmMachineID -** ID unic de computer utilizat de Windows SQM

  - **Data\_SusClientID-** identificator de actualizare Office computer 

  - **Data\_TaskState -** care este starea activității, cum ar fi rulare sau anulat 

  - **Data\_TotalClientCabSize -** dimensiunea fișierului cab al clientului nostru 

  - **Data\_TriggeringUI -** ce a declanșat interfața cu utilizatorul 

  - **Data\_UpdatesEnabled -** dacă sunt activate actualizările Office 

  - **Data\_Version -** versiunea de Office 

### <a name="officeclicktorunscenariorepairtaskfinalintegrate"></a>Office.ClickToRun.Scenario.RepairTaskFinalintegrate

Date despre instalări și inventar Office colectate atunci când clientul de reparare Office publică din nou fișiere .msi și extensii Office. Utilizat pentru a măsura succesul/eșecul reparării Office.

Se colectează următoarele câmpuri:

  - **Data\_15\_SourceType -** unde se află sursa Office 15, adică CDN sau local 

  - **Data\_15\_UpdatesEnabled -** dacă sunt activate actualizările Office 15 

  - **Data\_15\_UpdateVersion -** la ce versiune Office 15 actualizăm 

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion-** ce versiune de Office 16 actualizați la 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** produsele pe care le adăugăm 

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

  - **Data\_ProductsToAdd -** ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează, adică instalare 

  - **Data\_ScenarioSubType -** Ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

  - **Data\_SourceType -** unde se află sursa noastră, adică CDN 

  - **Data\_SqmMachineID -** ID unic de computer utilizat de Windows SQM 

  - **Data\_SusClientID-** identificator de actualizare Office computer 

  - **Data\_TaskState -** care este starea activității, cum ar fi rulare sau anulat 

  - **Data\_TotalClientCabSize -** dimensiunea fișierului cab al clientului nostru 

  - **Data\_TriggeringUI -** ce a declanșat interfața cu utilizatorul 

  - **Data\_UpdatesEnabled -** dacă sunt activate actualizările Office 

  - **Data\_Version -** versiunea de Office 

### <a name="officeclicktorunscenariorepairtaskfullrepair"></a>Office.ClickToRun.Scenario.RepairTaskFullrepair

Date despre instalări și inventar Office colectate atunci când clientul de reparare Office descarcă cea mai recentă versiune a clientului Clic și Pornire, pentru a pregăti computerul pentru dezinstalare și reinstalare. Utilizate pentru a măsura succesul/eșecul reparării Office.

Se colectează următoarele câmpuri:

  - **Data\_15\_SourceType -** unde se află sursa Office 15, adică CDN sau local 

  - **Data\_15\_UpdatesEnabled -** dacă sunt activate actualizările Office 15 

  - **Data\_15\_UpdateVersion -** la ce versiune Office 15 actualizăm 

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion-** ce versiune de Office 16 actualizați la 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** produsele pe care le adăugăm 

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

  - **Data\_ProductsToAdd -** ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează, adică instalare 

  - **Data\_ScenarioSubType -** Ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

  - **Data\_SourceType -** unde se află sursa noastră, adică CDN 

  - **Data\_SqmMachineID -** ID unic de computer utilizat de Windows SQM 

  - **Data\_SusClientID-** identificator de actualizare Office computer 

  - **Data\_TaskState -** care este starea activității, cum ar fi rulare sau anulat 

  - **Data\_TotalClientCabSize -** dimensiunea fișierului cab al clientului nostru 

  - **Data\_TriggeringUI -** ce a declanșat interfața cu utilizatorul 

  - **Data\_UpdatesEnabled -** dacă sunt activate actualizările Office 

  - **Data\_Version -** versiunea de Office 

### <a name="officeclicktorunscenariorepairtaskintegraterepair"></a>Office.ClickToRun.Scenario.RepairTaskIntegraterepair

Date despre instalări și inventar Office colectate atunci când clientul de reparare Office încearcă să repare unele intrări de registry problematice, cunoscute. Utilizate pentru a măsura succesul/eșecul reparării Office.

Se colectează următoarele câmpuri:

  - **Data\_15\_SourceType -** unde se află sursa Office 15, adică CDN sau local 

  - **Data\_15\_UpdatesEnabled -** dacă sunt activate actualizările Office 15 

  - **Data\_15\_UpdateVersion -** la ce versiune Office 15 actualizăm 

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion-** ce versiune de Office 16 actualizați la 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** produsele pe care le adăugăm 

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

  - **Data\_ProductsToAdd -** ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează, adică instalare 

  - **Data\_ScenarioSubType -** Ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

  - **Data\_SourceType -** unde se află sursa noastră, adică CDN 

  - **Data\_SqmMachineID -** ID unic de computer utilizat de Windows SQM 

  - **Data\_SusClientID-** identificator de actualizare Office computer 

  - **Data\_TaskState -** care este starea activității, cum ar fi rulare sau anulat 

  - **Data\_TotalClientCabSize -** dimensiunea fișierului cab al clientului nostru 

  - **Data\_TriggeringUI -** ce a declanșat interfața cu utilizatorul 

  - **Data\_UpdatesEnabled -** dacă sunt activate actualizările Office 

  - **Data\_Version -** versiunea de Office 

### <a name="officeclicktorunscenariorepairtaskremoveinstallation"></a>Office.ClickToRun.Scenario.RepairTaskRemoveinstallation

Date despre instalări și inventar Office colectate atunci când clientul de reparare Office elimină Office de pe dispozitiv pentru a pregăti o reinstalare la reparare. Utilizate pentru a măsura succesul/eșecul reparării Office.

Se colectează următoarele câmpuri:

  - **Data\_15\_SourceType -** unde se află sursa Office 15, adică CDN sau local 

  - **Data\_15\_UpdatesEnabled -** dacă sunt activate actualizările Office 15 

  - **Data\_15\_UpdateVersion -** la ce versiune Office 15 actualizăm 

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion-** ce versiune de Office 16 actualizați la 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** produsele pe care le adăugăm 

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

  - **Data\_ProductsToAdd -** ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează, adică instalare 

  - **Data\_ScenarioSubType -** Ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

  - **Data\_SourceType -** unde se află sursa noastră, adică CDN 

  - **Data\_SqmMachineID -** ID unic de computer utilizat de Windows SQM 

  - **Data\_SusClientID-** identificator de actualizare Office computer 

  - **Data\_TaskState -** care este starea activității, cum ar fi rulare sau anulat 

  - **Data\_TotalClientCabSize -** dimensiunea fișierului cab al clientului nostru 

  - **Data\_TriggeringUI -** ce a declanșat interfața cu utilizatorul 

  - **Data\_UpdatesEnabled -** dacă sunt activate actualizările Office 

  - **Data\_Version -** versiunea de Office 

### <a name="officeclicktorunscenarioupdatetaskintegrateupdate"></a>Office.ClickToRun.Scenario.UpdateTaskIntegrateupdate 

Date despre instalări și inventar Office colectate atunci când clientul Clic și Pornire actualizează licențe, dacă este necesar. Utilizat pentru a măsura succesul / eșecul actualizării Office.

Se colectează următoarele câmpuri:

  - **Data\_15\_SourceType -** unde se află sursa Office 15, adică CDN sau local 

  - **Data\_15\_UpdatesEnabled -** dacă sunt activate actualizările Office 15 

  - **Data\_15\_UpdateVersion -** la ce versiune Office 15 actualizăm 

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion-** ce versiune de Office 16 actualizați la 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** produsele pe care le adăugăm 

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

  - **Data\_ProductsToAdd -** ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează, adică instalare 

  - **Data\_ScenarioSubType -** Ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

  - **Data\_SourceType -** unde se află sursa noastră, adică CDN 

  - **Data\_SqmMachineID -** ID unic de computer utilizat de Windows SQM 

  - **Data\_SusClientID-** identificator de actualizare Office computer 

  - **Data\_TaskState -** care este starea activității, cum ar fi rulare sau anulat 

  - **Data\_TotalClientCabSize -** dimensiunea fișierului cab al clientului nostru 

  - **Data\_TriggeringUI -** ce a declanșat interfața cu utilizatorul 

  - **Data\_UpdatesEnabled -** dacă sunt activate actualizările Office 

  - **Data\_Version -** versiunea de Office 

### <a name="officeclicktorunscenarioupdatetaskpublishrsod"></a>Office.ClickToRun.Scenario.UpdateTaskPublishrsod

Date despre instalări și inventar Office colectate atunci când clientul Clic și Pornire actualizează setări de registry pentru fișiere binare noi. Utilizat pentru a măsura succesul/eșecul actualizării Office.

Se colectează următoarele câmpuri:

  - **Data\_15\_SourceType -** unde se află sursa Office 15, adică CDN sau local 

  - **Data\_15\_UpdatesEnabled -** dacă sunt activate actualizările Office 15 

  - **Data\_15\_UpdateVersion -** la ce versiune Office 15 actualizăm 

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion-** ce versiune de Office 16 actualizați la 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** produsele pe care le adăugăm 

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

  - **Data\_ProductsToAdd -** ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează, adică instalare 

  - **Data\_ScenarioSubType -** Ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

  - **Data\_SourceType -** unde se află sursa noastră, adică CDN 

  - **Data\_SqmMachineID -** ID unic de computer utilizat de Windows SQM 

  - **Data\_SusClientID-** identificator de actualizare Office computer 

  - **Data\_TaskState -** care este starea activității, cum ar fi rulare sau anulat 

  - **Data\_TotalClientCabSize -** dimensiunea fișierului cab al clientului nostru 

  - **Data\_TriggeringUI -** ce a declanșat interfața cu utilizatorul 

  - **Data\_UpdatesEnabled -** dacă sunt activate actualizările Office 

  - **Data\_Version -** versiunea de Office 

### <a name="officeclicktorunscenarioupdatetaskupdateapply"></a>Office.ClickToRun.Scenario.UpdateTaskUpdateapply

Date despre instalări și inventar Office colectate atunci când clientul Clic și Pornire închide aplicații care rulează, dacă este necesar, și instalează fișiere noi care au fost descărcate. Utilizate pentru a măsura succesul/eșecul reparării Office.

Se colectează următoarele câmpuri:

  - **Data\_15\_SourceType -** unde se află sursa Office 15, adică CDN sau local 

  - **Data\_15\_UpdatesEnabled -** dacă sunt activate actualizările Office 15 

  - **Data\_15\_UpdateVersion -** la ce versiune Office 15 actualizăm 

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion-** ce versiune de Office 16 actualizați la 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** produsele pe care le adăugăm 

  - **Data\_AddingProducts -** ce produse ni s-a solicitat să adăugăm 

  - **Data\_AvailableVersion to-** ce versiune de Office este disponibilă pentru actualizare

  - **Data\_CompletedWithoutActionInfo-** De ce nu am finalizat scenariul, adică aplicațiile erau deschise

  - **Data\_CompletionState -** dacă am finalizat activitatea

  - **Data\_CorruptionChecksOnly –-** în cazul în care doar căutăm deteriorări și nu actualizăm

  - **Data\_ErrorCode -** codul de eroare cu care am eșuat 

  - **Data\_ErrorDetails -** detalii suplimentare despre o eroare 

  - **Data\_ErrorMessage -** mesaj de eroare despre ce nu a funcționat bine 

  - **Data\_ErrorSource -** unde s-a produs eroarea

  - **Data\_ExceptionType -** excepția cu care am eșuat 

  - **Data\_HardlinkingException -** excepția pe care am întâmpinat-o atunci când am încercat să creăm hardlinkuri

  - **Data\_IsErrorCodeIgnorable -** dacă codul de eroare cu care am eșuat poate fi ignorat 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth -** dacă considerăm că codul de eroare poate fi ignorat 

  - **Data\_NewestPackageVersion -** cea mai nouă versiune de Office de pe computer 

  - **Data\_OldestPackageVersion -** cea mai veche versiune de Office de pe computer 

  - **Data\_PackageOperationSuccessful -** adevărat dacă am finalizat cu succes activitatea noastră în pachetul Office

  - **Data\_ProductsToAdd -** ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează, adică instalare 

  - **Data\_ScenarioSubType -** Ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

  - **Data\_SourceType -** unde se află sursa noastră, adică CDN 

  - **Data\_SqmMachineID -** ID unic de computer utilizat de Windows SQM

  - **Data\_SusClientID -** identificator de actualizare Office computer 

  - **Data\_TaskState -** care este starea activității, cum ar fi rulare sau anulat 

  - **Data\_TotalClientCabSize -** dimensiunea fișierului cab al clientului nostru 

  - **Data\_TriggeringUI -** ce a declanșat interfața cu utilizatorul 

  - **Data\_UpdatesEnabled -** dacă sunt activate actualizările Office 

  - **Data\_Version -** versiunea de Office 

  - **Data\_WorkstationLockState -** adevărat dacă credem că computerul este blocat

### <a name="officeclicktorunscenarioupdatetaskupdateclientdownload"></a>Office.ClickToRun.Scenario.UpdateTaskUpdateclientdownload

Date despre instalări și inventar Office colectate atunci când clientul Clic și Pornire descarcă o versiune mai nouă proprie. Utilizat pentru a măsura succesul/eșecul actualizării Office.

Se colectează următoarele câmpuri:

  - **Data\_15\_SourceType -** unde se află sursa Office 15, adică CDN sau local 

  - **Data\_15\_UpdatesEnabled -** dacă sunt activate actualizările Office 15 

  - **Data\_15\_UpdateVersion -** la ce versiune Office 15 actualizăm 

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion-** ce versiune de Office 16 actualizați la 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** produsele pe care le adăugăm 

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

  - **Data\_ProductsToAdd -** ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName-** ce scenariu rulează. adică, instalare 

  - **Data\_ScenarioSubType -** Ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

  - **Data\_SourceType -** unde se află sursa noastră, adică CDN 

  - **Data\_SqmMachineID -** ID unic de computer utilizat de Windows SQM

  - **Data\_SusClientID-** identificator de actualizare Office computer 

  - **Data\_TaskState -** care este starea activității, cum ar fi rulare sau anulat 

  - **Data\_TotalClientCabSize -** dimensiunea fișierului cab al clientului nostru 

  - **Data\_TriggeringUI -** ce a declanșat interfața cu utilizatorul 

  - **Data\_UpdatesEnabled -** dacă sunt activate actualizările Office 

  - **Data\_Version -** versiunea de Office 

### <a name="officeclicktorunscenarioupdatetaskupdatedetection"></a>Office.ClickToRun.Scenario.UpdateTaskUpdatedetection

Date despre instalări și inventar Office colectate atunci când clientul Clic și Pornire verifică dacă este disponibilă o nouă actualizare. Utilizat pentru a măsura succesul/eșecul actualizării Office.

Se colectează următoarele câmpuri:

  - **Data\_15\_SourceType -** unde se află sursa Office 15, adică CDN sau local 

  - **Data\_15\_UpdatesEnabled -** dacă sunt activate actualizările Office 15 

  - **Data\_15\_UpdateVersion -** la ce versiune Office 15 actualizăm 

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion-** ce versiune de Office 16 actualizați la 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** produsele pe care le adăugăm 

  - **Data\_AddingProducts -** ce produse ni s-a solicitat să adăugăm 

  - **Data\_AvailableVersion -** ce versiune de Office este disponibilă pentru actualizare

  - **Data\_ComAction -** O int care reprezintă o acțiune com pe care o efectuăm

  - **Data\_CompletedWithoutActionInfo-** De ce nu am finalizat scenariul, adică aplicațiile erau deschise

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

  - **Data\_PackageUpdateAvailable -** adevărat dacă avem o nouă versiune de Office disponibilă

  - **Data\_ProductsToAdd -** ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează, adică instalare

  - **Data\_ScenarioSubType -** Ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

  - **Data\_SourceType -** unde se află sursa noastră, adică CDN 

  - **Data\_SqmMachineID -** ID unic de computer utilizat de Windows SQM 

  - **Data\_SusClientID -** identificator de actualizare Office computer 

  - **Data\_TaskState -** care este starea activității, cum ar fi rulare sau anulat 

  - **Data\_TotalClientCabSize -** dimensiunea fișierului cab al clientului nostru 

  - **Data\_TriggeringUI -** ce a declanșat interfața cu utilizatorul 

  - **Data\_UpdatesEnabled -** dacă sunt activate actualizările Office 

  - **Data\_Version -** versiunea de Office 

### <a name="officeclicktorunscenarioupdatetaskupdatedownload"></a>Office.ClickToRun.Scenario.UpdateTaskUpdatedownload

Date despre instalări și inventar Office colectate atunci când clientul Clic și Pornire descarcă o nouă actualizare. Utilizat pentru a măsura succesul / eșecul actualizării Office.

Se colectează următoarele câmpuri:

  - **Data\_15\_SourceType -** unde se află sursa Office 15, adică CDN sau local 

  - **Data\_15\_UpdatesEnabled -** dacă sunt activate actualizările Office 15 

  - **Data\_15\_UpdateVersion -**  la ce versiune Office 15 actualizăm 

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion-** ce versiune de Office 16 actualizați la 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** produsele pe care le adăugăm 

  - **Data\_AddingProducts -** ce produse ni s-a solicitat să adăugăm 

  - **Data\_AvailableVersion -** ce versiune de Office este disponibilă pentru actualizare

  - **Data\_CompletedWithoutActionInfo-** De ce nu am finalizat scenariul, adică aplicațiile erau deschise

  - **Data\_CompletionState -** dacă am finalizat activitatea

  - **Data\_CorruptionChecksOnly -** în cazul în care doar căutăm deteriorări și nu actualizăm

  - **Data\_ErrorCode -** codul de eroare cu care am eșuat 

  - **Data\_ErrorDetails -** detalii suplimentare despre o eroare 

  - **Data\_ErrorMessage -** mesaj de eroare despre ce nu a funcționat bine 

  - **Data\_ErrorSource -** unde s-a produs eroarea

  - **Data\_ExceptionType -** excepția cu care am eșuat 

  - **Data\_FoundCorruptFiles -** adevărat dacă am găsit fișiere deteriorate

  - **Data\_IsErrorCodeIgnorable -** dacă codul de eroare cu care am eșuat poate fi ignorat 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth -** dacă considerăm că codul de eroare poate fi ignorat 

  - **Data\_NewestPackageVersion -** cea mai nouă versiune de Office de pe computer 

  - **Data\_OldestPackageVersion -** cea mai veche versiune de Office de pe computer 

  - **Data\_PackageOperationSuccessful -** adevărat dacă am finalizat cu succes activitatea noastră în pachetul Office

  - **Data\_PipelineExitCode -** codul de ieșire returnat de canalul de fișier 

  - **Data\_ProductsToAdd -** ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează, adică instalare 

  - **Data\_ScenarioSubType -** Ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

  - **Data\_SourceType -** unde se află sursa noastră, adică CDN 

  - **Data\_SqmMachineID -** ID unic de computer utilizat de Windows SQM 

  - **Data\_SusClientID-** identificator de actualizare Office computer 

  - **Data\_TaskState -** care este starea activității, cum ar fi rulare sau anulat 

  - **Data\_TotalClientCabSize -** dimensiunea fișierului cab al clientului nostru 

  - **Data\_TriggeringUI -** ce a declanșat interfața cu utilizatorul 

  - **Data\_UpdatesEnabled -** dacă sunt activate actualizările Office 

  - **Data\_Version -** versiunea de Office 

### <a name="officeclicktorunscenarioupdatetaskupdatefinalize"></a>Office.ClickToRun.Scenario.UpdateTaskUpdatefinalize

Date despre instalări și inventar Office colectate atunci când clientul Clic și Pornire curăță în urma actualizării și restaurează aplicații care au fost deschise anterior. Utilizate pentru a măsura succesul/eșecul reparării Office.

Se colectează următoarele câmpuri:

  - **Data\_15\_SourceType -** unde se află sursa Office 15, adică CDN sau local 

  - **Data\_15\_UpdatesEnabled -** dacă sunt activate actualizările Office 15 

  - **Data\_15\_UpdateVersion -** la ce versiune Office 15 actualizăm 

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion-** ce versiune de Office 16 actualizați la 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** produsele pe care le adăugăm 

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

  - **Data\_ProductsToAdd -** ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează, adică instalare 

  - **Data\_ScenarioSubType -** Ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

  - **Data\_SourceType -** unde se află sursa noastră, adică CDN 

  - **Data\_SqmMachineID -** ID unic de computer utilizat de Windows SQM 

  - **Data\_SusClientID -** identificator de actualizare Office computer 

  - **Data\_TaskState -** care este starea activității, cum ar fi rulare sau anulat 

  - **Data\_TotalClientCabSize -** dimensiunea fișierului cab al clientului nostru 

  - **Data\_TriggeringUI -** ce a declanșat interfața cu utilizatorul 

  - **Data\_UpdatesEnabled -** dacă sunt activate actualizările Office 

  - **Data\_Version -** versiunea de Office 

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

  - **Data\_IsForeGroundStreaming**– Dacă redăm în flux în prim plan sau în fundal

  - **Data\_IsInstallMode** – 1 dacă instalăm și descărcăm fișiere, 0 dacă nu

  - **Data\_SourceProtocol-** Dacă descărcăm dintr-o rețea de date de conținut, CDN, computerul pe care instalăm, local sau de la o resursă de pe rețeaua locală,

  - **Data\_Status** – succes și eroare 

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

- **BitField –** valoarea întreagă a argumentului BitField, care ne spune dacă s-a solicitat un canal de instalare/actualizare explicit. De exemplu, Canal Beta, Canal curent (previzualizare), Canal curent, Canal Enterprise lunar, Canal Enterprise semestrial (previzualizare) sau Canal Enterprise semestrial.

- **ChannelID -** întreg reprezentând valoarea de enumerare a canalului de actualizare/instalare selectat. De exemplu, Canal Beta, Canal curent (previzualizare), Canal curent, Canal Enterprise lunar, Canal Enterprise semestrial (previzualizare), Canal Enterprise semestrial sau nevalid.

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

Raportează acțiunea care citește intrarea etichetată din semnătura încorporată exe. Acesta este un concept nedovedit pe care iterația anterioară a programului setup.exe nu l-a implementat și este lucrul pe care ne bazăm pentru a transmite opțiunile de produs/limbă/număr de biți ale utilizatorului de la pagina web în proces, în cadrul setup.exe.
 
- **ErrorCode–**  Numărul întreg asociat cu o excepție netratată

- **ErrorDetails -** șir care descrie locația locului în care s-a produs o excepție netratată (funcție, fișier, număr linie, parametri suplimentari setați de lansator)

- **ErrorMessage -** șir definit în punctul în care a fost lansată o excepție netratată, descriind natura erorii

- **ErrorType-** Șir care descrie categoria unei excepții netratate

### <a name="officeclicktorununiversalbootstrappercollectparameters"></a>Office.ClickToRun.UniversalBootstrapper.CollectParameters

Raportează parametrii utilizați pentru instalarea Office

- **BitField –** valoarea întreagă a argumentului BitField, care ne spune dacă s-a solicitat un canal de instalare/actualizare explicit. De exemplu, Canal Beta, Canal curent (previzualizare), Canal curent, Canal Enterprise lunar, Canal Enterprise semestrial (previzualizare) sau Canal Enterprise semestrial.

- **ChannelID -** întreg reprezentând valoarea de enumerare a canalului de actualizare/instalare selectat. De exemplu, Canal Beta, Canal curent (previzualizare), Canal curent, Canal Enterprise lunar, Canal Enterprise semestrial (previzualizare), Canal Enterprise semestrial sau nevalid.

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

- **CleanFireflyAction –**   „adevărat” dacă activitatea CleanFireflyAction este programată să ruleze în timpul acestei instalări

- **CleanO15Action –**   „adevărat” dacă activitatea CleanO15Action este programată să ruleze în timpul acestei instalări

- **CMDMode -** Șirul prietenos care corespunde comutatorului de mod general care a fost detectat în argumentele cmd transmise către exe. Posibilitățile sunt: autorun, configurare, consumator, descărcare, ajutor, arhivator

- **DeliveryMechanism –**   Ghid-ul „FFNRoot” extras din Descriptorul de versiune XML (ștampilat de RDX), care ne informează de la ce audiență/canal a venit sursa de compilare

- **DownloadC2RClientAction -** „adevărat” dacă activitatea DownloadC2RClientAction este programată să ruleze în timpul acestei instalări

- **ErrorCode -** Valoarea întreagă asociată cu o excepție netratată

- **ErrorDetails -** șir care descrie locația locului în care s-a produs o excepție netratată (funcție, fișier, număr linie, parametri suplimentari setați de lansator)

- **ErrorMessage -** șir definit în punctul în care a fost lansată o excepție netratată, descriind natura erorii

- **ErrorType-** Șir care descrie categoria unei excepții netratate

- **ExitCode -**   valoarea întreagă asociată cu rezultatul rulării fazei de executare a aplicației de pregătire, indicând succesul comparativ cu anumite tipuri de erori

- **LaunchAction –**  „adevărat” dacă activitatea LaunchAction este programată să ruleze în timpul acestei instalări

- **LaunchUpdateAction –**  „adevărat” dacă activitatea LaunchUpdateAction este programată să ruleze în timpul acestei instalări

- **PreReqResult –**  valoarea de enumerare întreagă a rezultatului atunci când s-au efectuat verificări PreReq (acceptare/respingere/rerulare)

- **UnexpectedAction -** „adevărat” dacă activitatea UnexpectedAction (un caz de eroare) este programată să ruleze în timpul acestei instalări

- **VersionToInstall -** valoarea șirului din versiunea Office „16.0.xxxxx.yyyyy” care este instalată

### <a name="officeserviceabilitymanagerinventoryaddonheartbeat"></a>Office.ServiceabilityManager.InventoryAddon.Heartbeat

*[Acest eveniment a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

Acest eveniment este utilizat pentru obținerea metadatelor standard la fiecare rulare a programului de completare Inventar, care este parte a Office Serviceability Manager și este utilizat pentru informații de inventar Office pe computerele pentru care a optat un administrator IT. Metadatele de interes specific aici sunt ID-ul sesiunii și sunt folosite pentru legarea cu alte date stocate într-un serviciu cloud pentru fiecare entitate găzduită.

Acest eveniment nu conține câmpuri suplimentare fiindcă numai metadatele sunt relevante.

### <a name="officeserviceabilitymanagerinventoryaddonresults"></a>Office.ServiceabilityManager.InventoryAddon.Results

Acest eveniment este înregistrat când apelul către webservice efectuat în cadrul programului de completare Clic și Pornire Serviceability Manager Inventory se termină, indiferent dacă reușește sau nu. Aceasta este, în esență, ultima operațiune din programul de completare care urmărește starea generală a operațiunii.

Se colectează următoarele câmpuri:

- **ActionDetail** - detalii suplimentare pentru atunci când apare o eroare.
   - Dacă solicitarea HTTP reușește, ActionDetail va fi 0.
   - În cazul în care câmpul Rezultat nu este OK (adică, nu este 0), ceea ce înseamnă că solicitarea nu este trimisă, acest câmp va înregistra codul de eroare internă, care este același ca și câmpul Rezultat.
   - În cazul în care câmpul este OK (adică, este 0), ceea ce înseamnă că codul de răspuns HTTP >=300, se va înregistra codul de răspuns HTTP (de exemplu, 404).

- **Result** - semnalizări numerice ale codurilor de eroare returnate de apelurile API ale serviciului web Office. – de exemplu, 3 înseamnă că a existat o problemă cu inițializarea anteturilor HTTP.

- **Type** - informații suplimentare despre tip. În cazul Inventarului, aceste informații specifică tipul de sarcină trimisă, de exemplu, completă sau doar o deltă de modificări. 

-  **WebCallSource** - o valoare de enumerare (specificată ca un număr întreg) care indică programul de completare Serviceability Manager care a fost sursa apelului:
   - Inventar: 0
   - Configurație inventar: 1
   - Politică inventar: 2
   - Stare rețea inventar: 3
   - Manager de întreținere: 4
   - Posibilitate de gestionare: 5

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

### <a name="officeandroiddocsuipaywallcontrolautoredeempendingpurchaseresult"></a>Office.Android.DocsUI.PaywallControl.AutoRedeemPendingPurchaseResult

Telemetrie de inginerie critică pentru a înregistra rezultatul unei încercări automate de a încerca să valorificați achiziționările în așteptare a unui utilizator. Telemetrie de produs utilizate pentru reconcilierea informațiilor de tranzacție de achiziție cu sistemul de comerț Microsoft pentru a activa beneficiile asociate abonamentului.

Se colectează următoarele câmpuri:

- **EventDate** – marca de timp pentru când a avut loc evenimentul 

- **Result** – Int care denotă rezultatul de enumerare a operațiunii. 

- **SessionID** – GUID pentru conectarea evenimentelor după sesiune

### <a name="officeandroiddocsuipaywallcontrolpaywalluishown"></a>Office.Android.DocsUI.PaywallControl.PaywallUIShown

Telemetrie de utilizare critică pentru când se afișează controlul Paywall utilizatorului. Este utilizată pentru înțelegerea experienței de achiziție în cadrul aplicației pentru utilizator și pentru optimizarea acesteia pentru versiunile viitoare.

Se colectează următoarele câmpuri:

- **EventDate** – marca de timp pentru când a avut loc evenimentul 

- **IsModeFRE** – boolean pentru a indica tipul experienței, dialogul Upsell sau selectorul SKU

- **SessionID** – GUID pentru conectarea evenimentelor după sesiune

### <a name="officeandroiddocsuipaywallcontrolpurchasebuttonclicked"></a>Office.Android.DocsUI.PaywallControl.PurchaseButtonClicked

Telemetrie de utilizare critică pentru a afla când apasă utilizatorul butonul Achiziționare. Utilizat pentru a deduce modelul de utilizare și măsurătoarea de conversie pentru utilizatorii care încearcă să achiziționeze un abonament în aplicație.

Se colectează următoarele câmpuri:

- **EventDate** – marca de timp pentru când a avut loc evenimentul

- **IsDefaultSku** – boolean care indică dacă utilizatorul încearcă să achiziționeze Sku, afișat primul/implicit

- **ProductID** – șir ce identifică care utilizator de abonament încearcă să achiziționeze cum este configurat în magazin

- **SessionID** – GUID pentru conectarea evenimentelor după sesiune

### <a name="officeandroiddocsuipaywallcontrolpurchaseresult"></a>Office.Android.DocsUI.PaywallControl.PurchaseResult

Telemetria de inginerie critică pentru înregistrarea rezultatului de încercare de achiziționare declanșată manual de utilizator. Telemetrie de produs utilizate pentru reconcilierea informațiilor de tranzacție de achiziție cu sistemul de comerț Microsoft pentru a activa beneficiile asociate abonamentului.

Se colectează următoarele câmpuri:

- **EventDate** – marca de timp pentru când a avut loc evenimentul 

- **IsModeFre** – boolean pentru a indica dacă achiziționarea a fost efectuată din dialogul ecranul FRE upsell sau din selectorul SKU

- **Result** – Int care denotă rezultatul de enumerare a operațiunii.

- **SessionID** – GUID pentru conectarea evenimentelor după sesiune

### <a name="officeandroiddocsuipaywallcontrolpurchasetokenredemptionresponse"></a>Office.Android.DocsUI.PaywallControl.PurchaseTokenRedemptionResponse

*[Acest eveniment se numea anterior Office.Android.DocsUI.Views.PurchaseTokenRedemptionResponse.]*

Această telemetrie de produs este colectată pentru urmărirea și înregistrarea informațiilor cu privire la starea tranzacțiilor interne și la reconciliere, pentru a îmbunătăți fiabilitatea și performanța.   Microsoft utilizează date pentru a analiza și a îmbunătăți fiabilitatea și performanța procesării tranzacțiilor interne și a mecanismelor de reconciliere.

Se colectează următoarele câmpuri:

- **MicrosoftPurchaseOrderId** - ID comandă Microsoft trimis de Serviciul de federație cu amănuntul (RFS) pentru urmărire.

- **ResponseCode** - cod răspuns HTTP (int)

- **StatusCode** - RFS cod de stare de răspuns (RFS definit de enumerare integrată - finită)


### <a name="officeandroiddocsuipaywallcontrolseeallfeaturesanalytics"></a>Office.Android.DocsUI.PaywallControl.SeeAllFeaturesAnalytics

Colectăm această telemetrie de utilizare pentru a vedea cât timp este consumat de utilizator pe ecranul „Vedeți mai multe beneficii”.  Datele sunt utilizate pentru înțelegerea utilizării caracteristicii „Vedeți mai multe beneficii” și pentru optimizarea ulterioară a experienței în versiunile viitoare.

Se colectează următoarele câmpuri:

- **Duration** - întreg lung care indică timpul consumat, în milisecunde, de către utilizator pe ecranul „Vedeți toate caracteristicile”

- **EventDate** – marca de timp pentru când a avut loc evenimentul 

- **MostExplored** - întreg care denotă indexul elementului cel mai comutat dintr-o listă de aplicații Microsoft 365 și caracteristicile lor

- **SessionID** - identificatorul unic global (GUID) pentru a conecta evenimentele după sesiune

### <a name="officeandroiddocsuipaywallcontrolskuchooseranalytics"></a>Office.Android.DocsUI.PaywallControl.SkuChooserAnalytics

Telemetria de utilizare pentru a vedea cât timp petrece utilizatorul pe ecranul selector SKU. Telemetria de utilizare pentru a vedea cât timp petrece utilizatorul pe ecranul selector Sku.

Se colectează următoarele câmpuri:

- **Duration** – întreg lung care indică timpul consumat, în milisecunde, de către utilizator, pe ecranul selector SKU

- **EventDate** – marca de timp pentru când a avut loc evenimentul

- **SessionID** – GUID pentru conectarea evenimentelor după sesiune


### <a name="officeandroiddocsuiviewsdimeerror"></a>Office.Android.DocsUI.Views.DimeError

Acest eveniment este colectat pentru aplicația Office pentru Android (lansată pe Huawei și în China Stores) Acest eveniment indică o încercare nereușită de a cumpăra un abonament Microsoft 365 prin Dime (un webURL încărcat în clientul webview). Doar scenariile de eroare sunt capturate. Datele despre acest eveniment sunt doar date despre erori și sunt utilizate pentru a asigura starea de funcționare a fluxului de achiziții Dime din client.

Se colectează următoarele câmpuri:

- **CorrelationID** - ID care identifică în mod unic o sesiune de achiziții Dime.

- **ErrorReason** - indică motivul pentru care s-a produs eroarea.
  - 0 – Eroare necunoscută
  - 1 – Internet indisponibil
  - 2 – validare nereușită a identificatorului unic universal (UUID)
  - 3 – Identificatorul unic universal (UUID) este null sau necompletat
  - 4 – Eroare de injectare JavaScript în care aplicația Office pentru Android nu poate transfera authToken la Dime
  - 5 – WebURL de bază încărcat în client nu este valid


### <a name="officeandroiddocsuiviewspremiumfeatureupsell"></a>Office.Android.DocsUI.Views.PremiumFeatureUpsell

Acest eveniment capturează clicuri făcute de un utilizator gratuit pentru a vizualiza o caracteristică din spatele peretelui de plată. Aceste date se utilizează pentru a măsura interacțiunea utilizatorilor cu experiența contextuală de vânzări și pentru a înțelege ce caracteristici sunt preferate de utilizator pentru a-l determina să cumpere un abonament. Acest lucru ne ajută să investim pentru a îmbunătăți setul preferat de puncte de intrare. 

Se colectează următoarele câmpuri:

- **featureId** - TCID pentru caracteristica premium

- **FeatureName** - Titlu Caracteristică Premium

- **consultațiPlanButtonClick** - de câte ori se face clic pe "Vedeți butoanele de plan" în interfața de utilizator actualizată

### <a name="officeappleiapreviewyoursubscriptionios"></a>Office.Apple.IAPReviewYourSubscriptioniOS

Acest eveniment capturează metadatele bazate pe sesiune atunci când interfața de utilizator In-App-Purchase (IAP) este afișată utilizatorului și butoanele cu care interacționează ulterior utilizatorul. Aceste date sunt utilizate pentru a ne ajuta să înțelegem divergentele din fluxul de achiziționare și le compară cu pâlnia din altă experiență de achiziție, pentru a înțelege ce experiență este mai bună pentru utilizator. 

Se colectează următoarele câmpuri:

- **TipFlux** - Integral - Fluxul de unde a fost lansat IAP.

- **Restaurare** - Șir - eticheta regulii este înregistrată atunci când se face clic pe butonul restaurare

- **CaracteristiciPremium** - Șir - eticheta regulii este înregistrată atunci când se face clic pe butonul "CaracteristiciPremium"

- **Produs** - Șir - SKU-ul selectat de utilizatori


### <a name="officeappleinapppurchasecontext"></a>Office.Apple.InAppPurchaseContext

Acest eveniment măsoară telemetria de utilizare critică pentru punctul de intrare a ecranului de achiziționare în aplicație. Datele ajută la înțelegerea și îmbunătățirea experienței de utilizator prin identificarea punctului de intrare preferat pentru o achiziție în aplicație.

Se colectează următoarele câmpuri:

- **context** - Șir - Fluxul prin care utilizatorul a ajuns pe pagina de achiziționare a aplicației


### <a name="officeapplelicensingcommonpaywallcontrol"></a>Office.Apple.Licensing.CommonPaywallControl

Acest eveniment este utilizat pentru a înțelege experiența de achiziționare în aplicație (IAP) a utilizatorului. Ne permite să ne asigurăm că IAP funcționează conform așteptărilor și ne ajută să înțelegem problemele utilizatorilor, astfel încât să putem optimiza experiența IAP.  Colectarea se produce prin intermediul unuia dintre următoarele sub evenimente.

- **Office.iOS.Paywall.Paywall.Presented** - datele sunt colectate atunci când se afișează un control paywall pentru utilizator. Datele se utilizează pentru a construi o vizualizare în vederea măsurării la fiecare pas a ratei de conversie și pentru a asigura că interfața utilizator funcționează conform așteptărilor, utilizatorii confruntându-se cu divergențe minime în timpul experienței de achiziționare.

   Se colectează următoarele câmpuri:

  - **entryPoint** - Șir – butonul/fluxul din care a fost afișat Paywall. Cum ar fi „Buton upgrade premium” sau „Primul flux de rulare”
  - **isFRE** - Boolean – Afișăm prima experiență de rulare sau interfața utilizator obișnuită?

- **Office.iOS.Paywall.Paywall.Stats** - datele sunt colectate atunci când sunt afișate pentru utilizator interfața de utilizator Paywall, durata interacțiunii și dacă o achiziție a fost încercată, a reușit sau nu a reușit. Datele sunt utilizate pentru a măsura performanța interfeței utilizator și pentru a garanta funcționarea acesteia conform așteptărilor. 

   Se colectează următoarele câmpuri:

   - **entryPoint** - Șir – butonul/fluxul din care a fost afișat Paywall. Cum ar fi „Buton upgrade premium” sau „Primul flux de rulare”.
   - **isFRE** - Boolean – verifică dacă se afișează prima experiență de rulare sau interfața utilizator obișnuită.
   - **status** - Șir – stare de ieșire a Paywall. Cum ar fi „inițiat”, „paymentDone”, „provisionFailed”
   - **userDuration** - dublu – durata, în milisecunde, a timpului petrecut de utilizator în Paywall
  
- **Office.iOS.Paywall.SKUHinoser.BuyButtonTap** - se colectează date atunci când utilizatorul atinge butonul Achiziționare/Cumpărare. Datele sunt utilizate pentru a măsura performanța butonului și pentru a garanta funcționarea acestuia conform așteptărilor.

   Se colectează următoarele câmpuri:

   - **entryPoint** - Șir – butonul/fluxul din care a fost afișat Paywall. Cum ar fi „Buton upgrade premium” sau „Primul flux de rulare”.
   - **isDefaultSKU** - Bool - dacă utilizatorul achiziționează produsul recomandat de noi prin afișarea acestuia ca implicit.
   - **productId** - șir – ID-ul produsului din App Store pentru care a fost apăsat butonul Cumpărare
   - **toggleCount** - Int – de câte ori a comutat utilizatorul între vizualizare diferitelor produse înainte de a apăsa butonul Achiziționare, în sesiunea curentă de Paywall.

- **Office.iOS.Paywall.SKUChooser.Stats** - date colectate pentru a vedea a accesat utilizatorul selectorul SKU, cât timp a petrecut pe ecranul selectorului SKU și de ce a ieșit din selectorul SKU. Utilizând aceste informații, putem garanta că selectorul SKU funcționează conform așteptărilor și vom putea optimiza și îmbunătăți experiența utilizatorilor finali.

   Se colectează următoarele câmpuri:

   - **entryPoint** - Șir – butonul/fluxul din care a fost afișat Paywall. Cum ar fi „Buton upgrade premium” sau „Primul flux de rulare”.
   - **exitReason** - Șir – motivul ieșirii din selectorul SKU. Cum ar fi „Buybutton”, „CloseButton”
   - **isFRE** - Boolean – Afișăm prima experiență de rulare sau interfața utilizator obișnuită?
   - **userDuration** - Dublu – durata, în milisecunde, a timpului petrecut de utilizator în selectorul SKU.

- **Office.iOS.Paywall.FailedScreen.RetryButtonTap** - datele colectate pentru a afla când a eșuat Achiziționarea/Asigurarea accesului/Activarea, iar utilizatorul a apăsat butonul „Reîncercare”. Datele sunt utilizate în vederea depanării scenariilor de erori de achiziție și a remedierii acestora, pentru a vă asigura că funcționează conform așteptărilor.

   Se colectează următoarele câmpuri:

   - **failureReason** - șir – indică eroarea pentru care utilizatorul reîncearcă; de exemplu, „provisioningFailed”, „purchaseFailed”, „activationFailed”.
   - **productid** - șir – ID-ul produsului din App Store pentru care utilizatorul reîncearcă solicitarea nereușită.

- **Office.iOS.Paywall.SKUChooser.MoreBenefits.Stats** - date colectate atunci când utilizatorii ating „Vedeți mai multe avantaje” pentru a vedea toate serviciile, aplicațiile și caracteristicile incluse în achiziție. Acestea trebuie să extindă secțiuni care detaliază caracteristicile fiecărei aplicații. Acest eveniment colectează caracteristicile și aplicațiile extinse, împreună cu timpul consumat. Datele se utilizează pentru a garanta că interfața utilizator oferită utilizatorilor finali pentru a afla despre avantaje funcționează conform așteptărilor. 

   Se colectează următoarele câmpuri:

   - **appsExpanded** - șir - lista, separată prin virgulă, a serviciilor/aplicațiilor pentru care au fost extinse avantajele.
   - **productId** - șir - ID-ul produsului din App Store pentru care utilizatorul vizualizează mai multe avantaje oferite
   - **userDuration** - dublu – durata, în milisecunde, a timpului petrecut de utilizator pe ecranul Avantaje.

- **Office.iOS.Paywall.SuccessScreen.SeeAllBenefitsButtonTap** - acest eveniment se colectează atunci când utilizatorul atinge „Vedeți toate avantajele” după o achiziționare reușită, pentru a vedea aplicațiile și caracteristicile incluse în achiziție. Datele sunt utilizate pentru a măsura dacă performanța interfeței utilizator este conform așteptărilor.

   Se colectează următoarele câmpuri:

   - **productId** - șir - ID-ul produsului din App Store pentru care utilizatorul vizualizează toate avantajele oferite.

- **Office.iOS.Paywall.SKUChooser.ProductSwitched** - telemetrie de utilizare pentru a vizualiza interacțiunea utilizatorului final cu interfața de utilizator furnizată, pentru a comuta între SKU-uri diferite și a vă asigura că funcționează conform așteptărilor. 

   Se colectează următoarele câmpuri:

  - **productId**- șir - ID-ul App Store al produsului pe a cărui vizualizare utilizatorul tocmai a comutat din produsele disponibile în selectorul SKU.

- **Office.iOS.Paywall.StoreKit.Response** - telemetrie de inginerie critică, pentru a înregistra în jurnal rezultatul încercării de achiziție declanșate manual de utilizator și răspunsul de la App Store cu privire la eveniment. Datele sunt utilizate pentru a măsura starea unei încercări de achiziție și motivele erorii (dacă există) și pentru a efectua acțiuni de corectare, pentru a vă asigura că IAP și toate punctele de intrare au performanțele așteptate.

   Se colectează următoarele câmpuri:

   - **entryPoint** - Șir – butonul/fluxul din care a fost afișat Paywall. Cum ar fi „Buton upgrade premium” sau „Primul flux de rulare”.
   - **failureReason** - Șir – adăugat doar atunci când starea este „eroare”. Indică răspunsul de eroare dat de răspunsul de la App Store
   - **productId** - Șir – doar pentru „MakePurchase”, „PendingPurchase”, ID-ul de App Store al produsului pentru care s-a efectuat solicitarea.
   - **productsCount** -Int – doar pentru „ProductsFetch”, numărul de produse returnate de Store.
   - **requestType** - Șir – tipul solicitării StoreKit. Cum ar fi „ProductsFetch”, „PendingPurchase”
   - **status** - șir – succes sau eroare, indicând dacă solicitarea a fost realizată cu sau fără succes

- **Office.iOS.Paywall.Provisioning.Response** - telemetrie de inginerie critică și contractul cu Serviciul Federației de Retail Microsoft (RFS), pentru a colecta informațiile furnizate în acest eveniment. RFS este serviciul intern utilizat în cadrul Microsoft pentru verificarea încrucișată a achiziției. Acesta este utilizat pentru a obține starea de funcționare a apelului API efectuat la RFS, ceea ce ar ajuta la înțelegerea faptului că performanța integrării este conform așteptărilor.  

   Se colectează următoarele câmpuri:

   - **entryPoint** - Șir – butonul/fluxul din care a fost afișat Paywall. Cum ar fi „Buton upgrade premium” sau „Primul flux de rulare”.
   - **failureReason** - Șir – adăugat doar atunci când starea este „eroare”. Indică răspunsul de eroare dat de răspunsul de asigurare RFS.
   - **productId** - Șir – ID-ul produsului în App Store pentru care a fost făcută solicitarea
   - **status** - Șir – succes sau eroare, indică dacă solicitarea a fost realizată cu sau fără succes


### <a name="officedimesdkhealth"></a>Office.Dime.Sdk.Health

Acest eveniment capturează date care ajută să monitorizați starea componentelor Dime. De exemplu, pentru fluxul de achiziție din cadrul aplicației, atunci când un utilizator optează pentru a cumpăra un abonament Microsoft 365 din cadrul aplicației Office pentru Android sau de pe dispozitive care rulează Windows.

Se colectează următoarele câmpuri:

- **Data_ActivityErrorDescription** - descrierea erorii de activitate

- **Data_ActivityErrorMessage** - mesajul erorii de activitate 

- **Data_CampaignId** - ID-ul campaniei pentru atribuire

- **Data_ContentId** - bazat pe ID-ul de experiență; este mapat la ID-ul de flux și ID-ul de conținut 

- **Data_CorrelationVector** - vector de corelare pentru a corela Dime cu partenerii care utilizează vectorul de corelare

- **Data_CustomerImpacted** - utilizat pentru depanare, dacă clientul este afectat la încărcarea fluxului

- **Data_DimeActivityDuration** - durata de timp 

- **Data_DimeActivityMetadata** - metadate de activitate

- **Data_DimeActivityName** - nume de activitate pentru monitorizarea stării

- **Data_DimeActivityResult** - rezultat activitate, succes/ eroare/ eroare așteptată

- **Data_DimeVersion** - versiune de compilare

- **Data_DurationLevel** - severitate - 0/1/2

- **Data_EcsConfigIds** - ID-uri pentru experimente

- **Data_EcsCountry** - țara detectată

- **Data_EcsETag** - informații despre zbor

- **Data_Environment** -producție/preproducție de mediu Dime

- **Data_ExperienceId** - experiența pentru încărcare 

- **Data_FlowId** - bazat pe ID-ul de experiență; este mapat la ID-ul de flux și ID-ul de conținut 

- **Data_Language** - cultură

- **Data_Market** - piață detectată

- **Data_OTelJS_Version** - versiune de telemetrie Office

- **Data_PageSessionId** - ID-ul de sesiune al paginii

- **Data_PartnerId** - aplicația de apelare

- **Data_QosLevel** - severitate 0/1/2

- **Data_SDX_AssetId** - ID de activ al conținutului de găzduire pentru Win32 al serviciului Service Delivered Experience (SDX)

- **Data_SDX_BrowserToken** - tokenul browserului pentru Win32

- **Data_SDX_HostJsVersion** - versiunea de bibliotecă JavaScript pentru Win32

- **Data_SDX_Id** - Id Service Delivered Experience pentru Win32

- **Data_SDX_InstanceId** - ID-ul de instanță al SDX pentru Win32

- **Data_SDX_MarketplaceType** - tip de market SDX pentru Win32

- **Data_SDX_OfficeJsVersion** - Versiune JS Office pentru Win32

- **Data_PageSessionId** - ID-ul de sesiune SDX pentru Win32

- **Data_SDX_Version** - versiunea SDX pentru Win32

- **CollectionTime** – marca de timp a evenimentului

- **Data_TsgId** - ID ghid de depanare pentru fiecare activitate

- **Data_UserAgent** - antet Tag-uri


### <a name="officedocssharedpremiumfeaturemessagebar"></a>Office.Docs.Shared.PremiumFeatureMessageBar

Acest eveniment colectează atingerile utilizatorului gratuit pentru o caracteristică premium aflată în spatele paywallului. Datele sunt utilizate pentru a înțelege setul de caracteristici cu care interacționează consumatorii în timp ce se transformă în utilizatori plătiți. Acest lucru ne spune punctele de intrare preferate ale utilizatorilor și îmbunătățește experiența de utilizator.

Se colectează următoarele câmpuri:

- **featureId** - TCID pentru caracteristica premium pe care utilizatorul le atinge


### <a name="officelicensingaccepteulaforcurrentlicense"></a>Office.Licensing.AcceptEulaForCurrentLicense 

Se colectează atunci când utilizatorul obține licența și acceptă Termenii licenței pentru licența curentă

Este utilizat pentru a detecta dacă utilizatorul se află sau nu în stare bună, pentru sănătatea sistemului și în scopuri de diagnosticare dacă un utilizator raportează o problemă cu computerul

Se colectează următoarele câmpuri:

  - **ACID** - identificator GUID care reprezintă produsul Office pentru care are licență utilizatorul

  - **DwEulaId** - identificator numeric al tipului de Termeni ai licenței care au fost acceptați de către utilizator


### <a name="officelicensingactivatedeviceentitlement"></a>Office.Licensing.ActivateDeviceEntitlement

Acest eveniment se declanșează atunci când încercăm să activăm o ofertă Office permanentă bazată pe dispozitive pentru utilizator. Utilizăm aceste date pentru a monitoriza starea sistemelor și a serviciilor.

Se colectează următoarele câmpuri: 

- **Activity_Success** - ne spune dacă dispozitivul este licențiat cu o ofertă Office permanentă bazată pe dispozitiv.

- **Data_Count** - ne spune numărul de drepturi Office permanente bazate pe dispozitive asociate cu dispozitivul. Din punct de vedere tehnic, nu ar trebui să existe mai mult de unul.

- **Data_EligibleEntitlementsCount** - ne spune numărul de drepturi eligibile. Deoarece serviciul va returna toate drepturile de dispozitiv asociate dispozitivului, dar trebuie să verificăm acele oferte relevante pentru aplicația Office care rulează.

- **Data_Errors** - un șir cu o listă de erori în timp ce preluam licențele pentru drepturi, separate prin virgulă.

- **Data_LicensedEntitlementsCount** - ne spune numărul de drepturi pentru care preluam cu succes o licență. Ar putea exista erori de drepturi care să ne determine să nu putem obține o licență. 


### <a name="officelicensingactivation"></a>Office.Licensing.Activation 

După configurarea licenței pe computer, încercăm să activăm licența prin apelarea serviciului AVS. Astfel se raportează rezultatul apelului de activare

Este de importanță critică în a detecta câți utilizatori întâmpină probleme de activare. Dispunem de o detectare a anomaliilor pentru a detecta orice regresie. Acest lucru este de importanța critică absolută, deoarece avem o dependență externă de AVS, iar acest semnal indică dacă partenerii noștri externi sunt sănătoși. Este utilizat, de asemenea, în scopuri de diagnosticare și sănătate a sistemului dacă un utilizator raportează o problemă cu computerul

Se colectează următoarele câmpuri:

  - **Acid** - identificator GUID care reprezintă produsul Office pentru care are licență utilizatorul

  - **ReferralData** - identificator al OEM care a instalat Office pe computer

### <a name="officelicensingactivationwizard"></a>Office.Licensing.ActivationWizard 

Dacă nu putem activa automat licența dintr-un motiv sau altul, afișăm utilizatorului un expert de activare. Acesta raportează faptul că expertul i se afișează utilizatorului. Este de importanță critică pentru a detecta dacă utilizatorul se află în stare bună, fără să îi lipsească funcționalități, este utilizat pentru sănătatea sistemului și în scopuri de diagnosticare dacă un utilizator raportează o problemă cu computerul

Acest eveniment nu colectează niciun câmp.

### <a name="officelicensingbusbarcheckfordynamicbusbarexperiment"></a>Office.Licensing.BusBar.CheckForDynamicBusbarExperiment

Acest eveniment se declanșează o singură dată pentru fiecare tip de bară de business cu licențiere afișată care are activată bara de zbor business dinamică (grup de tratament). Acest eveniment de date raportează dacă există o campanie dinamică de bară de business a Platformei de Programare a Ciclului de Viață pregătită pe disc. Datele vor fi utilizate pentru a măsura starea noii tehnologii a barei de business cu licențiere dinamică a Platformei de Programare a Ciclului de Viață.

Se colectează următoarele câmpuri:

- **Does InformareAignExist (bool)** - Indică dacă campania este pe disc

- **Tip (int32)** - indică tipul de bară de business de licențiere


### <a name="officelicensingbusbarshowstashedbusbar"></a>Office.Licensing.BusBar.ShowStashedBusbar

Acest eveniment se declanșează atunci când bara dinamică de business Platformă de Programare a Ciclului de Viață nu se afișează și se afișează în schimb bara de business statică. Acest eveniment de date va fi utilizat pentru a vă asigura că revenirea la bara de business statică are succes.

Se colectează următoarele câmpuri:

- **Tip (int32)** - indică tipul de bară de business de licențiere


### <a name="officelicensingdialogswebviewdialogclose"></a>Office.Licensing.Dialogs.WebViewDialog.Close
 
Acest eveniment este utilizat ca semnal pentru a ne spune că experiența de cumpărare în cadrul aplicației este închisă fie de către utilizator, fie de aplicație. Datele sunt utilizate pentru a monitoriza și a avertiza cu privire la starea fluxului de cumpărare în cadrul aplicației, pentru a asigura că funcționează conform așteptărilor.  
 
Se colectează următoarele câmpuri:
 
- **Data_ClosedDialog** - semnalizare indicând faptul că utilizatorul a închis caseta de dialog

### <a name="officelicensingdialogswebviewdialoghandleerrornotification"></a>Office.Licensing.Dialogs.WebViewDialog.HandleErrorNotification
 
Acest eveniment este utilizat drept semnal care ne informează dacă experiența de achiziționare în cadrul aplicației a încercat să se încarce, dar s-a produs o eroare care a dus la neafișarea casetei de dialog. Datele sunt utilizate pentru a monitoriza și a alerta starea fluxului de achiziționare în cadrul aplicației, pentru a asigura funcționarea conform așteptărilor.  
 
Se colectează următoarele câmpuri:
  
- **Data_MoeErrorCode** - codul de eroare observat în cadrul casetei de dialog web

### <a name="officelicensingdialogswebviewdialogpreload"></a>Office.Licensing.Dialogs.WebViewDialog.Preload
 
Acest eveniment este utilizat drept semnal care ne informează dacă experiența de achiziționare în cadrul aplicației este în curs de încărcare în fundal. Datele sunt utilizate pentru a monitoriza și a alerta starea fluxului de achiziționare în cadrul aplicației, pentru a asigura funcționarea conform așteptărilor.  
 
Se colectează următoarele câmpuri:

 - Fără

### <a name="officelicensingdialogswebviewdialogshow"></a>Office.Licensing.Dialogs.WebViewDialog.Show
 
Acest eveniment este utilizat drept semnal care ne informează dacă experiența de achiziționare în cadrul aplicației se afișează utilizatorului. Datele sunt utilizate pentru a monitoriza și a alerta starea fluxului de achiziționare în cadrul aplicației, pentru a asigura funcționarea conform așteptărilor.  

Se colectează următoarele câmpuri:

 - Fără

### <a name="officelicensingdialogswebviewdialogtimeout"></a>Office.Licensing.Dialogs.WebViewDialog.Timeout

Acest eveniment este utilizat drept semnal care ne informează dacă experiența de achiziționare în cadrul aplicației a încercat să se încarce, dar a expirat. Datele sunt utilizate pentru a monitoriza și a alerta starea fluxului de achiziționare în cadrul aplicației, pentru a vă asigura funcționalitatea conform așteptărilor. 

Se colectează următoarele câmpuri:

 - Fără


### <a name="officelicensingenforcesigninqualified"></a>Office.Licensing.EnforceSignInQualified 

Acesta este semnalul care ne informează dacă experimentul pe care îl efectuăm pentru a impune semnătura utilizatorului ca parte a licențierii este reușit. Acest lucru este de importanță critică în a detecta succesul sau eșecul experimentului care impune utilizatorilor să se conecteze, ceea ce reprezintă un pas obligatoriu pentru stiva de licențiere modernă. Dacă nu se conectează, utilizatorii nu vor putea utiliza aplicația.

Se colectează următoarele câmpuri:

  - **Qualified** – identifică dacă utilizatorul este calificat pentru impunerea conectării

### <a name="officelicensingexpirationdialogshown"></a>Office.Licensing.ExpirationDialogShown

Se colectează când afișăm utilizatorului caseta de dialog de expirare care spune că licența sa a expirat. Este de importanță critică pentru a detecta dacă utilizatorul se află în stare bună, fără să îi lipsească funcționalități, este utilizat pentru sănătatea sistemului și în scopuri de diagnosticare, dacă un utilizator raportează o problemă cu computerul

Se colectează următoarele câmpuri:

  - **LicNotificationState** – un enumerator care ne informează ce fel de notificare se afișează pentru utilizator

### <a name="officelicensingfullvalidation"></a>Office.Licensing.FullValidation 

Se colectează la fiecare sesiune care raportează starea de licențiere a computerului și erorile vizualizate de utilizator din cauza cărora nu poate să utilizeze aplicația. Acest eveniment indică dacă computerul utilizatorului este în bună stare de funcționare sau nu. Avem configurată o detectare a anomaliilor pentru acest eveniment pentru a indica dacă o regresie sau un mecanism de activare provoacă un comportament inadecvat al utilizatorului. Și acesta este de importanță critică la diagnosticarea problemelor utilizatorului și pentru monitorizarea sănătății sistemului.

Se colectează următoarele câmpuri:

  - **Acid** - identificator GUID care reprezintă produsul Office pentru care are licență utilizatorul 
  
  - **ActivationAttributes** - tipul de mecanism de activare folosit de utilizator.

  - **IsSessionLicensing** - indiferent dacă momentan rulează sau nu în modul de activare computer partajat 

  - **LicenseCategory** - categoria de licență Office pe care o folosește utilizatorul 

  - **Licenses** - lista de nume a tuturor licențelor de Office prezente pe calculator 

  - **LicenseStatuses** - starea tuturor licențelor de Office prezente pe calculator 

### <a name="officelicensinggetentitlement"></a>Office.Licensing.GetEntitlement 

Colectăm acest lucru atunci când utilizatorul configurează un dispozitiv și apelăm serviciul nostru de licențiere pentru a detecta dacă utilizatorul autentificat are drepturi de Office sau nu. Acesta raportează rezultatul apelului respectiv. Este de importanță critică pentru a detecta dacă utilizatorul se află în stare bună și dacă îi lipsesc funcționalități, este utilizat pentru sănătatea sistemului și în scopuri de diagnosticare dacă un utilizator raportează o problemă cu computerul

Se colectează următoarele câmpuri:

- **EntitlementCount** - numărul de drepturi pe care le are utilizatorul


### <a name="officelicensinggetnextuserlicense"></a>Office.Licensing.GetNextUserLicense

Acest eveniment se declanșează atunci când preluați licența pentru drepturile Office bazate pe utilizator alese în timpul în prima experiență de rulare a activării. Utilizăm aceste date pentru a monitoriza starea sistemelor și a serviciilor.

Se colectează următoarele câmpuri:

- **Activity_Success** - Boolean: ne spune dacă am preluat cu succes o licență pentru ca dispozitivul să fie activat în aplicația sa Office.

- **Data_AllowNULPerpetual** - Boolean: ne spune dacă este activat flight pentru activarea vNext Perpetual.

- **Data_AttemptNulReactivation** - Boolean: ne spune dacă acesta este un scenariu de reactivare.

- **Data_CurrentMode** - 0 înseamnă SPP (stiva de licențiere moștenită), 2 înseamnă vNext (stiva de licențiere modernă).

- **Data_HasError** - Boolean: ne spune dacă am primit orice eroare la o tentativă de obținere a unei licențe pentru drepturile bazate pe utilizator alese.

- **Data_IsSubscription** - boolean: ne spune dacă reactivarea este pentru Office de abonament.

- **Data_NewMode** - 0 înseamnă SPP (stiva de licențiere moștenită), 2 înseamnă vNext (stiva de licențiere modernă). Ar trebui să ne așteptăm la 2, în cele mai multe cazuri.

- **Data_SkuToSkuNeeded** - Boolean: ne spune dacă trebuie să facem conversia SKU în SKU, întrucât SKU Office eligibil nu se potrivește cu SKU Office instalat.


### <a name="officelicensingheartbeat"></a>Office.Licensing.Heartbeat 

La fiecare sesiune, verificăm dacă au trecut 72 de ore de la ultima reînnoire de licență și încercăm să extindem valabilitatea licenței curente. Acest eveniment raportează succesul sau eșecul apelului pe care îl efectuăm pentru a ne asigura că putem extinde valabilitatea licenței și să păstrăm funcțională instalarea Office a utilizatorului. Este de importanță critică în diagnosticarea problemelor legate de abonament și serviciu pentru utilizator și în detectarea regresiilor pentru utilizatorii care dețin deja un abonament activat.

Se colectează următoarele câmpuri:

  - **Mode** - o reprezentare cu enumerator a stivei de licențiere Office care este utilizată la acest computer

### <a name="officelicensinginclientpinredemptioncallpinredemptionapi"></a>Office.Licensing.InClientPinRedemption.CallPinRedemptionAPI

Această telemetrie urmărește rezultatele apelului de serviciu de valorificare a pinului Office.

Se colectează următoarele câmpuri:

- **ClientTransactionId** - Identificator unic pentru apelul de serviciu.

- **ErrorCategory** - Fiecare tip de eroare poate aparține unei categorii mai generale, cum ar fi „reîncercare”.

- **ErrorType** - Motivul erorii, cum ar fi "AlreadyRedeemedByOther".

- **InAFOFlow** - valoare booleană care indică dacă ne aflăm în fluxul de valorificare AFO.

- **StatusCode** - Rezultat de un cuvânt al apelului de serviciu, cum ar fi „Creat”.

- **StatusMessage** - Detalii despre codul de stare, cum ar fi „Aprovizionat cu succes”.

- **UsingNulApi** - valoare booleană care indică dacă utilizăm noua stivă de licențiere.

### <a name="officelicensinginrfm"></a>Office.Licensing.InRFM 

Dacă dispozitivul intră în modul de funcționalitate redusă, trimitem acest semnal pentru a indica faptul că computerul nu este într-o stare bună de funcționare. Este de importanță critică pentru a detecta dacă utilizatorul se află în stare bună, fără să îi lipsească funcționalități, este utilizat pentru sănătatea sistemului și în scopuri de diagnosticare dacă un utilizator raportează o problemă cu computerul

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

În cazul în care observăm probleme cu fluxul de lucru de activare, declanșăm un expert de licențe și trimitem acest semnal pentru a indica problema. Este de importanță critică pentru a detecta dacă utilizatorul se află în stare bună, fără să îi lipsească funcționalități, este utilizat pentru sănătatea sistemului și în scopuri de diagnosticare dacă un utilizator raportează o problemă cu computerul

Se colectează următoarele câmpuri:

  - **Acid** - identificator GUID care reprezintă produsul Office pentru care are licență utilizatorul

  - **LicenseStatus** - starea licenței Office pe care o folosește utilizatorul

  - **MachineKey** - identificator alfanumeric al cheii de licență care a fost emise pentru utilizator

### <a name="officelicensinglaunchsetupoffice"></a>Office.Licensing.LaunchSetupOffice

Acest eveniment se declanșează atunci când valorificăm o ofertă Office pentru utilizatorul care fie a cumpărat un dispozitiv la pachet cu o autorizare prealabilă Office OEM, fie a introdus o cheie de produs. Utilizăm aceste date pentru a monitoriza starea sistemelor și a serviciilor.

Se colectează următoarele câmpuri:

- **Activity_Result_Tag** - ne spune cum am finalizat acest eveniment.

- **Data_DialogResult** - ne spune rezultatul general al procesului de valorificare.

- **Data_Scenario** - ne spune scenariul pentru care a avut loc valorificarea.


### <a name="officelicensinglicensingbar"></a>Office.Licensing.LicensingBar

Dacă dispozitivul întâmpină probleme de licențiere și în final afișăm utilizatorului o bară, trimitem acest semnal care raportează, de asemenea, tipul de bară afișată utilizatorului. Este de importanță critică pentru a detecta dacă utilizatorul se află în stare bună, fără să îi lipsească funcționalități, este utilizat pentru sănătatea sistemului și în scopuri de diagnosticare dacă un utilizator raportează o problemă cu computerul.

Se colectează următoarele câmpuri:

  - **SuppressNotification** - indică dacă am eliminat bara de licențiere

  - **Title** - titlul barei de licențiere care a fost afișată utilizatorului

  - **Type** - tipul de bară de licențiere care a fost afișată utilizatorului

### <a name="officelicensinglicexitofficeprocess"></a>Office.Licensing.LicExitOfficeProcess 

Dacă în final Office se închide/cade din cauza unei probleme de licențiere, trimitem acest semnal pentru a indica problema. Este de importanță critică pentru a detecta dacă utilizatorul se află în stare bună, fără să îi lipsească funcționalități, este utilizat pentru sănătatea sistemului și în scopuri de diagnosticare dacă un utilizator raportează o problemă cu computerul

Se colectează următoarele câmpuri:

  - **ExitCode** - codul intern care a cauzat ieșirea din aplicație

### <a name="officelicensingloadidentityticket"></a>Office.Licensing.LoadIdentityTicket

În cadrul procesului în care se încearcă licențierea dispozitivului, aplicația încearcă să încarce identitatea utilizatorului pentru a vedea dacă utilizatorul are drepturi de Office sau nu. Acest eveniment raportează succesul sau eșecul împreună cu codul de eroare. Este de importanță critică pentru a detecta dacă utilizatorul se află în stare bună, fără să îi lipsească funcționalități, este utilizat pentru sănătatea sistemului și în scopuri de diagnosticare dacă un utilizator raportează o problemă cu computerul.

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

Se colectează la fiecare sesiune a unui dispozitiv care rulează pe stiva de licențiere modernă. Se raportează starea de licențiere a computerului și erorile vizualizate de utilizator din cauza cărora nu poate să utilizeze aplicația. Acest eveniment indică dacă computerul utilizatorului este în bună stare de funcționare în  stiva de licențiere modernă. Avem configurată o detectare a anomaliilor pentru acest eveniment pentru a indica dacă o regresie provoacă un comportament inadecvat al utilizatorului. Și acesta este de importanță critică la diagnosticarea problemelor utilizatorului și pentru monitorizarea sănătății sistemului.

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

### <a name="officelicensingoobehandledigitalattachfailure"></a>Office.Licensing.OOBE.HandleDigitalAttachFailure

Acest eveniment se declanșează atunci când verificarea serviciului (consultați Office.Licensing.OOBE.SearchForDigitalAttach) nu a găsit pe acest dispozitiv o ofertă de atașare digitală care poate fi solicitată. În funcție de diferitele condiții ale dispozitivului, vom afișa utilizatorului casete de dialog diferite. Acest eveniment va înregistra în jurnal diverse scenarii privind modul în care gestionăm erorile de atașare digitală.

Se colectează următoarele câmpuri:

- **Activity_Result_Tag** ne spune cum trecem utilizatorul la diferite stări de eroare.
   - 0x222e318f - ar trebui să căutăm în continuare oferta de activare pentru Office.
   - 0x222e318e - vom reveni la modul OEM în această sesiune atunci când acest dispozitiv nu vine livrat cu o ofertă de atașare digitală.
   - 0x222e318d - fără conectivitate la internet, ceea ce ne va duce la afișarea casetei de dialog NoInternetConnectivity pentru utilizator 
   - 0 - vom afișa diverse erori de interfață utilizator, pe baza codului de eroare specific.

- **Data_DigitalAttachErrorType** - ne spune care este codul de eroare specific din apelul serviciului.

- **Data_FallbackFlight** - ne spune dacă este activat sau nu flight pentru UseAFOAsFallBack.


### <a name="officelicensingoobehandledigitalattachsuccess"></a>Office.Licensing.OOBE.HandleDigitalAttachSuccess

Acest eveniment se declanșează atunci când verificarea serviciului găsește pe acest dispozitiv o ofertă de atașare digitală care poate fi solicitată. În funcție de diferitele condiții ale dispozitivului, vom afișa utilizatorului casete de dialog diferite. Acest eveniment va înregistra în jurnal diverse scenarii privind modul în care gestionăm o atașare digitală reușită.

Se colectează următoarele câmpuri:

- **Activity_Result_Tag** - ne spune cum gestionăm scenariile reușite de atașare digitală.
   - 0 - putem încărca automat identitatea și am afișat utilizatorului interfața de utilizator „Aveți Office” (cu cont)..
   - 0x222e3191 - nu putem încărca automat identitatea, astfel că le vom afișa interfața de utilizator „Aveți Office” (fără cont).
   - 0x222e3193 - am afișat utilizatorului interfața utilizator „Aveți Office” (fără cont) sau nu trebuie să afișăm utilizatorului interfața utilizator „Aveți Office”, deoarece este o ofertă bazată pe dispozitiv.

- **Data_IsClaimTypeDevice** - ne spune dacă tipul de solicitare a ofertei de atașare digitală se bazează pe dispozitiv.

### <a name="officelicensingoobepopulatedigitalattachoffersignindex"></a>Office.Licensing.OOBE.PopulateDigitalAttachOfferSignInDEX

Producătorii de echipamente originale (OEM) vând dispozitive care sunt împreună cu Office (abonamente de un an sau permanente), care sunt plătite atunci când clientul își achiziționează computerul. Acest eveniment monitorizează când sunt găsite drepturi Office pre-acordate pentru dispozitiv și utilizatorul este deja conectat cu un cont Microsoft, pentru a ne permite să monitorizăm starea de funcționare a sistemului și a serviciilor.

Se colectează următoarele câmpuri:

- **Data_ExpirationDate** - ne spune data de expirare a ofertei de abonament

- **Data_IsSubscription** - ne spune dacă produsul de solicitat este un SKU de abonament sau un SKU permanent

- **Data_ProductName** - ne spune numele produsului ofertei de atașare digitală


### <a name="officelicensingoobesearchfordigitalattach"></a>Office.Licensing.OOBE.SearchForDigitalAttach

Producătorii de echipamente originale (OEM) vând dispozitive care sunt împreună cu Office (abonamente de un an sau permanente), care sunt plătite atunci când clientul își achiziționează computerul. Computerele care sunt configurate cu o anumită cheie de registry (OOBEMode: OEMTA) pot avea o ofertă Office atașată digital la acestea. Când pornim Office, efectuăm verificări ale serviciului, pentru a verifica dacă există o ofertă Office atașată digital. Această activitate este utilizată pentru a monitoriza acest lucru. 

Se colectează următoarele câmpuri:

- **Activity_Result_Tag** - ne spune rezultatul general al acestei verificări a serviciului. 
   - 0x222e318c - Flight pentru atașarea digitală dezactivat, astfel că nu se face nicio verificare a serviciului.
   - 0x222e318b - clientul nu are internet, deci nu se face nicio verificare a serviciului.
   - 0x222e318a - s-a găsit o ofertă de atașare digitală care poate fi valorificată
   - 0x222e3189 - s-a găsit o ofertă de atașare digitală care nu poate fi valorificată

- **Data_EnableDAFlight** - ne spune dacă flight pentru atașarea digitală care permite această verificare a serviciului este ACTIVAT sau nu.


### <a name="officelicensingoobeshowtouchlessattachfailuredialog"></a>Office.Licensing.OOBE.ShowTouchlessAttachFailureDialog

Producătorii de echipamente originale (OEM) vând dispozitive care sunt împreună cu Office (abonamente de un an sau permanente), care sunt plătite atunci când clientul își achiziționează computerul. Acest eveniment se declanșează atunci când apare o eroare în fluxul de activare și valorificare a atașării digitale pentru PC-urile OEM care vin împreună cu drepturi Office pre-acordate.  Utilizăm aceste date pentru a monitoriza starea sistemelor și serviciilor și pentru a remedia problemele legate de fluxul de activare pentru Office OEM.

Se colectează următoarele câmpuri:

- **Data_Continue** - ne spune dacă utilizatorul face clic pe "Continuare" în caseta de dialog.

- **Activity_Result_Tag** ne spune butonul pe care a făcut clic utilizatorul în caseta de dialog.
   - 0x222e319d - utilizatorul face clic pe „Reîncercare" în caseta de dialog
   - 0x222e319c - utilizatorul face clic pe „Continuare” în caseta de dialog
   - 0 - utilizatorul iese din caseta de dialog

- **Data_IsForDigitalAttach** - ne spune pe ce platformă și în ce flux de lucru se află utilizatorul - moștenit (activare pentru Office (AFO) sau modern (atașare digitală).

- **Data_Retry** - ne spune dacă utilizatorul face clic pe „Reîncercare” în caseta de dialog.


### <a name="officelicensingoobeshowtouchlessattachofferdialog"></a>Office.Licensing.OOBE.ShowTouchlessAttachOfferDialog

Producătorii de echipamente originale (OEM) vând dispozitive care sunt împreună cu Office (abonamente de un an sau permanente), care sunt plătite atunci când clientul își achiziționează computerul. Acest eveniment monitorizează când sunt găsite drepturi Office pre-acordate pentru dispozitiv și utilizatorul nu este conectat cu un cont Microsoft, pentru a ne permite să monitorizăm starea de funcționare a sistemului și a serviciilor.

Se colectează următoarele câmpuri:

- **Activity_Result_Tag** - ne spune dacă s-a găsit o identitate pentru utilizator
   - 0x222e3194 - nu putem obține identitatea utilizatorului (au anulat conectarea sau autentificarea nu a reușit).
   - 0 - am primit o identitate de la utilizator.

- **Data_ExpirationDate** - ne spune data de expirare a ofertei de abonament

- **Data_IsCentennial** - ne spune dacă aplicația Office care rulează se află pe platforma Centennial

- **Data_IsForDigitalAttach** - ne spune dacă această casetă de dialog este declanșată din fluxul de Atașare digitală sau din fluxul de activare pentru Office.

- **Data_IsSubscription** - ne spune dacă produsul de solicitat este un SKU de abonament sau un SKU permanent

- **Data_OExType** - ne spune dacă utilizatorul iese din caseta de dialog după ce face clic pe linkul ChangeAccount

- **Data_ProductName** - ne spune numele produsului ofertei de atașare digitală

- **Data_UseInAppRedemption** - ne spune dacă utilizăm valorificarea în aplicație pentru valorificarea web - acest lucru este relevant doar pentru fluxul de activare pentru Office.


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

*[Acest eveniment a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

Avem un experiment care oferă utilizatorului opțiunea de a încerca și a configura plata automată pentru Office direct din aplicație, fără să iasă din contextul aplicației. Acesta raportează succesul sau eșecul experimentului respectiv împreună cu codul de eroare Este de importanță critică pentru a detecta dacă utilizatorul se află în stare bună, fără să îi lipsească funcționalități, este utilizat pentru sănătatea sistemului și în scopuri de diagnosticare dacă un utilizator raportează o problemă cu computerul.

Se colectează următoarele câmpuri:

  - **StorePurchaseStatus** - reprezintă codul de eroare/codul de succes al apelului de achiziție care a fost efectuat prin Microsoft Store

### <a name="officelicensingsearchforsessiontoken"></a>Office.Licensing.SearchForSessionToken

Dacă utilizatorul rulează în modul de activare computer partajat, încercăm să căutăm un simbol de sesiune pe computer care permite utilizatorului să folosească aplicația. Acest eveniment raportează succesul sau eșecul scenariului împreună cu codul de eroare. Este de importanță critică pentru a detecta dacă utilizatorul se află în stare bună, fără să îi lipsească funcționalități, este utilizat pentru sănătatea sistemului și în scopuri de diagnosticare dacă un utilizator raportează o problemă cu computerul.

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

- **DexShouldRetry**- semnal că am întâmpinat o problemă recuperabilă (Internetul sau serverele sunt funcționale)

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

După obținerea cu succes a unui cod PIN Office valid legat la un calculator cu Office preinstalat, îi afișăm utilizatorului o casetă de dialog de conectare sau o casetă de dialog de valorificare.  După ce codul PIN a fost valorificat, afișăm caseta de dialog EULA.  Ca parte a procesului modernizare a caracterisiticii noastre AFO, am reîmprospătat cele două casete de dialog, pentru a oferi mai multe informații despre produsul Office care este livrat cu calculatorul.  Această telemetrie este utilizată pentru a urmări dacă caracteristica noastră reduce cu succes dezacordurile cu utilizatorul la valorificarea produsului său, urmărind fluxul și punctele de ieșire ale procesului de valorificare (ce casetă de dialog a fost respinsă).

Se colectează următoarele câmpuri:

- **ActionActivate** - semnal că utilizatorul a făcut clic pe butonul „Activare”.

- **ActionChangeAccount** - semnal că utilizatorul a făcut clic pe hyperlinkul „Utilizare alt cont”.

- **ActionCreateAccount** - semnal că utilizatorul a făcut clic pe butonul „Creare cont”.

- **ActionSignIn** - semnal că utilizatorul a făcut clic pe butonul „Conectare”.

- **CurrentView** - tip de dialog închis de utilizator.

- **DialogEULA** - semnal că am arătat caseta de dialog „Acceptare EULA”. 

- **DialogRedemption** - indică faptul că am afișat caseta de dialog de verificare AFO.

- **DialogSignIn** - indică faptul că am arătat caseta de dialog de conectare AFO.

- **EmptyRedemptionDefaults** - semnal că nu s-a reușit preluarea informațiilor de valorificare implicite.
 
- **GetRedemptionInfo** - semnal că vom prelua informațiile demografice pentru valorificare pin.

- **MalformedCountryCode** - semnalul că codul de țară necesar pentru valorificare pin este incorect.

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
    - 0x03113811      utilizatorul a închis un dialog
    - 0x2370e3a0      utilizatorul a închis un dialog    
    - 0x2370e3c1      mergeți la web pentru valorificare pin 
    - 0x2370e3a1      mergeți la web pentru valorificare pin
    - 0x2370e3c0      secvență de dialog în buclă, cauzată de utilizatorul care merge înainte și înapoi în fluxul de dialog
    - 0x2370e3a3      utilizatorul a făcut clic pe hyperlinkul „Nu acum“, care omite oferta AFO pentru acea sesiune
    - 0x2370e3a2      utilizatorul a făcut clic pe hyperlinkul „Nu îmi arătați niciodată aceasta“, care dezactivează oferta AFO


- **UseInAppRedemption** - ne spune dacă menținem utilizatorii în aplicație pentru valorificare sau îi trimitem pe web pentru a-și valorifica PIN-ul preluat (pre populat).

- **UseModernAFO** - ne spune dacă utilizăm noua sau vechea experiență AFO.

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

- **InAppTrialPurchase** - indică dacă lansarea este activată pentru lansarea de achiziție din Magazin SDK pentru a captura PI și a achiziționa o versiune de încercare în cadrul aplicației *[Acest câmp a fost șters din compilările curente Office, dar s-ar putea să apară încă în vechile compilări.]*

- **IsRS1OrGreater** - indică dacă versiunea sistemului de operare este mai mare decât RS1 sau nu, deoarece SDK de achiziție în Magazin ar trebui să fie utilizat doar dacă versiunea sistemului de operare este mai mare decât RS1

- **NotInitializedBeforeWhileAdding**: este doar informativ și indică dacă evenimentul a fost adăugat la o hartă a managerului de telemetrie fără să se înregistreze explicit pentru aceasta

- **OEMSendToWebForTrial** - indică dacă ediția flight este activată pentru a trimite utilizatorii pe web pentru a valorifica o versiune de încercare

- **StoreErrorConditions** - indică condițiile diverse sub care achiziția din magazin SDK putea să eșueze *[Acest câmp a fost eliminat din compilările curente Office, dar poate apărea în continuare în versiuni mai vechi.]*

- **StoreErrorHResult** - indică codul de eroare returnat din achiziția din magazin SDK *[Acest câmp a fost eliminat din compilările curente Office, dar poate apărea în continuare în compilări mai vechi.]*

- **StorePurchaseStatusResult** - indică rezultatul apelării achiziției  din magazin SDK, iar dacă utilizatorul a achiziționat sau nu, va ajuta să se determine dacă utilizatorul trebuie să primească licență pentru a utiliza Office *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în compilări mai vechi.]*

- **Tag** - utilizat pentru a indica de unde din cod a fost trimis evenimentul

- **UserSignedInExplicitly** - indică dacă utilizatorul s-a conectat în mod explicit, în acest caz, am redirecționa utilizatorii către web pentru versiunea de încercare *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

### <a name="officelicensingusegracekey"></a>Office.Licensing.UseGraceKey

Dacă, dintr-un motiv sau altul, nu putem să licențiem utilizatorul, instalăm o cheie de grație și trimitem acest semnal cu semnificație. Este de importanță critică pentru a detecta dacă utilizatorul se află în stare bună, fără să îi lipsească funcționalități, este utilizat pentru sănătatea sistemului și în scopuri de diagnosticare dacă un utilizator raportează o problemă cu computerul

Se colectează următoarele câmpuri:

  - **OpportunisticTokenRenewalAttempted** - indică dacă am încercat o reînnoire oportunistă pentru utilizator în modul de activare computer partajat

  - **ReArmResult** - indică rezultatul reactivării perioadei de probă a cheii instalate, ceea ce poate extinde valabilitatea licenței curente

### <a name="onenoteenrollmentresult"></a>OneNote.EnrollmentResult
 
Acest eveniment înregistrează starea la înscrierea în Intune.  Acest scenariu este specific conturilor activate pentru Intune.
 
Se colectează următoarele câmpuri:
 
- **EnrollmentResult** - rezultatul înscrierii în Intune

### <a name="skuproductpricenullevent"></a>SKU.PREȚ.PRODUS.NUL.EVENIMENT

Acest eveniment este utilizat pentru a capta evenimentele în vederea cuantificării impactului erorii, datorită căreia utilizatorii văd astăzi „Nul” în loc de un preț, pe ecranul selector SKU. Eroarea va fi diagnosticată în continuare, pentru a stabili o remediere. 

Se colectează următoarele câmpuri:

- **PrețNegăsit** - Prețurile nu se găsesc în magazin.

- **MagazinNeinițializat** - când magazinul nu este inițializat cu succes.


## <a name="microsoft-autoupdate-mau-events"></a>Evenimente Microsoft AutoUpdate (MAU)

### <a name="additionalappinfoinvalidpreference"></a>additionalappinfo.invalidpreference

Aceste rapoarte de evenimente despre preferința nevalidă sunt setate pentru a afișa mai multe informații cu privire la sfârșitul serviciului pentru un produs. Vom utiliza aceste informații pentru a recomanda clienților să își seteze corect preferințele pentru a vedea informații suplimentare.
 
Se colectează următoarele câmpuri:

- **App** – procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** – versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **Reason** - detalii despre intrarea nevalidă din preferințe

- **SessionId** - identificatorul pentru sesiune

### <a name="appdelegatelaunch"></a>appdelegate.launch

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


### <a name="appdelegateterminate"></a>appdelegate.terminate

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


### <a name="appinstallconnecttoxpc"></a>appinstall.connecttoxpc

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

### <a name="appinstalllogscanned"></a>appinstall.logscanned

Acest eveniment este utilizat pentru a determina dacă s-a procesat cu succes fișierul jurnal. Vom utiliza acest eveniment pentru a detecta și a rezolva problemele apărute în timpul instalării aplicațiilor. 
 
Se colectează următoarele câmpuri:

- **App** – procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** – versiunea aplicației

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

- **Payload** - rapoarte privind erorile găsite în timpul instalării și/sau scanării stării de finalizare a aplicației 

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

### <a name="appinstallxpcremoteobjecterror"></a>appinstall.xpcremoteobjecterror

Acest eveniment raportează o eroare găsită în timp ce încearcă să se conecteze la Instrumentul de Ajutor Privilegiat prin conexiunea XPC. Utilizăm acest eveniment pentru a urmări și a rezolva problemele posibile de instalare MAU.

Se colectează următoarele câmpuri:

- **App** – procesul aplicației care trimite evenimentul

- **AppID** - identificatorul aplicației.

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** – versiunea aplicației

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

- **Payload** - Conține informații despre natura erorii întâlnite cu înregistrarea aplicațiilor.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="appregistryconfig"></a>appregistry.config

Acest eveniment raportează despre orice erori întâlnite în timpul încărcării informațiilor din registry aplicație. Utilizăm acest raport pentru a consilia administratorii IT în formatul corect de configurare a înregistrărilor de aplicații client.
 
Se colectează următoarele câmpuri:

- **App** – procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** – versiunea aplicației

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

- **Payload** -conține informații despre natura erorii întâlnite cu înregistrarea aplicațiilor.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

### <a name="appregistryinfo"></a>appregistry.info

Acest eveniment indică faptul că aplicația a fost lansată. Vom utiliza acest eveniment pentru a lista aplicațiile pentru care MAU poate controla actualizările, numărul de copii disponibile, precum și versiunea și locația de instalare a acestora (implicită sau alta).

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


### <a name="appregistryremove"></a>appregistry.remove

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


### <a name="catalogerrorsignature"></a>catalog.errorsignature

Acest eveniment raportează diverse probleme cu fișierele descărcate, inclusiv nepotrivirile legate de semnătura furnizorului și valoarea hash din fișierul descărcat. Utilizăm acest eveniment pentru a detecta problemele cu publicarea setului manifest pentru aplicații.

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

- **FileHash** – valoarea hash a fișierului descărcat

- **NumeFișier** – numele fișierului care afișează nepotrivirea legată de valoarea hash

- **HashInCatalog** – intrare de valoare hash în fișierul catalog corespunzător

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Codul de** - conține informații despre problema de raportare a aplicației

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="cataloginvalid"></a>catalog.invalid

Acest eveniment înregistrează o condiție de eroare care indică catalogul de manifest nevalid descărcat. Utilizăm acest eveniment pentru a ne asigura că nu există erori în fișierele manifest publicate. 

Se colectează următoarele câmpuri:

- **App** – procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** – versiunea aplicației

- **CatalogFile** – Numele fișierului din catalog care a determinat condiția de eroare.

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - Țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** – Versiunea sistemului de operare

- **Event_ReceivedTime** - Ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="cloningtaskbegin"></a>cloningtask.begin

Acest eveniment indică începutul activității de clonare anterioare actualizării aplicațiilor. Utilizăm acest eveniment împreună cu evenimentul cloningtask.status, pentru a determina volumul de erori de clonare, în scopul de a stabili dacă caracteristica de clonare ar trebui să fie limitată pe diferite canale de public.
 
Se colectează următoarele câmpuri:

- **App** – procesul aplicației care trimite evenimentul

- **AppID** - identificatorul aplicației.

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** – versiunea aplicației

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

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

- **UpdateID** - identificatorul pentru actualizare.


### <a name="cloningtaskhelpertoolconnection"></a>cloningtask.helpertoolconnection

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

### <a name="cloningtaskstatus"></a>cloningtask.status

Acest eveniment indică starea procesului de clonare pentru ca aplicația să fie actualizată. Vom utiliza acest eveniment pentru a determina rata de succes, precum și tipurile de erori întâlnite care duce la nereușită. Acest eveniment este utilizat pentru a determina dacă caracteristica de clonare ar trebui să fie limitată în funcție de diferite canale de public.

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppID** - identificatorul aplicației.

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Error** - șirul conține informații despre eroare, dacă s-a produs o eroare în timpul activității de clonare.

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

- **Success** - reprezentarea șirului unei variabile Boolean.

- **UpdateID** - identificatorul pentru actualizare.

### <a name="cloningtaskstatusfinish"></a>cloningtask.status.finish

Acest eveniment raportează despre finalizarea activității de „clonare“. Acest eveniment face parte din raportul pâlniei de actualizare și îl utilizăm pentru a determina starea de funcționare a actualizărilor aplicației.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppID** - identificatorul aplicației

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

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

- **Success** - indică dacă activitatea de clonare a reușit

- **UpdateID** - identificatorul actualizării.


### <a name="configurationchannel"></a>configuration.channel

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


### <a name="configurationmetadata"></a>configuration.metadata

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

### <a name="configurationsystemversion"></a>configuration.systemVersion

Acest eveniment indică faptul că o încercare de a recupera versiunea de sistem a eșuat. De asemenea, conține informații despre informațiile colectate din sistem de Microsoft AutoUpdate (MAU). Utilizăm acest eveniment pentru a determina dacă MAU ar trebui să răspundă pentru erori. Rețineți că versiunea de sistem este utilizată pentru a determina dacă o actualizare poate să fie aplicată la dispozitivul clientului.
 
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

- **Payload** - conține informații despre eroarea întâlnită în timpul recuperării șirului versiunii de sistem macOS.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

### <a name="controlleralertmanagerreinstallresponse"></a>controller.alertmanager.reinstallresponse

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

    
### <a name="controlleralertmanagertmpdiskfull"></a>controller.alertmanager.tmpdiskfull

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


### <a name="controlleralertmanagertmpdiskfullretry"></a>controller.alertmanager.tmpdiskfullretry

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
    

### <a name="controlleralertmanagertmpdiskfullretrycancel"></a>controller.alertmanager.tmpdiskfullretrycancel

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

    
### <a name="controllercheckwindownoupdatefoundok"></a>controller.checkwindow.noupdatefoundok

Acest eveniment indică faptul că nu au fost găsite actualizări în urma unei verificări a actualizărilor. Utilizăm acest eveniment pentru a ne asigura că actualizările sunt oferite corect, pentru a optimiza încărcarea serviciilor și pentru a defini frecvența de verificare a actualizărilor. De asemenea, dorim să optimizăm frecvența lansărilor noastre, pe baza așteptărilor utilizatorilor în ceea ce privește actualizările.

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

    

### <a name="controllercheckwindowupdatecheck"></a>controller.checkwindow.updatecheck

Acest eveniment indică faptul că a fost efectuată o verificare a actualizărilor. Utilizăm acest eveniment pentru a ne asigura că actualizările sunt oferite corect, pentru a optimiza încărcările serviciilor și pentru a defini cât de frecvente ar trebui să fie verificările actualizărilor noastre. De asemenea, dorim să ne optimizăm cadența de lansare pe baza așteptărilor utilizatorilor față de actualizări.

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


### <a name="controllercheckwindowupdatecheckcancel"></a>controller.checkwindow.updatecheckcancel

Acest eveniment denotă faptul că procesul de verificare a actualizărilor a fost anulat (fie de către utilizator, fie de sistem). Utilizăm acest eveniment pentru a ne asigura că actualizările sunt oferite corect, pentru a optimiza încărcările serviciilor și pentru a defini cât de frecvente ar trebui să fie verificările actualizărilor noastre. De asemenea, dorim să ne optimizăm cadența de lansare pe baza așteptărilor utilizatorilor față de actualizări.

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

    
### <a name="controllercheckwindowupdatecheckcanceluser"></a>controller.checkwindow.updatecheckcanceluser

Acest eveniment indică faptul că procesul de verificare a actualizărilor a fost anulat de către utilizator. Utilizam acest eveniment pentru a ne asigura că actualizările sunt oferite corect, pentru a optimiza încărcările serviciilor și pentru a defini cât de frecvente ar trebui să fie verificările actualizărilor noastre. De asemenea, dorim să optimizăm cadența de lansare pe baza așteptărilor utilizatorilor față de actualizări.

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

    
### <a name="controllercheckwindowupdatesfound"></a>controller.checkwindow.updatesfound

Acest eveniment denotă faptul că procesul de verificare a actualizărilor a avut ca rezultat actualizări găsite. Utilizăm acest eveniment pentru a ne asigura că actualizările sunt oferite corect.

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

    
### <a name="controllercheckwindowuptodate"></a>controller.checkwindow.uptodate

Acest eveniment indică faptul că nu au fost găsite actualizări în urma procesului de verificare a actualizărilor, deoarece aplicațiile de pe dispozitiv sunt actualizate.  Utilizăm acest eveniment pentru a ne asigura că actualizările sunt oferite corect.

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


### <a name="controllerdownloadwindowapplaunchwithpendingupdate"></a>controller.downloadwindow.applaunchwithpendingupdate

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

    
### <a name="controllerdownloadwindowcloseapplicationdialog"></a>controller.downloadwindow.closeapplicationdialog

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

    
### <a name="controllerdownloadwindowcurtasknull"></a>controller.downloadwindow.curtasknull

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

    
### <a name="controllerdownloadwindowdownloadcancel"></a>controller.downloadwindow.downloadcancel

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

    
### <a name="controllerdownloadwindowdownloadfailed"></a>controller.downloadwindow.downloadfailed

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

    
### <a name="controllerdownloadwindowdownloadfailedok"></a>controller.downloadwindow.downloadfailedok

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


### <a name="controllerdownloadwindowdownloadpathmissing"></a>controller.downloadwindow.downloadpathmissing

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


### <a name="controllerdownloadwindowdownloadtasknull"></a>controller.downloadwindow.downloadtasknull

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


### <a name="controllerdownloadwindowfilesignaturenotverified"></a>controller.downloadwindow.filesignaturenotverified

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


### <a name="controllerdownloadwindowinstallcomplete"></a>controller.downloadwindow.installcomplete

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


### <a name="controllerdownloadwindownetworkunavailablealert"></a>controller.downloadwindow.networkunavailablealert

Acest eveniment denotă faptul că conectivitatea la rețea s-a pierdut în timpul descărcării actualizărilor.  Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează conform așteptărilor și pentru a ajuta la depanarea erorilor.

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

    
### <a name="controllerdownloadwindownetworkunavailablealertok"></a>controller.downloadwindow.networkunavailablealertok

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

    
### <a name="controllerdownloadwindownoconnectionok"></a>controller.downloadwindow.noconnectionok

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


### <a name="controllerdownloadwindowrepairrequired"></a>controller.downloadwindow.repairrequired

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

### <a name="controllerdownloadwindowupdateaborted"></a>controller.downloadwindow.updateaborted

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


### <a name="controllerdownloadwindowupdatefailed"></a>controller.downloadwindow.updatefailed

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


### <a name="controllerdownloadwindowupdatesuccessful"></a>controller.downloadwindow.updatesuccessful

Acest eveniment indică faptul că toate actualizările din lotul actual au avut succes. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează conform așteptărilor și pentru a ajuta la depanarea erorilor.

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


### <a name="controllerdownloadwindowuserpaused"></a>controller.downloadwindow.userpaused

Acest eveniment indică faptul că toate actualizările din lotul actual au avut succes. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează conform așteptărilor și pentru a ajuta la depanarea erorilor.

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


### <a name="controllerdownloadwindowuserresumed"></a>controller.downloadwindow.userresumed

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


### <a name="controllermainwindowsetautomaticchecking"></a>controller.mainwindow.setautomaticchecking

Acest eveniment indică faptul că dispozitivul a fost înscris în modul de Actualizare automată. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.

Se colectează următoarele câmpuri:

 - **App** – procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** – versiunea aplicației

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


### <a name="controllermainwindowsetautomaticdownloadinstall"></a>controller.mainwindow.setautomaticdownloadinstall

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

    
### <a name="controllermainwindowsetmanualchecking"></a>controller.mainwindow.setmanualchecking

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

    
### <a name="controllertemplateawindowcancel"></a>controller.templateawindow.cancel

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

    
### <a name="controllertemplateawindowenroll"></a>controller.templateawindow.enroll

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



### <a name="controllertemplateawindowinstall"></a>controller.templateawindow.install

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


### <a name="controllerupdatewindowbegindownloadingapps"></a>controller.updatewindow.begindownloadingapps

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

    
### <a name="controllerupdatewindownetworkretry"></a>controller.updatewindow.networkretry

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

    
### <a name="controllerupdatewindownetworkretrycancel"></a>controller.updatewindow.networkretrycancel

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


### <a name="controllerupdatewindownetworkunavailable"></a>controller.updatewindow.networkunavailable

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


### <a name="controllerupdatewindownoupdateavailable"></a>controller.updatewindow.noupdateavailable

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


### <a name="controllerupdatewindownoupdatestoselect"></a>controller.updatewindow.noupdatestoselect

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


### <a name="controllerupdatewindowupdateavailable"></a>Controller.UpdateWindow.UpdateAvailable

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

    
### <a name="controllerupdatewindowupdateavailablecancel"></a>controller.updatewindow.updateavailablecancel

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


### <a name="downloadactorpause"></a>downloadactor.pause

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


### <a name="downloadactorredirect"></a>downloadactor.redirect

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

    
### <a name="downloadactorresume"></a>downloadactor.resume

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


### <a name="downloadactorresumeerror"></a>downloadactor.resumeerror

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

    
### <a name="downloadactorstatus"></a>downloadactor.status

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


### <a name="downloadmanifestconfiguration"></a>downloadmanifest.configuration

Acest eveniment raportează o eroare cu configurația Microsoft AutoUpdate (MAU), fie cu configurarea Server particularizat din preferințe sau cu definițiile de punct final din Asistentul de actualizare din componentele MAU instalate. Utilizăm acest eveniment pentru a recomanda administratorilor IT să seteze puncte finale din serverul manifest corecte
 
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

- **Payload** - indică dacă eroarea se află în configurarea serverelor particularizate sau în componentele instalate MAU

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="downloadmanifestdownloadcatalogfail"></a>downloadmanifest.downloadcatalogfail

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

    
### <a name="downloadmanifestdownloadcatalogsuccess"></a>downloadmanifest.downloadcatalogsuccess

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


### <a name="downloadmanifestdownloadfail"></a>downloadmanifest.downloadfail

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


### <a name="downloadmanifestdownloadfromurl"></a>downloadmanifest.downloadfromurl

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


### <a name="downloadmanifestdownloading"></a>downloadmanifest.downloading

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


### <a name="downloadmanifestdownloadsuccess"></a>downloadmanifest.downloadsuccess

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

    
### <a name="downloadmanifestdownloadurl"></a>downloadmanifest.downloadurl

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


### <a name="downloadmanifestfilenameerror"></a>downloadmanifest.filenameerror

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


### <a name="downloadmanifestinvalidhash"></a>downloadmanifest.invalidhash

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


### <a name="downloadmanifestmissingdaemon"></a>downloadmanifest.missingdaemon

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


### <a name="downloadmanifestsignatureerror"></a>downloadmanifest.signatureerror

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


### <a name="downloadmanifeststatus"></a>downloadmanifest.status

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


### <a name="downloadmgrdownloadend"></a>downloadmgr.downloadend

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


### <a name="downloadmgrdownloadstart"></a>downloadmgr.downloadstart

Acest eveniment înregistrează actualizarea care urmează să fie descărcată. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează conform așteptărilor și pentru a ajuta la depanarea erorilor.
 
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

### <a name="downloadtaskdownloadbegin"></a>downloadtask.downloadbegin

Acest eveniment indică începutul activității de descărcare pentru o actualizare de aplicație. Acesta face parte din pâlnia de actualizare și îl utilizăm pentru a determina starea de funcționare a actualizărilor de aplicații.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppID** - identificatorul pentru aplicația actualizată

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **BundleVersion** - versiunea aplicației actualizată

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **PreviousUpdateID** - identificatorul pentru o actualizare de aplicație

- **SessionId** - identificatorul pentru sesiune

- **UpdateID** - identificatorul pentru o actualizare de aplicație

- **UpdatePkg** - numele pachetului de actualizare aplicată

- **UpdateVersion** - versiunea aplicației după actualizare


### <a name="downloadtaskdownloadfailure"></a>downloadtask.downloadfailure

Acest eveniment înregistrează faptul că s-a produs o eroare la descărcarea unui fișier pachet. Înregistrăm calea actualizării și eroarea. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppID** - identificatorul aplicației care are eroarea de descărcare.

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Error** - eroarea observată în timpul descărcării.

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține numele actualizării care este descărcată și eroarea observată. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

- **UpdateID** - identificatorul actualizării care se descarcă.


### <a name="downloadtaskdownloadsuccess"></a>downloadtask.downloadsuccess

Descărcarea cu succes a unui fișier pachet. Înregistrăm calea actualizării utilizate. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppID** - identificatorul aplicației.

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

- **UpdateID** - identificatorul actualizării descărcate.

### <a name="downloadtaskupdatertypeerror"></a>downloadtask.updatertypeerror

Acest eveniment raportează o eroare de tip actualizator în fișierul manifest descărcat. Folosim acest eveniment pentru a notifica proprietarul fișierului manifest, astfel încât eroarea să poată fi remediată.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppID** - identificatorul pentru aplicația actualizată

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

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

- **UpdateID** - identificatorul pentru o actualizare de aplicație

- **UpdaterType** - tipul de actualizator specificat în fișierul manifest descărcat

- **UpdateURL** - URL-ul pachetului de actualizare care trebuie aplicat

### <a name="downloadtaskurlerror"></a>downloadtask.urlerror

Acest eveniment raportează o eroare din URL-ul specificat în fișierul manifest descărcat. Folosim acest eveniment pentru a notifica proprietarul fișierului manifest, astfel încât eroarea să poată fi remediată.
 
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

- **Error** - indică tipul erorii întâlnite

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

- **UpdateID** - identificatorul pentru o actualizare de aplicație

- **UpdateURL** - URL-ul pachetului de actualizare care trebuie aplicat

### <a name="fbachangelastupdate"></a>fba.changelastupdate

Acest eveniment raportează atunci când Microsoft Auto Update (MAU) a căutat actualizări. Folosim acest eveniment pentru depanare atunci când nu se oferă o actualizare unui anumit dispozitiv pentru o perioadă prelungită de timp.

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

- **Payload** - conține Data Ora când MUA a căutat actualizări

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="fbacheckforupdate"></a>fba.checkforupdate

Acest eveniment indică faptul că un proces de fundal verifică actualizările. Folosim acest eveniment pentru a ne asigura că procesul de actualizare funcționează conform așteptărilor și pentru a ajuta la depanarea erorilor.
 
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


### <a name="fbacheckforupdateskip"></a>fba.checkforupdateskip

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


### <a name="fbaforceinstallmsgsent"></a>fba.forceinstallmsgsent

Acest eveniment indică faptul că a fost inițiată o actualizare forțată din interfața utilizator. Acest eveniment face parte din pâlnie și este folosit pentru a determina buna funcționare a caracteristicii de actualizare forțată.

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

- **Payload** - text static

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

### <a name="fbaforceupdatecheck"></a>fba.forceupdatecheck

Acest eveniment indică faptul că verificarea actualizărilor este forțată. Utilizăm acest eveniment pentru a determina volumul de verificări forțate ale actualizărilor, care au loc în afara ciclului normal de verificare a actualizărilor.

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

- **HowToCheck** - cum se verifică setările

- **Payload** - text static

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

### <a name="fbaguiappopen"></a>fba.guiappopen

Acest eveniment indică faptul că interfața de utilizator este lansată în modul de Verificare automată, având o aplicație cu actualizare aplicabilă deschisă acum. Acest eveniment este folosit pentru a determina volumul de lansări de interfață cu utilizatorul din modul de Verificare automată pentru dezvoltarea caracteristicilor viitoare.

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

- **HowToCheck** - cum se verifică setările

- **Payload** - text static

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

### <a name="fbainstallpending"></a>fba.installpending

Acest eveniment indică faptul că Microsoft Auto Update (MAU) a trimis o notificare cu privire la actualizările în așteptare. Acest eveniment este folosit pentru a determina volumul de actualizări care sunt inițiate din notificările de utilizator și este utilizat pentru a îmbunătăți experiența utilizatorilor, prin minimizarea întreruperilor pentru utilizator în versiunile ulterioare.

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

- **HowToCheck** - cum se verifică setările

- **Payload** - text static

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

### <a name="fbalaunch"></a>fba.launch

Acest eveniment indică începutul Asistentului de actualizare Microsoft cu privire la metoda de lansare. Acest eveniment este utilizat pentru a determina dacă Asistentul pentru actualizare Microsoft este lansat într-un context incorect.

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

- **HowToCheck** - cum se verifică setările

- **Payload** - text static

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

### <a name="fbalaunchbyagent"></a>fba.launchbyagent

Acest eveniment indică faptul că Asistentul pentru actualizare Microsoft a fost lansat prin intermediul Agentului de lansare. Acest eveniment este utilizat pentru a determina volumul Asistentului de actualizare Microsoft lansat din interfața de utilizator pentru dezvoltare viitoare.

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

- **HowToCheck** - cum se verifică setările

- **Payload** - text static

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

### <a name="fbalaunchfromprotocol"></a>fba.launchfromprotocol

Acest eveniment indică faptul că Asistentul de actualizare Microsoft a fost lansat prin intermediul protocolului de URL. Acest eveniment este utilizat pentru a determina volumul Asistentului de actualizare Microsoft lansat prin URL pentru dezvoltare viitoare.

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

- **HowToCheck** - cum se verifică setările

- **Payload** - conține informații despre schema URL și gazdă URL

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

### <a name="fbalaunchgui"></a>fba.launchgui

Acest eveniment indică faptul că Asistentul de actualizare Microsoft încearcă să lanseze Interfața grafică cu utilizatorul (GUI). Acest eveniment este folosit pentru a determina volumul de lansări UI inițiate din Asistentul de actualizare Microsoft, pentru a ajuta cu dezvoltarea viitoare, inclusiv cu minimizarea întreruperii utilizatorului din cauza lansării frecvente de UI.

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

- **HowToCheck** - cum se verifică setările

- **Payload** - text static

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="fbalaunchstatus"></a>fba.launchstatus

Acest eveniment înregistrează eșecurile daemonului MAU în timp ce încearcă să se lanseze. Folosim acest eveniment pentru a ne asigura că procesul de actualizare funcționează conform așteptărilor și pentru a ajuta la depanarea erorilor.
 
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

- **Error** - conține OSStatus (codul de stare Apple) care reflectă starea lansării.

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține OSStatus (codul de stare Apple) care reflectă starea lansării. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

- **Success** - șirul de caractere boolean care indică dacă s-a lansat cu succes sau nu procesul daemon MAU.


### <a name="fbamausilentupdate"></a>fba.mausilentupdate

Acest eveniment indică faptul că Asistentul de actualizare Microsoft inițiază actualizări silențioase. Acest eveniment este utilizat pentru a determina volumul actualizărilor aplicate fără intervenția utilizatorului, pentru a contribui la îmbunătățirea experienței utilizatorului.

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

- **HowToCheck** - cum se verifică setările

- **Activity Result** - text static *[Acest câmp a fost eliminat din compilările de Office actuale, dar poate apărea în continuare în compilări mai vechi.]*

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **Motivul** - textul static care indică faptul că o actualizare silențioasă nu poate continua, întrucât interfața utilizator este deschisă

- **SessionId** - identificatorul pentru sesiune

### <a name="fbamoreinfofromappnotification"></a>fba.moreinfofromappnotification

Acest eveniment raportează despre informațiile pe care le distribuie o aplicație înregistrată prin intermediul Microsoft auto update (MAU). De exemplu, mesajele de la sfârșitul serviciului sunt transmise prin notificarea MAU. Folosim acest eveniment pentru a determina volumul de dispozitive care afișează această notificare specială, pentru a determina reușita diseminării informațiilor.

Se colectează următoarele câmpuri:

- **AdditionalInfoID** - identifică în mod unic „Mai multe informații” fiind transmise prin MAU.

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

- **HowToCheck** - cum se verifică setările

- **NotificationEvent** - textul static care indică tipul de notificare în curs de aplicare.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

### <a name="fbamultipledaemon"></a>fba.multipledaemon

Acest eveniment indică faptul că a fost detectată o altă instanță a asistentului de actualizare Microsoft, iar instanța curentă va fi încheiată. Vom folosi acest eveniment pentru a determina volumul de dispozitive care încearcă să ruleze mai multe instanțe ale asistentului de actualizare și să proiecteze o soluție, dacă este necesar.

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

- **HowToCheck** - cum se verifică setările

- **Payload** - text static

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

### <a name="fbanofifyappclosed"></a>fba.nofifyappclosed

Acest eveniment indică faptul că asistentul de actualizare Microsoft trimite o notificare pentru actualizări în așteptare, deoarece nu există nicio aplicație înregistrată deschisă, iar actualizările pot continua fără a întrerupe utilizatorul. Folosim acest eveniment pentru a determina volumul de actualizări care se pot aplica, dar aveți nevoie de acțiunea utilizatorului pentru a face acest lucru. Acest eveniment este folosit pentru a contribui la îmbunătățirea experienței de utilizator.

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
    
- **HowToCheck** - cum se verifică setările
    
- **Payload** - text static
    
- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)
    
- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP
    
- **SessionId** - identificatorul pentru sesiune

### <a name="fbanofifyappopen"></a>fba.nofifyappopen

Acest eveniment indică faptul că asistentul de actualizare Microsoft trimite o notificare pentru actualizări în așteptare, deoarece există aplicații înregistrate deschise, iar pentru a continua actualizările trebuie închise aplicațiile.  Folosim acest eveniment pentru a determina volumul de actualizări care necesită intervenția utilizatorului.  Acest eveniment este folosit pentru a contribui la îmbunătățirea experienței de utilizator.

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

- **HowToCheck** - cum se verifică setările

- **Payload** - text static

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

### <a name="fbasettimerfail"></a>fba.settimerfail  

Acest eveniment indică faptul că o încercare de a configura cronometrul pentru a declanșa o actualizare viitoare a eșuat. Acest eveniment este esențial și îl folosim pentru a determina volumul de erori pentru a crea soluții temporare, dacă este necesar.

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

- **HowToCheck** - cum se verifică setările

- **Payload** - conține informațiile despre ora ultimei actualizări și utilizarea calendarului

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="fbasilentupdateoptin"></a>fba.silentupdateoptin

Acest eveniment indică faptul că utilizatorul optează pentru actualizări silențioase. Folosim acest eveniment pentru a ne asigura că procesul de actualizare funcționează conform așteptărilor și pentru a ajuta la depanarea erorilor.
 
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

### <a name="fbaskipforcedupdate"></a>fba.skipforcedupdate

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


### <a name="fbastartforcedupdate"></a>fba.startforcedupdate

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


### <a name="fbaterminate"></a>fba.terminate

Acest eveniment indică faptul că demonul MAU s-a terminat în mod normal. Folosim acest eveniment pentru a ne asigura că procesul de actualizare funcționează conform așteptărilor și pentru a ajuta la depanarea erorilor.
 
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


### <a name="fbaupdatefound"></a>fba.updatefound

Acest eveniment indică faptul că demonul MAU a găsit actualizări disponibile pentru a oferi. Folosim acest eveniment pentru a ne asigura că procesul de actualizare funcționează conform așteptărilor și pentru a ajuta la depanarea erorilor.
 
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

    
### <a name="fbaupdatetimer"></a>fba.updatetimer

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


### <a name="fbasilentupdateallappsclosed"></a>fbasilentupdate.allappsclosed

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


### <a name="fbasilentupdateapplaunchafterupdate"></a>fbasilentupdate.applaunchafterupdate

Acest eveniment înregistrează o încercare de a relansa aplicația după o actualizare silențioasă și modul de actualizare (clonă sau nu). Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppID** - identificatorul aplicației.

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Error** - detaliul erorii survenite în timpul lansării aplicației după actualizare.

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține un identificator utilizat pentru urmărirea unei activități de actualizare și numele aplicației care urmează să fie lansată. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*
    
- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)
    
- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="fbasilentupdateapplaunchwileinstalling"></a>fbasilentupdate.applaunchwileinstalling

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


### <a name="fbasilentupdateappneedtoclose"></a>fbasilentupdate.appneedtoclose

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


### <a name="fbasilentupdateappterminationeventreceived"></a>fbasilentupdate.appterminationeventreceived

Acest eveniment indică faptul că Microsoft Autoupdate a primit un eveniment Apple care informează că aplicația a fost oprită. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppID** - identificatorul aplicației.

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Error** - detaliul despre eroarea survenită în timpul terminării aplicației.

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține un identificator utilizat pentru urmărirea unei activități de actualizare și ID-ul pachetului aplicației. Acesta poate conține și un șir de erori dacă Microsoft Autoupdate determină că aplicația încă rulează, chiar dacă a fost primit un eveniment de oprire. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

- **UpdateID** - identificatorul actualizării aplicației.


### <a name="fbasilentupdateclientsession"></a>FBASilentUpdate.ClientSession

Acest eveniment este folosit pentru a calcula indicatorul de stare de funcționare a actualizării esențiale calculate pentru Microsoft AutoUpdate (MAU). Acest eveniment ne permite să indicăm ce sesiune de actualizare (descărcare sau instalare) gestionează backend-ul în acest moment.
 
Se colectează următoarele câmpuri:

- **App** – procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** – versiunea aplicației

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

- **Payload** - indică ce sesiune de actualizare (descărcare sau instalare) gestionează backend-ul în acest moment.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="fbasilentupdatecodesignfailure"></a>fbasilentupdate.codesignfailure

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


### <a name="fbasilentupdatedownload"></a>fbasilentupdate.download

Acest eveniment denotă faptul că o actualizare este în curs de descărcare. Folosim acest eveniment pentru a ne asigura că procesul de actualizare funcționează conform așteptărilor și pentru a ajuta la depanarea erorilor.
 
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

- **ScreenLocked** – indicați dacă descărcarea este inițiată în spatele ecranului blocat

- **SessionId** - identificatorul pentru sesiune


### <a name="fbasilentupdatedownloadfailed"></a>fbasilentupdate.downloadfailed

Acest eveniment indică faptul că s-a produs o eroare în timpul descărcării unei actualizări. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppID** - identificatorul aplicației.

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Error** - detaliul erorii survenite în timpul descărcării actualizării aplicației.

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține un identificator utilizat pentru urmărirea unei activități de actualizare și numele unei actualizări. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

- **UpdateID** - identificatorul actualizării aplicației.

- **UpdateName** - numele actualizării aplicației.


### <a name="fbasilentupdatedownloadinbackground"></a>fbasilentupdate.downloadinbackground

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


### <a name="fbasilentupdatedownloadingrepairupdate"></a>fbasilentupdate.downloadingrepairupdate

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

- **ScreenLocked** – indicați dacă descărcarea este inițiată în spatele ecranului blocat

- **SessionId** - identificatorul pentru sesiune


### <a name="fbasilentupdateduplicatedownloadattempted"></a>fbasilentupdate.duplicatedownloadattempted

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


### <a name="fbasilentupdateinstallattemptfailed"></a>fbasilentupdate.installattemptfailed

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


### <a name="fbasilentupdateinstallcomplete"></a>fbasilentupdate.installcomplete

Acest eveniment indică faptul că toate actualizările din lot au terminat instalarea. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează conform așteptărilor și pentru a ajuta la depanarea erorilor.
 
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


### <a name="fbasilentupdateinstalled"></a>fbasilentupdate.installed

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

    
### <a name="fbasilentupdateinstalling"></a>fbasilentupdate.installing

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

### <a name="fbasilentupdateinstallstatus"></a>fbasilentupdate.installstatus

Acest eveniment raportează despre starea activității de actualizare a aplicației. Acest eveniment face parte din pâlnia de actualizare a aplicației și o utilizăm pentru a monitoriza starea de funcționare a actualizărilor aplicației.

Se colectează următoarele câmpuri: 

- **App** - procesul aplicației care trimite evenimentul

- **AppID** - identificatorul pentru aplicația actualizată

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

- **HowToCheck** - cum se verifică setările

- **Payload** - conține informații referitoare la afișarea vizualizării statusului

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

- **Success** - indică dacă actualizarea aplicației a fost reușită

- **UpdateID** - identificatorul pentru o actualizare de aplicație

- **UpdateName** - numele actualizării așa cum apare în fișierul manifest descărcat

- **UpdatePkg** - numele pachetului de actualizare aplicată

### <a name="fbasilentupdatenotificationerror"></a>fbasilentupdate.notificationerror

Acest eveniment raportează despre o eroare întâlnită în timpul încercării de a trimite notificarea utilizatorului. Acest eveniment va fi folosit pentru a depana cauza erorii și a efectua acțiuni de revizuire.

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

- **ErrType** - indică tipul erorii întâlnite

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowToCheck** - cum se verifică setările

- **Message** - conținutul notificării

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

- **Title** - titlul notificării

- **Type** - tipul notificării

### <a name="fbasilentupdatenotificationremoved"></a>fbasilentupdate.notificationremoved

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


### <a name="fbasilentupdatequeueinstall"></a>fbasilentupdate.queueinstall

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


### <a name="fbasilentupdaterequiredappsclosed"></a>fbasilentupdate.requiredappsclosed

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

### <a name="fbasilentupdatetimerforapptermination"></a>FBASilentUpdate.TimerForAppTermination

Acest eveniment este folosit pentru a calcula indicatorul de stare de funcționare a actualizării esențiale calculate pentru Microsoft AutoUpdate (MAU). Acest eveniment ne permite să monitorizăm evenimentul de încetare a utilizării aplicației deschise și durata stării de deschidere.
 
Se colectează următoarele câmpuri:

- **App** – procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** – versiunea aplicației

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

- **Payload** – indică dacă un cronometru a fost setat pentru o aplicație deschisă atunci când a fost declanșată instalarea actualizării. 

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

### <a name="fbasilentupdateupdateavailablenotification"></a>fbasilentupdate.updateavailablenotification

Acest eveniment indică faptul că este declanșată o notificare de actualizare disponibilă. Trebuie să ne asigurăm că fluxul de solicitare a actualizărilor se declanșează atunci când este detectată o actualizare. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează în mod corespunzător și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Notificare particularizată** - valoare booleană care indică dacă s-a utilizat o notificare particularizată.

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - text care indică natura evenimentului. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="fbasilentupdateuserclicknotification"></a>fbasilentupdate.userclicknotification

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


### <a name="fbasilentupdateuserselectinstalllater"></a>fbasilentupdate.userselectinstalllater

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


### <a name="fbasilentupdateuserselectinstallnow"></a>fbasilentupdate.userselectinstallnow

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


### <a name="guidashboardrowviewupdatestate"></a>gui.dashboardrowview.updatestate

Acest eveniment raportează despre o eroare găsită în timp ce s-a încercat afișarea informațiilor despre aplicație în interfața de utilizator MAU. Folosim acest eveniment pentru a asigura starea de funcționare a MAU și punctul de eroare și urmărire adresă.

Se colectează următoarele câmpuri:

- **App** – procesul aplicației care trimite evenimentul

- **AppID** - identificatorul aplicației.

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** – versiunea aplicației

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

- **Payload** -conține informații despre natura erorii întâlnite cu înregistrarea aplicațiilor.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="guidashboardviewappisopendialogdisplay"></a>gui.dashboardview.appisopendialog.display 

Acest eveniment indică faptul că interfața de utilizator a afișat o casetă de dialog pentru a închide o aplicație deschisă în vederea continuării cu actualizarea aplicației. Acest eveniment este utilizat pentru a determina volumul de actualizări întârziate cu scopul de a oferi îmbunătățiri viitoare pentru a minimiza întreruperea utilizatorului.

Se colectează următoarele câmpuri: 

- **App** - procesul aplicației care trimite evenimentul

- **AppID** - identificatorul pentru aplicația actualizată

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

- **HowToCheck** - cum se verifică setările

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

- **UpdateID** - identificatorul pentru o actualizare de aplicație

- **UpdateName** - numele actualizării așa cum apare în fișierul manifest descărcat

### <a name="guidashboardviewappisopendialogbuttonclicked"></a>gui.dashboardview.appisopendialogbutton.clicked

Acest eveniment indică dacă s-a ignorat actualizarea aplicației sau se mai încearcă o dată după ce se afișează o casetă de dialog deschisă pentru aplicație. Acest eveniment este utilizat pentru a determina volumul de actualizări ignorate și utilizate pentru îmbunătățiri viitoare cu scopul de a minimiza întreruperea utilizatorului.

Se colectează următoarele câmpuri:   

- **App** - procesul aplicației care trimite evenimentul

- **AppID** - identificatorul pentru aplicația actualizată

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **ButtonType** - Ignorați sau retrageți

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului 

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowToCheck** - cum se verifică setările

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

- **UpdateID** - identificatorul pentru o actualizare de aplicație

- **UpdateName** - numele actualizării așa cum apare în fișierul manifest descărcat

### <a name="guidashboardviewupdateinprogressdialogdisplay"></a>gui.dashboardview.updateinprogressdialog.display

Acest eveniment înregistrează dacă o casetă de dialog a fost afișată pentru utilizatori indicând dacă actualizarea mai este în curs.
 
Se colectează următoarele câmpuri:

- **App** – procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** – versiunea aplicației

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

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

### <a name="guidashboardviewupdatemodebuttonclicked"></a>gui.dashboardview.updatemodebutton.clicked

Acest eveniment indică modul de actualizare schimbat din controlul interfeței utilizator. Acest eveniment este folosit pentru a stabili volumul de dispozitive care trec la un mod la altul și este utilizat pentru a determina de ce clienții renunță la actualizările automate. 

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

- **HowToCheck** - cum se verifică setările

- **Payload** - menționați dacă descărcarea automată este dezactivată

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

### <a name="guifeedbackwindowbuttonclicked"></a>gui.feedbackwindow.buttonclicked

Acest eveniment raportează dacă feedbackul este trimis sau anulat înainte de trimitere. Acest eveniment este utilizat pentru a determina volumul de feedback trimis într-o anumită versiune de lansare. Acest lucru vă ajută să izolați mai devreme eventuale probleme.

Se colectează următoarele câmpuri: 

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **ButtonType** - menționați dacă feedbackul este trimis sau anulat

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare
 
- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowToCheck** - cum se verifică setările

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

### <a name="guipreferenceviewconsentsheetdisplay"></a>gui.preferenceview.consentsheet.display

Acest eveniment indică faptul că o foaie de consimțământ este afișată, dacă este disponibilă. Acest eveniment este folosit pentru a determina volumul de dispozitive înscrise recent în canalul public aplicabil (Insider rapid/Insider lent). De asemenea, folosim acest eveniment pentru a ne asigura că afișarea casetei de dialog de consimțământ funcționează pentru a afișa condițiile de utilizare.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **ChannelName** - canal pentru care se afișează caseta de dialog de consimțământ

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowToCheck** - cum se verifică setările

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

### <a name="guipreferenceviewconsentsheetlicenseerror"></a>gui.preferenceview.consentsheet.licenseerror

Acest eveniment raportează despre eroarea întâlnită în timpul încercării de afișare a casetei de dialog de consimțământ. Acest eveniment este esențial și este folosit pentru a corecta orice problemă cauzată de o modificare a produsului, dacă este cazul.

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

- **ErrorCode** - cod de eroare întâlnit

- **ErrorDomain** - domeniu de eroare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowToCheck** - cum se verifică setările

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

### <a name="guipreferenceviewswitchchannel"></a>gui.preferenceview.switchchannel

Acest eveniment raportează despre tranziția dintre canalele selectate de utilizator. Acest eveniment este folosit pentru a determina de ce clienții renunță la canalele Insider.  

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

- **HowToCheck** - cum se verifică setările

- **PickedFrom** - Canal vechi

- **PickedTo** - Canal nou

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

### <a name="guiupdatemanagerapplaunchduringupdate"></a>gui.updatemanager.applaunchduringupdate

Acest eveniment raportează că a fost lansată o aplicație în timpul actualizării, iar Microsoft AutoUpdate finalizează aplicația lansată. Rețineți că lansarea unei aplicații în timp ce este actualizată poate avea drept consecință deteriorarea aplicațiilor. Vom utiliza acest eveniment pentru a ne asigura că procesul de actualizare nu este afectat de aplicația lansată înainte să fie gata de utilizare.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppID** - identificatorul aplicației care a fost lansat în timpul actualizărilor.

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

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

- **Success** - Valoarea Boolean a șirului care indică dacă aplicația a fost finalizată cu succes.

- **UpdateID** - identificatorul actualizării aplicației.

### <a name="guiupdatemanagerdownloadupdateforapp"></a>gui.updatemanager.downloadupdateforapp

Acest eveniment raportează despre starea finalizării descărcării pentru o actualizare. Folosim acest eveniment pentru a asigura starea de funcționare a procesului de actualizare și punctul de eroare de urmărire/adresă.

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppID** - identificatorul aplicației.

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

- **IsRepair** - Șirul Boolean indică dacă actualizarea specială este o descărcare de reparare.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

- **isRepair** - precizează dacă descărcarea a fost pentru o descărcare de reparare pentru o actualizare eșuată anterior.

- **UpdateID** - identificatorul actualizării.

- **UpdateName** - numele actualizării.


### <a name="guiupdatemanagererror"></a>gui.updatemanager.error

Acest eveniment raportează din nou orice eroare întâlnită în timpul actualizărilor de aplicație. Acest lucru poate indica o eroare în secvența de execuție Microsoft AutoUpdate (MAU).  Folosim acest raport cu scopul de a aplica actualizări la MAU pentru a răspunde pentru scenarii de erori comune.

Se colectează următoarele câmpuri:

- **App** – procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** – versiunea aplicației

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

- **Payload** - conține informații despre eroarea întâmpinată în timpul actualizării aplicației.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

- **Success** - Valoarea Boolean a șirului care indică dacă aplicația a fost finalizată cu succes.

### <a name="guiupdatemanagerinstallcleanupforapp"></a>gui.updatemanager.installcleanupforapp

Acest eveniment indică faptul că fișierele temporare create în timpul instalării aplicației s-au curățat cu succes. Acesta face parte din pâlnia de actualizare utilizată pentru a determina starea de funcționare a actualizării aplicației.
 
Se colectează următoarele câmpuri:

- **App** – procesul aplicației care trimite evenimentul

- **AppID** - identificatorul aplicației.

- **AppInfo_Language** - limba în care rulează aplicația

- **AppState** – numărul întreg indică starea de aplicare după tentativa de actualizare.

- **AppVersionLong** – versiunea aplicației

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

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

- **UpdateID** – identificatorul actualizării.


### <a name="guiupdatemanagerinstallsuccessforapp"></a>gui.updatemanager.installsuccessforapp

Acest eveniment indică actualizarea cu succes a aplicației. Acest eveniment face parte din pâlnia de actualizare pe care o utilizăm pentru a determina starea de funcționare a actualizării.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppID** - identificatorul aplicației.

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

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

- **Success** - șirul Boolean indică dacă s-au instalat cu succes actualizări.

- **UpdateID** - identificatorul actualizării.

### <a name="guiupdatemanagerinstallupdateforapp"></a>gui.updatemanager.installupdateforapp

Acest eveniment indică începutul procesului de instalare curent pentru o actualizare de aplicație. Acest eveniment face parte din pâlnia de actualizare a aplicației pe care o utilizăm pentru a determina starea de funcționare a actualizării.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppID** - identificatorul aplicației.

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

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

- **UpdateID** - identificatorul actualizării.

### <a name="guiupdatemanagerqueueinstallforapp"></a>gui.updatemanager.queueinstallforapp

Acest eveniment indică începutul procesului de instalare curent pentru o actualizare de aplicație. Acest eveniment face parte din pâlnia de actualizare a aplicației pe care o utilizăm pentru a determina starea de funcționare a actualizării.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppID** - identificatorul aplicației.

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

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

- **UpdateID** - identificatorul actualizării.

### <a name="guiupdatemanagerrelaunchapp"></a>gui.updatemanager.relaunchapp

Acest eveniment înregistrează dacă s-au relansat cu succes aplicațiile după actualizări.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppID** - identificatorul aplicației.

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

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

- **Success** - Valoarea Boolean a șirului care indică dacă aplicația a fost finalizată cu succes.

- **UpdateID** - identificatorul actualizării.

- **UpdateName** - numele actualizării.

### <a name="installdatacheckrunning"></a>installdata.checkrunning

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

    
### <a name="installdatacleanup"></a>installdata.cleanup

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


### <a name="installedappacknowledgedcoreappleevent"></a>installedapp.acknowledgedcoreappleevent

Acest eveniment indică faptul că Microsoft AutoUpdate (MAU) a primit un eveniment de confirmare Apple al unei aplicații înregistrate de a închide aplicația pentru a continua cu actualizarea de aplicație în așteptare. Acest eveniment este utilizat pentru a contribui la dezvoltarea viitoarelor îmbunătățiri, pentru a minimiza întreruperea utilizatorului în timpul actualizărilor aplicației. 

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppID** - identificatorul pentru aplicația actualizată

- **AppInfo_Language** - limba în care rulează aplicația

- **AppleEventClass** -indică tipul de eveniment trimis/recunoscut

- **AppleEventID** - identificator unic pentru evenimentul trimis/recunoscut

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

- **HowToCheck** - cum se verifică setările

- **Payload** - conține număru de înregistrări

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

- **UpdateID** - identificatorul actualizării.


### <a name="installedappinvalidbundle"></a>installedapp.invalidbundle

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

    
### <a name="installedappinvalidpreference"></a>installedapp.invalidpreference

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

    
### <a name="installedappnilbundleid"></a>installedapp.nilbundleid

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


### <a name="installedappnilbundlename"></a>installedapp.nilbundlename

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


### <a name="installedapprespondedcoreappleevent"></a>installedapp.respondedcoreappleevent

Acest eveniment indică faptul că Microsoft AutoUpdate (MAU) a primit un cod Apple de răspuns la eveniment de la o aplicație înregistrată pentru a închide aplicația, în vederea continuării actualizării aplicației în așteptare. Acest eveniment este utilizat pentru a contribui la dezvoltarea viitoarelor îmbunătățiri, pentru a minimiza întreruperea utilizatorului în timpul actualizărilor aplicației. 

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppID** - identificatorul pentru aplicația actualizată

- **AppInfo_Language** - limba în care rulează aplicația

- **AppleEventClass** -indică tipul de eveniment trimis/recunoscut

- **AppleEventID** - identificator unic pentru evenimentul trimis/recunoscut

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

- **HowToCheck** - cum se verifică setările

- **Payload** - conține număru de înregistrări

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

- **UpdateID** - identificatorul actualizării.


### <a name="installedappsendcoreappleevent"></a>installedapp.sendcoreappleevent

Acest eveniment indică faptul că Microsoft AutoUpdate (MAU) trimite un eveniment Apple unei aplicații înregistrate pentru a rezilia aplicația pentru a continua cu actualizarea de aplicație în așteptare. Acest eveniment este utilizat în prezent pentru a contribui la dezvoltarea viitoarelor îmbunătățiri, pentru a minimiza întreruperea utilizatorului în timpul actualizărilor aplicației. 

Se colectează următoarele câmpuri:

- **Acknowledged** - indică dacă aplicația vizată a recunoscut primirea evenimentului

- **App** - procesul aplicației care trimite evenimentul

- **AppID** - identificatorul pentru aplicația actualizată

- **AppInfo_Language** - limba în care rulează aplicația

- **AppleEventClass** -indică tipul de eveniment trimis/recunoscut

- **AppleEventID** - identificator unic pentru evenimentul trimis/recunoscut

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

- **HowToCheck** - cum se verifică setările

- **Payload** - conține număru de înregistrări

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

- **Success** - indică dacă aplicația vizată a raportat reușita operațiunii

- **UpdateID** - identificatorul actualizării.
    
### <a name="installstatuscodesign"></a>installstatus.codesign

Acest eveniment înregistrează starea binară a semnăturii codului pentru sistemul de operare. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează conform așteptărilor și pentru a ajuta la depanarea erorilor.
 
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


### <a name="installstatusdaemon"></a>installstatus.daemon

Acest eveniment înregistrează starea aplicației daemon Actualizare automată Microsoft. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează conform așteptărilor și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **BundleReachable** - valoare booleană care indică dacă a existat o problemă la accesarea pachetului de aplicații Microsoft AutoUpdate.

- **Channel** - preferința pentru public

- **Codesigned** - valoare booleană, care indică dacă Asistentul de actualizare a fost proiectat în comun în mod corect.

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **Exists** - valoare booleană care indică dacă asistentul de actualizare există pe disc.

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **Payload** - conține o indicație privind existența componentei Daemon în locația așteptată și dacă codul acesteia este semnat. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="installstatushelper"></a>installstatus.helper

Acest eveniment înregistrează starea instrumentului de asistență Actualizare automată Microsoft. Folosim acest eveniment pentru a ne asigura că procesul de actualizare funcționează conform așteptărilor și pentru a ajuta la depanarea erorilor.
 
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

    
### <a name="installupdatestaskapplaunched"></a>installupdatestask.applaunched

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

    
### <a name="installupdatestaskapplaunchwithpendingupdate"></a>installupdatestask.applaunchwithpendingupdate

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

    
### <a name="installupdatestaskcodesignverificationfail"></a>installupdatestask.codesignverificationfail

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


### <a name="installupdatestaskcodesignverificationstart"></a>installupdatestask.codesignverificationstart

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


### <a name="installupdatestaskcodesignverificationsuccess"></a>installupdatestask.codesignverificationsuccess

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


### <a name="installupdatestaskfailsilentinstall"></a>installupdatestask.failsilentinstall

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

    
### <a name="installupdatestaskmultiplerelocatablepackage"></a>installupdatestask.multiplerelocatablepackage

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

    
### <a name="installupdatestaskremoveclone"></a>installupdatestask.removeclone

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


### <a name="installupdatestaskretryfail"></a>installupdatestask.retryfail

Acest eveniment indică faptul că au fost întâmpinate erori în timpul procesului de reîncercare a instalării. Folosim acest eveniment pentru a ne asigura că procesul de actualizare funcționează conform așteptărilor și pentru a ajuta la depanarea erorilor.
 
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

   
### <a name="installupdatestaskretryproxyerror"></a>installupdatestask.retryproxyerror

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

    

### <a name="installupdatestaskretryresponse"></a>installupdatestask.retryresponse

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


### <a name="installupdatestaskretrysuccess"></a>installupdatestask.retrysuccess

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


### <a name="installupdatestasksetreopengui"></a>installupdatestask.setreopengui

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

- **Payload** - text care indică succesul operațiunii. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

- **Succes** - Boolean care indică succesul operațiunii.

### <a name="installupdatestaskupdatestatus"></a>installupdatestask.updatestatus

Acest eveniment raportează despre starea activității de instalare. Acesta face parte dintr-o pâlnie actualizată și este utilizată pentru a determina starea de funcționare a actualizărilor aplicației.

Se colectează următoarele câmpuri: 

- **App** - procesul aplicației care trimite evenimentul

- **AppID** - identificatorul pentru aplicația actualizată

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Error** - indică orice erori întâmpinate în timpul procesului de actualizare, dacă este completată

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowToCheck** - cum se verifică setările

- **IOC** - indică dacă s-a utilizat caracteristica instalare la clonare

- **Payload** - text static, pentru a indica începutul procesului de instalare, dacă există

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

- **Success** -  indică dacă procesul de instalare s-a finalizat cu succes

- **UpdateID** - identificatorul pentru o actualizare de aplicație

- **UpdateName** - numele actualizării așa cum apare în fișierul manifest descărcat

- **UpdatePkg** - numele pachetului de actualizare aplicată

### <a name="lifecyclecomplimentproclaunch"></a>Lifecycle.complimentproclaunch

Acest eveniment indică încercarea de a lansa Microsoft Update Assistant din Microsoft AutoUpdate sau din Microsoft AutoUpdate din Microsoft Update Assistant. Acest eveniment este utilizat pentru a determina și a asigura starea Microsoft AutoUpdate și Microsoft Update Assistant.

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

- **Eroare** - orice eroare raportată în timpul încercării de lansare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowToCheck** - cum se verifică setările

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **Motivul** - motivul pentru care încercați să lansați procesul de compliment

- **SessionId** - identificatorul pentru sesiune

- **Success** - indică dacă actualizarea aplicației a fost reușită

### <a name="lifecyclelaunch"></a>Lifecycle.launch

Acest eveniment indică pornirea AutoUpdate sau Microsoft Update Assistant. Acest eveniment este utilizat, de asemenea, pentru a raporta orice problemă survenită în timpul procesului de lansare, precum și ca metodă de raportare utilizată pentru lansare în cazul Microsoft Update Assistant.

*[Acest eveniment înlocuiește evenimentele fba.launch și appdelegate.launch.]*

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

- **Error** - orice eroare găsită la lansare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowToCheck** - cum se verifică setările

- **LaunchedBy** - metodă utilizată pentru lansarea Microsoft Update Assistant, dacă este cazul

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

### <a name="lifecycleperiodiccheck"></a>Lifecycle.periodiccheck

Acest eveniment raportează periodic despre starea procesului MicrosoftAutoUpdate. Mai exact, raportează despre activitățile pe care le așteaptă procesul pentru finalizarea Asistentului de actualizare și, în cazul interfeței de utilizator, raportează dacă procesul se încheie din cauza inacțiunii utilizatorului.  Vom utiliza acest eveniment pentru a determina ce împiedică Asistentul de actualizare să finalizeze actualizările și să se închidă și dacă interfața de utilizator se încheie din cauza inacțiunii utilizatorului.

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **dataCollectionDialog** - boolean care indică dacă procesul așteaptă răspunsul utilizatorului la caseta de dialog Colectare date

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **forcedUpdateDialog** - boolean care indică dacă procesul așteaptă răspunsul utilizatorului la caseta de dialog Actualizare forțată

- **HowToCheck** - cum se verifică setările

- **isBusy** - boolean care indică dacă procesul este ocupat cu actualizarea activă

- **isInactive** - boolean care indică dacă procesul așteaptă acțiunea utilizatorului de mai mult timp

- **isWaiting** - boolean care indică dacă procesul așteaptă răspunsul utilizatorului la notificare

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

- **SessionLength** - durata sesiunii procesului curent în secunde


### <a name="lifecycleterminate"></a>Lifecycle.terminate

Acest eveniment indică terminarea Microsoft AutoUpdate sau Microsoft Update Assistant. Acest eveniment este utilizat pentru a determina starea Microsoft AutoUpdate și Microsoft Update Assistant.

*[Acest eveniment înlocuiește evenimentele fba.terminate și appdelegate.terminate.]*

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

- **HowToCheck** - cum se verifică setările

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

- **SessionLength** - durata sesiunii procesului curent în secunde



### <a name="msupdateclieventhandler"></a>msupdate.cli.eventhandler

Acest eveniment este folosit pentru a calcula utilizarea diferitelor tipuri de interfețe cu linie de comandă API din Microsoft AutoUpdate (MAU).

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppID** - identificatorul aplicației care trimite interfața cu linie de comandă API către MAU.

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

- **EventType** - tipul de eveniment trimis de aplicație către interfața liniei de comandă MAU.

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="msupdateclieventhandlerapplyupdatesappids"></a>msupdate.cli.eventhandler.applyupdates.appids

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


### <a name="msupdateclieventhandlerconfig"></a>msupdate.cli.eventhandler.config

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


### <a name="msupdateclieventhandlerupdates"></a>msupdate.cli.eventhandler.updates

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

    
### <a name="msupdatemonitorprogressdownloaded"></a>msupdate.monitor.progress.downloaded

Acest eveniment indică faptul că s-au descărcat actualizări. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează conform așteptărilor și pentru a ajuta la depanarea erorilor.
 
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


### <a name="msupdatemonitorprogressfailure"></a>msupdate.monitor.progress.failure

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

    
### <a name="msupdatemonitorprogressfinished"></a>msupdate.monitor.progress.finished

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


### <a name="msupdatemonitorprogressqueued"></a>msupdate.monitor.progress.queued

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


### <a name="sauforcedupdateautodismiss"></a>sauforcedupdate.autodismiss

Acest eveniment indică faptul că se respinge caseta de dialog de actualizare forțată afișată din cauza inactivității utilizatorului. Acest eveniment este utilizat pentru a determina volumul de actualizări forțate care continuă fără ca utilizatorii să furnizeze o intrare la notificarea afișată. Acest eveniment este folosit pentru a îmbunătăți interfața de utilizator cu scopul de a minimiza întreruperea.

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

- **HowToCheck** - cum se verifică setările

- **Activity Result** - text static *[Acest câmp a fost eliminat din compilările de Office actuale, dar poate apărea în continuare în compilări mai vechi.]*

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **Motiv** - Text static

- **SessionId** - identificatorul pentru sesiune

### <a name="sauforcedupdateclose"></a>sauforcedupdate.close

Acest eveniment indică faptul că utilizatorul a ales să închidă caseta de dialog a actualizării forțate. Acest eveniment este utilizat pentru a determina volumul de actualizări forțate amânat de acțiunea utilizatorului. Acest eveniment este folosit pentru a îmbunătăți interfața de utilizator cu scopul de a minimiza întreruperea. 

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

- **HowToCheck** - cum se verifică setările

- **Payload** - text static

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

### <a name="sauforcedupdatecompleteautodismiss"></a>sauforcedupdate.completeautodismiss

Acest eveniment indică faptul că se respinge caseta de dialog a actualizării forțate afișate din caracteristica termen limită din cauza inactivității utilizatorului. Acest eveniment este utilizat pentru a determina volumul de actualizări forțate care continuă fără ca utilizatorii să furnizeze o intrare la notificarea afișată. Acest eveniment este folosit pentru a îmbunătăți interfața de utilizator cu scopul de a minimiza întreruperea în ceea ce privește caracteristica termen limită.

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

- **HowToCheck** - cum se verifică setările

- **Payload** - text static

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

### <a name="sauforcedupdatecompleteclose"></a>sauforcedupdate.completeclose

Acest eveniment indică finalizarea cu succes a unei actualizări forțate. Acest eveniment este folosit pentru a determina starea de funcționare a caracterisiticii de actualizate forțată. 

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

- **HowToCheck** - cum se verifică setările

- **Payload** - text static

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

### <a name="sauforcedupdatedisplay"></a>sauforcedupdate.display

Acest eveniment indică faptul că o casetă de dialog cu actualizare forțată s-a finalizat cu succes.  Acest eveniment face parte din pâlnia actualizării forțate și este folosit pentru a determina starea de funcționare a caracteristicii de actualizare forțată.

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

- **HowToCheck** - cum se verifică setările

- **Payload** - text static

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

### <a name="sauforcedupdatedisplayfinalhour"></a>sauforcedupdate.displayfinalhour

Acest eveniment indică faptul că o casetă de dialog cu actualizare forțată de ultima oră a fost afișată. Acest eveniment face parte din pâlnie de actualizare forțată și este folosit pentru a determina starea de funcționare a caracteristicii de actualizare forțată.

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

- **HowToCheck** - cum se verifică setările

- **Payload** - text static

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

### <a name="sauforcedupdatedone"></a>sauforcedupdate.done

Acest eveniment indică faptul că o actualizare forțată s-a finalizat cu succes. Acest eveniment face parte din pâlnie de actualizare forțată și este folosit pentru a determina starea de funcționare a caracteristicii de actualizare forțată. 

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

- **HowToCheck** - cum se verifică setările

- **Payload** - text static

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

### <a name="sauforcedupdateenabled"></a>sauforcedupdate.enabled

Acest eveniment este declanșat atunci când Microsoft AutoUpdate (MAU) determină ca actualizarea forțată să fie aplicabilă.  Acest eveniment este folosit pentru a determina starea caracterisiticii de actualizate forțată. 

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

- **Enabled** - indică dacă este activată actualizarea forțat

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowToCheck** - cum se verifică setările

- **InvalidUpdates** - contor de actualizări forțate setat cu versiuni de actualizare nevalide

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

### <a name="sauforcedupdateforcedupdatedismiss"></a>sauforcedupdate.forcedupdatedismiss

Acest eveniment indică faptul că se respinge caseta de dialog referitoare la ultima oră de actualizare forțată afișat din cauza inactivității utilizatorului. Acest eveniment este utilizat pentru a determina volumul de actualizări forțate care continuă fără ca utilizatorii să furnizeze o intrare la notificarea afișată. Acest eveniment este folosit pentru a îmbunătăți interfața de utilizator cu scopul de a minimiza întreruperea. 

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

- **HowToCheck** - cum se verifică setările

- **Activity Result** - text static *[Acest câmp a fost eliminat din compilările de Office actuale, dar poate apărea în continuare în compilări mai vechi.]*

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **Motiv** - Text static

- **SessionId** - identificatorul pentru sesiune

### <a name="sauforcedupdateforcequitandupdatenow"></a>sauforcedupdate.forcequitandupdatenow

Acest eveniment indică începutul actualizării forțate inițiate de utilizator. Acest eveniment face parte din pâlnie și este folosit pentru a determina starea de funcționare a caracteristicii de actualizare forțată. 

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

- **HowToCheck** - cum se verifică setările

- **Payload** - text static

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune 

### <a name="sauforcedupdateforceterminate"></a>sauforcedupdate.forceterminate

Acest eveniment indică începutul actualizării forțate, cu aplicația finalizată forțat.  Acest eveniment face parte din pâlnie și este folosit pentru a determina starea de funcționare a caracteristicii de actualizare forțată.

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

- **HowToCheck** - cum se verifică setările

- **Payload** - conține numărul de aplicații de finalizat

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

### <a name="sauforcedupdatequitandupdatenow"></a>sauforcedupdate.quitandupdatenow

Acest eveniment indică faptul că utilizatorul a ales să închidă aplicația și să aplice actualizarea. Acest eveniment face parte din pâlnie și este folosit pentru a determina starea de funcționare a caracteristicii de actualizare forțată. 

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

- **HowToCheck** - cum se verifică setările

- **Payload** - text static

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

### <a name="sauforcedupdatesnooze"></a>sauforcedupdate.snooze

Acest eveniment indică faptul că utilizatorul a ales să amâne actualizarea forțată. Acest eveniment face parte din pâlnie și este folosit pentru a determina starea de funcționare a caracteristicii de actualizare forțată. 

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

- **Durata** - Text care indică durata amânării

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowToCheck** - cum se verifică setările

- **Activity Result** - text static *[Acest câmp a fost eliminat din compilările de Office actuale, dar poate apărea în continuare în compilări mai vechi.]*

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

### <a name="sauforcedupdateterminate"></a>sauforcedupdate.terminate

Acest eveniment indică începutul actualizării forțate, cu aplicația finalizată. Acest eveniment face parte din pâlnie și este folosit pentru a determina starea de funcționare a caracteristicii de actualizare forțată.

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

- **HowToCheck** - cum se verifică setările

- **Payload** - conține numărul de aplicații de finalizat

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

### <a name="sauforcedupdateupdatenow"></a>sauforcedupdate.updatenow

Acest eveniment indică faptul că utilizatorul a ales să actualizeze aplicația acum.  Acest eveniment face parte din pâlnie și este folosit pentru a determina starea de funcționare a caracteristicii de actualizare forțată.

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

- **HowToCheck** - cum se verifică setările

- **Payload** - text static

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


### <a name="updateapplaunchdetected"></a>update.applaunchdetected

Acest eveniment indică faptul că a fost lansată o aplicație atunci când era în desfășurare o actualizare. Acest eveniment este folosit pentru a determina volumul de aplicații lansate în timpul actualizării și este utilizat pentru îmbunătățirea experienței de utilizator în versiunile viitoare.

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppID** - identificatorul pentru aplicația actualizată

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

- **HowToCheck** - cum se verifică setările

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

- **Success** - indică dacă aplicația lansată s-a terminat cu succes

- **UpdateID** - identificatorul pentru o actualizare de aplicație

### <a name="updateappterminationreceived"></a>update.appterminationreceived

Acest eveniment indică faptul că o aplicație cu actualizare blocată s-a finalizat și dacă Microsoft AutoUpdate (MAU) poate continua actualizarea. Acesta face parte dintr-o pâlnie și este utilizată pentru a determina starea de funcționare a actualizărilor aplicației.

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppID** - identificatorul pentru aplicația actualizată

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Error** - indică dacă există și alte instanțe de aplicație care rulează în continuare, împiedicând MAU să continue

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowToCheck** - cum se verifică setările

- **Payload** - text static pentru a indica ca MAU să continue actualizarea

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

- **UpdateID** - identificatorul pentru o actualizare de aplicație

### <a name="updateblockedappclosed"></a>update.blockedappclosed

Acest eveniment indică faptul că Microsoft AutoUpdate (MAU) a detectat că o aplicație cu actualizare blocată s-a închis și poate continua actualizarea. Acest eveniment face parte din pâlnie și este utilizat pentru a determina starea de funcționare a actualizărilor aplicației. 

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppID** - identificatorul pentru aplicația actualizată

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria.

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare.

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat. 

- **HowToCheck** - cum se verifică setările

- **Payload** - text static

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

- **UpdateID** - identificatorul pentru o actualizare de aplicație

### <a name="updateblockedinstallskip"></a>update.blockedinstallskip

Acest eveniment înregistrează o eroare găsită atunci când se încearcă omiterea unei actualizări de aplicație. Acest eveniment este esențial și este utilizat pentru a investiga erorile raportate.  

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppID** - identificatorul pentru aplicația actualizată

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

- **HowToCheck** - cum se verifică setările

- **Payload** - conține informații despre eroarea întâmpinată

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

### <a name="updateclientsession"></a>update.clientsession

Acest eveniment este raportat atunci când se modifică starea dispozitivului de client, determinând asistentul de actualizare Microsoft să întrerupă sau să reia procesul de actualizare. Acest eveniment face parte din pâlnie și este utilizat pentru a determina starea de funcționare a actualizărilor aplicației. 

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

- **HowToCheck** - cum se verifică setările

- **Payload** - indică dacă Microsoft AutoUpdate (MAU) se reia sau se întrerupe

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

### <a name="updateclonedisablereason"></a>update.clonedisablereason

Acest eveniment înregistrează o condiție indicând că o caracteristică Install-On-Clone este dezactivată pentru o anumită actualizare. Utilizăm acest eveniment pentru a monitoriza starea caracteristicii Install-On-Clone și pentru a furniza un serviciu îmbunătățit.

Se colectează următoarele câmpuri:

- **App** – procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** – versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - Țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** – Versiunea sistemului de operare

- **Event_ReceivedTime** - Ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **Reason** - Motivul pentru care Instalați pe clonare este dezactivată pentru această actualizare.

- **SessionId** - Identificatorul pentru sesiune


### <a name="updatedownloadbegin"></a>update.download.begin 

Acest eveniment indică începutul procesului de actualizare a aplicației. Acesta face parte dintr-o pâlnie actualizată și este utilizată pentru a determina starea de funcționare a actualizărilor aplicației. 

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppID** - identificatorul pentru aplicația actualizată

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

- **HowToCheck** - cum se verifică setările

- **IsRepair** - indică dacă actualizarea este pentru a repara actualizarea eșuată

- **Payload** - indică dacă s-a încercat anterior o descărcare

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

- **UpdateName** - numele actualizării așa cum apare în fișierul manifest descărcat

### <a name="updatedownloadfinish"></a>update.download.finish

Acest eveniment indică finalizarea fazei de descărcare pentru actualizarea aplicației. Acesta face parte dintr-o pâlnie actualizată și este utilizată pentru a determina starea de funcționare a actualizărilor aplicației.  

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppID** - identificatorul pentru aplicația actualizată

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

- **HowToCheck** - cum se verifică setările

- **IsRepair** - indică dacă actualizarea este pentru a repara actualizarea eșuată

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

- **UpdateID** - identificatorul pentru o actualizare de aplicație

- **UpdateName** - numele actualizării așa cum apare în fișierul manifest descărcat

### <a name="updatedownloadresume"></a>update.downloadresume

Acest eveniment raportează că s-a produs o eroare în timpul ce se încerca reluarea activității de descărcare întreruptă. Acest eveniment este esențial și este utilizat pentru a investiga erorile raportate. 

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppID** - identificatorul pentru aplicația actualizată

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Error** - indică tipul erorii întâlnite

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowToCheck** - cum se verifică setările

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

- **UpdateID** - identificatorul pentru o actualizare de aplicație

### <a name="updateerror"></a>update.error

Acest eveniment raportează că s-a produs o eroare în timpul ce se încerca actualizarea aplicației înregistrate.  Acest eveniment este esențial și este utilizat pentru a investiga erorile raportate. 

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

- **Error** - conține informații despre tipul de eroare întâmpinată

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowToCheck** - cum se verifică setările

- **Payload** - conține informații despre tipul de eroare întâmpinată

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

### <a name="updateinstallcleanupforapp"></a>update.installcleanupforapp

Acest eveniment indică faptul că instalarea actualizărilor s-a finalizat și Microsoft AutoUpdate (MAU) este în curs de curățare.  Acesta face parte din pâlnia de actualizare și îl utilizăm pentru a determina starea de funcționare a actualizărilor de aplicații.

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppID** - identificatorul pentru aplicația actualizată

- **AppInfo_Language** - limba în care rulează aplicația

- **AppState** - starea aplicației înregistrate. Poate indica eroarea, reparare în așteptare etc.

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

- **HowToCheck** - cum se verifică setările

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

- **UpdateID** - identificatorul pentru o actualizare de aplicație

### <a name="updateinstallupdateforapp"></a>update.installupdateforapp

Acest eveniment este folosit pentru a raporta despre începutul procesului de instalare a actualizării aplicațiilor. Acesta face parte din pâlnia de actualizare și îl utilizăm pentru a determina starea de funcționare a actualizărilor de aplicații. 

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppID** - identificatorul pentru aplicația actualizată

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Error** - Erori găsite, dacă există

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowToCheck** - cum se verifică setările

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

- **UpdateID** - identificatorul pentru o actualizare de aplicație

- **UpdateName** - numele actualizării așa cum apare în fișierul manifest descărcat

### <a name="updateinstallupdateforappsuccess"></a>update.installupdateforapp.success

Acest eveniment raportează despre starea activității de instalare. Acesta face parte din pâlnia de actualizare și îl utilizăm pentru a determina starea de funcționare a actualizărilor de aplicații. 

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppID** - identificatorul pentru aplicația actualizată

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

- **ForcedUpdate** - Indicarea șirului dacă o actualizare este forțată de administratorul IT

- **HowToCheck** - cum se verifică setările

- **Payload** - indică dacă vizualizarea statusului a fost afișată în timpul procesului de instalare

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

- **Success** - indicarea reușitei returnată de la instalarea activității

- **UpdateID** - identificatorul pentru o actualizare de aplicație

### <a name="updateinstallvariance"></a>Update.InstallVariance

Acest eveniment este folosit pentru a calcula indicatorul stării de funcționare a actualizării esențiale pentru MAU. Acest eveniment ne permite să determinăm indicatorii succesului caracteristicii de instalare prioritare și să verificăm integritatea caracteristicii.
 
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

- **Payload** - conține lista de ID-uri de aplicație și prioritatea lor corespunzătoare de instalare reprezentată în numere.

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

### <a name="updatemultipleappupdates"></a>update.multipleappupdates 

Acest eveniment indică faptul că mai multe actualizări ale aplicației sunt în curs de desfășurare în fundal. Acesta face parte din pâlnia de actualizare și îl utilizăm pentru a determina starea de funcționare a actualizărilor de aplicații.

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

- **HowToCheck** - cum se verifică setările

- **Payload** - conține informații despre numărul de aplicații actualizate

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

### <a name="updatepreviousidnil"></a>update.previousidnil

Acest eveniment indică faptul că s-a descărcat un pachet de actualizare a reparațiilor, dar nu există nicio informație de descărcare anterioară. Acest eveniment este esențial și este utilizat pentru a investiga erorile raportate. 

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppID** - identificatorul pentru aplicația actualizată

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Error** - indică tipul erorii întâlnite

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowToCheck** - cum se verifică setările

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

### <a name="updatequeueinstallforapp"></a>update.queueinstallforapp 

Acest eveniment indică faptul că un pachet de actualizare descărcat a fost plasat într-o coadă pentru instalare.  Acesta face parte din pâlnia de actualizare și îl utilizăm pentru a determina starea de funcționare a actualizărilor de aplicații.

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppID** - identificatorul pentru aplicația actualizată

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

- **HowToCheck** - cum se verifică setările

- **Payload** - text static, pentru a indica faptul că aplicația trebuie să se închidă, dacă există

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

- **UpdateID** - identificatorul pentru o actualizare de aplicație

- **UpdateName** - numele actualizării așa cum apare în fișierul manifest descărcat

### <a name="updaterelaunchafterupdate"></a>update.relaunchafterupdate 

Acest eveniment indică faptul că actualizarea aplicației s-a finalizat și este relansată. Acesta face parte din pâlnia de actualizare și îl utilizăm pentru a determina starea de funcționare a actualizărilor de aplicații. 

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppID** - identificatorul pentru aplicația actualizată

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Error** - conține informații despre orice erori întâlnite în timp ce încercați să relansați aplicația

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowToCheck** - cum se verifică setările

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

- **UpdateID** - identificatorul pentru o actualizare de aplicație

### <a name="updatetimerforapptermination"></a>update.timerforapptermination 

Acest eveniment indică începutul/sfârșitul cronometrării pentru verificarea aplicației de stare. Acest eveniment vine la pachet și este utilizat pentru a determina dacă toate obiectele de cronometrare sunt eliminate atunci când actualizarea aplicației progresează.

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

- **HowToCheck** - cum se verifică setările

- **Payload** - indică dacă cronometru a fost adăugat sau șters

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune


### <a name="updatecoreappregistration"></a>updatecore.appregistration

Acest eveniment înregistrează încercări de a înregistra o aplicație și rezultatul / motivul. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează conform așteptărilor și pentru a ajuta la depanarea erorilor.
 
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


### <a name="updatecoreloadinglaunchagent"></a>updatecore.loadinglaunchagent

Acest eveniment indică faptul că Agentul de lansare este încărcat. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează conform așteptărilor și pentru a ajuta la depanarea erorilor.
 
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

### <a name="updatecorerunnstaskcommand"></a>updatecore.runnstaskcommand

Acest eveniment raportează despre o eroare în timpul încercării de a lansa o activitate. Acest eveniment este esențial și este utilizat pentru a investiga erorile raportate.  

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

- **HowToCheck** - cum se verifică setările

- **Payload** - conține calea către comanda executată

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

### <a name="updatecoreserverconnectionfail"></a>updatecore.server.connectionfail

Acest eveniment înregistrează erorile întâmpinate în timp ce contactați CDN. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează conform așteptărilor și pentru a ajuta la depanarea erorilor.
 
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

### <a name="updatecoreservernullurl"></a>updatecore.server.nullurl

Acest eveniment raportează o eroare care indică faptul că nu s-a putut ajunge la un anumit server. Acest eveniment este utilizat pentru a determina rată de eșec a actualizării cauzată de problema rețelei. 

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

- **HowToCheck** - cum se verifică setările

- **Payload** - text static

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

### <a name="updatefilterhelpercannotretrievebuilddate"></a>updatefilterhelper.cannotretrievebuilddate

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


### <a name="updatefilterhelperinvalidappid"></a>updatefilterhelper.invalidappid

Acest eveniment raportează o eroare care indică faptul că nu s-au găsit fișiere manifest care să se potrivească ID-ului de aplicație preluat de la răspunsul web. Acest eveniment este utilizat pentru a investiga erorile raportate.

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

- **HowToCheck** - cum se verifică setările

- **Payload** - conține ID-ul aplicației în răspunsul web

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

### <a name="updatefilterhelperinvalidappidfromwebservices"></a>updatefilterhelper.invalidappidfromwebservices

Acest eveniment raportează o eroare care indică faptul că ID-ul de aplicație preluat de la răspunsul web nu este în formatul așteptat. Acest eveniment este utilizat pentru a investiga erorile raportate.

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

- **HowToCheck** - cum se verifică setările

- **Payload** - text static

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

### <a name="updatefilterhelperinvalidresponsefromupdatefiltering"></a>updatefilterhelper.invalidresponsefromupdatefiltering

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


### <a name="updatefilterhelpermissingbuilddate"></a>updatefilterhelper.missingbuilddate

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


### <a name="updatefilterhelperupdatebypassedoldage"></a>updatefilterhelper.updatebypassedoldage

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


### <a name="updatefindercheckerror"></a>updatefinder.check.error

Acest eveniment raportează o eroare care s-a produs în timpul verificării actualizărilor. Acest eveniment este esențial și este utilizat pentru a investiga erorile raportate. 

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Code** - Codul de eroare 

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Domain** - domeniu de eroare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowToCheck** - cum se verifică setările

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

 
### <a name="updatefindercheckstart"></a>updatefinder.check.start

Acest eveniment se înregistrează ori de câte ori inițiam o verificare a operațiunii de actualizare. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează conform așteptărilor și pentru a ajuta la depanarea erorilor.
 
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


### <a name="updatefindercheckstatus"></a>updatefinder.check.status

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


### <a name="updatefindercheckupdatefound"></a>updatefinder.check.updatefound

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


### <a name="updatefindercheckupdatenotfound"></a>updatefinder.check.updatenotfound

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


### <a name="updatefindercheckuptodate"></a>updatefinder.check.uptodate

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


### <a name="updatefinderofferupdatesinvalidappid"></a>updatefinder.offerupdates.invalidappid

Acest eveniment raportează o eroare în timp ce se încearcă să se evalueze dacă se aplică o actualizare. Acest eveniment este esențial și este utilizat pentru a investiga erorile raportate.  

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **CatalogID** - identificator pentru catalogul accesat

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowToCheck** - cum se verifică setările

- **IsNullID** - indică dacă ID-ul este nul

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

### <a name="updatefinderofferupdatesminoscheckfail"></a>updatefinder.offerupdates.minoscheckfail

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

### <a name="updatefinderofferupdatesmissingtrigger"></a>updatefinder.offerupdates.missingtrigger

Acest eveniment raportează o eroare în timp ce se încearcă să se evalueze declanșatoarele din manifestul de actualizare a aplicației descărcate. Acesta este esențial și este utilizat pentru a investiga erorile raportate.  

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

- **HowToCheck** - cum se verifică setările

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

- **TriggerKey** - cheia declanșatoare găsită în manifest

- **Triggers** - dicționarul declanșatoarelor găsit în manifest

### <a name="updatefinderofferupdatesnullbundleforappid"></a>updatefinder.offerupdates.nullbundleforappid

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


### <a name="updatefinderofferupdatesupdaterulematched"></a>updatefinder.offerupdates.updaterulematched

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

    
### <a name="updatefinderregisteredapps"></a>updatefinder.registeredapps

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

### <a name="updatefindersuiteinvalidsuiteversion"></a>updatefinder.suite.invalidsuiteversion

Acest eveniment raportează o eroare a versiunii suitei în timp ce se încearcă să se evalueze dacă se aplică o actualizare. Acest eveniment este esențial și este utilizat pentru a investiga erorile raportate.

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

- **HowToCheck** - cum se verifică setările

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

- **Suite** - numele suitei avută în vedere

### <a name="updatefindersuitekeyvaluemissing"></a>updatefinder.suite.keyvaluemissing

Acest eveniment raportează o eroare în timpul încercării de a adăuga o aplicație la Suite. Acest eveniment este esențial și este utilizat pentru a investiga erorile raportate.

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppID** - identificatorul pentru aplicația actualizată

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

- **HowToCheck** - cum se verifică setările

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune 

- **Suite** - numele aplicației suitei va fi adăugată

    
### <a name="updatefindersuitemissingcollateral"></a>updatefinder.suite.missingcollateral

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


### <a name="updatefindersuitestaleversion"></a>updatefinder.suite.staleversion

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


### <a name="updatefindersuiteupdateapplicable"></a>updatefinder.suite.updateapplicable

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


### <a name="updatefindersuiteupdatenotapplicabledefaultpath"></a>updatefinder.suite.updatenotapplicabledefaultpath

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

    
### <a name="updatefindersuiteupdatenotapplicableversion"></a>updatefinder.suite.updatenotapplicableversion

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


### <a name="updatefindersuiteupdatenotoffered"></a>updatefinder.suite.updatenotoffered

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


### <a name="updatefindersuiteupdateoffered"></a>updatefinder.suite.updateoffered

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


### <a name="updatemanagercheckupdate"></a>updatemanager.checkupdate

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


### <a name="updatemanagernetwork"></a>updatemanager.network

Acest eveniment înregistrează disponibilitatea rețelei. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează conform așteptărilor și pentru a ajuta la depanarea erorilor.
 
Se colectează următoarele câmpuri:

- **App** – procesul aplicației care trimite evenimentul

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** – versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - Țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - Modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Event_ReceivedTime** - Ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

- **ServerReacheable** - Boolean care indică dacă rețeaua este disponibilă.

    
### <a name="updatemanagerupdatespending"></a>updatemanager.updatespending

Acest eveniment indică faptul că s-au găsit actualizări și instalarea este în așteptare. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează conform așteptărilor și pentru a ajuta la depanarea erorilor.
 
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

### <a name="updatestatuscodesign"></a>UpdateStatus.Codesign

Acest eveniment raportează starea din verificarea proiectării în comun a asistentului de actualizare Microsoft care rulează după instalarea actualizărilor aplicației de client. Vom utiliza acest eveniment pentru a ne asigura că furnizăm pachetele valide și vom actualiza aplicația instalată la cea mai recentă versiune.

Se colectează următoarele câmpuri:

- **App** - procesul aplicației care trimite evenimentul

- **AppID** - identificatorul pentru aplicația actualizată

- **AppInfo_Language** - limba în care rulează aplicația

- **AppVersionLong** - versiunea aplicației

- **Channel** - preferința pentru public

- **Device_NetworkCountry** - țara dispozitivului (pe baza adresei IP)

- **DeviceID** - identificatorul dispozitivului

- **DeviceInfo_Model** - modelul hardware al dispozitivului

- **DeviceInfo_NetworkType** - tipul de rețea (Wi-Fi, cu fir, necunoscut)

- **DeviceInfo_OsBuild** - versiunea sistemului de operare

- **Error** - orice eroare observată în timpul procesului de verificare a proiectării în comun

- **Event_ReceivedTime** - ora la care s-a primit telemetria

- **EventInfo_Name** - numele evenimentului de telemetrie în curs de înregistrare

- **EventInfo_Time** - ora la care a avut loc evenimentul înregistrat 

- **HowTocheck** - preferința pentru verificarea actualizărilor

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

- **Success** - indică dacă verificarea proiectării în comun a fost realizată cu succes

- **UpdateID** - identifică în mod unic actualizarea aplicată 

- **UpdateName** - numele actualizării așa cum este descris în manifestul actualizat

- **UpdatePkg** - numele pachetului de actualizare aplicat

### <a name="urlutilitiesgetmauinfo"></a>urlutilities.getmauinfo

Acest eveniment raportează că s-a produs o eroare atunci când se accesează pachetul de aplicații Microsoft AutoUpdate (MAU). Acest eveniment este esențial și este utilizat pentru a investiga erorile raportate.

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

- **HowToCheck** - cum se verifică setările

- **Payload** - conține informații despre eroarea întâmpinată

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune
   
### <a name="webservicescheckforsilentupdates"></a>webservices.checkforsilentupdates

Acest eveniment indică faptul că au fost găsiți candidați pentru actualizarea silențioasă. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează conform așteptărilor și pentru a ajuta la depanarea erorilor.
 
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


### <a name="webservicesdeltaupdater"></a>webservices.deltaupdater

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


### <a name="webservicesserviceaction"></a>webservices.serviceaction

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


### <a name="webservicesserviceresponse"></a>webservices.serviceresponse

Acest eveniment înregistrează solicitările către serviciul MAU, timpii de răspuns și erorile. Utilizăm acest eveniment pentru a ne asigura că procesul de actualizare funcționează conform așteptărilor și pentru a ajuta la depanarea erorilor.
 
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

    
### <a name="webservicessilentupdate"></a>webservices.silentupdate

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

### <a name="webservicesupdatefiltering"></a>webservices.updatefiltering

Acest eveniment indică filtrarea efectuată în lista de actualizări aplicabile prin intermediul serviciilor web. Vom folosit acest eveniment pentru a ne asigura că blocurile de aplicație funcționează corect dacă trebuie să blocăm o actualizare.

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

- **HowToCheck** - cum se verifică setările

- **Payload** - conține informații despre numărul de actualizări blocate prin servicii web

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

### <a name="webserviceswebcontent"></a>webservices.webcontent

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

### <a name="webserviceswhatsnew"></a>webservices.whatsnew

Acest eveniment este declanșat atunci când Microsoft AutoUpdate (MAU) interoghează servicii web pe caracteristica „Noutăți” pentru aplicațiile înregistrate. Acest eveniment este utilizat pentru a determina starea caracteristicii „Noutăți”. 

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

- **HowToCheck** - cum se verifică setările

- **Payload** - conține informații despre numărul de aplicații cu noutăți

- **PipelineInfo_ClientCountry** - țara dispozitivului (pe baza adresei IP)

- **PipelineInfo_ClientIp** - primii 3 octeți ai adresei IP

- **SessionId** - identificatorul pentru sesiune

## <a name="onenote-sync-events"></a>Evenimente de sincronizare OneNote

### <a name="officeonenotestoragenotebooksyncresult"></a>Office.OneNote.Storage.NotebookSyncResult
 
Acest eveniment înregistrează rezultatul sincronizării blocnotesului. Este utilizat pentru a afla numărul țintelor de sincronizare unice la calcularea scorului de sincronizare OneNote.
 
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

### <a name="onenotestorageconnectivitychanged"></a>OneNote.Storage.ConnectivityChanged

Evenimentul înregistrează dacă un utilizator are conectivitate la internet sau nu. Acestea sunt utilizate pentru a corela celelalte măsurători de performanță pentru starea de bună funcționare, permițându-ne să ignorăm evenimentele care au loc în timp ce un utilizator nu are conectivitate la internet, deoarece nu ne așteptăm ca latența noastră de serviciu să fie acceptabilă dacă nu există conectivitate la internet. Aceasta ne permite să calculăm numărul exact al sesiunilor pentru măsurătorile noastre ale sectoarelor clienților (per entitate găzduită, per sector). Se utilizează de asemenea pentru a filtra rapoartele de erori, deoarece există numeroase erori de sincronizare care pot apărea fără conectivitate de rețea, dar care ar justifica o anchetă în caz contrar.

Dacă nu primim aceste date, nu vom putea monitoriza cu exactitate performanța produselor noastre sau nu vom determina dacă erorile experimentate de un utilizator sunt previzibile sau vor fi necesare investigații suplimentare.

Următoarele câmpuri sunt colectate:

- **InternetConnectivityNowAvailable** - dacă starea de conectivitate s-a modificat, fiind acum internet

### <a name="onenotestoragelegacyinboundlatency"></a>OneNote. Storage.LegacyInboundLatency

Semnalul critic utilizat pentru a urmări performanța operațiunilor de sincronizare de intrare care comunică direct cu SharePoint, inclusiv corelarea informațiilor, permițându-ne să monitorizăm și să investigăm performanța încărcării datelor în serviciul nostru. Acest semnal este colectat doar pentru cea mai slabă performanță de descărcare din ultimele 300 de secunde (numărul de secunde este configurabil de Microsoft, în funcție de performanța și condițiile serviciilor).

Acest lucru este utilizat pentru a asigura starea de bună funcționare a serviciilor, permițându-ne să vedem ce entități găzduite întâmpină intrări de date inacceptabil de lent în serviciul nostru, informații despre datele pe care le încarcă atunci când au întâmpinat o intrare lentă și cât de răspândită este problema de latență. Este utilizat de asemenea pentru a raporta starea serviciilor și performanța clienților noștri, pentru a măsura tendințele în timp și a avertiza problemele în mod automat în scopul diminuării efortului tehnic. Dacă nu avem aceste date, ne vom putea garanta performanța adecvată de descărcare atunci când un utilizator sincronizează modificările din SharePoint pe computer.

Următoarele câmpuri sunt colectate: 

- **IsEducationNotebook** - o valoare logică care precizează dacă blocnotesul este de tip școlar

- **NotebookId** - ID-ul blocnotesului de care aparține încărcarea

- **TimeToConfirmSyncedWithServerInMs** - durata în milisecunde care a trecut pentru a efectua încărcarea

### <a name="onenotestoragelegacyoutboundlatency"></a>OneNote.Storage.LegacyOutboundLatency

Semnalul critic utilizat pentru a urmări performanța operațiunilor de sincronizare de ieșire care comunică direct cu SharePoint, inclusiv corelarea informațiilor, permițându-ne să monitorizăm și să investigăm performanța încărcării datelor în serviciul nostru. Acest semnal este colectat doar pentru cea mai slabă performanță de descărcare din ultimele 300 de secunde (numărul de secunde este configurabil de Microsoft, în funcție de performanța și condițiile serviciilor).

Acest lucru este utilizat pentru a asigura starea de bună funcționare a serviciilor, permițându-ne să vedem ce entități găzduite întâmpină ieșiri de date inacceptabil de lente în serviciul nostru, informații despre datele pe care le încarcă atunci când au întâmpinat o ieșire lentă și cât de răspândită este problema de latență. Este utilizat de asemenea pentru a raporta starea serviciilor și performanța clienților noștri, pentru a măsura tendințele în timp și a avertiza problemele în mod automat în scopul diminuării efortului tehnic. Dacă nu avem aceste date, ne vom putea garanta performanța adecvată de descărcare atunci când utilizatorii sincronizează modificările din SharePoint. 

Următoarele câmpuri sunt colectate: 

- **IsEducationNotebook** - o valoare logică care precizează dacă blocnotesul este de tip școlar

- **NotebookId** - ID-ul blocnotesului de care aparține încărcarea

- **TimeToConfirmSyncedWithServerInMs** - durata în milisecunde care a trecut pentru a efectua încărcarea

### <a name="onenotestoragerealtimefiledataobjectdownload"></a>OneNote.Storage.RealTime.FileDataObjectDownload 

Semnalul critic utilizat pentru urmărirea performanței atunci când un utilizator intră într-un obiect de date de fișier (de exemplu un fișier sau o imagine încorporată), care este descărcat direct din serviciul nostru și nu ca parte a unei operațiuni de sincronizare de pe o pagină, secțiune sau blocnotes. Acest semnal este colectat doar pentru cea mai slabă performanță de descărcare din ultimele 300 de secunde (numărul de secunde este configurabil de Microsoft, în funcție de performanța și condițiile serviciilor).

Acest lucru este utilizat pentru a asigura starea de bună funcționare a serviciilor, permițându-ne să vedem ce entități găzduite întâmpină descărcări inacceptabil din lente în serviciul nostru, cât de răspândită este problema de latență și pentru a raporta comportamentul nostru în timp, permițându-ne să măsurăm tendințele performanței serviciului. Dacă vedem o latență inacceptabilă pentru un obiect fișier, vom utiliza de asemenea aceste date pentru a le corela cu alte semnale din partea clientului și serviciului referitoare la obiect, pentru îmbunătățirea procesului nostru de descărcare. De asemenea, am divizat datele în funcție de extensia obiectului fișier descărcat, deoarece avem așteptări diferite în funcție de eventualitatea ca fișierul să fie prezentat inline pe pânza noastră (de exemplu o imagine) sau să fie un fișier non-inline (cum ar fi un document text). Dacă nu primim aceste date nu vom avea posibilitatea să monitorizăm performanța acestor descărcări

Următoarele câmpuri sunt colectate: 

- **FileSizeInBytes** - dimensiunea în byți a fișierului descărcat 

- **IsImage** - o valoare logică ce determină în curs de descărcare are o extensie care se potrivește cu o listă predefinită de formate comune de imagine (.bmp, .emf, .gif, .jpe, .jpeg, .jpg, .png) pe care o afișăm inline pe pânză

- **TimeToDownload** - durata de timp care a trecut pentru a descărca cu succes obiectul FDO din stocarea noastră blob pe dispozitiv 

### <a name="onenotestoragerealtimewebsocketdownload"></a>OneNote.Storage.RealTime.WebSocketDownload

Semnalul critic utilizat pentru a urmări performanța operațiunilor de sincronizare de intrare, inclusiv corelarea informațiilor, permițându-ne să monitorizăm și să investigăm performanța descărcării datelor din serviciul nostru (onenote.com). Acest semnal este colectat doar pentru cea mai slabă performanță de descărcare din ultimele 300 de secunde (numărul de secunde este configurabil de Microsoft, în funcție de performanța și condițiile serviciilor).

Acest lucru este utilizat pentru a asigura starea de bună funcționare a serviciilor, permițându-ne să vedem ce entități găzduite întâmpină intrări de date inacceptabil de lente din serviciul nostru, informații despre datele pe care le descărcau atunci când au întâmpinat o intrare lentă și cât de răspândită este problema de latență. Este utilizat de asemenea pentru a raporta starea serviciilor și performanța clienților noștri, pentru a măsura tendințele în timp și a avertiza problemele în mod automat în scopul diminuării efortului tehnic. 

Dacă vedem o latență inacceptabilă pentru o secțiune sau un blocnotes, vom utiliza de asemenea aceste date pentru a le corela cu alte semnale din partea clientului și serviciului referitoare la același document pentru a identifica regresia performanței clienților, permițându-ne să furnizăm un serviciu mai performant.

Dacă nu primim aceste date, nu vom putea monitoriza performanța acestui aspect al serviciului nostru sau impactul modificărilor secundare pe server ce le-am putea găsi necesare datorită utilizării sau a altor factori.

Următoarele câmpuri sunt colectate:

- **DeviceSessionId** - ID-ul sesiunii de dispozitiv

- **IsEducationNotebook** - o valoare logică care precizează dacă blocnotesul este de tip școlar

- **IsHierarchyResource** - o valoare logică care precizează dacă resursa este o resursă de ierarhie

- **NotebookId** - ID-ul blocnotesului de care aparține încărcarea

- **ResourceId** - ID-ul resursei pe care o încărcăm

- **SectionId** - ID-ul secțiunii de care aparține încărcarea

- **ServerSessionId** - ID-ul sesiunii de server de care aparține încărcarea

- **TimeToConfirmSyncedWithServerInMs** - durata în milisecunde între un utilizator navigând la o pagină și stiva de replicare confirmând că acea pagină este sincronizată cu serverul.

- **TimeToFirstUpdateInMs** - durata în milisecunde între motorul de sincronizare care începe replicarea intrării unei pagini și acea operațiune de replicare care ajunge la sincronizarea cu starea serverului.

### <a name="onenotestoragerealtimewebsocketupload"></a>OneNote.Storage.RealTime.WebSocketUpload

Semnalul critic utilizat pentru a urmări performanța operațiunilor de sincronizare de ieșire, inclusiv corelarea informațiilor, permițându-ne să monitorizăm și să investigăm performanța încărcării datelor la serviciul nostru (onenote.com)

Acest lucru este utilizat pentru a asigura starea de bună funcționare a serviciilor, permițându-ne să vedem ce entități găzduite întâmpină ieșiri de date inacceptabil de lente în serviciul nostru, informații despre datele pe care le încarcă atunci când au întâmpinat o ieșire lentă și cât de răspândită este problema de latență. Este utilizat de asemenea pentru a raporta starea serviciilor și performanța clienților noștri, pentru a măsura tendințele în timp și a avertiza problemele în mod automat în scopul diminuării efortului tehnic. Vom utiliza de asemenea aceste date pentru a urmări impactul și eficiența îmbunătățirilor pe care le facem clienților și serviciilor noastre. 

Dacă vedem o latență inacceptabilă pentru o secțiune sau un blocnotes, vom utiliza de asemenea aceste date pentru a le corela cu alte semnale din partea clientului și serviciului referitoare la același document pentru a identifica regresia performanței, permițându-ne să furnizăm o experiență mai performantă.

Dacă nu primim aceste date, nu vom putea monitoriza performanța acestui aspect al serviciului nostru sau impactul modificărilor secundare pe server ce le-am putea găsi necesare datorită utilizării sau a altor factori.

Următoarele câmpuri sunt colectate: 

- **DeviceSessionId** - ID-ul sesiunii de dispozitiv

- **IsEducationNotebook** - o valoare logică care precizează dacă blocnotesul este de tip școlar

- **IsHierarchyResource** - o valoare logică care precizează dacă resursa este o resursă de ierarhie

- **IsWorstTime** - o valoare logică indicând dacă timpul este un eveniment de încărcare obișnuit sau cel mai slab timp pe care l-am văzut la acest client în ultimele 300 de secunde (numărul de secunde este configurabil de Microsoft în funcție de performanța și starea serviciilor).

- **NotebookId** - ID-ul blocnotesului de care aparține încărcarea

- **RecommendedPutIntervalInMs** - ora la care serviciul a comunicat către client intervalul de plasare recomandat

- **ResourceId** - ID-ul resursei pe care o încărcăm

- **SectionId** - ID-ul secțiunii de care aparține încărcarea

- **SenderRequestId** - ID-ul expeditorului care face încărcare

- **ServerSessionId** - ID-ul sesiunii de server de care aparține încărcarea

- **UploadNonSuspendedTimeInMs** - durata în milisecunde care a trecut pentru a efectua încărcarea excluzând timpul în când a fost suspendată aplicația

- **UploadTimeInMs** - durata în milisecunde care a trecut pentru a efectua încărcarea

- **WaitTimeInMs** - timpul în milisecunde între solicitarea încărcării și pornirea acesteia

- **WebUrl** - WebUrl-ul încărcării (conectat ca PiiWz)

### <a name="onenotestoragesynchealth"></a>OneNote.Storage.SyncHealth

Semnalul critic utilizat pentru a urmări erorile și excepțiile care au avut loc în stiva de sincronizare din clientul OneNote, permițându-ne să monitorizăm și să atenuăm aceste condiții neașteptate.

Acest lucru este utilizat pentru a asigura starea de bună funcționare a serviciilor, permițându-ne să vedem aproape în timp real rapoartele de erori de la clienți, ceea ce ne face să răspundem la problemele de sincronizare pe măsură ce apar. Este utilizat de asemenea pentru a identifica cât de răspândită și cât de severă este o problemă prin corelarea etichetei de erori cu codul client pentru a identifica sursa eșecului. De asemenea, realizăm agregarea acestor date pentru a obține informații despre performanța noastră în timp și despre impactul și eficiența îmbunătățirilor pe care le facem pentru clienții și serviciile noastre. Dacă nu avem aceste date, nu vom putea răspunde proactiv condițiilor de eroare din serviciul nostru de sincronizare fără escaladarea clienților.

Următoarele câmpuri sunt colectate: 

- **Service** - serviciul de sincronizare utilizat de client atunci când s-a produs eroarea (sincronizare moștenită sau modernă)

- **Tag** - eticheta (o valoare de identificare) reprezentând eroarea pe care a întâmpinat-o clientul în timpul operațiunii de sincronizare

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

Nu sunt colectate date necesare de serviciu de Configurația Serviciilor.

## <a name="telemetry-events"></a>Evenimente de telemetrie

### <a name="appdeeplink"></a>app.deep.link

Acest eveniment ne ajută să urmărim utilizarea lansării întâlnirii din calendar, pe diferite puncte finale. Acest eveniment ne permite să detectăm două lucruri: când este lansată o întâlnire prin Skype for Business și când este lansată prin Teams, precum și dacă este instalată aplicația Teams.

Se colectează următoarele câmpuri: 

- **cont** - Informația arhivată a contului care a efectuat acțiunea

- **action_type** - acțiune efectuată, cum ar fi lansarea întâlnirii sau de instalarea aplicației

- **aplicație** - Aplicația care a fost lansată printr-un link profund, cum ar fi Teams sau Skype for Business

- **context** - Experiența la care s-a navigat în cadrul aplicației, de exemplu, office_union - word, office_union - excel etc.

- **sursă** - Originea unei acțiuni, de exemplu, inițiată de utilizator, efectuată automat de client etc.


### <a name="officeandroiddocsuipaywallcontrolpaywalloperationmetrics"></a>Office.Android.DocsUI.PaywallControl.PaywallOperationMetrics

*[Acest eveniment se numea anterior Office.Android.DocsUI.Views.PaywallOperationMetrics.]*

Microsoft îl utilizează pentru a obține starea de bună funcționare, succesul sau ratele de eroare pentru utilizator cu privire la achiziții, pentru a asigura investițiile corespunzătoare pentru a îmbunătăți experiența de achiziționare a clientului pe platformele mobile.

Se colectează următoarele câmpuri:

- **OperationTimeInMs** - timpul necesar pentru finalizarea operațiunii de achiziționare (lung – milisecunde)

- **PaywallOperationResult** - succes / cod de eroare / utilizator anulat (enumerare / număr întreg – finit)

- **PaywallOperationType** - tipul operațiunii Paywall (enumerare / număr întreg – finit)

### <a name="officeandroiddocsuipaywallcontrolpaywallsessiondata"></a>Office.Android.DocsUI.PaywallControl.PaywallSessionData

*[Acest eveniment se numea anterior Office.Android.DocsUI.Views.PaywallSessionData.]*

Metadate bazate pe sesiune atunci când interfața de utilizator Paywall este afișată utilizatorului. Microsoft le utilizează pentru a obține traseul utilizatorului și a înțelege versiunile de dispozitiv și de sistem de operare folosite de utilizator cu scopul de a susține deciziile privind investițiile în îmbunătățirea experienței în aceste domenii.

Se colectează următoarele câmpuri:

- **Versiunea aplicației** - cod de versiune al aplicației consumatoare

- **ClientId** - identificator anonim unic non-PII de dispozitiv (GUID/șir)

- **Punct de intrare** - identificator unic pentru punctele de intrare contextuale sau constante din aplicația consumatoare

- **isTablet** - dacă dispozitivul afișează UX tabletă

- **OSVersion** - versiunea sistemului de operare Android al dispozitivului

- **SessionId** - GUID: identificator unic de sesiune Paywall


### <a name="officefirstrunappletelemetryoptin"></a>Office.FirstRun.Apple.TelemetryOptIn

Acest eveniment este colectat pentru aplicațiile Office care rulează pe platforme Apple. Evenimentul este utilizat pentru a monitoriza starea de funcționare a fluxului nostru de optare pentru telemetrie în prima experiență de rulare. Culegem un cod care denotă ce tip de opțiune de colectare a datelor de diagnostic a fost selectată de către utilizator.

Se colectează următoarele câmpuri:

- **Data_EventId** - un cod care indică preferința de colectare a datelor de diagnostic selectată de utilizator.

### <a name="officeonenotegetsharepointidsfordocument"></a>Office.OneNote.GetSharePointIdsForDocument

Datele colectate înregistrează eșecul și succesul de preluare a ID-urilor SharePoint (SPO) pentru un URL de document. Succesul și eșecul (inclusiv motivul erorii) apelului sunt înregistrate pentru toate platformele. Acest marcator este necesar pentru a urmări și a diagnostica starea apelului pentru a obține IDuri. ID-urile sunt necesare pentru a avea date a paginii OneNote (aparținând blocnotesurilor stocate SharePoint) afișate în flux. 

Se colectează următoarele câmpuri:

- **ErrorCode** -integrarea valorii erorii

- **ErrorMessage** - șir care descrie eroarea

- **FailureType** -string pentru a determina tipul de eroare

- **HttpStatusCode** - cod de eroare HTTP pentru apel de rețea

- **InnerErrorCode** - integrare cod

- **InnerErrorMesage** - mesajul pentru eroare

- **IsSuccess** - valoare booleană pentru semnalizarea reușită

### <a name="officeonenotegetsharepointidsfordocumentw32old"></a>Office.OneNote.GetSharePointIdsForDocumentW32Old

Telemetria înregistrează eșecul și succesul de preluare a ID-urilor SharePoint (SPO) pentru un URL de document. Succesul și eșecul (inclusiv motivul erorii) apelului sunt înregistrate. Acest lucru este conectat doar în platforma veche Win32. Acest marcator este necesar pentru a urmări și a diagnostica starea apelului pentru a obține IDuri. ID-urile sunt necesare pentru a avea date a paginii OneNote (aparținând blocnotesurilor stocate SharePoint) afișate în flux. 

Se colectează următoarele câmpuri:

- **ErrorCode** -integrarea valorii erorii

- **ErrorMessage** - șir care descrie eroarea

- **FailureType** -string pentru a determina tipul de eroare

- **HttpStatusCode** - cod de eroare HTTP pentru apel de rețea

- **InnerErrorCode** - integrare cod

- **InnerErrorMesage** - mesajul pentru eroare

- **IsSuccess** - valoare booleană pentru semnalizarea reușită


### <a name="officesystemgracefulexitgracefulappexitdesktop"></a>Office.System.GracefulExit.GracefulAppExitDesktop

Evenimentul este declanșat de o întrerupere elegantă a aplicației pentru aplicațiile client Office, cum ar fi, dar fără a se limita la, Word, Excel, PowerPoint și Outlook. Utilizăm Ieșirea elegantă pentru a măsura starea de funcționare a produselor client Office. Acesta se dorește a fi un semnal esențial pentru activitate utilizat de către inginerii Office pentru a deduce stabilitatea produselor.

Se colectează următoarele câmpuri:

- **AppBuild** - identificator versiune compilată pentru procesul afectat.
- **AppMajor** - identificator versiune majoră pentru procesul afectat.
- **AppMinor** - identificator versiune minoră pentru procesul afectat.
- **AppRevision** - identificator versiune compilată pentru procesul afectat.
- **BootCompleted** - dacă procesul Office a finalizat inițializarea.
- **DetectionTime** - ora la care s-a detectat ieșirea neprevăzută.
- **EcsETag** - identificator de experiment pentru proces.
- **HasEdit** - editarea documentelor a survenit în timpul procesului Office.
- **HasOpen** - documentul a fost deschis în timpul procesului Office.
- **InstallMethod** - dacă pentru versiunea de compilare curentă a Office s-a efectuat upgrade, dacă s-a revenit la ea sau dacă este o instalare nouă.
- **OfficeUILang** - limba procesului Office.
- **PreviousBuild** - versiune compilată instalată anterior.
- **SafeMode** - a fost procesul Office în modul de siguranță.
- **SessionId** - identificator unic al procesului.
- **SessionInitTime** - ora la care a început procesul afectat.

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

  - **OfficeArchitectureText** - arhitectura de produs Office ca șir (de exemplu, x86, arm).

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

Evenimentul este declanșat de o întrerupere anormală a aplicației (de exemplu, anularea managerului de activități, suspendarea aplicației etc.) pentru aplicațiile client Office, cum ar fi, dar fără a se limita la, Word, Excel, PowerPoint și Outlook. Utilizăm măsurători ale ieșirilor neelegante din aplicație pentru a măsura starea de funcționare a produselor client Office. Acesta este un semnal esențial pentru activitate utilizat pentru a deduce stabilitatea produselor.

Se colectează următoarele câmpuri:

  - **AffectedProcessAppBuild -** identificator versiune compilată pentru procesul afectat. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

  - **AffectedProcessAppBuildRevision -** Identificator revizuire compilare pentru procesul afectat. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

  - **AffectedProcessAppMajorVer -** - Identificator versiune majoră pentru procesul afectat. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

  - **AffectedProcessAppMinorVer -** Identificator versiune minoră pentru procesul afectat. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

  - **AffectedProcessAppName -** numele procesului afectat. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*
  
  - **AffectedProcessAppVersion** Identificator versiune pentru procesul afectat.

  - **AffectedProcessExeBuildVersion -** numărul versiunii compilate a procesului afectat. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

  - **AffectedProcessExeMajorVersion -** numărul versiunii majore a procesului afectat. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

  - **AffectedProcessExeMinorVersion -** numărul versiunii minore a procesului afectat. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

  - **AffectedProcessExeRevisionVersion -** numărul versiunii compilate a procesului afectat. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

  - **AffectedProcessIsDebug -** dacă procesul afectat este o compilare de depanare. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

  - **AffectedProcessIsLabMachine -** dacă procesul afectat este într-un laborator Microsoft. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

  - **AffectedProcessOsEnvironment -** identificator de sistem de operare pentru procesul afectat. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

  - **AppName -** numele aplicației afectate. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

- **AppUsedVirtualMemory** - memorie virtuală utilizată de aplicația Office

- **BucketId** - identificator bucket Watson pentru cădere

- **CabGuid** - identificator Globally Unique Identifier (GUID) pentru cab Watson.

- **CallStack** - Stiva de apeluri interne Microsoft care provoacă căderea.

- **CrashedAssignedFlights -** ediții flight atribuite procesului care a suferit o cădere. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

- **CrashedConfigIds -** configurația atribuită procesului care a suferit o cădere. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

- **CrashedEcsETag -** Identificator de experiment pentru procesul care a suferit o cădere.

- **CrashedImpressionId -** identificatorul de impresie al procesului care a suferit o cădere. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

- **CrashedModuleName -** numele modulului cu erori

- **CrashedProcessSessionID -** identificator unic al procesului care a suferit o cădere. 

- **CrashedProcessSessionInitTime -** ora la care a început procesul afectat. 

- **CrashedProcessSessionUninitTime** - ora la care s-a încheiat procesul afectat.

- **HexCrashTag -** - identificatorul unic pentru codul căderii.

- **CrashType -** identificator de bucket pentru tipul de cădere.

- **DetectionTime -** ora la care s-a detectat ieșirea neprevăzută. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

- **ErrorString -** descrierea erorii. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

- **ExceptionAddress -** adresa din programul unde a apărut eroarea. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

- **ExceptionCode -** identificator de bucket pentru excepție.

- **ExceptionInfo** - informații de sistem pentru excepție.

- **FaultAppName -** numele aplicației defecte. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*
- **HangTypeCode** - reprezintă clasa de agățat în cazul în care procesul atârnat în timpul execuției.

- **InstallMethod -** dacă pentru versiunea de compilare curentă a Office s-a efectuat upgrade, dacă s-a revenit la ea sau dacă este o instalare nouă.

- **InstallType -** identificator pentru metoda prin care a fost instalat Office. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

- **InstallTypeName -** un identificator pentru metoda prin care a fost instalat Office. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

- **IsLabMachine -** dacă Office rulează într-un laborator Microsoft. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

- **IsMsftInternal -** dacă utilizatorul Windows care rulează Office este angajat Microsoft. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

- **ModuleBaseAddress -** adresa de bază a modulului cu erori. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

- **ModuleBuildVersion -** numărul versiunii compilate a modulului cu erori. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

- **ModuleMajorVersion -** numărul versiunii majore a modulului cu erori. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

- **ModuleMinorVersion -** numărul versiunii minore a modulului cu erori. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

- **ModuleName -** numele modulului cu erori. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

- **ModuleOffset -** deplasare în octeți (în hexazecimale) de la adresa de bază unde a apărut eroarea.

- **ModuleRevisionVersion -** numărul versiunii de revizuire compilate a modulului cu erori. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

- **ModuleSize -** dimensiunea modulului cu erori în octeți. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

- **ModuleVersion** - versiune a modulului defect responsabil pentru o cădere.

- **OfficeArchitectureText** - arhitectura instalației: x64, x86 etc.

- **OpenUILang -** Limba interfeței cu utilizatorul pentru aplicația Office.

- **OSEnvironment -** identificator pentru mediul în care rulează Office.

- **PreviousBuild -** versiune compilată instalată anterior

- **ProcessorArchitecture** - procesor arhitectură pentru mediul înconjurător: x64, x86 etc.

- **SessionFlags** - definește condițiile din sesiune, cum ar fi: s-a deschis fișierul sau s-a editat, s-a deschis un document în cloud, a fost finalizată secvența de încărcare etc. 

- **StackHash** - furnizează o identitate codificată pentru stiva de erori din Office.

- **SystemAvailableMemory** - memoria disponibilă în sistemul de operare

- **UAETypeName -** identificator de bucket privind modul brusc în care s-a închis aplicația. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

- **UninitLibletId –** identificatorul unic pentru componenta cu erori a căderii.

- **VerifyElseCrashTag -** identificator unic al locului unde a căzut aplicația. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

- **WatsonReportId** - identificator de raport trimis serviciului Windows Watson.

- **WerEventCreatedTime** - marcă de timp pentru eveniment de raportare a erorilor Windows.

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

  - **AddinExecution -** semnalizare care informează dacă un program de completare a fost executat și nu s-a terminat în timpul unei ieșiri abrupte din aplicație. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

  - **AppUsedVirtualMemory** - memorie virtuală utilizată de aplicația Office

  - **BootCompleted-** A fost boot Office finalizată la momentul căderii. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

  - **BucketId** - identificator bucket Watson pentru cădere
 
  - **CabGuid** - identificator Globally Unique Identifier (GUID) pentru cab Watson.

  - **CallStack** - Stiva de apeluri interne Microsoft care cauzează căderea.

  - **CrashedAppBuild -** identificator versiune compilată pentru procesul afectat. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

  - **CrashedAppMajor -** identificator versiune majoră pentru procesul afectat. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*
 
  - **CrashedAppMinor -** identificator versiune minoră pentru procesul afectat. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

  - **CrashedAppVersion** - identificator versiune aplicație pentru procesul defectat.

  - **CrashedEcsETag** - un identificator de experiment pentru procesul defect.

  - **CrashedModuleName** - numele modulului cu erori.

  - **CrashedProcessSessionId** - un identificator unic al procesului care a suferit o cădere.

  - **CrashedProcessSessionInitTime** - ora la care a început procesul afectat.

  - **CrashedProcessSessionUninitTime** - ora la care s-a încheiat procesul afectat.

  - **HexCrashTag -** - identificatorul unic pentru codul căderii.

  - **CrashTime** - momentul în care se menționează că clientul a terminat negrațios. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

  - **CrashType** - identificator de bucket pentru tipul de cădere.

  - **DetectionTime** - ora la care s-a detectat ieșirea neprevăzută. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

  - **ExceptionAddress** - adresa din programul unde a apărut eroarea. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

  - **ExceptionCode** - identificator de bucket pentru excepție.

  - **ExceptionInfo** - informații de sistem pentru excepție.

  - **Refacerea** - a creat utilizatorul și a înmânat procesul Office într-o nouă sesiune. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

  - **HangTypeCode** - reprezintă clasa de agățat în cazul în care procesul atârnat în timpul execuției.

  - **HasEdit-** - a fost utilizatorul care a editat un document în clientul defectat. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

  - **HasOpen-** - fost un document deschis în clientul prăbușit. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

  - **HexCrashTag -**  identificatorul unic pentru codul căderii. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

  - **HexExceptionAddress** - adresa în hexazecimale din programul unde a apărut eroarea. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

  - **HexExceptionCode** - identificator de bucket în hexazecimale pentru excepție. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

  - **HexModuleBaseAddress** - adresa de bază în hexazecimale a modulului cu erori. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

  - **HexModuleOffset** - deplasare în octeți (în hexazecimale) de la adresa de bază unde a apărut eroarea. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

  - **HexModuleSize** - dimensiune modul cu erori în octeți în hexazecimale. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

  - **HexVerifyElseCrashTag** - identificator unic în hexazecimale al locului unde a căzut aplicația. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

  - **InstallMethod** - dacă pentru versiunea de compilare curentă a Office s-a efectuat upgrade, dacă s-a revenit la ea sau dacă este o instalare nouă.

  - **IsLabMachine** - dacă Office rulează într-un laborator Microsoft. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

  - **ModuleBaseAddress** - adresa de bază a modulului cu erori. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

  - **ModuleOffset** - deplasare în octeți (în hexazecimale) de la adresa de bază unde a apărut eroarea.

  - **ModuleSize** - dimensiunea modulului cu erori în octeți. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

  - **ModuleStamp** - marcaj în modul de eșec.

  - **ModuleVersion** - versiune a modulului defect responsabil pentru o cădere.

  - **OfficeArchitectureText** - arhitectura de produs Office ca șir (de exemplu, x86, arm).

  - **OpenUILang -** - limba interfeței cu utilizatorul pentru aplicația Office.

  - **PreviousBuild** - versiune compilată instalată anterior

  - **ProcessorArchitecture** - procesor arhitectură pentru mediul înconjurător: x64, x86 etc.

  - **SafeMode** - a fost sesiunea pornită în modul de siguranță. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

  - **SessionFlags** - definește condițiile din sesiune, cum ar fi: s-a deschis fișierul sau s-a editat, s-a deschis un document în cloud, a fost finalizată secvența de încărcare etc. 

  - **StackHash** - furnizează o identitate codificată pentru stiva de erori din Office.

  - **SystemAvailableMemory** - memoria disponibilă în sistemul de operare

  - **UAEOSEnvironment** - identificator de mediu pentru sistemul de operare. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

  - **UninitLibletId –** identificatorul unic pentru componenta cu erori a căderii.

  - **VerifyElseCrashTag** - identificator unic al locului unde a căzut aplicația. *[Acest câmp a fost eliminat din compilările curente de Office, dar poate apărea în continuare în versiuni mai vechi.]*

  - **WatsonReportId** - identificator de raport trimis serviciului Windows Watson.

  - **WerEventCreatedTime** - marcă de timp pentru eveniment de raportare a erorilor Windows.


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

  - **QueueFlushCount** - numărul de goliri ale cozii de așteptare

  - **QueueFlushDueToSizeLimit** - dimensiunea la care telemetria golește coada de așteptare

  - **QueueFlushesDueToSize** - numărul de goliri ale cozii de așteptare cauzate de dimensiunea zonei tampon

  - **QueueHardLimit** - limită de închidere telemetrie

  - **QueueLimitHitTime** - când s-a atins limita de închidere

  - **ResultTime** - ora acestui eveniment

### <a name="officetelemetryrulesenginediskthrottled"></a>Office.Telemetry.RulesEngineDiskThrottled

Limitare măsurători DQ. Este obligatorie pentru a avea încredere în toate celelalte date.

Se colectează următoarele câmpuri:

  - **DiskWriteLimit** - limita dimensiunii pe disc pentru datele de telemetrie

  - **DiskWriteTotal** - total scriere pe disc pentru datele de telemetrie

  - **SessionDiskWriteTotal** - total scriere pe disc sesiune pentru datele de telemetrie

  - **ThrottlingTimestamp** - ora la care a fost limitată sesiunea

### <a name="officetelemetryrulesenginemediumcostthrottled"></a>Office.Telemetry.RulesEngineMediumCostThrottled

Limitare măsurători DQ. Este obligatorie pentru a avea încredere în toate celelalte date.

Acest eveniment nu colectează niciun câmp.

### <a name="officetelemetryrulesenginespikethrottled"></a>Office.Telemetry.RulesEngineSpikeThrottled

Limitare măsurători DQ. Este obligatorie pentru a avea încredere în toate celelalte date.

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

Limitare măsurători DQ. Este obligatorie pentru a avea încredere în toate celelalte date.

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
