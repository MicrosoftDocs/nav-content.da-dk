---
title: Bruge Dynamics NAV-indholdspakken til Power BI
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: ad9519b8ce9c244480308ccc99c05e78e4926b06
ms.contentlocale: da-dk
ms.lasthandoff: 10/16/2017

---

# <a name="using-the-dynamics-nav-content-pack-for-power-bi"></a>Bruge Dynamics NAV-indholdspakken til Power BI
Du kan nemt få indsigt i dine Dynamics NAV-data med Power BI og Dynamics NAV-indholdspakken. Power BI henter dine data og opretter derefter et out-of-the-box dashboard og rapporter baseret på dataene.  

Indholdspakken er konfigureret til arbejde med salgstal og finansielle data fra demonstrationsregnskabet, som du får, når du tilmelder dig eksempelvisningen af Dynamics NAV.  

- Vælg en visualisering på dashboardet for at få vist en af syv underliggende rapporter.  
- Filtrer rapporten, eller tilføj felter, du vil overvåge.  
- Fastgør denne brugerdefinerede visning til dashboardet for fortsat sporing.  
Dashboardet og de underliggende rapporter opdateres dagligt. Du kan kontrollere opdateringsplanen og ændre hyppigheden på datasættet.  

## <a name="accessing-dynamics-nav-in-power-bi"></a>Adgang til Dynamics NAV i Power BI
Når du vil have vist dine Dynamics NAV-data i Power BI, skal du have følgende:  

