---
title: Date de serviciu obligatorii pentru Office
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
description: Oferiți administratorilor Office o prezentare generală a datelor de serviciu obligatorii care sunt colectate despre experiențele de mod conectat din Office.
hideEdit: true
ms.openlocfilehash: eaa659e375d3d5c29d5410ab53db7ae583df6e9d
ms.sourcegitcommit: 02c4120c0b10bfe378d21d60699ae49aaef97834
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/15/2019
ms.locfileid: "37510632"
---
# <a name="required-service-data-for-office"></a>Date de serviciu obligatorii pentru Office 

> [!IMPORTANT]
> Informațiile din acest articol se aplică la versiunea 1904 sau o versiune mai recentă a următorului software client Office instalat pe un computer care rulează Windows:
> - Office 365 ProPlus și Office 365 Business
> - Office 365 Personal, Office 365 pentru acasă sau alte versiuni de Office, care fac parte dintr-un abonament Office 365.
> - Project și Visio care sunt oferite cu anumite planuri de abonament, cum ar fi planul Project Online Professional sau Visio Online Plan 2.
>
> Informațiile se aplică și la versiunea 16.28 sau la versiunile mai recente ale următoarelor aplicații Office pentru Mac: Excel, Outlook, OneNote, PowerPoint și Word.

Office constă din aplicațiile software client și experiențe conectate proiectate pentru a vă permite să creați, să comunicați și să colaborați mai eficient. Lucrul cu alte persoane într-un document stocat pe OneDrive pentru business sau traducerea conținutului unui document Word într-o altă limbă sunt exemple de experiențe de mod conectat.

Datele de serviciu obligatorii sunt esențiale, deoarece ne permit să furnizăm aceste experiențe de mod conectat în cloud, precum și să contribuim la securizarea lor și la funcționarea lor așa cum așteaptă clienții noștri. Datele de serviciu obligatorii sunt alcătuite din trei tipuri de informații.

- **Conținutul creat de utilizator**, care este conținutul pe care l-ați creat utilizând Office, cum ar fi textul introdus într-un document Word și este utilizat împreună cu experiența în mod conectat.
- **Datele funcționale**, care includ informațiile necesare ca o experiență în mod conectat să efectueze activități, cum ar fi informațiile de configurație despre aplicație.
- **Datele de diagnosticare serviciu**, care includ datele necesare pentru a menține serviciul securizat, actualizat și într-o stare de funcționare conform așteptărilor. Întrucât aceste date sunt strâns legate de experiența în mod conectat, ele sunt separate de nivelurile de date de diagnosticare obligatorii sau opționale.

## <a name="example-of-required-service-data-for-a-connected-experience"></a>Exemple de date de serviciu obligatorii pentru experiențe în mod conectat

Pentru a vă ajuta să înțelegeți datele de serviciu obligatorii, vom prezenta în continuare un exemplu ce utilizează PowerPoint Designer, care este o experiență de mod conectat pe care o puteți utiliza atunci când creați diapozitive pentru o prezentare. PowerPoint Designer vă ajută să vă îmbunătățiți diapozitivele generând automat idei de proiectare din care puteți alege. În timp ce plasați conținutul într-un diapozitiv, Designer operează în fundal, pentru a corela conținutul respectiv cu aspecte proiectate profesionist.

Datele de serviciu obligatorii care sunt trimise la Microsoft pentru a activa această experiență de mod conectat pentru dvs. ar putea include următoarele:

- *Conținut creat de utilizator*, cum ar fi text sau imagini pe care le-ați adăugat la diapozitiv.
- *Date funcționale*, cum ar fi diapozitivul la care lucrați și aspectul său.
- *Date de diagnosticare serviciu*, cum ar fi evenimentele care ne spun dacă ideea de proiectare a fost aplicată corect la diapozitiv și dacă apelurile de serviciu au fost efectuate corect.

## <a name="view-and-manage-required-service-data"></a>Vizualizarea și gestionarea datelor de serviciu obligatorii

