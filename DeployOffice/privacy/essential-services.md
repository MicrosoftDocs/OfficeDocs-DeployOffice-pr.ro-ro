---
title: Servicii esențiale pentru Office
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
description: Oferă administratorilor Office informații despre servicii esențiale în Office, cum ar fi Clic și Pornire și Licențiere, și asigură o listă de evenimente și câmpuri de date pentru aceste servicii esențiale.
hideEdit: true
ms.openlocfilehash: 31a0eb94d96e43eddb400670437b0d618eb5f30e
ms.sourcegitcommit: 9956e9e774e334a1894f1bb95e628eb71e0b5b2d
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/02/2019
ms.locfileid: "33559227"
---
# <a name="essential-services-for-office"></a>Servicii esențiale pentru Office

> [!IMPORTANT]
> Informațiile din acest articol se aplică la versiunea 1904 sau o versiune mai recentă a următorului software client Office instalat pe un computer care rulează Windows:
> - Office 365 ProPlus și Office 365 Business
> - Office 365 Personal, Office 365 pentru acasă sau alte versiuni de Office, care fac parte dintr-un abonament Office 365.
> - Project și Visio care sunt oferite cu anumite planuri de abonament, cum ar fi planul Project Online Professional sau Visio Online Plan 2.


Office constă din aplicațiile software client și experiențe conectate proiectate pentru a vă permite să creați, să comunicați și să colaborați mai eficient. Deși puteți controla multe dintre experiențele conectate care sunt la dispoziția dvs. sau a utilizatorilor dvs. în cazul în care sunteți administratorul organizației dvs., există un set de servicii care sunt esențiale pentru modul în care funcționează Office și care, prin urmare, nu pot fi dezactivate. De exemplu, serviciul de licențiere care confirmă că aveți licența corectă pentru a utiliza Office. Datele de serviciu necesare cu privire la aceste servicii sunt colectate și trimise la Microsoft, indiferent ce alte setări de politică privind confidențialitatea ați configurat. Puteți vedea aceste date utilizând Vizualizatorul de date de diagnosticare.

Pentru mai multe informații, consultați următoarele:

