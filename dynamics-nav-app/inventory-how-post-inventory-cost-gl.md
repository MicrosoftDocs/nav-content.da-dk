---
title: "Fremgangsmåde: Bogføre kostpriser i finansregnskabet"
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: 34eec596392e9316e807d3c073c3b8e59dbc12e9
ms.contentlocale: da-dk
ms.lasthandoff: 10/16/2017

---

# <a name="how-to-post-inventory-costs-to-the-general-ledger"></a>Fremgangsmåde: Bogføre kostpriser i finansregnskabet   
Når du bogfører lagertransaktioner, f.eks. salgsleverancer, købsfakturaer eller lagerreguleringer, registreres ændringen i antal og priser i vareposterne og værdiposterne. For at afspejle ændringen af lagerværdien i dine finansielle regnskaber skal du bogføre lagerværdien i de relaterede lagerkonti i finansbogholderiet.

Du kan bogføre lagerværdier i finansregnskabet på to måder:

- Automatisk, så lagerværdier bogføres i finansregnskabet, hver gang du bogfører en lagertransaktion.
- Manuelt, så lagerværdier kun bogføres i finansregnskabet, når du foretager en kørsel.


## <a name="to-post-inventory-costs-automatically"></a>Sådan bogføres lagerværdier automatisk
1. I øverste højre hjørne skal du vælge ikonet **Søg efter side eller rapport**, angive **Lageropsætning** og derefter vælge det relaterede link.
2. I vinduet **Lageropsætning** skal du markere afkrydsningsfeltet **Aut. lagerværdibogføring**.

For hver lagertransaktion du bogfører, bogføres den relevante værdi på lagerkontoen, reguleringskontoen og vareforbrugskontoen i finansregnskabet.

Selvom du bruger automatisk bogføring af lagerværdien, er det stadig nødvendigt at udføre kørslen Reguler kostværdi - vareposter jævnligt for at sikre, at værdien af varerne overføres til de relevante udgående transaktioner, f.eks salg eller overflytninger. Dette er især vigtigt i de situationer, hvor du sælger varer, inden du fakturerer købet af varerne.

Hvis der opstår fejl i opsætningen af dimensioner under bogføring af lagerværdien i finansregnskabet, vil bogføringen blive afsluttet med en fejl.

## <a name="to-post-inventory-costs-manually"></a>Sådan bogføres lagerværdier manuelt
1. I øverste højre hjørne skal du vælge ikonet **Søg efter side eller rapport**, angive **Bogfør lageromkostninger til finans** og derefter vælge det relaterede link.
2. Du kan bogføre lagerværdier i finansregnskabet ved at udføre kørslen. Når du udfører denne kørsel, oprettes finansposter ud fra værdiposterne. Du kan bogføre posterne, så de opsummeres pr. bogføringsgruppe.

**Bemærk**: Når du udfører kørslen, kan du finde fejl, der relaterer til manglende opsætning eller inkompatibel opsætning af dimensioner. Hvis kørslen finder fejl i opsætningen af dimensioner, bliver disse fejl tilsidesat, og kørslen bruger dimensionerne for værdiposten. For alle andre typer fejl springer kørslen bogføring af værdiposter over, og anfører dem i slutningen af rapporten under overskriften “Poster, der er sprunget over”. Du skal rette fejlene, inden du kan bogføre posterne.

Hvis du vil se en liste over fejl før kørslen af bogføringen, kan du køre rapporten **Bogfør lageromkostning - kontrol**. Denne kontrolrapport viser alle de fejl, som fanges under en bogføringstest. Du kan derefter rette fejlene og udføre kørslen til bogføring af lagerreguleringer uden at springe nogen poster over.

Hvis du ganske enkelt vil have en oversigt over, hvilke værdier der kan bogføres i finansregnskabet uden at gennemføre bogføringen, kan du udføre kørslen Bogfør lagerregulering uden at bogføre værdierne i finansregnskabet. Dette kan du gøre ved at fjerne markeringen i feltet Bogfør på anmodningssiden. Når du derefter udfører kørslen, oprettes der kun en rapport, der viser de værdier, der er klar til at blive bogført i finansregnskabet, men de er ikke bogført.

## <a name="see-also"></a>Se også
[Administrere lager](inventory-manage-inventory.md)    
[Fremgangsmåde: Regulere varepriser](inventory-how-adjust-item-costs.md)  
[Administrere salg](sales-manage-sales.md)  
[Administrere køb](purchasing-manage-purchasing.md)

