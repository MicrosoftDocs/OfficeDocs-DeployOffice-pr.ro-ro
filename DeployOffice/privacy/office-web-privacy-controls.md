---
title: Utilizarea setărilor de politică pentru a gestiona controalele de confidențialitate pentru Office pentru aplicațiile web
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
audience: ITPro
ms.topic: article
ms.service: o365-proplus-itpro
localization_priority: Priority
ms.collection: Ent_O365
ms.custom:
- Ent_Office_ProPlus
- Ent_Office_Privacy
description: Furnizează administratorilor Office informații despre cum să gestioneze setările de confidențialitate pentru Office pentru aplicațiile web.
hideEdit: true
ms.openlocfilehash: b5131d5ffc09b28a3b5731a417fcd6d383fb7d01
ms.sourcegitcommit: da41d41b443c8392c96e64a4d2fc674957abddf5
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/11/2020
ms.locfileid: "47431973"
---
# <a name="use-policy-settings-to-manage-privacy-controls-for-office-for-the-web-applications"></a>Utilizarea setărilor de politică pentru a gestiona controalele de confidențialitate pentru Office pentru aplicațiile web

> [!NOTE]
> Pentru o listă de produse Office care sunt reglementate de aceste informații despre confidențialitate, consultați [Controale de confidențialitate disponibile pentru produsele Office](products-versions-privacy-controls.md).

În calitate de administrator al organizației dvs., puteți să controlați dacă utilizatorii dvs. au opțiunea de a utiliza experiențe conectate opționale atunci când utilizează Office pentru aplicațiile web, cum ar fi Word pentru web sau PowerPoint pentru web. Această opțiune este disponibilă doar pentru utilizatorii dvs. dacă aceștia sunt conectați cu contul lor de la locul de muncă sau de la școală, atunci când utilizează Office pentru aplicațiile web. Pentru a controla dacă utilizatorii dvs. au posibilitatea de a utiliza experiențe conectate opționale, utilizați *Permite utilizarea experienței suplimentare opționale conectate în setarea de politică* Office.

## <a name="overview-of-optional-connected-experiences"></a>Prezentare generală a experiențelor conectate opționale în Office

Experiențele cu conexiune opțională sunt servicii susținute de cloud, care sunt disponibile pentru utilizatorii dvs. atunci când utilizează Office. Exemple de experiențe conectate opționale includ crearea unei diagrame de hartă în Excel sau inserarea unei imagini online în documentul dvs. Word, ambele bazându-se pe serviciile furnizate de Microsoft Bing. Utilizarea acestor servicii susținute de cloud sunt opționale. 

Experiențele cu conectare opțională nu sunt incluse în acordul comercial al organizației dvs. cu Microsoft. În schimb, experiențele cu conexiune opțională sunt oferite de Microsoft direct utilizatorilor dvs. și sunt reglementate de [Acordul de Servicii Microsoft](https://www.microsoft.com/servicesagreement). În unele cazuri, conținutul sau funcționalitățile de la terți sunt furnizate prin aceste experiențe conectate opționale și se pot aplica și alte condiții.

Este posibil ca unele experiențe cu conexiune opțională să nu fie disponibile în Office pentru aplicațiile web, dar sunt disponibile atunci când utilizați alte versiuni de Office, cum ar fi versiunea desktop pe un dispozitiv care rulează Windows.

Pentru mai multe informații, consultați [Prezentare generală a experiențelor conectate opționale în Office](optional-connected-experiences.md).

## <a name="configure-the-policy-setting-by-using-the-office-cloud-policy-service"></a>Configurarea setării de politică utilizând serviciul politica Office Cloud

Puteți utiliza *Permite utilizarea experienței suplimentare opționale conectate în Office* setarea de politică pentru a controla dacă utilizatorii dvs. au posibilitatea de a utiliza experiențe conectate opționale. Pentru a configura această setare de politică pentru aceste aplicații Office pentru web trebuie să utilizați [ Serviciul de politică pentru cloud Office](../overview-office-cloud-policy-service.md).  

Dacă nu configurați această setare de politică, aceste experiențe conectate opționale vor fi disponibile pentru utilizatorii dvs. Dacă dezactivați această setare de politică, utilizatorii dvs. nu vor putea utiliza nicio experiență conectată opțional.

Pentru Office pentru aplicațiile web, setarea de politică se aplică atunci când utilizatorii dvs. lucrează la documente Office salvate în stocare bazată pe web de la Microsoft, cum ar fi OneDrive pentru Business sau SharePoint Online.

Pentru că utilizați serviciul Office Cloud pentru politică, această setare de politică se aplică și atunci când utilizatorii dvs. utilizează Office pe dispozitive Windows, Mac, iOS sau Android. Nu puteți configura această setare de politică doar pentru atunci când utilizatorii dvs. utilizează Office pentru aplicațiile web. Dar puteți să creați o configurație de politică care să includă această setare de politică și să aveți acea configurație de politică aplicată doar pentru utilizatorii care accesează documente anonim utilizând Office pentru aplicațiile web.

Dacă alegeți să puneți experiențe conectate opționale la dispoziția utilizatorilor dvs., utilizatorii vor primi o notificare de confidențialitate prima dată când utilizează aplicația Office pentru web. Această notificare le permite utilizatorilor să știe că le-ați oferit opțiunea de a utiliza aceste experiențe conectate opționale. De asemenea, notificarea informează utilizatorii cu privire la faptul că experiențele conectate opționale sunt furnizate sub acordul de servicii Microsoft. Deoarece această notificare reprezintă informații importante pentru utilizatorii dvs., notificarea trebuie să fie afișată și nu poate fi dezactivată, ascunsă sau acceptată în numele utilizatorilor.

## <a name="users-can-choose-to-turn-off-optional-connected-experiences"></a>Utilizatorii pot alege să dezactiveze experiențe conectate opționale

Dacă alegeți să efectuați experiențe conectate opționale la dispoziția utilizatorilor dvs., utilizatorii dvs. pot accesa [setările de confidențialitate ale contului](https://support.microsoft.com/office/3e7bc183-bf52-4fd0-8e6b-78978f7f121b#ID0EAADAAA=Online) și vor alege să își dezactiveze accesul la experiențe conectate opționale. Această opțiune este disponibilă în setările de confidențialitate ale contului doar dacă utilizatorii dvs. sunt conectați cu contul de la locul de muncă sau de la școală. Nu este nicio modalitate prin care dvs., ca administrator, să împiedicați utilizatori individuali din organizația dvs. să dezactiveze accesul la experiențele conectate opționale din setările de confidențialitate a contului lor, dacă le-ați acordat utilizatorilor alegerea de a folosi experiențele conectate opționale.

## <a name="related-articles"></a>Articole asociate

- [Prezentare generală a controalelor de confidențialitate pentru Aplicații Microsoft 365 pentru întreprindere](overview-privacy-controls.md)
- [Utilizați setările de politică pentru a gestiona controale de confidențialitate pentru Aplicații Microsoft 365 pentru întreprindere](manage-privacy-controls.md)
- [Utilizați preferințele pentru a gestiona controalele de confidențialitate ale Office pentru Mac](mac-privacy-preferences.md)
- [Utilizați preferințele pentru a gestiona controalele de confidențialitate ale Office pe dispozitivele iOS.](ios-privacy-preferences.md)
- [Utilizați setările de politică pentru a gestiona controale de confidențialitate pentru Office pe dispozitivele Android](android-privacy-controls.md)