Puteți vedea datele de diagnosticare a serviciului utilizând Vizualizatorul de date de diagnosticare. Pentru mai multe informații, consultați [Exemple de evenimente pentru datele de diagnosticare serviciu](#examples-of-events-for-service-diagnostic-data).

Vă oferim capacitatea de a alege tipurile de experiențe de mod conectat pe care doriți să le utilizați în Office, care determină apoi ce date de serviciu obligatorii sunt trimise către noi. PowerPoint Designer, de exemplu, este una dintre cele câteva experiențe de mod conectat care analizează conținutul. Dacă alegeți să dezactivați experiența de mod conectat care analizează conținutul, nu se trimit către noi date de serviciu obligatorii despre PowerPoint Designer, deoarece PowerPoint Designer nu va fi disponibil pentru utilizare.

De asemenea, datele de serviciu obligatorii sunt colectate și trimise la Microsoft pentru servicii esențiale Office, cum ar fi serviciul de licențiere care confirmă că sunteți corect licențiat pentru a utiliza Office. Aceste date pentru servicii esențiale sunt trimise indiferent de alte setări legate de confidențialitate pe care le-ați configurat.

Pentru mai multe informații, consultați următoarele:

- [Experiențe în mod conectat în Office](connected-experiences.md)
- [Servicii esențiale pentru Office](essential-services.md)
- [Utilizarea Vizualizatorului de date de diagnosticare cu Office](https://support.office.com/article/cf761ce9-d805-4c60-a339-4e07f3182855)

Dacă sunteți administratorul organizației dvs., ați putea fi interesat și de următoarele:

- [Prezentare generală a controalelor de confidențialitate pentru Office 365 ProPlus](overview-privacy-controls.md)
- [Utilizați setările de politică pentru a gestiona controale de confidențialitate pentru Office 365 ProPlus](manage-privacy-controls.md)
- [Utilizați preferințele pentru a gestiona controalele de confidențialitate ale Office pentru Mac](mac-privacy-preferences.md)
- [Utilizați preferințele pentru a gestiona controalele de confidențialitate ale Office pe dispozitivele iOS.](ios-privacy-preferences.md)

## <a name="examples-of-events-for-service-diagnostic-data"></a>Exemple de evenimente pentru datele de diagnosticare serviciu

Datele de diagnosticare de serviciu apar în Vizualizatorul de date de diagnosticare și sunt organizate în aceleași categorii care sunt utilizate pentru date de diagnosticare obligatorii și opționale. De exemplu, *Utilizare produse și servicii* sau *Performanță produse și servicii.*

Evenimentele pentru datele de diagnosticare de serviciu ne furnizează informațiile necesare efectuarea unei experiențe în mod conectat așa cum așteaptă un client. De exemplu, dacă serviciul utilizat de experiența în mod conectat a început cu succes și dacă a fost disponibil atunci când a fost necesar, dacă au existat erori sau alte probleme neprevăzute (căderi) la interacțiunea cu serviciul și capacitatea de răspuns sau performanța serviciul.

Următorul tabel oferă câteva exemple de evenimente pentru datele de diagnosticare de serviciu.

| **Nume**      | **Descriere**    |
| ---------- | --------------------- |
| Office.Excel.Coauth.SaveXrr     | Un eveniment declanșat în Excel, atunci când se utilizează serviciul de colaborare care raportează detalii despre revizuiri individuale care sunt scrise în jurnalul de revizuire. Acesta furnizează monitorizarea latenței și indică erorile din Excel care sunt legate de colaborare  |
| Office.Excel.Coauth.CloseWorkbook  | Un eveniment declanșat în Excel atunci când utilizați serviciul de colaborare care raportează când un registru de lucru este închis. Acest lucru este necesar în determinarea erorilor cu reîncărcarea și reîmprospătarea automată. Furnizează măsurători ale succesului pentru activitățile de serviciu de colaborare.   |
| Office.Security.OCX.NonTrustedEncounter    | Un eveniment declanșat în aplicațiile Office (inclusiv Word, Excel, Outlook, PowerPoint și Visio) atunci când un utilizator deschide un document care nu prezintă încredere și are un control ActiveX. Acesta este utilizat pentru a evalua pe larg utilizarea controalelor ActiveX încorporate în documente Office și a conduce diminuarea riscurilor de securitate ca răspuns la incidentele de securitate.  |
| Office.Security.UrlReputation.GetUrlReputation | Un eveniment declanșat în aplicațiile Office (inclusiv Word, Excel, PowerPoint, Visio și Publisher) care urmărește succesul sau eșecul apelurilor Linkuri sigure. Acesta este utilizat pentru a vă asigura că serviciul Linkuri sigure funcționează corect și pentru a diagnostica probleme.  |
| Office.Voice.VoiceManager.StreamingAudio   | Un eveniment declanșat în aplicațiile Office (inclusiv Word, Outlook și PowerPoint) care oferă informații despre starea de funcționare a redării în flux audio în serviciul de vorbire. Acesta conține informații despre dimensiunea audio redată în flux și despre erorile care pot apărea. Aceste informații sunt utilizate pentru a monitoriza starea de funcționare a serviciilor și pentru a diagnostica orice probleme care au fost raportate de clienți. |
