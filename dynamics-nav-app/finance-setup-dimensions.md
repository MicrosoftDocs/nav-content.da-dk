---
title: Oprette dimensioner
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 1b7a293982dfc7ff73c163ad1711e2bce098e98e
ms.contentlocale: da-dk
ms.lasthandoff: 10/16/2017

---

# <a name="set-up-dimensions"></a>Oprette dimensioner
Du skal angive, hvilke dimensioner og dimensionsværdier du vil bruge i virksomheden. Du bør også angive, hvilke dimensioner du vil bruge som globale og genvejsdimensioner. Du skal nøje overveje, hvilke dimensioner der er mest nyttige som globale dimensioner og genvejsdimensioner i regnskabet.  
Du definerer alle de forskellige dimensioner, som du vil spore i vinduet **Dimensioner**. Dette vindue indeholder én linje for hver dimension, f.eks. *Projekt*, *Afdeling*, *Område* og *Sælger*.  

Du skal også oprette dimensionsværdier for hver dimension, f.eks. alle afdelingerne i din virksomhed. Dimensionsværdierne kan oprettes i en hierarkisk struktur - ligesom kontoplanen - så data kan opdeles i forskellige granularitetsniveauer, og dimensionsdelmængder kan lægges sammen.  

Du kan angive to globale dimensioner, som automatisk vil være tilgængelige overalt, f.eks. i rapporter og kørsler. Du kan også angive seks supplerende genvejsdimensioner, der vil være tilgængelige som et felt i kladde- og dokumentlinjer. Hvis du vil anvende de resterende dimensioner, skal du åbne et separat vindue, hvor dimensionerne for den pågældende linje vises.  

Du kan oprette det antal dimensioner, som du har brug for, og du kan oprette et ubegrænset antal dimensionsværdier til hver dimension. Alle dimensioner, som du opretter, kan bruges på kladde- og bilagsposter samt i dimensionsrelaterede rapporter og kørsler.  

## <a name="set-up-default-dimensions-for-customers-vendors-and-other-accounts"></a>Oprette standarddimensioner for kunder, leverandører og andre konti
Du kan oprette en standarddimension for en specifik konto. Denne kode kopieres så til kladden eller dokumentet, når kontonummeret på linjen er angivet. Du kan slette og ændre koden efter behov. Du kan også oprette en obligatorisk dimension, så det ikke er muligt at bogføre en post med en bestemt type konto, medmindre kontoen har en tildelt dimensionsværdi.  

Desuden kan du indstille en standarddimension for hver kontotype, så denne kode kopieres til kladden eller dokumentet, når kontotype angives på linjen. Men du kan altid ændre koden på dokumentet, hvis det er relevant.  

Endelig kan du også oprette en obligatorisk dimension, så det ikke er muligt at bogføre en post med en bestemt type konto, medmindre kontoen har en tildelt dimensionsværdi.

## <a name="see-also"></a>Se også
[Arbejde med dimensioner](finance-dimensions.md)  
[Definere centrale finansielle processer](finance-setup-finance.md)

