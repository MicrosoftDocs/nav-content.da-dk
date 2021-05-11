---
title: Tilpasse sider i Dynamics Windows-klient
description: "Få at vide, hvordan du kan tilpasse brugergrænsefladen, så den passer til din måde at arbejde på."
author: jswymer
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 07/26/2017
ms.author: jswymer
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: e22f3464c6a4dd917880ad0b903880fe5f57a37d
ms.contentlocale: da-dk
ms.lasthandoff: 10/23/2017

---
# <a name="personalizing-your-workspace-in-the-dynamics-windows-client"></a>Tilpasse dit arbejdsområde i Dynamics Windows-klienten
Du kan tilpasse, dit arbejdsområde, så det passer til dit arbejde og dine præferencer ved at ændre sidernes layout, så de kun viser de oplysninger, du har brug for, hvor du har brug for det. De tilpasningsændringer, du foretager, påvirker kun det, du ser, ikke hvad andre brugere ser. Du kan tilpasse mange dele af brugergrænsefladen, herunder hvilke handlinger der skal medtages på båndet, hvordan felterne skal placeres i oversigtspaneler eller i faktabokse, og hvilke menupunkter der skal medtages i navigationsruden.

> [!NOTE]  
> Du kan også tilpasse sider ved hjælp af [!INCLUDE[nav_web_md](includes/nav_web_md.md)]. Få at vide, hvordan tilpasning fungerer mellem to klienter, under [Oversigt over tilpasning](ui-personalization-overview.md).

## <a name="how-to-personalize-your-workspace"></a>Fremgangsmåde: Tilpasse dit arbejdsområde
Du kan udføre det mest af tilpasningen ved hjælp af funktionen **Tilpas**, som du kan åbne fra praktisk talt alle typer af sider ved at gøre følgende:

1.  Åbn den side, du vil tilpasse.
2.  I øverste venstre hjørne skal du vælge menuikonet **Program** ![Knappen Programmenu på menulinjen](media/applicationmenuicon.png "ApplicationMenuIcon"), vælge **Tilpas** og derefter vælge en af tilpasningsmulighederne.

Desuden er der nogle grundlæggende ændringer af brugergrænsefladen, f.eks. justering af størrelsen på et vindue eller udvidelse af bredden på kolonner, som du kan foretage direkte på siden uden for indstillingen **Tilpas**.

## <a name="general-information"></a>Generelle oplysninger
Under tilpasning af brugergrænsefladen, er det en god ide at huske følgende ting:

-   Du kan registrere flere tilpasninger af den samme side baseret på forskellige adgangspunkter til siden. Vinduet Salgsordrer kan f.eks. tilpasses, så det ser anderledes ud, når det åbnes fra vinduet Debitorkort i forhold til, hvordan det ser ud, når det åbnes fra rollecentret Salgsordrebehandler. Det punkt, hvorfra du får adgang til den side, der skal tilpasses, er registreret i denne specifikke sidetilpasning. Derfor kan der være flere sidetilpasningsposter i databasen, som du kan se i vinduet **Slet brugertilpasning**.

-   Programmet kan konfigureres til at vise og skjule elementer i brugergrænsefladen (f.eks. felter, oversigtspaneler og faktabokse) baseret på licens eller brugertilladelser. Du kan kun få vist og tilpasse elementfelter, du har tilladelse til.

## <a name="customize-ribbons"></a>Tilpasse bånd
Båndet giver dig adgang til flere handlinger. Når du tilpasser båndet, kan du optimere det til dine arbejdsgange og præferencer. Hvis du f.eks. ofte bruger vinduet **Dimensioner**, kan du tilføje handlingen **Dimensioner** til handlingsgruppen **Proces**. Du kan også fjerne handlinger, du aldrig bruger, så du får et bedre overblik.  

Du kan udføre følgende opgaver for at tilpasse bånd på sider:  

-   Tilføje, omdøbe eller fjerne faner, grupper, handlinger og menuer.  
-   Ændre rækkefølgen af handlinger.  
-   Gendanne båndets standardindstilling.  