- Adgang til Dynamics NAV. Du kan finde flere oplysninger i [Dynamics NAV](http://go.microsoft.com/fwlink/?LinkID=759714).  
- Adgang til Power BI. Du kan finde flere oplysninger i [Power BI](https://powerbi.microsoft.com).

Du kan finde flere oplysninger på Power BI-webstedet om [at tilføje Dynamics NAV-indholdspakken til Power BI](http://go.microsoft.com/fwlink/?LinkID=760850).  

Når du vil have adgang til Dynamics NAV-indholdspakken i Power BI, skal du i forbindelsesvinduet angive følgende oplysninger:

| Felt       | Beskrivelse              |
|-------------|--------------------------|
|**URL-adresse til OData Feed**|OData URL-adressen, så Power BI kan få adgang til din virksomhed, f.eks. https://mybusiness.com:7048/MS/OData/Company('CRONUS%20US').|
|**Godkendelsesmetode**|Vælg **Basic**.|
|**Brugernavn**|Den mailkonto, som du brugte til at tilmelde dig Dynamics NAV, f.eks. *me@mybusiness.com*.|
|**Adg.kode**|Dette er webtjenesteadgangsnøglen til din brugerkonto i Dynamics NAV.|

Det betyder, at du skal have to oplysninger fra Dynamics NAV: OData URL-adressen og webtjenesteadgangsnøglen til brugerkontoen.  
**Hente URL-adressen**  
Når du tilføjer Dynamics NAV til Power BI, skal du angive en URL-adresse, så Power BI kan få adgang til data fra din virksomhed. I forbindelsesvinduet omtales URL-adressen som **URL-adresse til OData Feed**, og den skal have følgende format:

         https://mybusiness.projectmadeira.com:7048/MS/OData/Company('CRONUS%20US')  
I dette eksempel er *mybusiness* navnet på Dynamics NAV-tjenesten, og *CRONUS US* er navnet på demonstrationsvirksomheden, hvor *%20* repræsenterer området i navnet.   
Du henter URL-adressen ved i Dynamics NAV at søge efter og åbne vinduet **Webtjeneste**. Dette vindue viser de webtjenester, der aktuelt er tilgængelige, og du kan kopiere linket fra feltet **URL-adresse til OData** til en af standard OData-webtjenesterne.  
**Sådan henter du webtjenesteadgangsnøglen**  
Hvis du vil bruge data fra Dynamics NAV i Power BI skal du i vinduet **Opret forbindelse til Dynamics NAV** angive dit brugernavn, der er din mailkonto, og en adgangskode. Adgangskoden er den webtjenesteadgangsnøgle, der er konfigureret til din brugerkonto i Dynamics NAV.  
Du kan få en webtjenesteadgangsnøgle ved i Dynamics NAV at søge efter vinduet **Brugere** og derefter åbne kortet til din brugerkonto. I oversigtspanelet **Webtjenesteadgang** skal du kopiere oplysningerne i feltet **Webtjenesteadgangsnøgle**. Hvis feltet er tomt, skal du på båndet vælge **Angiv webtjenesteadgangsnøgle**, vælge feltet **Nøglen udløber aldrig** og derefter klikke på knappen OK. Derefter kan du kopiere nøglen.  

## <a name="getting-data-from-dynamics-nav"></a>Hente data fra Dynamics NAV
Dynamics NAV-dashboardet viser de mest almindelige rapporter, du kan bruge til at registrere din virksomhed. Dataene er hentet fra Dynamics NAV-virksomheden ved hjælp af webtjenester, der læser data direkte. I Dynamics NAV kan du i vinduet **Webtjenester** se webtjenester, der er konfigureret til dig, herunder følgende, der forbruges af indholdspakken i Power BI:  

- ItemSalesAndProfit  
- ItemSalesByCustomer  
- powerbifinance-setup  
- SalesDashboard  
- SalesOpportunities  
- SalesOrdersBySalesPerson  
- TopCustomerOverview  

**Bemærk**: Hvis du ændrer navnet på en af disse webtjenester, vises data ikke i Power BI.  
Hvis du vil tilføje andre data i Power BI, skal du finde tabellerne i Dynamics NAV, vise dem som webtjenester og derefter føje dem til indholdspakken. Dette er et avanceret scenarie, og det anbefales, at du starter med de data, der allerede findes i Power BI.  

## <a name="troubleshooting"></a>Fejlfinding
Power BI-dashboardet er baseret på de publicerede webtjenester, der er anført ovenfor, og viser data fra demonstrationsvirksomheden eller din egen virksomhed, hvis du indlæser data fra dit aktuelle økonomiopsætningssystem. Men hvis noget går galt indeholder dette afsnit en løsning til de mest almindelige problemer.  

**"Parametervalideringen mislykkedes, kontroller, at alle parametre er gyldige"**  
Hvis du får denne fejlmeddelelse, når du har angivet URL-adressen til Dynamics NAV, skal du kontrollere, at følgende krav opfyldt:  

- URL-adressen følger dette mønster nøjagtigt:

    https://mybusiness.projectmadeira.com:7048/MS/OData/Company('CRONUS%20US')  
- Slet tekst, der evt. står efter firmanavn i parentes  
- Kontroller, at der ikke er nogen efterfølgende skråstreg i slutningen af URL-adressen.  
- Sørg for, at det er en sikker forbindelse, som når URL-adressen starter med *https*.  


**"Logon mislykkedes"**  
Hvis fejlmeddelelsen "Logon mislykkedes" vises, når du logger på dashboardet ved hjælp af dine legitimationsoplysninger til Dynamics NAV, kan det skyldes en af følgende situationer:

* Den konto, du bruger, har ikke rettigheder til at læse Dynamics NAV-data fra din konto.

    Kontroller din brugerkonto i Dynamics NAV, og kontroller, at du har brugt den rigtige webtjenesteadgangsnøgle som adgangskode, og prøv derefter igen.  
* Den Dynamics NAV-forekomst, du prøver at oprette forbindelse til, har ikke et gyldigt SSL-certifikat. I dette tilfælde kan du se en mere detaljeret fejlmeddelelse ("kan ikke etablere SSL-tillidsrelation").

    **Bemærk**: Selvsignerede certifikater understøttes ikke.  


**"UPS"**  
Hvis du får vist en "UPS"-fejlmeddelelse, når du er færdig med godkendelsesdialogboksen, skyldes dette oftest problemer med forbindelsen til dataene til indholdspakken.

* Kontroller, at URL-adressen følger det mønster, der blev angivet tidligere:

    https://mybusiness.projectmadeira.com:7048/MS/OData/Company('CRONUS%20US')  
* En almindelig fejl er at angive hele URL-adressen til en bestemt webtjeneste:

    https://mybusiness.projectmadeira.com:7048/MS/OData/Company('CRONUS%20US')/powerbifinance-setup  
* Eller du kan have glemt at angive firmanavnet:

    https://mybusiness.projectmadeira.com:7048/MS/OData/  


## <a name="see-also"></a>Se også
[Velkommen til Dynamics NAV](across-get-started.md)  