- [Date de serviciu obligatorii pentru Office](required-service-data.md)
- [Utilizarea Vizualizatorului de date de diagnosticare cu Office](https://support.office.com/article/cf761ce9-d805-4c60-a339-4e07f3182855)
- [Experiențe conectate în Office](connected-experiences.md)

Dacă sunteți administratorul organizației dvs., ați putea fi interesat și de următoarele:

- [Prezentare generală a controalelor de confidențialitate pentru Office 365 ProPlus](overview-privacy-controls.md)
- [Utilizați setările de politică pentru a gestiona controale de confidențialitate pentru Office 365 ProPlus](manage-privacy-controls.md)

## <a name="list-of-essential-services-for-office"></a>Listă de servicii esențiale pentru Office 

Următorul tabel conține o listă a serviciilor esențiale pentru Office și o descriere a fiecărui serviciu.

| **Serviciu**  | **Descriere**  |
| ------ | ---- |
| [Autentificare](#authentication-events) | Autentificare este un serviciu multi-platformă care validează identitatea dvs. de utilizator Office.  Este necesar pentru a vă permite să vă conectați la Office, să vă activați licența de Office și să accesați fișierele stocate în cloud; oferă o experiență unitară la nivelul sesiunilor de Office și al dispozitivelor dvs.    |
| [Clic și Pornire](#click-to-run-events) | Clic și Pornire este tehnologia de instalare utilizată pentru a instala și a actualiza Office pe Windows. Aceasta caută noi versiuni de Office și, atunci când este disponibilă o nouă versiune, o descarcă și o instalează. Clic și Pornire va detecta dacă sunt necesare actualizări Office, inclusiv actualizări de securitate, le va descărca și le va instala.     |
| [Serviciul de configurație avansată (ECS)](#experimentation-and-configuration-service-ecs-events) | ECS oferă Microsoft capacitatea de a reconfigura instalările Office fără a fi nevoie să implementați din nou Office. Este utilizat pentru a controla implementarea treptată de caracteristici sau actualizări, în timp ce impactul implementării este monitorizat pe baza datelor de diagnosticare colectate. Este utilizat, de asemenea, pentru a atenua problemele de securitate sau de performanță cu o caracteristică sau actualizare. În plus, ECS acceptă modificările de configurare legate de datele de diagnosticare pentru a vă ajuta să vă asigurați că evenimentele corespunzătoare sunt colectate. |
| [Licențiere](#licensing-events)     | Licențiere este un serviciu bazat pe cloud care acceptă activarea Office pentru noile instalări și păstrează licența pe dispozitivele dvs. după ce Office a fost activat. Acesta înregistrează fiecare dintre dispozitivele dvs. și activează Office, verifică starea abonamentului Office și gestionează cheile de produs.    |
| [Configurare servicii](#services-configuration-events)  | Configurare servicii oferă capacitatea de a efectua actualizări la setările de configurare Office pentru a activa sau a dezactiva caracteristici client. Este apelat de fiecare dată când pornește o aplicație Office și oferă detalii despre alte configurații și servicii Office. Configurare servicii controlează, de asemenea, ce servicii sunt desemnate ca servicii esențiale.  |
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

### <a name="officeidentityfbapromptwin32"></a>Office.Identity.FbaPromptWin32

Colectate atunci când Office prezintă utilizatorului o solicitare de conectare prin Autentificare bazată pe formulare.

Împreună cu achizițiile de simbol silențios, solicitările de autentificare sunt utilizate pentru a stabili dacă utilizatorul se află într-o stare de autentificare întreruptă, care, pentru utilizator, generează ceea ce este în esență o stare de client neconectat sau, în cel mai rău caz, autentificarea întreruptă poate să împiedice achiziționarea licenței, rezultatul fiind un client complet inutilizabil.

Solicitările de conectare Autentificare bazată pe formulare (FBA) sunt utilizate pentru unele scenarii de autentificare la nivel local și, de obicei, dorim să ne asigurăm că nu se întâmplă acest lucru, deoarece toată lumea ar trebui să utilizeze Autentificare modernă din cauza vulnerabilităților de securitate asociate cu FBA.

**Se colectează următoarele câmpuri:**

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

  - **Data\_ProductReleaseId** - produsul pe care îl instalăm, adică Office 365 ProPlus

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

  - **Data\_ProductReleaseId-** produsul pe care îl instalăm, adică Office 365 ProPlus

### <a name="officeclicktorunscenarioinstalltaskconfigure"></a>Office.ClickToRun.Scenario.InstallTaskConfigure

Date despre instalări și inventar Office colectate atunci când programul de instalare Office plasează fișiere recent descărcate. Utilizat pentru a măsura succesul/eșecul unei instalări de Office.

Se colectează următoarele câmpuri:

  - **Data\_15\_SourceType -** unde se află sursa Office 15, adică CDN sau local 

  - **Data\_15\_UpdatesEnabled -** dacă sunt activate actualizările Office 15 

  - **Data\_15\_UpdateVersion -** la ce versiune Office 15 actualizăm 

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled -** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion -** la ce versiune Office 16 actualizăm 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts -** produsele pe care le adăugăm 

  - **Data\_AddingProducts -** ce produse vi s-a solicitat să adăugați 

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

  - **Data\_ProductsToRemove -** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts -** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează. adică, instalare 

  - **Data\_ScenarioSubType -** ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

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

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion -** la ce versiune Office 16 actualizăm 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** produsele pe care le adăugăm 

  - **Data\_AddingProducts -** ce produse ni s-a solicitat să adăugăm 

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

  - **Data\_ProductsToAdd -** ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează. adică, instalare 

  - **Data\_ScenarioSubType -** ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

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

  - **Data\_15\_UpdateVersion  -** la ce versiune Office 15 actualizăm

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled -** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion  -** la ce versiune Office 16 actualizăm 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts -** produsele pe care le adăugăm 

  - **Data\_AddingProducts -** ce produse ni s-a solicitat să adăugăm 

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

  - **Data\_ProductsToAdd -** ce produse Office adăugăm 

  - **Data\_ProductsToRemove -** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts -** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează. adică, instalare 

  - **Data\_ScenarioSubType -** ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

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

  - **Data\_16\_UpdateVersion -** la ce versiune Office 16 actualizăm 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** produsele pe care le adăugăm 

  - **Data\_AddingProducts -** ce produse ni s-a solicitat să adăugăm 

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

  - **Data\_ProductsToAdd -** ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName  -** ce scenariu rulează. adică, instalare

  - **Data\_ScenarioSubType -** ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

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

  - **Data\_16\_UpdateVersion -** la ce versiune Office 16 actualizăm 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** produsele pe care le adăugăm 

  - **Data\_AddingProducts -** ce produse ni s-a solicitat să adăugăm 

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

  - **Data\_ProductsToAdd -** ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează. adică, instalare

  - **Data\_ScenarioSubType -** ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

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

  - **Data\_15\_UpdateVersion  -** la ce versiune Office 15 actualizăm

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion -** la ce versiune Office 16 actualizăm 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** produsele pe care le adăugăm 

  - **Data\_AddingProducts -** ce produse ni s-a solicitat să adăugăm 

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

  - **Data\_ProductsToAdd -** ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName  -** ce scenariu rulează. adică, instalare 

  - **Data\_ScenarioSubType -** ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

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

  - **Data\_15\_UpdateVersion  -** la ce versiune Office 15 actualizăm

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion -** la ce versiune Office 16 actualizăm 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** produsele pe care le adăugăm 

  - **Data\_AddingProducts -** ce produse ni s-a solicitat să adăugăm 

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

  - **Data\_ProductsToAdd -** ce produse Office adăugăm 

  - **Data\_ProductsToRemove-**  ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName  -** ce scenariu rulează. adică, instalare

  - **Data\_ScenarioSubType -** ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

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

  - **Data\_15\_UpdateVersion  -** la ce versiune Office 15 actualizăm

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion -** la ce versiune Office 16 actualizăm 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts -** produsele pe care le adăugăm 

  - **Data\_AddingProducts -** ce produse ni s-a solicitat să adăugăm 

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

  - **Data\_ProductsToAdd -** ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName  -** ce scenariu rulează. adică, instalare

  - **Data\_ScenarioSubType -** ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

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

  - **Data\_15\_UpdateVersion  -** la ce versiune Office 15 actualizăm

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion -** la ce versiune Office 16 actualizăm 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** produsele pe care le adăugăm 

  - **Data\_AddingProducts -** ce produse ni s-a solicitat să adăugăm 

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

  - **Data\_ProductsToAdd -** ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează, adică instalare 

  - **Data\_ScenarioSubType -** ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

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

  - **Data\_15\_UpdateVersion -**  la ce versiune Office 15 actualizăm 

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion -** la ce versiune Office 16 actualizăm 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** produsele pe care le adăugăm 

  - **Data\_AddingProducts -** ce produse ni s-a solicitat să adăugăm 

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

  - **Data\_ProductsToAdd -** ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează. adică, instalare 

  - **Data\_ScenarioSubType -** ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

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

  - **Data\_15\_UpdateVersion -**  la ce versiune Office 15 actualizăm 

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType  -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled -** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion  -** la ce versiune Office 16 actualizăm 

  - **Data\_16\_Version  -** versiunea Office 16 

  - **Data\_AddingFixedProducts -** produsele pe care le adăugăm 

  - **Data\_AddingProducts  -** ce produse ni s-a solicitat să adăugăm 

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

  - **Data\_ProductsToAdd -** ce produse Office adăugăm 

  - **Data\_ProductsToRemove-**  ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează. adică, instalare 

  - **Data\_ScenarioSubType -** ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

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

  - **Data\_16\_UpdateVersion -** la ce versiune Office 16 actualizăm 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** produsele pe care le adăugăm 

  - **Data\_AddingProducts -** ce produse ni s-a solicitat să adăugăm 

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

  - **Data\_ProductsToAdd -** ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează. adică, instalare 

  - **Data\_ScenarioSubType -** ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

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

  - **Data\_15\_UpdateVersion -**  la ce versiune Office 15 actualizăm 

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion -** la ce versiune Office 16 actualizăm 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** produsele pe care le adăugăm 

  - **Data\_AddingProducts -** ce produse ni s-a solicitat să adăugăm 

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

  - **Data\_ProductsToAdd -** ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează. adică, instalare 

  - **Data\_ScenarioSubType -** ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

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

  - **Data\_16\_UpdateVersion -** la ce versiune Office 16 actualizăm 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** produsele pe care le adăugăm 

  - **Data\_AddingProducts -** ce produse ni s-a solicitat să adăugăm 

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

  - **Data\_ProductsToAdd -** ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează. adică, instalare 

  - **Data\_ScenarioSubType -** ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

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

  - **Data\_16\_UpdateVersion -** la ce versiune Office 16 actualizăm 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** produsele pe care le adăugăm 

  - **Data\_AddingProducts -** ce produse ni s-a solicitat să adăugăm 

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

  - **Data\_ProductsToAdd -** ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează. adică, instalare 

  - **Data\_ScenarioSubType -** ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

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

  - **Data\_15\_UpdateVersion -** la ce versiune Office 15 actualizăm 

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion -** la ce versiune Office 16 actualizăm 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** produsele pe care le adăugăm 

  - **Data\_AddingProducts -** ce produse ni s-a solicitat să adăugăm 

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

  - **Data\_ProductsToAdd -** ce produse Office adăugăm 

  - **Data\_ProductsToRemove-**  ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează. adică, instalare 

  - **Data\_ScenarioSubType -** ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

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

  - **Data\_16\_UpdateVersion -** la ce versiune Office 16 actualizăm 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** produsele pe care le adăugăm 

  - **Data\_AddingProducts -** ce produse ni s-a solicitat să adăugăm 

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

  - **Data\_ProductsToAdd -** ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează. Adică, instalare 

  - **Data\_ScenarioSubType -** ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

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

  - **Data\_16\_UpdateVersion -** la ce versiune Office 16 actualizăm 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** produsele pe care le adăugăm 

  - **Data\_AddingProducts -** ce produse ni s-a solicitat să adăugăm 

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

  - **Data\_ProductsToAdd -** ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează. adică, instalare 

  - **Data\_ScenarioSubType -** ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

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

  - **Data\_16\_UpdateVersion -** la ce versiune Office 16 actualizăm 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** produsele pe care le adăugăm 

  - **Data\_AddingProducts -** ce produse ni s-a solicitat să adăugăm 

  - **Data\_AvailableVersion to-** ce versiune de Office este disponibilă pentru actualizare

  - **Data\_CompletedWithoutActionInfo -** de ce nu am finalizat scenariul, adică aplicațiile erau deschise 

  - **Data\_CompletionState -** dacă am finalizat activitatea

  - **Data\_CorruptionChecksOnly - ** în cazul în care doar căutăm deteriorări și nu actualizăm

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

  - **Data\_ProductsToAdd -** ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează. adică, instalare 

  - **Data\_ScenarioSubType -** ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

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

  - **Data\_16\_UpdateVersion -** la ce versiune Office 16 actualizăm 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** produsele pe care le adăugăm 

  - **Data\_AddingProducts -** ce produse ni s-a solicitat să adăugăm 

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

  - **Data\_ProductsToAdd -** ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName-** ce scenariu rulează. adică, instalare 

  - **Data\_ScenarioSubType -** ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

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

  - **Data\_16\_UpdateVersion -** la ce versiune Office 16 actualizăm 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** produsele pe care le adăugăm 

  - **Data\_AddingProducts -** ce produse ni s-a solicitat să adăugăm 

  - **Data\_AvailableVersion -** ce versiune de Office este disponibilă pentru actualizare

  - **Data\_ComAction -** O int care reprezintă o acțiune com pe care o efectuăm

  - **Data\_CompletedWithoutActionInfo -** de ce nu am finalizat scenariul, adică aplicațiile erau deschise 

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

  - **Data\_ProductsToAdd -** ce produse Office adăugăm 

  - **Data\_ProductsToRemove-**  ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează. adică, instalare

  - **Data\_ScenarioSubType -** ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

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

  - **Data\_15\_UpdateVersion -**  la ce versiune Office 15 actualizăm 

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion -** la ce versiune Office 16 actualizăm 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** produsele pe care le adăugăm 

  - **Data\_AddingProducts -** ce produse ni s-a solicitat să adăugăm 

  - **Data\_AvailableVersion -** ce versiune de Office este disponibilă pentru actualizare

  - **Data\_CompletedWithoutActionInfo-** de ce nu am finalizat scenariul, adică aplicațiile erau deschise

  - **Data\_CompletionState -** dacă am finalizat activitatea

  - **Data\_CorruptionChecksOnly -** în cazul în care doar căutăm deteriorări și nu actualizăm

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

  - **Data\_ProductsToAdd -** ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează. adică, instalare 

  - **Data\_ScenarioSubType -** ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

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

  - **Data\_15\_UpdateVersion -**  la ce versiune Office 15 actualizăm 

  - **Data\_15\_Version -** versiunea Office 15 

  - **Data\_16\_SourceType -** unde se află sursa Office 16, adică CDN sau local 

  - **Data\_16\_UpdatesEnabled-** dacă sunt activate actualizările Office 16 

  - **Data\_16\_UpdateVersion -** la ce versiune Office 16 actualizăm 

  - **Data\_16\_Version -** versiunea Office 16 

  - **Data\_AddingFixedProducts-** produsele pe care le adăugăm 

  - **Data\_AddingProducts -** ce produse ni s-a solicitat să adăugăm 

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

  - **Data\_ProductsToAdd -** ce produse Office adăugăm 

  - **Data\_ProductsToRemove-** ce produse Office eliminăm 

  - **Data\_RemovingFixedProducts-** produsele pe care le eliminăm 

  - **Data\_RemovingProducts -** produsele pe care ni s-a solicitat să le eliminăm 

  - **Data\_ScenarioInstanceID -** GUID unic pentru scenariul care rulează 

  - **Data\_ScenarioName -** ce scenariu rulează. adică, instalare 

  - **Data\_ScenarioSubType -** ce tip de scenariu rulăm, adică Dezinstalare, Reinstalare 

  - **Data\_SourceType -** unde se află sursa noastră, adică CDN 

  - **Data\_SqmMachineID -**  ID unic de computer utilizat de Windows SQM 

  - **Data\_SusClientID -** identificator de actualizare Office computer 

  - **Data\_TaskState -** care este starea activității, cum ar fi rulare sau anulat 

  - **Data\_TotalClientCabSize -** dimensiunea fișierului cab al clientului nostru 

  - **Data\_TriggeringUI -** ce a declanșat interfața cu utilizatorul 

  - **Data\_UpdatesEnabled -** dacă sunt activate actualizările Office 

  - **Data\_Version -** versiunea de Office 

### <a name="officeclicktoruntransportexperimentaltransportpipelinecreatetransport"></a>Office.ClickToRun.Transport.ExperimentalTransport.PipelineCreateTransport

Date despre instalări și inventar Office colectate atunci când clientul Clic și Pornire creează un flux de transport pentru a descărca fișiere Office. Utilizat pentru a stabili starea de funcționare a diferitelor tehnologii de transport (de ex., HTTP, BITS, DO) care este de importanță critică la descărcarea corespunzătoare a Office pentru instalare și actualizări.

Se colectează următoarele câmpuri:

  - **Data\_IsForeGroundStreaming** – Dacă redăm în flux în prim plan sau în fundal

  - **Data\_IsInstallMode** - 1 dacă instalăm și descărcăm fișiere, 0 în caz contrar

  - **Data\_SourceProtocol-** dacă descărcăm dintr-o rețea de date de conținut, CDN, computerul pe care instalăm, local sau de la o resursă de pe rețeaua locală,

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


## <a name="experimentation-and-configuration-service-ecs-events"></a>Evenimente Experimentation and Configuration Service (ECS)

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

  - **LicenseCategory** - categoria de licență Office pe care o utilizează utilizatorul 

  - **Licenses** - lista de nume a tuturor licențelor de Office prezente pe calculator 

  - **LicenseStatuses** - starea tuturor licențelor de Office prezente pe calculator 

### <a name="officelicensinggetentitlement"></a>Office.Licensing.GetEntitlement 

Colectăm acest lucru atunci când utilizatorul configurează un dispozitiv și apelăm serviciul nostru de licențiere pentru a detecta dacă utilizatorul autentificat are drepturi de Office sau nu. Acesta raportează rezultatul apelului respectiv. Este de importanță critică pentru a detecta dacă utilizatorul se află în stare bună și dacă îi lipsesc funcționalități, este utilizat pentru sănătatea sistemului și în scopuri de diagnosticare dacă un utilizator raportează o problemă cu computerul

Acest eveniment nu colectează niciun câmp.

### <a name="officelicensingheartbeat"></a>Office.Licensing.Heartbeat 

La fiecare sesiune verificăm dacă au trecut 72 de ore de la ultima reînnoire de licență și încercăm să extindem valabilitatea licenței curente. Acest eveniment raportează succesul sau eșecul apelului pe care îl efectuăm pentru a ne asigura că putem extinde valabilitatea licenței și să păstrăm funcțională instalarea Office a utilizatorului. Este de importanță critică în diagnosticarea problemelor legate de abonament și serviciu pentru utilizator și în detectarea regresiilor pentru utilizatorii care dețin deja un abonament activat.

Se colectează următoarele câmpuri:

  - **Mode** - o reprezentare cu enumerator a stivei de licențiere Office care este utilizată la acest computer

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

  - **LicenseStatus** - starea licenței Office pe care o utilizează utilizatorul

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

  - **Office.Licensing.NextUserLicensingEligible -** Acest semnal ne informează dacă un utilizator este calificat să treacă la noua noastră stivă de licențiere. Este de importanță critică pentru a cuantifica impactul asupra utilizatorilor existenți pe măsură ce implementăm noua noastră stivă de licențiere și ne asigurăm că utilizatorii nu pierd funcționalitatea

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

Este vorba despre metadatele de licențiere colectate de pe dispozitiv la fiecare pornire care raportează indicatorul acid al licenței, starea licenței, tipul de licență și alte proprietăți ale acesteia care sunt esențiale în identificarea caracteristicilor puse la dispoziția utilizatorului. Este de importanță critică în a identifica setul de caracteristici puse la dispoziția utilizatorului, precum și dacă utilizatorului îi lipsește o anumită funcționalitate. Este utilizat, de asemenea, pentru calculele Utilizatorilor activi zilnic/lunar și pentru diferite alte rapoarte ale unor echipe la nivelul Office (marketing/DIG/licențiere) deoarece precizează produsul tip folosit de utilizator, indiferent că este un produs cu abonament sau că utilizatorului îi lipsește o funcționalitate de importanță critică.

Se colectează următoarele câmpuri:

  - **FullValidationMode** – mod care indică faptul că suntem în curs de verificare completă a validării licenței 

  - **IsRFM** - indică dacă utilizatorul se află în modul de funcționalitate redusă sau nu 

  - **IsSCA** - indică dacă rulăm în modul de activare am rulează în modul de activare computer partajat 

  - **IsSubscription** - indică dacă utilizatorul utilizează o licență de abonament sau nu 

  - **IsvNext** - indică dacă utilizăm noua stivă de licențiere modernă sau nu 

  - **LicenseCategory** - categoria de licență Office pe care o utilizează utilizatorul 

  - **LicenseStatus** - starea licenței Office pe care o utilizează utilizatorul 

  - **LicenseType** - tipul de licență Office folosită de utilizator 

  - **LicensingACID** - identificator GUID care reprezintă produsul Office pentru care are licență utilizatorul 

  - **OlsLicenseId** - identificator alfanumeric al licenței care a fost emise pentru utilizator 

  - **SkuIdIsNull** – indică dacă am întâmpinat o eroare și nu cunoaștem produsul pe care rulează utilizatorul 

  - **SlapiIsNull** – indică dacă am întâmpinat o problemă la popularea unuia dintre obiectele de licențiere 

### <a name="officelicensingonlinerepair"></a>Office.Licensing.OnlineRepair 

Dacă dintr-un motiv sau altul nu putem activa un utilizator și trebuie să îi afișăm o casetă de dialog care îi solicită să intre online și să încerce să parcurgă pașii de reparare, se declanșează acest eveniment. Este de importanță critică pentru a detecta dacă utilizatorul se află în stare bună, fără să îi lipsească funcționalități, este utilizat pentru sănătatea sistemului și în scopuri de diagnosticare dacă un utilizator raportează o problemă cu computerul

Acest eveniment nu colectează niciun câmp.

### <a name="officelicensingpurchase"></a>Office.Licensing.Purchase 

Avem un experiment care oferă utilizatorului opțiunea de a încerca și a configura plata automată pentru Office direct din aplicație, fără să iasă din contextul aplicației. Acesta raportează succesul sau eșecul experimentului respectiv împreună cu codul de eroare Este de importanță critică pentru a detecta dacă utilizatorul se află în stare bună, fără să îi lipsească funcționalități, este utilizat pentru sănătatea sistemului și în scopuri de diagnosticare dacă un utilizator raportează o problemă cu computerul.

Se colectează următoarele câmpuri:

  - **StorePurchaseStatus** - reprezintă codul de eroare/codul de succes al apelului de achiziție care a fost efectuat prin Microsoft Store

### <a name="officelicensingsearchforsessiontoken"></a>Office.Licensing.SearchForSessionToken

Dacă utilizatorul rulează în modul de activare computer partajat, încercăm să căutăm un simbol de sesiune pe computer care permite utilizatorului să folosească aplicația. Acest eveniment raportează succesul sau eșecul scenariului împreună cu codul de eroare Este de importanță critică pentru a detecta dacă utilizatorul se află în stare bună, fără să îi lipsească funcționalități, este utilizat pentru sănătatea sistemului și în scopuri de diagnosticare dacă un utilizator raportează o problemă cu computerul.

Se colectează următoarele câmpuri:

  - **LoadLicenseResult** - reprezintă codul de eroare/codul de succes al operației noastre de încărcare a licențelor pentru utilizatorul curent

  - **OpportunisticTokenRenewalAttempted** - indică dacă am încercat să reînnoim simbolul de sesiune al utilizatorului în mod oportunist

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

### <a name="officelicensingusegracekey"></a>Office.Licensing.UseGraceKey

Dintr-un motiv sau altul, nu putem să licențiem utilizatorul; instalăm o cheie de grație și trimitem acest semnal cu semnificație. Este de importanță critică pentru a detecta dacă utilizatorul se află în stare bună și dacă îi lipsesc funcționalități, este utilizat pentru sănătatea sistemului și în scopuri de diagnosticare dacă un utilizator raportează o problemă cu computerul

Se colectează următoarele câmpuri:

  - **OpportunisticTokenRenewalAttempted** - indică dacă am încercat o reînnoire oportunistă pentru utilizator în modul de activare computer partajat

  - **ReArmResult** - indică rezultatul reactivării perioadei de probă a cheii instalate, ceea ce poate extinde valabilitatea licenței curente

## <a name="services-configuration-events"></a>Evenimente de configurare servicii

Configurare servicii nu colectează niciun eveniment cu date necesare de diagnosticare a serviciului.

## <a name="telemetry-events"></a>Evenimente de telemetrie

### <a name="officesystemidentitychanged"></a>Office.System.IdentityChanged

Informații privind identitatea utilizatorului necesare pentru îndeplinirea solicitărilor persoanei vizate.

Se colectează următoarele câmpuri:

  - **IdentityChanged** - întotdeauna adevărată. Identitatea s-a modificat.

  - **TimerDetectedChange** - dacă modificarea a fost detectată prin metoda ping cu temporizare regulată.

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

  - **ProcessFileName -** numele de executabil al aplicației care rulează

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

  - **ProcessFileName -** numele de executabil al aplicației care rulează

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

  - **ProcessFileName -** numele de executabil al aplicației care rulează

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

<!-- end list -->

  - **WindowsErrorReportingMachineId** - identificator computer atribuit Tehnologie Windows de raportare a erorilor al dispozitivului pe care rulează Office.

  - **WindowsSqmMachineId** - identificator computer atribuit Windows al dispozitivului pe care rulează Office.

### <a name="officesystemsystemhealthmetadataoperatingsystem"></a>Office.System.SystemHealthMetadataOperatingSystem

Metadatele necesare pentru a izola reproducerea unui erori.

Se colectează următoarele câmpuri:

  - **CollectionTime** - ora la care acest eveniment a fost atașat la coadă pentru încărcare

  - **IsTerminalServer** - adevărat/fals este client server terminal

  - **OsBuild** - versiunea compilată a sistemului de operare.

  - **OsBuildRevision** - revizuire compilare SO

  - **OSEnvironment** -Windows, iOS, Mac, Android etc.

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

Utilizat pentru a captura măsurători privind căderea.

Se colectează următoarele câmpuri:

  - **CrashedAppBuild -** identificator versiune compilată pentru procesul afectat.

  - **CrashedAppMajor -** identificator versiune majoră pentru procesul afectat.

  - **CrashedAppMinor -** identificator versiune minoră pentru procesul afectat.

  - **CrashedAppRevision -** identificator versiune compilată pentru procesul afectat.

  - **CrashedConfigIds -** configurația atribuită procesului care a suferit o cădere.

  - **CrashedEcsETag -** Identificator de experiment pentru procesul care a suferit o cădere.

  - **CrashedImpressionId -** identificatorul de impresie al procesului care a suferit o cădere.

  - **CrashedModuleName -** numele modulului cu erori.

  - **CrashedSessionId -** identificator unic al procesului care a suferit o cădere.

  - **CrashedSessionInitTime -** ora la care a început procesul afectat.

  - **CrashType -** identificator de bucket pentru tipul de cădere.

  - **DetectionTime -** ora la care s-a detectat ieșirea neprevăzută.

  - **ExceptionAddress -** adresa din programul unde a apărut eroarea.

  - **ExceptionCode -** identificator de bucket pentru excepție.

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

  - **PreviousBuild -** versiune compilată instalată anterior

  - **UAEOSEnvironment -** identificator de mediu pentru sistemul de operare.

  - **VerifyElseCrashTag -** identificator unic al locului unde a căzut aplicația.

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

  - **DialogCancelled** - a fost anulată caseta de dialog a Vizualizatorului datelor de diagnosticare

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