### <a name="to-customize-a-ribbon"></a>Sådan tilpasses et bånd
1. Åbn den side, du vil ændre.
2. I øverste venstre hjørne skal du vælge menuikonet **Program** ![Programmenuknap på menulinjer](media/applicationmenuicon.png "Programmenuikon") vælge **Tilpas** og derefter vælge **Tilpas bånd**.

Dialogboksen **Organiser handlinger på båndet** opdeles i to ruder. Ruden **Tilgængelige handlinger** viser alle de handlinger, kan du føje til siden. Ruden **Vis handlinger i denne rækkefølge** viser strukturen af de handlinger, der aktuelt vises på siden.

-   Elementer på rodniveau definere faner.

    -   Elementer på andet niveau definerer en gruppe under en fane.

        -   Elementer på tredje niveau definerer en menu over handlinger i en gruppe

### <a name="add-a-group"></a>Tilføje gruppe
Vælg den fane, under hvilken du vil have gruppen, og vælg derefter **Opret gruppe**. Du kan ikke tilføje en gruppe under en menu.

### <a name="add-a-menu"></a>Tilføje en menu
Vælg den gruppe, under hvilken du vil have menuen, og vælg derefter **Opret menu**. Du kan kun tilføje en menu til en gruppe eller en anden menu.

#### <a name="add-an-action"></a>Tilføje en handling
Vælg den i ruden **Tilgængelige handlinger**, vælg **Tilføj** for at føje den til ruden **Vis handlinger i denne rækkefølge**, og brug derefter knapperne **Flyt op** og **Flyt ned** til at placere den, hvor du ønsker det.

Du kan ikke tilføje en handling til en fane, kun til en gruppe eller en menu.

###  <a name="limitations-and-recommendations"></a>Begrænsninger og anbefalinger
Vær opmærksom på følgende begrænsninger, når du tilpasser båndet:  

-   Systemfaner eller -grupper, f.eks. **Start** og **Ny** kan ikke flyttes eller omdøbes. Placeringen af nogle grupper, f.eks **Nyt bilag**, ligger fast.  
-   Handlinger eller grupper, der har dynamisk synlighed, kan ikke tilføjes eller fjernes.
-   Du kan kun oprette menuer inden i grupper, ikke i faner.  
-   Du kan indlejre en menu i en anden menu, men det anbefales ikke.  
-   Hvis du oplever uventet adfærd med grupper og handlinger efter at have tilpasset båndet, skal du gøre følgende:  

    1.  Tom, men slet ikke gruppen, hvor problemet forekommer.  
    2.  Luk dialogboksen ved hjælp af knappen **OK**.  
    3.  Åbn dialogboksen igen, og føj handlingerne til gruppen igen.  

> [!IMPORTANT]  
>  Eventuelle tilpasninger, der ændrer båndet, kan påvirke vejledningen i Hjælp til [!INCLUDE[navnow_md](includes/navnow_md.md)], fordi navigationstrin i Hjælp kan henvise til et andet båndlayout.

## <a name="customize-fasttabs"></a>Tilpasse oversigtspaneler
Oversigtspaneler hjælper med at organisere oplysninger om sider i enkle håndterbare grupper. Du kan tilpasse oversigtspaneler på sider, så de understøtter din arbejdsproces. Du vil måske vise færre oversigtspaneler eller skjule bestemte felter på oversigtspaneler. Du kan også overføre de vigtigste felter, så de medtages i oversigtspanelernes hoved, når oversigtspanelerne er skjult.  

### <a name="to-customize-a-fasttab"></a>Sådan tilpasses et oversigtspanel  

1.  Åbn den side, du vil ændre.
2.  Vælg menuikonet **Program** ![Programmenuknap på menulinjer](media/applicationmenuicon.png "Programmenuikon"), vælg **Tilpas**, og vælg derefter **Tilpas bånd**.  
3.  I dialogboksen **Tilpas <Page Name>** skal du vælge **Oversigtspaneler**.  

### <a name="add-move-or-remove-fasttabs"></a>Tilføje, flytte og fjerne oversigtspaneler
Feltet **Vis oversigtspaneler i denne rækkefølge** indeholder de oversigtspaneler, der i øjeblikket er på siden, og den rækkefølge, som de vises i. Brug knapperne **Tilføj**, **Fjern** og **Flyt op** og **Flyt ned** for at foretage ændringer.

