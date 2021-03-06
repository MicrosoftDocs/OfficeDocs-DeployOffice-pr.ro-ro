---
title: Date de diagnosticare opționale pentru Office
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
description: Oferă administratorilor Office informații despre datele de diagnosticare opționale din Office, inclusiv exemple de evenimente.
hideEdit: true
ms.openlocfilehash: 7dc10c50baed0306e3e7fc6dd70e0d798a72d0bc
ms.sourcegitcommit: e64b8f2b7f92a3972d8dc83f47d84648fbe17370
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 11/06/2020
ms.locfileid: "48931266"
---
# <a name="optional-diagnostic-data-for-office"></a>Date de diagnosticare opționale pentru Office

> [!NOTE]
> Pentru o listă de produse Office care sunt reglementate de aceste informații despre confidențialitate, consultați [Controale de confidențialitate disponibile pentru produsele Office](products-versions-privacy-controls.md).

Datele de diagnosticare se folosesc pentru a păstra Office în siguranță și la zi, pentru a detecta, a diagnostica și a remedia problemele și pentru a îmbunătăți produsele. Aceste date nu includ numele sau adresa de e-mail a unui utilizator, nici conținutul fișierelor acestuia sau informații despre aplicații care nu au legătură cu Office.

Aceste date de diagnosticare sunt colectate și trimise la Microsoft despre software-ul client Office care rulează pe dispozitivul utilizatorului. Anumite date de diagnosticare sunt obligatorii, în timp ce altele sunt opționale. Vă oferim posibilitatea de a alege dacă să ne trimiteți datele de diagnosticare obligatorii sau opționale, utilizând controalele de confidențialitate, cum ar fi setările de politici pentru organizații. Puteți vedea datele de diagnosticare care ne sunt trimise utilizând Vizualizatorul de date de diagnosticare.

> [!NOTE]
> Dacă utilizați o versiune de Office 2019 sau Office 2016 care nu vă oferă dvs. sau administratorului posibilitatea de a alege dacă doriți să ne trimiteți date de diagnosticare obligatorii sau opționale, sunt trimise doar datele de diagnosticare obligatorii. De exemplu, dacă utilizați Office Professional Plus 2019 sau Office Standard 2016, care nu oferă această opțiune, sunt trimise doar datele de diagnosticare obligatorii. Office 2013 nu trimite date de diagnosticare obligatorii sau opționale. Pentru mai multe informații despre versiunile de Office care oferă această posibilitate, consultați [Controale de confidențialitate disponibile pentru produsele Office](products-versions-privacy-controls.md).

***Datele de diagnosticare opționale** sunt date suplimentare care ne ajută să îmbunătățim produsele și furnizează informații detaliate care ne ajută să detectăm, să diagnosticăm și să remediem problemele.

