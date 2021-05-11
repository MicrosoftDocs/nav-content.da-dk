---
title: Aktivere debitorbetalinger via betalingstjenester
description: "Gør det lettere for kunderne at betale deres fakturaer ved at aktivere betalingstjenester."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: online payment
ms.date: 07/07/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: a16640e014e157d4dbcaabc53d0df2d3e063f8f9
ms.openlocfilehash: f56df1759d375548b7415234c9b303a49e50687d
ms.contentlocale: da-dk
ms.lasthandoff: 10/26/2017

---
# <a name="how-to-enable-customer-payments-through-payment-services"></a>Fremgangsmåde: Aktivere debitorbetalinger via betalingstjenester
Som et alternativ til opkrævning af betalinger via bankoverførsel eller kreditkort kan dine kunder betale dig via deres konto hos betalingstjenester såsom PayPal eller WorldPay.  

Når du har aktiveret en betalingstjeneste i [!INCLUDE[d365fin](includes/d365fin_md.md)], vises der et link til tjenesten på de salgsdokumenter, som du sender med mail til dine kunder. Kunder kan bruge linket til at gå til betalingstjenesten og betale fakturaen direkte fra salgsdokumentet. Hvis du ikke vil indsætte linket, f.eks. hvis en debitor betaler kontant, kan du fjerne betalingstjenesten fra fakturaen inden bogføringen.  

PayPal Payments Standard- og WorldPay Payments Standard-udvidelserne installeres i [!INCLUDE[d365fin](includes/d365fin_md.md)] og er klar til aktivering.  

## <a name="to-enable-a-payment-service-in-included365finincludesd365finmdmd"></a>Sådan aktiverer du en betalingstjeneste i [!INCLUDE[d365fin](includes/d365fin_md.md)]
1. Vælg ikonet ![Søg efter side eller rapport](media/ui-search/search_small.png "Ikonet Søg efter side eller rapport"), angiv **Betalingstjenester**, og vælg derefter det relaterede link.  
2. I vinduet **Betalingstjenester** skal du vælge handlingen **Ny**.  
3. Vælg betalingstjenesten, og luk derefter vinduet.  
4. I vinduet **Betalingstjenester** skal du vælge handlingen **Konfigurer**.  
5. Udfyld felterne efter behov. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
6. Luk vinduet.  

## <a name="to-select-a-payment-service-on-a-sales-invoice"></a>Sådan vælger du en betalingstjeneste på en salgsfaktura
1. På startsiden skal du vælge handlingen **Salgsfakturaer**.  
2. Åbn den faktura, du vil betale med betalingstjenesten.  
3. Vælg betalingstjenesten i feltet **Betalingstjeneste**.  

    > [!NOTE]  
>   Feltet **Betalingstjeneste** er kun tilgængeligt, hvis du har aktiveret betalingstjenesten.  

## <a name="see-also"></a>Se også  
[Konfigurere salg](sales-setup-sales.md)  
[Salg](sales-manage-sales.md)  
[Tilpasse [!INCLUDE[d365fin](includes/d365fin_md.md)] ved hjælp af udvidelser](ui-extensions.md)  
[Arbejde med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