### <a name="show-and-hide-fields-on-fasttabs"></a>Vise og skjule felter i oversigtspaneler
Marker det oversigtspanel, du vil ændre, i feltet **Vis oversigtspaneler i denne rækkefølge**, og vælg derefter **Tilpas oversigtspanel**. Brug knapperne til at tilpasse de felter, du vil have vist og deres rækkefølge på siden.

Angiv **Vigtighed** på følgende måde:
-   Hvis du vil have vist feltet i overskriften til oversigtspanelet, når oversigtspanelet er skjult, skal du angive det til **Forfremmet**.
- Hvis du vil feltet til at være skjult, medmindre brugeren vælger handlingen **Vis flere felter** på oversigtspanelet, skal du angive det til **Flere**.
-   **Standard** er standarden eller den normale indstilling.

### <a name="set-up-field-for-quick-entry"></a>Angive felt som genvej
Vælg afkrydsningsfeltet **Genvej** for at føje feltet til feltlisten Genvej. Når du arbejder på siden og trykker på Enter i et felt, springer markøren til næste felt, der er angivet til at være af typen Genvej.

## <a name="customize-factboxes"></a>Tilpasse faktabokse
Du kan bruge faktabokse til at få vist oplysninger med relation til den post, som du har markeret på listen eller har åbnet på en opgaveside. Du kan vælge, hvilke faktabokse der skal vises i faktaboksruden. Du kan også tilpasse faktaboksene, så kun de felter, du har brug for, vises.  

### <a name="to-show-or-hide-the-factbox-pane"></a>Vise eller skjule faktaboksruden
Faktabokse er indeholdt i ruden Faktaboks, som du kan vælge at vise eller skjule på sidebasis. Dette gør det muligt let at skjule flere faktabokse uden at skulle fjerne dem enkeltvist.

1.  Åbn den side, du vil ændre.
2.  Vælg menuikonet **Program** ![Programmenuknap på menulinjer](media/applicationmenuicon.png "Programmenuikon"), vælg **Tilpas**, og vælg derefter **Faktabokse**. Hvis afkrydsningsfeltet er markeret, betyder det, at ruden Faktaboks vises.  

### <a name="to-customize-the-factbox-pane"></a>Sådan tilpasses ruden Faktaboks  
1.  Åbn den side, du vil ændre.
2.  Vælg menuikonet **Program** ![Programmenuknap på menulinjer](media/applicationmenuicon.png "Programmenuikon"), vælg **Tilpas**, og vælg derefter **Vælg faktabokse**.  

### <a name="add-a-factbox"></a>Tilføje en faktaboks  

Vælg den faktaboks, du vil føje til ruden Faktaboks, i feltet **Tilgængelige faktabokse**, og vælg derefter knappen **Tilføj**.  

### <a name="remove-a-factbox"></a>Fjerne en faktaboks  

I feltet **Vis faktabokse i denne rækkefølge** skal du vælge faktaboksen og derefter knappen **Fjern**.   

### <a name="change-the-order-of-the-factboxes"></a>Ændre faktaboksenes rækkefølge  

Vælg den faktaboks, du vil flytte, i feltet **Vis faktabokse i denne rækkefølge**, og klik derefter på knapperne **Flyt op** eller **Flyt ned**, indtil faktaboksen er på det ønskede sted.  

### <a name="change-the-fields-in-a-factbox"></a>Ændre felterne i en faktaboks  

1.  I feltet **Vis faktabokse i denne rækkefølge** skal du vælge faktaboksen og derefter knappen **Tilpas del**.  

2.   Feltet **Tilgængelige felter** viser en ovesigt alle de felter, du kan vælge mellem. Feltet **Viste felter** viser alle de felter, der aktuelt vises i faktaboksen. Brug knapperne til at tilføje, fjerne og flytte felterne.   


