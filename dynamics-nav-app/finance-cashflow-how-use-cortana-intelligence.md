---
title: "Fremgangsmåde: Oprette pengestrømsprognoser"
author: bholtorf
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 1fdb53b0f58ada22475fe1c1510146c156a60410
ms.contentlocale: da-dk
ms.lasthandoff: 10/23/2017

---

# <a name="how-to-make-predictive-cash-flow-forecasts"></a>Fremgangsmåde: Oprette pengestrømsprognoser
Pengestrømsprognoser hjælper dig med at sikre, at din virksomhed har nok likviditet til at opfylde sine finansielle forpligtelser, og er nyttige, når du skal regulere budgetter. Hvis du f.eks. har overskydende likviditet, kan du afbetale på din gæld, og det er en fordel at få en tidlig advarsel, hvis likviditeten er begrænset.

Cortana Intelligence bruger Azure Machine Learning-tjenesten til at oprette pålidelige prognoser. Prognoser fra Cortana Intelligence kan f.eks. hjælpe dig til at forudse og undgå likviditetsunderskud. Tjenesten kombinerer historiske oplysninger med aktuel bogføring af køb og salg, herunder posteringer med forfaldsdatoer i fremtiden. Disse omfatter:
* Købsordrer
* Salgsordrer
* Bogførte salgs- og købsfakturaer
* Kreditnotaer

## <a name="before-you-start"></a>Før du starter  
Der er nogle få ting, du skal gøre, før du bruger Cortana Intelligence til pengestrømsprognoser:
* Hvis du ikke allerede bruger pengestrømsprognoser, skal du konfigurere:
    * En eller flere konfigurationer i **Pengestrømskonfiguration**.
    * Konti til skyldige beløb, tilgodehavender, salgsordrer og indkøbsordrer. Cortana Intelligence bruger posteringerne i disse konti.
    * En eller flere pengestrømsprognoser i **Pengestrømsprognose**. Sørg for at medtage købsordrer, salgsordrer, tilgodehavender og skyldige beløb som kilder.  
    Yderligere oplysninger finder du ved at søge efter _pengestrømsprognoser_ i Hjælp.
* Find URL-adressen og API-nøglen for API til den prognosewebtjeneste, der skal bruges.  
    Du kan bruge Azure Machine Learning eller en anden tjeneste, hvis du har en. Der findes også en offentlig model med navnet _Prognosemodel til Microsoft Dynamics NAV_, som er tilgængelig online i Cortana Intelligence-galleriet. Sådan bruges modellen:

    1. I en webbrowser skal du gå til [Cortana Intelligence-galleriet](https://go.microsoft.com/fwlink/?linkid=828352)
    2. Søg efter _Prognosemodel til Microsoft Dynamics NAV_, og åbn derefter modellen i Azure Machine Learning Studio.
    3. Brug din Microsoft-konto til at tilmelde dig et arbejdsområde og derefter kopiere modellen.
    4. Kør modellen, og udgiv den som en webtjeneste.
    5. Notér URL-adressen for API og API-nøglen. Du bruger disse legitimationsoplysninger, når du konfigurerer Cortana Intelligence i [!INCLUDE[navnow](includes/navnow_md.md)].  

* Overvej, hvor ofte du vil beregne prognosen. Tjenesten Azure Machine Learning har begrænsninger vedrørende anvendelse. Hvis du f.eks. har mange af varer, kan det være bedre ikke at beregne så ofte.
* Tildel til rollecenteret Regnskabsmedarbejder.

## <a name="set-up-cortana-intelligence"></a>Konfigurere Cortana Intelligence
Du kan bruge en assisteret opsætningsvejledning til at konfigurere pengestrømsprognoser. Vejledningen hjælper dig med f.eks. at angive, hvor ofte prognosen skal opdateres, de konti, den skal baseres på, oplysninger om, hvornår du betaler skatter, og om du vil bruge Cortana Intelligence.  

Hvis du allerede bruger pengestrømsprognoser og bare vil slå Cortana Intelligence til, kan du også bruge en manuel proces. Når du logger på vises en notifikation i en blå bjælke øverst i arbejdsområdet. Hvis du vil konfigurere Cortana Intelligence med det samme, skal du vælge **Ja tak**. Meddelelsen vises kun én gang. Hvis du lukker den, skal du bruge den manuelle proces til at konfigurere Cortana Intelligence.  

**Tip!** Overvej længden på de perioder, som tjenesten skal bruge i beregningerne. Jo flere data du angiver, desto mere nøjagtige forudsigelser får du. Hold også øje med store variationer mellem perioderne. De kan også påvirke forudsigelserne. Hvis Cortana Intelligence ikke finder nok data, eller dataene varierer meget, opretter tjenesten ikke en forudsigelse.

Sådan bruges den assisterede opsætningsvejledning:
1. I rollecenteret Regnskabsmedarbejder under diagrammet **Pengestrømsprognose** skal du klikke på handlingen **Åbn assisteret opsætning**.
2. Udfyld felterne efter behov i hvert trin i vejledningen.

Sådan bruges en manuel proces:
1. Søg efter **Pengestrømskonfiguration**, og vælg derefter det relaterede link.
2. Udvid oversigtspanelet **Cortana Intelligence**, og udfyld derefter felterne efter behov.

## <a name="turn-on-cortana-intelligence-for-cash-flow-forecasts"></a>Aktivere Cortana Intelligence til pengestrømsprognoser
1. Søg efter **Pengestrømsprognoser**, og vælg derefter det relaterede link.
2. Vælg handlingen **Pengestrømskladde**.
3. På siden **Pengestrømskladde** skal du vælge handlingen **Foreslå kladdelinjer**.  
4. Under **Kildetyper skal inkludere** skal du markere afkrydsningsfeltet **Cortana Intelligence-prognose**.

## <a name="investigate-a-cash-flow-forecast"></a>Undersøge en pengestrømsprognose
Hvis du vil kigge nærmere på dataene under prognosen, herunder variansen, skal du vælge kolonnen **Cortana Intelligence**. Den første række i tabellen viser variansen. De øvrige rækker er arrangeret efter kildedokument.  

Du kan f.eks. se, hvordan prognosen:    
* Håndterer bekræftet salg og køb
* Fratrækker skyldige beløb og tilføjer tilgodehavender
* Springer dubletter af salgsordrer og købsordrer over

## <a name="see-also"></a>Se også  
[Arbejde med Dynamics NAV](ui-work-product.md)

