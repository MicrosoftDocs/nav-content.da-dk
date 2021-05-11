---
title: "Sådan udskrives Remitteringsadvisering"
description: "Du kan hjælpe dine kreditorer med at udføre afstemninger ved at udskrive remitteringsadvisering, før du bogfører en betalingskladde, og når du har bogført en betaling."
documentationcenter: 
author: bholtorf
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/26/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: a16640e014e157d4dbcaabc53d0df2d3e063f8f9
ms.openlocfilehash: 71c84b4a7bad83e6008c0fa34f908e133b014a59
ms.contentlocale: da-dk
ms.lasthandoff: 10/26/2017

---

#<a name="how-to-print-remittance-advice"></a>Sådan udskrives Remitteringsadvisering
Du kan udskrive remitteringsadvisering, før du bogfører en betalingskladde, og når du har bogført en betaling. Denne advisering viser kreditorfakturanumre, som hjælper kreditorer til at udføre afstemninger.

##<a name="to-print-remittance-advice"></a>Sådan udskrives remitteringsadvisering
1. Vælg ikonet ![Søg efter side eller rapport](media/ui-search/search_small.png "Ikonet Søg efter side eller rapport"), angiv **Udbetalingskladder**, og vælg derefter det relaterede link.  
2. I vinduet **Udbetalingskladde** kan du vælge den betaling, der skal udskrives remitteringsadvisering for.  
3. Vælg handlingen **Udskriv remitteringsadvisering**.  
4. I kørslen **Remitteringsadvis – Kladde** på oversigtspanelet **Finanskladdelinje** skal du vælge de relevante filtre.  
  
    >[!Note]
    > Du kan filtrere med kreditorens eksterne dokumentnummer for at matche betalinger med fakturaer.

5. På oversigtspanelet **Kreditor** skal vælge de relevante filtre.  
6. Vælg **Udskriv** for at udskrive rapporten, eller vælg **Vis udskrift** for at få vist den nu.  

## <a name="using-remittance-advice-reports"></a>Brug af remitteringsadvis-rapporter
I følgende tabel beskrives de rapporter, som du kan bruge med remitteringsadvis:

|Rapport|Description|
|----|----|
|Rapporten Remitteringsadvis – Kladde|Denne rapport angiver, hvilke dokumenter der er inkluderet i betalingen. For finanskladdelinjer kan du angive, den kladdetype og det kladdenavn, hvorfra remitteringsadviseringen bliver udskrevet, datoen for den første aktivitet, der skal udskrives og filtrer efter et dokumentnummer. For kreditorer kan du angive de kreditornumre, der skal medtages i rapporten. |
|Rapporten Remitteringsadvis – Poster| Denne rapport angiver, hvilke dokumenter der er inkluderet i betalingen. Du kan definere rapportindholdet ved at angive filtre. Du kan angive yderligere felter under fanen ved at vælge feltet **Felt**. For kreditorposter kan du angive de kreditorer der skal medtages i rapporten, datoen for den første aktivitet, der skal udskrives, valutaen og løbenummeret, der skal medtages. |

> [!Note]
> Rapporten Remitteringsadvis - Kladde understøtter ikke direkte scenarier for udligning valuta eller betalingstolerancer. Du kan finde flere oplysninger i [Fremgangsmåde: Muliggøre udligning af finansposter i forskellige valutaer](finance-how-enable-application-ledger-entries-different-currencies.md).

> [!Tip]
> Du kan finde flere oplysninger om, hvordan du arbejder med rapporter, i [Vise testrapporter inden bogføring](ui-how-view-test-reports-posting.md), [Arbejde med rapporter](ui-work-report.md) og [Søgning i, filtrering og sortering af data](ui-enter-criteria-filters.md).

##<a name="see-also"></a>Se også  
[Velkommen til Dynamics NAV](across-get-started.md)