## <a name="customize-columns-in-a-list-or-on-document-lines"></a>Tilpasse kolonner på en liste eller på dokumentlinjer
For at få et bedre overblik over de oplysninger, du skal bruge, kan du tilpasse oversigtssider og kortsider ved at tilføje eller fjerne kolonner i gitrene, omarrangere kolonner og tilføje en låst rude.  

### <a name="to-add-remove-and-arrange-columns"></a>Sådan tilføjer, fjerner og arrangerer du kolonner  

1.  Du kan tilføje, fjerne eller omarrangere kolonner på to måder:

    -   Vælg menuikonet **Program** ![Programmenuknap på menulinjer](media/applicationmenuicon.png "Programmenuikon"), vælg **Tilpas**, og vælg derefter **Vælg kolonner**.
    -   Højreklik på en kolonneoverskrift, og vælg **Vælg kolonner**.

2.  I dialogboksen **Vælg, hvilke kolonner der skal vises på listen** indeholder ruden **Tilgængelige kolonner** de kolonner, der er skjult. Ruden **Vis kolonner i denne rækkefølge** indeholder kolonner, der vises. Brug knapperne **Tilføj** og **fjern** til at flytte kolonner fra et felt til det andet. Brug knapperne **Flyt op** og **Flyt ned** til at placere kolonnerne.

>[!TIP]
>Vælg afkrydsningsfeltet **Genvej** for at føje feltet til feltlisten Genvej. Når du arbejder på siden og trykker på Enter i et felt, springer markøren til næste felt, der er angivet til at være af typen Genvej.

### <a name="to-set-the-freeze-pane"></a>Sådan angives den låste rude
En liste kan have mange kolonner, og det kan tvinge brugerne til at rulle vandret for at få vist alle kolonner. Der kan være nogle kolonner, du altid ønsker at få vist, selv når du ruller. For at opnå dette kan du tilføje en lodret låst rude for at begrænse visse kolonner fra rulning. Det giver dig mulighed at sikre, at kun de mindre vigtige kolonner flyttes, når du ruller.

For at angive den fastlåste rude skal du vælge den kolonne, hvorefter den fastlåste rude skal starte, og derefter vælge **Tilføj låst rude**.

## <a name="customizing-the-navigation-pane"></a>Tilpasse navigationsruden
Navigationsruden viser en menu med links til forskellige oversigtssider. Disse links er grupperet under knapper for rodniveau.

### <a name="to-customize-the-navigation-pane"></a>Sådan tilpasses navigationsruden  

Vælg menuikonet **Program** ![Programmenuknap på menulinjer](media/applicationmenuicon.png "Programmenuikon"), vælg **Tilpas**, og vælg derefter **Tilpas navigationsrude**.  

### <a name="rename-or-rearrange-buttons-in-the-navigation-pane"></a>Omdøbe eller flytte knapper i navigationsruden  
Marker den knap, du vil flytte, omdøbe eller fjerne, i den venstre rude i dialogboksen **Tilpas navigationsrude**, og vælg derefter den relevante knap i midten af vinduet.

Du kan ikke flytte, omdøbe eller fjerne knappen **Start**. Knappen **Afdelinger** kan fjernes fra navigationsruden, men ikke omdøbes eller flyttes.

### <a name="add-a-new-menu-button"></a>Tilføje en ny menuknap
Du kan oprette en ny rodniveauknap og derefter tilføje en menu med links til at åbne forskellige sider under knappen.

1. I dialogboksen **Tilpas navigationsrude** skal du vælge **Ny** og derefter skrive et navn i feltet **Navn**.
2.  Vælg knappen **OK**.

Du kan tilføje links til knappen.  

### <a name="add-a-link-to-a-button"></a>Tilføje et link til en knap   
Hvis du har rettighed til at få vist en liste, f.eks. salgsordrelisten, kan du tilføje et link til listen fra en knap i navigationsruden.  

1.  Marker den menu, du vil tilføje hyperlinket til, i feltet **Navigationsrudeknapper** i dialogboksen **Tilpas navigationsrude**.  

2.  Vælg knappen **Tilføj**.  

