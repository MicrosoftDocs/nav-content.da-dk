---
title: "Konfiguration af brugergrænsefladen for brugere"
description: "Som administrator kan du konfigurere virksomhedens standardbrugergrænseflader ved at tilpasse sidelayouts for forskellige brugerprofiler i virksomheden."
author: jswymer
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customize pages, configure user interface, customize UI
ms.date: 07/01/2017
ms.author: jswymer
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 7ba3d45a856eb38fe99fc5012b4e2f2d8609f9ce
ms.contentlocale: da-dk
ms.lasthandoff: 10/16/2017

---
# <a name="configuring-the-user-interface-ui-for-users"></a>Konfiguration af brugergrænsefladen for brugere
Som administrator kan du konfigurere virksomhedens standardbrugergrænseflader ved at tilpasse sidelayouts for forskellige brugerprofiler i virksomheden. Du skal være administrator med SUPER-tilladelsessættet for at udføre dette arbejde. Desuden skal profiler oprettes, og de relevante brugere skal tildeles dem. Du kan finde flere oplysninger i [Administrere brugere, profiler og rollecentre](admin-users-profiles-roles.md).  
  
Du kan konfigurere brugergrænsefladen for flere brugere ved at tilpasse sider til en bestemt profil, der er tildelt brugere. Det gøres ved hjælp af [!INCLUDE[nav_windows](includes/nav_windows_md.md)], og tilpasningen sker på samme måde, som når individuelle brugere tilpasser deres egne arbejdsområder, dvs. ved hjælp af funktionen **Tilpas**. Forskellen er, at du åbner [!INCLUDE[nav_windows](includes/nav_windows_md.md)] i konfigurationstilstanden. Typiske tilpasninger omfatter, hvilke handlinger der skal medtages på båndet, hvordan felter skal placeres i oversigtspaneler eller faktabokse, og hvilke menupunkter der skal medtages i navigationsruden. 

