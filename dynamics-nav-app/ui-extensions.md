---
title: Installation af udvidelser for at tilpasse Dynamics NAV
description: "F� mere at vide om tilf�jelse af funktioner og tilpasning af Dynamics NAV ved at installere udvidelser."
documentationcenter: 
author: edupont04
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: app, add-in, manifest, customize
ms.date: 07/07/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: a16640e014e157d4dbcaabc53d0df2d3e063f8f9
ms.openlocfilehash: 109eb8d0e2a38566739878ef513ffa3bec8dcd30
ms.contentlocale: da-dk
ms.lasthandoff: 10/26/2017

---
# <a name="customizing-dynamics-nav-using-extensions"></a>Tilpasse Dynamics NAV ved hj�lp af udvidelser
Du kan �ndre [!INCLUDE[d365fin](includes/d365fin_md.md)] ved at installere udvidelser, der f.eks. tilf�jer funktioner, �ndrer funktionsm�der eller giver dig adgang til nye onlinetjenester.
N�r du starter [!INCLUDE[d365fin](includes/d365fin_md.md)] f�rste gang, er der allerede installeret nogle udvidelser for dig. Med tiden g�res flere udvidelser tilg�ngelige for dig, og du kan derefter v�lge, om du vil bruge udvidelsen eller ej.

Microsoft leverer f.eks. en udvidelse, der giver integration med PayPal Payments Standard. Denne udvidelse er installeret som standard.
Men hvis en anden udvidelse, som tilbyder integration med en anden betalingstjeneste, stilles til r�dighed, kan du installere nye udvidelse og derefter v�lge, hvilken af to de tjenester du vil bruge.  

Du kan administrere udvidelserne i vinduet **Udvidelsesstyring**. Du kan �bne vinduet fra Start. Du kan ogs� v�lge ikonet **S�g efter side eller rapport** ![S�g efter side eller rapport](media/ui-search/search_small.png "Ikonet S�g efter side eller rapport") i det �verste h�jre hj�rne, angive **Udvidelser** og derefter v�lge det relaterede link.  

> [!NOTE]  
>   Hvis du mener, at du skal have adgang til en udvidelse, men ikke kan finde de relevante funktioner, skal du v�lge vinduet **Udvidelsesstyring** � hvis filtypen ikke er angivet der, kan du installere den som beskrevet i f�lgende afsnit.  

## <a name="installing-an-extension"></a>Installation af en udvidelse
Du kan hente nye udvidelser fra markedspladsen p� [AppSource.microsoft.com](https://appsource.microsoft.com/en-us/marketplace/apps?product=dynamics-365%3Bdynamics-365-for-financials&page=1). Her kan du se alle tilg�ngelige udvidelser til [!INCLUDE[d365fin](includes/d365fin_md.md)], og du kan f� apps, udvidelser og indholdspakker til andre Microsoft-produkter. Angiv de relevante filtre, kig p� oplysningerne om hver udvidelse og hent en udvidelse til [!INCLUDE[d365fin](includes/d365fin_md.md)].  
> [!NOTE]  
>   Log p� [AppSource.microsoft.com](https://appsource.microsoft.com/) ved hj�lp af den mailkonto, du bruger til [!INCLUDE[d365fin](includes/d365fin_md.md)]. Brug den samme mailkonto til andre tjenester og produkter for at opn� en ensartet oplevelse.  

Du kan ogs� f� adgang til markedspladsen i [!INCLUDE[d365fin](includes/d365fin_md.md)]. I vinduet **Udvidelsesstyring** kan du se de udvidelser, der er installeret, og du kan �bne siden **Markedsplads for udvidelse** for at se de udvidelser til [!INCLUDE[d365fin](includes/d365fin_md.md)], der er tilg�ngelige i AppSource. Hvis du v�lger linket *Flere apps*, �bnes [AppSource.microsoft.com](https://appsource.microsoft.com/en-us/marketplace/apps?product=dynamics-365%3Bdynamics-365-for-financials&page=1).  

Hvis du v�lger en udvidelse, du kan finde oplysninger om, hvad den g�r, og du kan f� adgang til hj�lp for at f� mere at vide om udvidelsen. N�r du v�lger at hente en udvidelse, skal du acceptere vilk�rene for anvendelse. Hvis du henter udvidelsen fra AppSource-webstedet, logges du p� [!INCLUDE[d365fin](includes/d365fin_md.md)] for at fuldf�re installationen.  

N�r du installerer en udvidelse, kan det v�re n�dvendigt at konfigurere den, f.eks. angive en konto til brug sammen med udvidelsen **PayPal Payments Standard til [!INCLUDE[d365fin](includes/d365fin_md.md)]**.
Andre udvidelser f�jer simpelthen felter til en eksisterende side, eller de tilf�jer en ny side f.eks.   

Hvis du fjerner en udvidelse, og du senere skifter mening, kan du installere den igen. N�r du fjerner en udvidelse, som du har brugt, bevares dataene, s� de stadig tilg�ngelige, hvis du installerer udvidelsen igen.  

Nogle udvidelser er fra Microsoft, mens andre udvidelser leveres af [andre virksomheder](ui-extensions-other.md). Alle udvidelser testes, f�r de bliver tilg�ngelige for dig, men det anbefales, at du bruger de links, der f�lger med hver udvidelse, for at f� mere at vide om udvidelsen, f�r du v�lger at installere den.  

Microsoft tilbyder f�lgende udvidelser:  

* [Overf�rsel af data med Dynamics GP](ui-extensions-dynamicsgp-data-migration.md)  
* [PayPal Payments Standard](ui-extensions-paypal-payments-standard.md)  
* [Overflytning af QuickBooks Data](ui-extensions-quickbooks-data-migration.md)  
* [Salgs- og lagerprognose](ui-extensions-sales-forecast.md)  
* [Ceridian l�n](ui-extensions-ceridian-payroll.md)  
* [Import af Quickbooks-l�nfiler](ui-extensions-quickbooks-payroll.md)  
* [WorldPay Payments Standard](ui-extensions-worldpay-payments-standard.md)
* [Britiske GetAddress.io-postnumre](ui-extensions-getaddressio.md)
* [Overf�rsel af QuickBooks Online-data](ui-extensions-quickbooks-online-data-migration.md)
* [Revisorportal](ui-extensions-accountant-portal.md)  
* [Billedanalyse](ui-extensions-image-analyzer.md)

> [!NOTE]  
>  Der findes ingen nye udvidelser i AppSource umiddelbart efter, at vi har oplyst om en opdatering. Du kan holde �je med udvidelser p� [AppSource.microsoft.com](https://appsource.microsoft.com/en-us/marketplace/apps?product=dynamics-365%3Bdynamics-365-for-financials&page=1).

## <a name="see-also"></a>Se ogs�
[Fremgangsm�de: Aktivere debitorbetaling via PayPal](sales-how-enable-payment-service-extensions.md)  
[Overf�re virksomhedsdata fra andre �konomisystemer](upload-data.md)    
[[!INCLUDE[d365fin](includes/d365fin_md.md)]-udvidelser fra andre leverand�rer](ui-extensions-other.md)  
[Velkommen til [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)  

##