Dacă alegeți să ne trimiteți date de diagnosticare opționale, sunt incluse și datele de diagnosticare obligatorii. De asemenea, pot fi trimise fișiere jurnal de diagnostic pentru Office, care conțin informații foarte asemănătoare cu datele de diagnostic opționale. Pentru mai multe informații despre acele fișiere jurnal, consultați [Prezentare generală a fișierelor jurnal de diagnosticare pentru Office](https://support.microsoft.com/office/fba86aac-70dc-4858-ae1f-ec2034346cdf).

Exemplele de date de diagnosticare opționale includ datele pe care le colectăm despre formele inserate de utilizatori în documente Word, astfel încât să oferim opțiuni mai bune, și datele pe care le colectăm despre timpul necesar ca un diapozitiv PowerPoint să apară pe ecran; astfel, putem îmbunătăți experiența dacă ea este lentă.

Pentru mai multe informații despre datele de diagnosticare, consultați articolele următoare:

- [Date de diagnosticare obligatorii pentru Office](required-diagnostic-data.md)
- [Utilizarea Vizualizatorului de date de diagnosticare cu Office](https://support.microsoft.com/office/cf761ce9-d805-4c60-a339-4e07f3182855)

Dacă sunteți administratorul organizației dvs., v-ar putea interesa și următoarele articole:

- [Prezentare generală a controalelor de confidențialitate pentru Aplicații Microsoft 365 pentru întreprindere](overview-privacy-controls.md)
- [Utilizați setările de politică pentru a gestiona controale de confidențialitate pentru Aplicații Microsoft 365 pentru întreprindere](manage-privacy-controls.md)
- [Utilizați preferințele pentru a gestiona controalele de confidențialitate ale Office pentru Mac](mac-privacy-preferences.md)
- [Utilizați preferințele pentru a gestiona controalele de confidențialitate ale Office pe dispozitivele iOS.](ios-privacy-preferences.md)
- [Utilizați setările de politică pentru a gestiona controale de confidențialitate pentru Office pe dispozitivele Android](android-privacy-controls.md)

## <a name="categories-of-optional-diagnostic-data"></a>Categorii de date de diagnosticare opționale

Datele de diagnosticare opționale sunt organizate în următoarele categorii:

- Inventar și instalare software
- Utilizarea produselor și a serviciilor
- Performanța produselor și a serviciilor
- Conectivitatea și configurarea dispozitivelor

Aceste categorii sunt afișate în Vizualizatorul de date de diagnosticare și sunt aceleași care se utilizează pentru datele de diagnosticare obligatorii.

Următoarele secțiuni oferă o descriere a fiecărei categorii și exemple de evenimente pentru fiecare categorie.

## <a name="software-setup-and-inventory-events"></a>Evenimente de inventar și instalare software

Această categorie include evenimentele care pot acoperi zonele următoare:

- Produsul instalat, versiunea și starea de instalare
- Programele de completare software și setările lor.
- Condițiile de eroare ale documentelor, caracteristicilor și programelor de completare care pot compromite securitatea, inclusiv pregătirea pentru actualizarea produselor.

Următorul tabel oferă exemple de evenimente din această categorie și o descriere a acelor evenimente.

| _ *Nume eveniment**   | **Descriere eveniment**  |
| ---- | ---- |
| Office.Extensibility.AppCommands.GetRibbonUpdatesForUserId | Acest eveniment indică dacă Word actualizează cu succes panglica din Interfața de utilizator Word atunci când utilizatorul își schimbă identitatea. Folosim acest eveniment pentru a detecta configurarea incorectă și alte probleme care ar afecta interfața de utilizator Office. |
| Office.Extensibility.AppCommands.AppCmdInstall   | Acest eveniment oferă informații despre programul de completare Office instalat de utilizator, inclusiv ID-ul de aplicație, versiunea și compilarea sistemului de operare, succesul instalării și durata sa.  |

## <a name="product-and-service-usage-events"></a>Evenimente privind utilizarea produselor și a serviciilor

Această categorie include evenimentele care pot acoperi zonele următoare:

- Succesul funcționalității aplicației. Limitat la deschiderea și închiderea aplicației și a documentelor, editarea fișierelor și partajarea fișierelor (colaborare).
- Stabilirea dacă au avut loc anumite evenimente de caracteristici, cum ar fi pornirea sau oprirea, și dacă respectiva caracteristică rulează.
- Caracteristici de accesibilitate în Office

Următorul tabel oferă exemple de evenimente din această categorie și o descriere a acelor evenimente.

| **Nume eveniment**   | **Descriere eveniment**  |
| ------ | ------- |
| Office.Word.Commanding.Highlight  | Acest eveniment indică faptul că Word a executat comanda pentru a evidenția textul. Utilizăm acest eveniment pentru a detecta erorile din comanda de evidențiere text.  |
| Office.Translator.AddInLoaded   | Un mesaj repetat care indică faptul că respectiva caracteristică Traducător s-a încărcat și s-a redat cu succes.  |
| Office.Graphics.GVizInsertShape |Urmărește utilizarea caracteristicii Inserare imagine în Word și raportează detalii privind tipurile de forme inserate și sursa acestora.| 
| Office.PowerPoint.PPT.Desktop.SummaryZoomInsertionRule   | Acest eveniment determină dacă există secțiuni prezente într-un document atunci când utilizatorul inserează caracteristica Zoom de rezumat și dacă utilizatorul alege să șteargă secțiunile existente. |
| Office.Security.SecureReaderHost.ProtectedViewValidation | Urmărește când și de ce se deschide un fișier în Vizualizarea protejată. Se folosește pentru a diagnostica anumite situații în care Vizualizarea protejată poate să nu fie corect declanșată, pentru a vă asigura că această caracteristică funcționează corect. |

## <a name="product-and-service-performance-events"></a>Evenimente privind performanța produselor și a serviciilor

Această categorie include evenimentele care pot acoperi zonele următoare:

- Ieșirile neașteptate ale aplicației (blocări) și starea aplicației atunci când se întâmplă acest lucru.
- Timpii de răspuns slabi sau performanțele scăzute pentru scenarii precum pornirea aplicației sau deschiderea unui fișier.
- Erorile în funcționalitatea unei caracteristici sau a unei experiențe de utilizator.

Următorul tabel oferă exemple de evenimente din această categorie și o descriere a acelor evenimente.

| **Nume eveniment**    | **Descriere eveniment**   |
| --------------- | -------------- |
| Office.Word.Word.CoreSaveTime100ns     | Acest eveniment înregistrează performanța unei activități de salvare a documentelor în Word. Utilizăm acest eveniment pentru a detecta erorile și problemele de performanță din activitatea de salvare a documentelor în Word.|
| Office.Identity.SignInForWamAccountAad  | Acest eveniment este trimis atunci când un utilizator este conectat la un cont Azure Active Directory cu biblioteca Web Account Manager (WAM). Acest eveniment trimite metadate, cum ar fi AppName, AppVersion și ErrorCode, dacă evenimentul nu a reușit. |
| Office.PowerPoint.PPT.Desktop.FileOpen.FirstSlideMasterThumbnailRenderTime | Acest eveniment colectează durata de timp necesară pentru a reda prima miniatură coordonator de diapozitive în PowerPoint.  |
| Office.Extensibility.Diagnostics   | Acest eveniment oferă informații generale de diagnosticare pentru programele de completare Office, cum ar fi rapoartele de eroare pentru depanare.|

## <a name="device-connectivity-and-configuration-events"></a>Evenimente privind conectivitatea și configurarea dispozitivelor

Această categorie include evenimentele care pot acoperi zonele următoare:

- Starea conexiunii la rețea și setările dispozitivelor, cum ar fi memoria.

Următorul tabel oferă exemple de evenimente din această categorie și o descriere a acelor evenimente.

| **Nume eveniment**                    | **Descriere eveniment**                                                                                                                                                     |
| ------ | ----- |
| Office.Graphics.ArtViewValidate | Acest eveniment înregistrează rezultatele Vizualizării grafice care acceptă Interfața de utilizator pentru elemente grafice. Folosim evenimentul pentru a colecta date de utilizare și de eroare despre redarea elementelor grafice. |
| Office.Graphics.ARCExceptionScope | Acest eveniment urmărește erorile de redare provenite de la motorul de redare. |
| Office.Extensibility.ODPLatency   | Acest eveniment oferă informații despre conexiunea de rețea și viteza utilizatorului.     |