3.  Gå til det hyperlink, du tilføje, og vælg derefter knappen **OK**.  
> [!TIP]
> Hvis du finder et hyperlink på siderne **Afdelinger**, kan du også tilføje det til navigationsruden. Du kan finde flere oplysninger under afsnittet Tilføje et hyperlink fra afdelinger til rollecenteret.  

### <a name="move-or-copy-a-link-from-one-button-to-another"></a>Flytte eller kopiere et link fra én menu til en anden  

1.  Marker den menu, hvor hyperlinket vises aktuelt, i feltet **Navigationsrudeknapper** i dialogboksen **Tilpas navigationsrude**.  

2.  Marker det hyperlink, du vil flytte, i ruden **Lister**, og vælg derefter **Flyt til** eller **Kopier til**  

3.  Markér den navigationsknap, du vil tilføje linket til, og vælg derefter knappen **OK**.  

### <a name="rearrange-the-order-of-a-links-under-a-button"></a>Ændre rækkefølgen af links under en knap  

1.  Marker det hyperlink, du vil flytte, i ruden **Lister**.  

2.  Brug knapperne **Flyt op** og **Flyt ned** til at placere hyperlinket.

## <a name="adding-department-links-to-the-role-center"></a>Tilføje afdelingslinks til rollecenteret
Nogle gange kan du finde et link på en side af typen **Afdelinger**, som du gerne vil føje til rollecenteret for at give let adgang. Hvor du kan placere linket i rollecenteret afhænger af kategorien af linket på siden **Afdelinger**.

I følgende tabel beskrives de typer hyperlinks, der findes i hver kategori på siderne af typen **Afdelinger**, og hvor i rollecenteret du kan tilføje dem.  

|**Kategori**|**Indeholder**|**Tilføj hyperlink til**|  
|------------------|------------------|---------------------|  
|Lister|Listesider|Knappen **Startside** i navigationsrude|  
|Opgaver|Opgavesider, kørsler, kladder|Fanen **Handlinger** på båndet|  
|Rapporter og analyse|Rapporter, kørsler, matrixvinduer|Fanen **Rapporter** på båndet|  
|Dokumenter|Bilag som f.eks. fakturaer og rykkere|**Rapporter** på båndet|  
|Arkiver/historik|Bogførte/færdige bilag, registre|Knappen **Startside** i navigationsrude|  
|Opsætning|Opsætningsvinduer|Fanen **Handlinger** på båndet|  

### <a name="to-copy-department-links-to-your-role-center"></a>Sådan kopieres afdelingslinks til dit rollecenter  

1.  Åbn siden **Afdelinger**.  

2.  Højreklik på linket, og vælg derefter på én af følgende muligheder (kun én af disse muligheder er tilgængelig).  

    |**Vælg**|**Sådan tilføjes hyperlinket til**|  
    |----------------|----------------------------|  
    |**Føj til navigationsrude**|Knappen **Startside** i navigationsruden i rollecenteret.|  
    |**Tilføj til handlinger på båndet Rollecenter**|Menuen **Handlinger** på båndet i Rollecenter|  
    |**Tilføj til rapporter på båndet Rollecenter**|Menuen **Rapporter** på båndet i Rollecenter|  

3.  Bekræft den meddelelse, der vises.  

 Det nye hyperlink vises nu i den menu, du har føjet den til. Men du skal evt. flytte hyperlinket til et andet sted i menuen. Hvis du f.eks. har føjet et hyperlink til navigationsruden, vises den i menuen **Hjem**, men du kan flytte den til en anden menu i navigationsruden. Du kan finde flere oplysninger i afsnittet Tilpasse navigationsruden.

## <a name="adding-charts-to-role-centers-and-list-pages"></a>Tilføje diagrammer til rollecentre og listesider
Når du har komplekse oplysninger, kan du få vist en visuel repræsentation af dataene for at se tendenser og træffe beslutninger. Du kan f.eks. overvåge saldi pr. bankkonto for din virksomhed i et diagram. Du kan bruge diagramruden til visuelt at vise data fra en liste på følgende typer af sider:  

-   I dit rollecenter, hvor du kan vælge mellem foruddefinerede generiske diagrammer.  

-   På en listeside, hvor du kan vælge at få vist en liste som et diagram.  

