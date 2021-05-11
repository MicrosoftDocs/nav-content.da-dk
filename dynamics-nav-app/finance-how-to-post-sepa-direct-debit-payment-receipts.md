---
title: "Bogfør SEPA Direct Debit-betalinger"
description: "Når en Direct Debit-opkrævning er behandlet af din bank, kan du fortsætte med at bogføre kvittering for betaling for de involverede salgsfakturaer."
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/21/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 9b0e82feb77be2e66b618aab7322215637d4f89e
ms.contentlocale: da-dk
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-post-sepa-direct-debit-payment-receipts"></a>Fremgangsmåde: Bogføre SEPA Direct Debit-betalingskvitteringer
Når en Direct Debit-opkrævning er behandlet af din bank, kan du fortsætte med at bogføre kvittering for betaling for de involverede salgsfakturaer. Du kan finde flere oplysninger i [Fremgangsmåde: Opret poster i SEPA Direct Debit-opkrævning, og eksportér til en bankfil](finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md).  

Du kan bogføre betalingskvitteringen direkte fra vinduet **Direct Debit-opkrævninger** eller vinduet **Poster i Direct Debit-opkrævning**. Alternativt kan du overføre arbejdet til en anden bruger ved at udarbejde de relaterede kladdelinjer.  

## <a name="to-post-a-direct-debit-payment-receipt-from-the-direct-debit-collections-window"></a>Sådan bogføres en betalingskvittering i Direct Debit fra vinduet Direct Debit-opkrævninger  
1. Vælg ikonet ![Søg efter side eller rapport](media/ui-search/search_small.png "Ikonet Søg efter side eller rapport"), angiv **Direct Debit-opkrævninger**, og vælg derefter det relaterede link.  
2. Vælg en linje for en Direct Debit-opkrævning, der er eksporteret til en bankfil og er blevet behandlet af banken. Du kan finde flere oplysninger i [Fremgangsmåde: Opret poster i SEPA Direct Debit-opkrævning, og eksportér til en bankfil](finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md).  
3. Vælg handlingen **Bogfør betalingskvitteringer**.  
4. I vinduet **Bogfør Direct Debit-opkrævning** skal du udfylde felterne som beskrevet i følgende tabel.  

    |Felt|Description|  
    |---------------------------------|---------------------------------------|  
    |**Direct Debit-opkrævningsnr.**|Angiv den Direct Debit-samling, som du vil bogføre betalingskvittering for.|  
    |**Finanskladdetype**|Angiv, hvilken finanskladdeskabelon der skal bruges til bogføring af betalingskvitteringen, f.eks. skabelonen til indbetalinger.|  
    |**Finanskladdenavn**|Angiv, hvilket finanskladdenavn der skal bruges til bogføring af betalingskvitteringen.|  
    |**Opret kun kladde**|Markér dette afkrydsningsfelt, hvis du ikke vil bogføre betalingskvitteringen, når du vælger knappen **OK**. Kvitteringen for betalingen forberedes i den angivne journal og vil ikke blive bogført, før nogen bogfører de pågældende kladdelinjer.|  

5. Vælg knappen **OK**.  

## <a name="see-also"></a>Se også  
 [Indhente betalinger med SEPA Direct Debit](finance-collect-payments-with-sepa-direct-debit.md)   
 [Salg](sales-manage-sales.md)