> [!TIP]  
>  Du kan hurtigt implementere brugergrænsefladekonfigurationer for en profil, hvis du allerede har en konfigureret profil i en anden [!INCLUDE[d365fin](includes/d365fin_md.md)]-database. Du kan derefter eksportere profilen og så importere den til den aktuelle database. Du kan finde flere oplysninger i [Eksporte og importere profiler](admin-profiles.md#ExportImportProfile).  
  
## <a name="general-information"></a>Generelle oplysninger
Overvej følgende oplysninger, før du begynder at konfigurere Brugergrænsefladen:
-   Før du begynder at konfigurere brugergrænsefladen, kan programmet konfigureres til at vise og skjule elementer i brugergrænsefladen (f.eks. felter, oversigtspaneler og faktabokse) baseret på licens eller brugertilladelser. Du kan finde flere oplysninger om, hvordan du gør dette, i [Fjernelse af elementer fra brugergrænsefladen i overensstemmelse med tilladelser](https://msdn.microsoft.com/en-us/dynamics-nav/removing-elements-from-the-user-interface-according-to-permissions).

    Hvis du vil se effekten af indstillingen Fjernelse af brugergrænsefladeelementer, kan du logge på som testbruger med tilladelsessættet for den profil, du konfigurerer. Årsagen er, at du som administrator har SUPER-tilladelsessættet, og at du derfor ikke kan se og teste den resulterende brugergrænseflade under dit eget logon.    
-   Når du opretter ændringer af brugergrænsefladen for en side, som en bruger har tilpasset, bevares brugerens tilpasning af brugergrænsefladen, og den overskrives ikke med den nye sidekonfiguration. Når du annullerer konfigurationen af brugergrænsefladen på en side, som en bruger efterfølgende har tilpasset, annulleres brugerens tilpasning af brugergrænsefladen heller ikke.
-   Den eneste situation, hvor konfigurationen af brugergrænsefladen overskriver tilpasningen af brugergrænsefladen er, når et element fjernes af konfiguration. Hvis administratoren f.eks. fjerner et felt, som brugeren har omdøbt eller flyttet, fjernes dette felt stadig fra brugerens brugergrænseflade.
-   Du kan registrere brugergrænsefladekonfigurationer af den samme side baseret på forskellige adgangspunkter til siden. Vinduet **Salgsordrer** kan f.eks. tilpasses, så det ser anderledes ud, når det åbnes fra vinduet **Debitorkort** i forhold til, hvordan det ser ud, når det åbnes fra rollecentret **Salgsordrebehandler**. Det punkt, hvorfra du får adgang til den side, der skal tilpasses, er registreret i denne specifikke sidetilpasning. Derfor kan der være flere sidetilpasningsposter i databasen, som du kan se i vinduet **Slet profilkonfiguration**.  
-   I modsætning til når brugerne ændrer størrelsen af vinduer eller bredden af kolonner på deres egen computer, gemmes sådanne grundlæggende visningsændringer, du foretager under konfigurationen af brugergrænsefladen for en profil, ikke i profilen og vil ikke være tilgængelige for brugere, der er tildelt profilen. Grundlæggende visningsændringer er computerspecifikke.   

## <a name="configure-a-profile-with-the-includenavwindowsincludesnavwindowsmdmd-in-configuration-mode"></a>Konfigurere en profil med [!INCLUDE[nav_windows](includes/nav_windows_md.md)] i konfigurationstilstand
1.  Åbn en kommandoprompt, og skriv følgende kommando for at skifte til installationsmappen for [!INCLUDE[nav_windows](includes/nav_windows_md.md)]. Eksempler:  
  
    ```  
    cd C:\Program Files\(x86)\Microsoft Dynamics NAV\110\RoleTailored Client  
    ```  
  
2.  Skriv følgende kommando for at starte [!INCLUDE[nav_windows](includes/nav_windows_md.md)] i konfigurationstilstand for en bestemt profil:  
  
    ```  
    Microsoft.Dynamics.Nav.Client.exe -configure -profile:"profileid"  
    ```  
  
     Erstat **profileid** med navnet på den profil, du vil konfigurere.  
  
     Hvis du f.eks. vil konfigurere profilen Regnskabschef, skal du bruge følgende kommando:  
  
    ```  
    Microsoft.Dynamics.Nav.Client.exe -configure -profile:"Accounting Manager"  
    ``` 

3. Du er nu klar til at starte konfiguration af brugergrænsefladen på samme måde, som individuelle brugere tilpasser deres egne arbejdsområder. Du kan finde flere oplysninger under [Tilpasse dit arbejdsområde i [!INCLUDE[nav_windows](includes/nav_windows_md.md)]](ui-personalization-windows-client.md). 

## <a name="cancel-ui-configuration"></a>Annullere konfigurationen af brugergrænseflade
Du kan annullere tilpasninger af brugergrænsefladen, du har foretaget som konfiguration for en profil, på tre måder:  
  
-   Annuller alle tilpasninger af brugergrænsefladen, du har foretaget til en profil, ved hjælp af knappen **Fjern konfigurerede sider** i vinduet **Profilkort**.  
  
-   Annuller tilpasninger af brugergrænsefladen, du har foretaget for bestemte sider for en profil, ved at slette rækker i vinduet **Slet profilkonfiguration**.  
  
-   Annuller tilpasninger af brugergrænsefladen, du har foretaget i et bestemt område af brugergrænsefladen for en bestemt side for en profil, ved hjælp af knappen **Gendan standardindstillinger** i vinduet **Tilpas**.  
  
### <a name="general-information"></a>Generelle oplysninger  
-   Brugere kan foretage tilpasninger af brugergrænsefladen under deres egne brugerlogon for at tilpasse deres brugergrænseflade. Når du annullerer konfigurationen af brugergrænsefladen, som en bruger efterfølgende har tilpasset, annulleres brugerens tilpasning af brugergrænsefladen ikke. Når du opretter en ny konfiguration af brugergrænsefladen for en side, som en bruger har tilpasset, bevares brugerens tilpasning af brugergrænsefladen og overskrives ikke med den nye sidekonfiguration.  

    Den eneste situation, hvor konfigurationen af brugergrænsefladen overskriver tilpasningen af brugergrænsefladen er, når et element fjernes af konfiguration. Hvis administratoren f.eks. fjerner et felt, som brugeren har omdøbt eller flyttet, fjernes dette felt stadig fra brugerens brugergrænseflade.  
  
-   I vinduet **Slet brugertilpasning** og med knappen **Gendan standarder** i vinduet **Tilpas** kan brugere annullere tilpasning af brugergrænsefladen, de har foretaget på sider under deres eget brugerlogon. Når de gør det, nulstilles layoutet for disse sider til en tilpasning af brugergrænsefladen, som administratoren har konfigureret for profilen. Hvis profilen ikke er konfigureret, kan layoutet af brugerens sider nulstilles til standardprofilkonfigurationen. Du kan finde flere oplysninger om, hvordan brugere annullere tilpasning, i [Annullere tilpasning](ui-personalization-windows-client.md#CancelPersonalization).
  
### <a name="to-cancel-all-ui-customization-that-you-have-made-for-a-profile"></a>Sådan annulleres alle tilpasninger af brugergrænsefladen, du har foretaget for en profil  
  
1.  I feltet **Søg** skal du angive **Profiler** og derefter vælge det relaterede link.  
  
2.  Vælg profilen, hvor du vil annullere alle tilpasninger af brugergrænsefladen, og vælg derefter **Rediger** i gruppen **Administrer** under fanen **Startside**.  
  
3.  I vinduet **Profilkort** under fanen **Handlinger** i gruppen **Funktioner** skal du vælge **Fjern konfigurerede sider**.  
  
> [!NOTE]  
>  Alle tilpasninger af brugergrænsefladen for profilen, både dem, der er installeret sammen med programmet, og dem, der er foretaget af administratoren, annulleres. Ingen sidelayout, der er specifikke for profilen, forbliver i databasen.  
  
### <a name="to-cancel-ui-customization-that-you-have-made-for-specific-page-for-a-profile"></a>Sådan annulleres tilpasninger af brugergrænsefladen, du har foretaget for en bestemt side for en profil  
  
1.  I feltet **Søg** skal du indtaste **Slet profilkonfiguration** og derefter vælge det relaterede link.  
  
2.  Vælg det profil-/sidesæt, hvor du vil annullere din tilpasning af brugergrænsefladen, og vælg derefter **Slet** i gruppen **Administrer** under fanen **Startside**.  
  
    > [!IMPORTANT]  
    >  Hvis du har konfigureret forskellige tilpasninger af brugergrænsefladen af den samme side, der er baseret på forskellige navigationsstier til siden, så hver enkelt sidetilpasning vil blive vist i vinduet **Slet profilkonfiguration** med de samme oplysninger. Der er ingen oplysninger, der kan identificere, hvilken række der er relateret til hvilken navigationssti. Derfor skal du enten slette rækker én efter én efterfulgt af visuel kontrol på siden, eller du kan slette alle rækker med tilpasninger af brugergrænsefladen for profilen/siden.
    >    
    >  Al tilpasning af brugergrænsefladen for siden til profilen, du nogensinde har foretaget ved installationen, eller siden du sidst brugte vinduet **Slet profilkonfiguration**, annulleres. Layoutet af siden nulstilles til standardlayoutet for sideobjektet.  
  
### <a name="to-cancel-ui-customization-that-you-have-made-for-a-specific-ui-area-for-a-specific-page-for-a-profile"></a>Sådan annulleres tilpasninger af brugergrænsefladen, du har foretaget i et bestemt område af brugergrænsefladen for en bestemt side for en profil  
  
Du kan fortryde ændringer, du har foretaget i individuelle brugergrænseflade-områder, f.eks. et bånd, ved hjælp af knappen **Gendan standardindstillinger** i vinduet **Tilpas**. Alternativt kan du fortryde alle ændringer af brugergrænsefladen, du har foretaget for en profil, ved hjælp af vinduet **Slet profilkonfiguration**.  
  
Tilpasningen af brugergrænsefladen for profilen i et bestemt brugergrænsefladeområde på den pågældende side er annulleret. Layoutet af brugergrænsefladeområdet på siden nulstilles til standardkonfigurationen, som er konfigureret af administratoren eller installeret sammen med programmet.  
  
## <a name="see-also"></a>Se også  
[Tilpasning [!INCLUDE[navnow_md](includes/navnow_md.md)]](ui-customizing-overview.md)   