### <a name="to-add-a-generic-chart-to-your-role-center"></a>Sådan føjes et generisk diagram til dit rollecenter  

1.  I rollecenteret skal du vælge menuikonet **Program** ![Programmenuknap på menulinjer](media/applicationmenuicon.png "Programmenuikon"), vælge **Tilpas** og derefter **Tilpas denne side**.  

2.  I feltet **Tilgængelige dele** i vinduet **Tilpas Rollecenter** skal du vælge **Diagramdel** og derefter vælge **Tilføj**.  

3.  Brug knapperne **Flyt op**, **Flyt ned**, **Flyt til venstre** og **Flyt til højre** til at placere diagramdelen på Rollecenter.  

4.  Markér diagramdelen, vælg **Tilpas del**.  

5.  I vinduet **Tilpas diagram** skal du vælge det foruddefinerede diagram, som du vil have vist, og derefter vælge **OK**.  

### <a name="to-view-a-list-as-a-chart"></a>Sådan vises en liste som et diagram  

1.  På listesiden skal du vælge handlingen **Vis som diagram**.  

2.  Vælg et mål og en dimension for at oprette et brugerdefineret diagram. Vælg en sekundær dimension, hvis du vil se yderligere oplysninger. Du kan f.eks. oprette et simpelt søjlediagram, vælge en dimension på x-aksen, og derefter vælge dimensionen **Antal dimensioner** på y-aksen.  

> [!NOTE]  
>  Diagramruden er som standard skjult, da den kan nedsætte ydeevnen. Du bør kun vise diagrammet, når du skal have oplysninger.  

## <a name="handling-external-files-and-automation-objects"></a>Håndtere eksterne filer og automatiseringsobjekter
Når [!INCLUDE[navnow_md](includes/navnow_md.md)] modtager en ekstern fil, får du vist en dialogboks. Udover at vælge, hvad der skal gøres med filen, kan du beslutte, hvordan denne filtype skal behandles, næste gang den er modtaget.  

Når [!INCLUDE[navnow_md](includes/navnow_md.md)] er påkrævet for at køre et automatiseringsobjekt, får du vist en dialogboks. Du kan bestemme, om denne type objekt altid eller aldrig skal kunne køre.  

### <a name="to-specify-how-to-handle-external-files"></a>Sådan angives det, hvordan du håndterer eksterne filer  

1.  Når du får vist dialogboksen, skal du fjerne markeringen i afkrydsningsfeltet **Spørg altid, før denne filtype åbnes**, hvis du vil have [!INCLUDE[navnow_md](includes/navnow_md.md)] til at huske, hvad du har valgt i trin 2. Næste gang denne type fil skal behandles, vises dialogboksen ikke, og filen behandles som beskrevet i trin 2.  

     Alternativt kan du markere afkrydsningsfeltet **Spørg altid, før denne filtype åbnes** for altid at få vist dialogboksen, når denne filtype modtages.  

2.  Vælg **Åbn**, **Gem** eller **Annuller**. Filen behandles ud fra dit valg.  

### <a name="to-specify-how-to-handle-automation-objects"></a>Sådan angives det, hvordan du håndterer automatiseringsobjekter  

Når du får vist dialogboksen, skal du markere afkrydsningsfeltet **Tillad altid**, hvis du ønsker, at [!INCLUDE[navnow_md](includes/navnow_md.md)] altid skal køre denne type automatiseringsobjekt. Næste gang denne type automatiseringsobjekt skal køres, vises dialogboksen ikke, og automatiseringsobjektet køres direkte.  

Alternativt kan du markere afkrydsningsfeltet **Tillad aldrig**. Næste gang denne type automatiseringsobjekt skal køres, vises dialogboksen ikke, og automatiseringsobjektet kører ikke.  

## <a name="CancelPersonalization"></a>Annullere tilpasning
Annullering af tilpasning kan opdeles i to kategorier:

-   Annullering af ændringer, du har foretaget ved hjælp af funktionen **Tilpas**.
-   Annullering af ændringer af grundlæggende brugergrænseflade.

