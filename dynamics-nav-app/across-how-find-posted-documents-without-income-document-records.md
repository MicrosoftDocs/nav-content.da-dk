---
title: "Søge efter dokumenter uden vedhæftede filer"
Description: "Du kan søge efter finansposter for bogførte købs- og salgsdokumenter, der ikke har indgående elektroniske dokumenter, f.eks. importerede fakturaer."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: electronic document, e-invoice, incoming document, OCR, ecommerce, document exchange, import invoice
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 515026b4da842afeda1759f50313dc26bcfd3350
ms.contentlocale: da-dk
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-find-posted-documents-without-incoming-document-records"></a>Fremgangsmåde: Finde bogførte dokumenter uden indgående dokumentposter
Fra vinduerne **Kontoplan** og **Finansposter** kan du bruge en søgefunktionen til at finde finansposter for bogførte og købs- og salgsdokumenter, som ikke har indgående dokument poster og derefter knytte centralt til eksisterende poster eller oprette nye med vedhæftede dokument filer.

## <a name="to-find-posted-documents-without-incoming-document-records"></a>Sådan findes bogførte dokumenter uden indgående dokumentposter
1. Vælg ikonet ![Søg efter side eller rapport](media/ui-search/search_small.png "Ikonet Søg efter side eller rapport"), angiv **Kontoplan**, og vælg derefter det relaterede link.
2. Vælg en linje for en finanskonto, for hvis finansposter du vil se bogførte købs- og salgsdokumenter uden indgående dokumentposter, og vælg derefter handlingen **Bogførte dokumenter uden indgående bilag**.
3. Alternativt kan du vælge handlingen **Poster**.
4. I vinduet **Finansposter** skal du vælge handlingen **Bogførte dokumenter uden indgående dokumenter**.

Vinduet **Bogførte dokumenter uden indgående dokument** åbnes og viser bogførte købs- åbnes og salgsdokumenter uden indgående dokumentposter repræsenteret af finansposter på den finanskonto, som du åbnede vinduet for. Vinduet kan vise højst 1000 linjer. Som standard indeholder feltet **Datofilter** derfor et filter, der begrænser linjerne til poster med bogføringsdatoer fra begyndelsen af den aktuelle regnskabsperiode til arbejdsdatoen.

## <a name="to-connect-found-documents-to-existing-incoming-document-records"></a>Sådan knyttes fundne dokumenter med eksisterende indgående bilagsposter
1. I vinduet **Bogførte dokumenter uden indgående dokument** skal du vælge linjen for et bogført dokument, du vil knytte til en eksisterende indgående dokumentpost og derefter vælge handlingen **Vælg indgående bilag**.
2. Vælg den indgående dokumentpost, som du vil knytte til det bogførte fundne dokument, i vinduet **Indgående bilag**, og vælg derefter **OK**.
3. I vinduet **Bogførte dokumenter uden indgående dokument** er den valgte indgående dokumentpost nu tilknyttet det bogførte dokument, som du kan se i faktaboksen **Indgående bilagsfiler**.

Hvis der ikke findes en relevant indgående dokument post i vinduet **Indgående bilag** kan du oprette den. Du kan finde flere oplysninger under [Fremgangsmåde: Oprette indgående dokumentposter](across-how-create-income-document-records.md).

## <a name="see-also"></a>Se også
[Behandle indgående bilag](across-process-income-documents.md)  
[Indgående bilag](across-income-documents.md)  
[Køb](purchasing-manage-purchasing.md)  
[Arbejde med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

