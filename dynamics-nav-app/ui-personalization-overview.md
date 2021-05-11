---
title: "Tilpasse dit arbejdsområde - Oversigt"
description: "Få at vide, hvordan du kan tilpasse brugergrænsefladen, så den passer til din måde at arbejde på."
documentationcenter: 
author: jswymer
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.date: 07/26/2017
ms.author: jswymer
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 04334d3bb50b37b9643b848ca4f59b015f03ad04
ms.contentlocale: da-dk
ms.lasthandoff: 10/16/2017

---
# <a name="personalizing-your-workspace---overview"></a>Tilpasse dit arbejdsområde - Oversigt
Du kan *tilpasse*, dit arbejdsområde, så det passer til dit arbejde og dine præferencer ved at ændre sidernes layout, så de kun viser de oplysninger, du har brug for, hvor du har brug for det. De tilpasningsændringer, du foretager, påvirker kun det, du ser, ikke hvad andre brugere ser.

Du kan bruge dit arbejdsområde ved hjælp af [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] og [!INCLUDE[nav_web_md](includes/nav_web_md.md)]. De tilpasningsændringer, du foretager, kan også ses i [!INCLUDE[nav_phone_md](includes/nav_phone_md.md)] og [!INCLUDE[nav_web_md](includes/nav_phone_md.md)].
  
> [!NOTE]  
> Administratoren i din virksomhed har måske allerede tilpasset brugergrænsefladen til rollespecifikt layout for alle brugere, der har den samme profil som dig og bruger det samme rollecenter. Tilpasninger, du foretager i dit arbejdsområde, gemmes under din brugerkonto, så de bevares, også selvom en administrator ruller en ny række af rollespecifikke layouts ud i virksomheden. Du kan finde flere oplysninger i [Konfiguration af brugergrænsefladen](admin-configure-user-interface.md).

## <a name="comparing-personalization-in-the-dynamics-nav-windows-and-web-clients"></a>Sammenligne tilpasning i Dynamics NAV Windows- og webklienterne
Du kan tilpasse mange dele af brugergrænsefladen, afhængigt af siden, f.eks. hvilke felter eller kolonner der vises, og hvor de er placeret, hvilke handlinger der medtages på båndet osv. Mange af disse ting kan du gøre både i Windows-klienten og webklienten. Følgende tabel indeholder en oversigt over tilpasningsmuligheder i hver enkelt klient.

|  Tilpas  ||  Windows-klient  |  Webklient  |
|---------------|-|------------------|--------------|
|Felter i oversigtspaneler||||
||Tilføje, flytte og fjerne |x|x|
||Vis i skjult hoved|x||
||Skjul under handlingen **Vis flere felter**|x||
|Lister eller dokumentlinjer ||||
||Tilføje, flytte og fjerne kolonner  |x|x|
||Tilføje, flytte og fjerne låst rude  |x|x|
|Faktabokse|||
||Flytte og fjerne|x|x|
||Tilføj|x||
||Tilføje, flytte og fjerne felter|x|x|
|Køindikatorer||||
||Flytte og fjerne|x|x|
||Tilføj |x||
|Diagrammer||||
||Flytte og fjerne|x|x|
||Tilføj|x| |
|Båndet og handlinger||x||
|Navigationsrude||x||

En anden forskel er, at når der tilpasses ved hjælp af Windows-klienten, kan du få forskellige tilpassede versioner af den samme side, der er baseret på forskellige adgangspunkter til siden. Siden **Salgsordrer** kan f.eks. tilpasses, så den ser anderledes ud, når den åbnes fra siden **Debitorkort** i forhold til, hvordan den ser ud, når den åbnes fra rollecentret **Salgsordrebehandler**. Når du tilpasse en side ved hjælp af webklienten, er der kun én tilpasset version pr. side, så ændringerne vises på siden, uanset hvorfra du åbner den.

##  <a name="PersonalizationWinWeb"></a>Arbejde med tilpasning mellem Dynamics NAV Windows-og webklienten
Før du begynder at tilpasse sider, er det vigtigt at forstå, hvordan tilpasningen mellem Windows-klienten og webklienten fungerer. Hvis du altid kun bruger enten Windows-klienten eller webklienten, er disse oplysninger er ikke så relevante. Det bliver dog vigtigt, hvis du begynder at tilpasse sider ved brug af bruger begge klienter, eller når du overgår fra at bruge Windows-klienten til at bruge webklienten permanent.  

-   Hvis du bruger Windows-klienten til at tilpasse en bestemt side fra starten, vises ændringerne fra tilpasningen af siden også i [!INCLUDE[nav_web_md](includes/nav_web_md.md)].

-   Så længe du fortsætte med at bruge Windows-klienten til at tilpasse siden, vil alle de tilpasningsændringer, du foretager, også gælde på siden i webklienten.

-   Men så snart du begynder at tilpasse siden ved hjælp af webklienten, opdeles tilpasningen af den pågældende side mellem de to klienter, og du får en tilpasset version for hver klient. I webklienten fjernes de tidligere tilpasninger på siden, hvilket betyder, at siden vender tilbage til sit oprindelige layout, og du skal i alt væsentligt starte tilpasningen af siden fra bunden. De tidligere tilpasninger i Windows-klienten er uændrede.

- Fremover, skal du tilpasse siden i Windows- og webklienten uafhængigt af hinanden, hvilket medfører, at siden muligvis kan se forskellige i hver enkelt klient. Telefon- og tabletklienter viser de samme sidetilpasninger som webklienten.  

> [!Tip]  
>Hvis du åbner siden **Slet brugertilpasning**, kan du se alle de sider, der er blevet tilpasset af hver enkelt bruger. Kolonnen **Ældre tilpasning** giver dig en angivelse af, om tilpasningen blev udført i Windows-klienten eller webklienten. Hvis der er markeret i kolonnen, blev tilpasningen foretaget i Windows-klienten (eller i webklienten før [!INCLUDE[navnow_md](includes/navnow_md.md)]).

## <a name="see-also"></a>Se også
[Tilpasse dit arbejdsområde i Dynamics NAV Windows-klienten](ui-personalization-windows-client.md)  
[Tilpasse dit arbejdsområde i Dynamics NAV-webklienten](ui-personalization-user.md)  
[Administration af tilpasning](ui-personalization-manage.md)  
[Tilpasning Dynamics NAV](ui-customizing-overview.md)  