### <a name="cancel-customization"></a>Annullere tilpasning
Hvis du vil annullere alle tilpasninger af brugergrænsefladen, du nogensinde har foretaget for en side med dit gældende brugerlogon, eller siden du sidst annullerede tilpasninger af brugergrænsefladen, kan du bruge vinduet **Slet brugertilpasning**. Layoutet af siden, som du sletter dine personlige indstillinger for, nulstilles derefter til standardkonfigurationen for din profil.  

Hvis du kun vil annullere tilpasning af brugergrænsefladen, du har foretaget i et bestemt område af brugergrænsefladen på en side, som f.eks. båndet, kan du bruge knappen **Gendan standarder** i vinduet **Tilpas**. Layout af det specifikke område for brugergrænsefladen på siden nulstilles derefter til standardkonfigurationen for din profil.  

#### <a name="to-cancel-all-ui-customization-that-you-have-made-to-a-page"></a>Sådan annulleres alle tilpasninger af brugergrænsefladen, du har foretaget for en side  

1.  I feltet **Søg** skal du indtaste **Slet brugertilpasning** og derefter vælge det relaterede link.  

2.  Vælg siden, hvor du vil annullere din tilpasning af brugergrænsefladen, og vælg derefter **Slet** i gruppen **Vis** under fanen **Startside**.  

> [!NOTE]  
>  Al tilpasning af brugergrænsefladen for siden, du nogensinde har foretaget med dit nuværende brugerlogon, eller siden du sidst brugte vinduet **Slet brugertilpasning**, annulleres. Layoutet af siden nulstilles til standardkonfigurationen for din profil, som administratoren har konfigureret den, eller som den er installeret med [!INCLUDE[navnow](includes/navnow_md.md)].  

#### <a name="to-cancel-ui-customization-that-you-have-made-to-a-ui-area-on-a-page"></a>Sådan annulleres tilpasninger af brugergrænsefladen, du har foretaget for et brugergrænsefladeområde på en side  

1.  Fra den side hvor du har tilpasset et område af brugergrænsefladen, f.eks båndet, skal du vælge menuikonet **Program** ![Knappen Programmenu på menulinjen](media/applicationmenuicon.png "Programmenuikon"), vælge **Tilpas**, og derefter vælge **Tilpas <UI area>**.  

2.  I bunden af vinduet **Tilpas** skal du vælge knappen **Gendan standarder**.  

> [!NOTE]  
>  Al tilpasning af brugergrænsefladeområdet, du nogensinde har foretaget for siden med dit nuværende brugerlogon, eller siden du sidst brugte knappen **Gendan standarder**, annulleres. Layoutet af brugergrænsefladeområdet nulstilles til standardkonfigurationen for din profil, som administratoren har konfigureret den, eller som den er installeret med [!INCLUDE[navnow](includes/navnow_md.md)].

### <a name="cancel-basic-ui-changes"></a>Annuller ændringer af grundlæggende brugergrænseflade
Du annullerer grundlæggende ændringer af brugergrænsefladen ved at åbne vinduet **Nulstil brugerdefinerede indstillinger** fra dit rollecenter.  

Grundlæggende ændringer af brugergrænsefladen er bl.a.:
 -  Ændring af størrelsen og placeringen af et vindue.
 -  Ændring af kolonnebredden
 -  Ændring af højden på kolonneoverskrifter.
 -  Sortering af kolonner på en liste.
 -  Visning af lister som diagram.
 -  Sådan angives det, hvordan eksterne filer og automatiseringsobjekter håndteres.  

#### <a name="to-cancel-basic-ui-changes"></a>Sådan annulleres ændringer af grundlæggende brugergrænseflade

1.  Gå til rollecenteret.  

     I menuen **Program** ![Programmenuknap på menulinjen](media/applicationmenuicon.png "Programmenuikon") skal du vælge **Tilpas** og derefter vælge **Nulstil brugerdefinerede indstillinger**.  

