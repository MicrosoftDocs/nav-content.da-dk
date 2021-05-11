---
title: Designoplysninger - Genbestillingspunktets rolle
description: "Dette emne beskriver vigtigheden af at angive et genbestillingspunkt, så du ved, hvornår du skal bestille mere til lager."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: desigh, reorder, demand, supply
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 8035a670077e53981e9c366d22bdb20df06d8c1b
ms.contentlocale: da-dk
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-the-role-of-the-reorder-point"></a>Designoplysninger: Genbestillingspunktets rolle
Udover den generelle afstemning af udbud og efterspørgsel, skal planlægningssystemet også overvåge lagerniveauer for de pågældende varer for at respektere de definerede genbestillingsmetoder.  
  
Et genbestillingspunkt repræsenterer behov under leveringstid. Når den projekterede lagerbeholdning kommer under den lagerbeholdning, der er defineret af genbestillingspunktet, er det tid til at bestille mere. I mellemtiden forventes lagerføring at reduceres gradvist og eventuelt nå nul (eller sikkerhedslagerniveau), indtil genopfyldningen ankommer.  
  
Planlægningssystemet vil derfor foreslå en forsyningsordre, der er planlagt fremad, når den forventede lagerbeholdning er under genbestillingspunktet.  
  
Genbestillingspunktet afspejler et bestemt lagerniveau. Lagerniveauer kan dog flytte betydeligt under intervallet, og planlægningssystemet skal derfor hele tiden overvåge den forventede disponible beholdning.  
  
## <a name="see-also"></a>Se også  
[Designoplysninger: Genbestillingsmetoder](design-details-reordering-policies.md)   
[Designoplysninger: Planlægningsparametre](design-details-planning-parameters.md)   
[Designoplysninger: Håndtering af genbestillingsmetoder](design-details-handling-reordering-policies.md)   
[Designoplysninger: Forsyningsplanlægning](design-details-supply-planning.md)
