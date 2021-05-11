---
title: Administrere profiler og rollecentre
description: "Få at vide, hvordan du administrerer rollecentre i Dynamics NAV."
author: jswymer
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: profiles, roles, role centers, user roles
ms.date: 09/01/2017
ms.author: jswymer
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: a16640e014e157d4dbcaabc53d0df2d3e063f8f9
ms.openlocfilehash: a657c409c9cd361a505f1fd61dbb5254b25c5144
ms.contentlocale: da-dk
ms.lasthandoff: 10/26/2017

---
# <a name="managing-profiles-and-role-centers"></a>Administrere profiler og rollecentre
Profiler er samlinger af [!INCLUDE[navnow_md](includes/navnow_md.md)]-brugere, der deler det samme rollecenter. Et rollecenter er en sidetype, hvor du kan indsætte forskellige dele. Hver del er en beholder, hvor du kan være vært for andre sider eller foruddefinerede systemdele, f.eks. Outlook-del eller dele, som tilføjer opgaver, notifikationer eller noter.  

## <a name="about-profiles-and-role-centers"></a>Om profiler og rollecentre
Du kan bruge profiler til at kæde brugere sammen med foruddefinerede rollecentre. Et rollecenter er en hjemmeside for alle brugere af en profil, der er konfigureret, så den afspejler opgaverne og prioriteterne for brugerne af profilen. Ordrebehandler Rollecenter er f.eks. konfigureret til at afspejle en ordrebehandlers opgaver og prioriteter. Et rollecenter giver nem adgang til de oplysninger, som brugerne skal bruge for at udføre deres arbejde. Rollecenteret bestemmer f.eks. de køindikatorer, eller felter, der vises, når brugere logger på første gang, og links fra navigationssiden.

Den profil, der bruges, vises i overskriften i rollecentrets hovedindholdsområde. En administrator kan tilpasse dette rollecenter, så det opfylder behovene for en bestemt rolle i en bestemt virksomhed. Rollecenteret for ordrebehandling kan derefter tilpasses yderligere på en enkelt computer for at opfylde behovet hos en person, der udfører jobbet som en ordrebehandler. Denne person kan tilpasse rollecenteret ved at gemme forespørgsler, tilføje filtre, og tilføje eller fjerne felter.

Profiler og rollecentre svarer til rollerne og ansvarsområderne i organisationen. [!INCLUDE[navnow_md](includes/navnow_md.md)] indeholder et sæt standardprofiler, som hver svarer til og fungerer som et link til et rollecenter. Administratorer kan redigere eksisterende profiler eller oprette nye.  

> [!NOTE]  
>  Profiler er ikke direkte kædet sammen med de roller og tilladelser, som udgør sikkerhedssystemet, men profilbrugere skal have tilladelser, der justeres med deres roller i sikkerhedssystemet. Du kan finde flere oplysninger i [Sikkerhed i det rolledefinerede miljø](http://go.microsoft.com/fwlink?LinkId=147633) i MSDN-biblioteket.

## <a name="to-create-a-profile"></a>Sådan oprettes en profil
1.  Vælg ikonet ![Søg efter side eller rapport](media/ui-search/search_small.png "Ikonet Søg efter side eller rapport"), angiv **Profiler**, og vælg derefter det relaterede link.  

2.  Vælg handlingen **Ny** for at åbne vinduet **Nyt profilkort**.  

3.  I feltet **Profil-id** skal du angive et navn, der beskriver den tiltænkte rolle for brugeren.  

4.  Gå til feltet **Beskrivelse** , og angiv en beskrivelse af profil-id'et, f.eks. **Ordrebehandler**.  

5.  Angiv feltet **Rollecenter-id** for det rollecenter, der skal tildeles til profilen.  

6.  Hvis du vil gøre dette rollecenter til standardrollecenter for profilen, skal du vælge afkrydsningsfeltet **Standardrollecenter**.  

7.  Vælg knappen **OK**. .  

Proceduren for ændring af en eksisterende profil er den samme, bortset fra at du kan vælge en eksisterende profil på siden Profiler i stedet for at vælge handlingen **Ny**.  


##<a name="copying-a-profile"></a>Kopiere en profil
Kopiering af en profil kan spare tid, hvis du vil bruge samme indstillinger på en profil, og du kun vil ændre nogle få indstillinger.

1.  Åbn den profil, du vil kopiere, og vælg derefter handlingen **Kopier profil**.

2.  I feltet **Nyt profil-id** skal du indtaste et navn på den profil, du vil kopiere.

3.  Angiv feltet **Ny profils område** til et af følgende:

    - **System** for at gøre den nye profil tilgængelig for alle lejerdatabaser, der bruger programmet.
    - **Lejer** for at gøre den nye profil tilgængelig for kun den aktuelle lejerdatabase.
4. Tryk på knappen **OK**, når du er færdig.

## <a name="ExportImportProfile"></a>Eksportere og importere profiler

Du kan eksportere og importere profiler som XML-filer til og fra den en [!INCLUDE[d365fin](includes/d365fin_md.md)]-database. Eksport og import af en profil kan spare dig tid, når du konfigurerer brugergrænsefladen, fordi du kan genbruge en eksisterende profil i stedet at konfigurere en profil forfra. Hvis du har en profil, der er konfigureret i en [!INCLUDE[d365fin](includes/d365fin_md.md)]-database, og du vil genbruge alle eller nogle af de samme profilkonfigurationer i en anden database, kan du eksportere profilen til en XML-fil. Du kan derefter importere XML-filen med profilen til anden databasen.

-   Hvis du vil eksportere en profil, skal du søge efter og åbne siden **Udlæs profiler**, vælge profilen på listen og derefter vælge handlingen **Eksportér** handling. Gem XML-filen på en placering på computeren eller netværket.

-   Hvis du vil importere en profil, skal du søge efter og åbne siden **Indlæs profiler**, vælge XML-filen med profilen og derefter vælge knappen **OK**.

    > [!NOTE]  
    >  Du kan ikke importere en profil, der allerede findes i databasen, selvom XML-filen har et andet navn eller har et andet indhold. Før du kan importere den nye profil, skal du slette den eksisterende profil.



## <a name="see-also"></a>Se også  
[Fremgangsmåde: Administrere brugere og rettigheder](ui-how-users-permissions.md)  
[Tilpasse brugergrænsefladen](ui-customizing-overview.md)   
<!--[Security Overview](../Security%20Overview.md)-->