2.  Vælg knappen **Nulstil indstillinger for brugergrænseflade**. Alternativt kan du vælge knappen **Nulstil alt** for også at annullere dine beslutninger omkring håndtering af filer og automatiseringsobjekter.  

 Alle grundlæggende ændringer af brugergrænsefladen, du nogensinde har foretaget med dit nuværende brugerlogon i [!INCLUDE[navnow_md](includes/navnow_md.md)], eller siden du sidst trykkede på knappen **Nulstil indstillinger for brugergrænseflade**, annulleres. Brugergrænsefladen nulstilles til standardkonfigurationen for din profil.  

#### <a name="to-cancel-your-decision-for-running-or-saving-external-files"></a>Sådan annulleres din beslutning for kørsel eller lagring af eksterne filer  

1.  Gå til rollecenteret.  

     I menuen **Program** ![Programmenuknap på menulinjen](media/applicationmenuicon.png "Programmenuikon") skal du vælge **Tilpas** og derefter vælge **Nulstil brugerdefinerede indstillinger**.  

2.  Vælg knappen **Nulstil beslutning om filhåndtering**. Alternativt kan du vælge knappen **Nulstil alt** for også at annullere dine visningsændringer og beslutning for håndtering af automatiseringsobjekter.  

 Alle beslutninger omkring standardhåndtering af filtyper, du nogensinde har taget med dit nuværende brugerlogon, eller siden du sidst brugte knappen **Adgang til klientfil**, annulleres og nulstilles til standardkonfigurationen for din profil. Næste gang [!INCLUDE[navnow_md](includes/navnow_md.md)] modtager en ekstern fil af enhver type, får du vist en dialogboks med indstillingerne **Gem**, **Kør** og **Annuller**  

### <a name="to-cancel-your-decision-for-handling-automation-objects"></a>Sådan annulleres din beslutning for håndtering af automatiseringsobjekter  

1.  Gå til rollecenteret.  

     I menuen **Program** ![Programmenuknap på menulinjen](media/applicationmenuicon.png "Programmenuikon") skal du vælge **Tilpas** og derefter vælge **Nulstil brugerdefinerede indstillinger**.  

2.  Vælg knappen **Nulstil beslutninger om automatisering**. Alternativt kan du vælge knappen **Nulstil alt** for også at annullere dine visningsændringer og beslutning om at køre eller gemme eksterne filer.  

 Alle beslutninger omkring, hvordan automatiseringsobjekter skal køres, du nogensinde har taget dig med dit nuværende brugerlogon, eller siden du sidst brugte knappen **Nulstil beslutninger om automatisering**, annulleres. Filhåndteringens funktionsmåde nulstilles til standardkonfigurationen for din profil. Næste gang [!INCLUDE[navnow_md](includes/navnow_md.md)] skal køre et automatiseringsobjekt af enhver type, får du vist en dialogboks med indstillinger, **Tillad altid** og **Tillad aldrig**.    

<!--Use the following table to get more information about customizing the different elements of the UI.

| To | See |
| --- | --- |
| Change which actions to show on the ribbon and how the actions are grouped. |[How to: Customize FastTabs](purchasing-how-record-purchases.md) |
|Change which FastTabs to show and which fields to include on the FastTabs.|[How to: Request Quotes](purchasing-how-request-quotes.md)|
|Add, remove, or arrange columns in a list or document-lines that represent fields in the underlying tables. |[ How to: Add or Remove Columns in a List or on Document Lines](purchasing-how-purchase-products-sale.md) |
| Rename or rearrange buttons, create a new menu button, add a link to a menu, or rearrange the order of a menu. |[ How to: Customize the Navigation Pane](purchasing-how-correct-cancel-unpaid-purchase-invoices.md) |
| Add a link from a department page to your Role Center. |[How to: Process Purchase Returns or Cancellations](purchasing-how-register-new-vendors.md) |
|Add a chart to your Role Center or to a list page.|[How to: Combine Receipts on a Single Invoice](purchasing-how-to-combine-receipts.md)|
| Unod personalization that you have made to your user interface, either for a specific area on a page, such as a ribbon, or for the whole page.|[How to: Cancel Personalization](ui-customization-cancel.md)|
-->


## <a name="see-also"></a>Se også
[Tilpasse dit arbejdsområde i Dynamics-webklienten](ui-personalization-user.md)  
[Oversigt over tilpasning](ui-personalization-overview.md)  

