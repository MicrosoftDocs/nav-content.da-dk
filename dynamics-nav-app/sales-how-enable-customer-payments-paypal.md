---
title: "Fremgangsmåde: Aktivere debitorbetalinger via PayPal"
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
ms.openlocfilehash: 15f30a03c3e7ccc865ef527a707794c2c6428b2f
ms.contentlocale: da-dk
ms.lasthandoff: 10/16/2017

---

# <a name="how-to-enable-customer-payments-through-paypal"></a>Fremgangsmåde: Aktivere debitorbetalinger via PayPal#
Som et alternativ til opkrævning af betalinger via bankoverførsel eller kreditkort kan du tilbyde dine kunder at betale via deres PayPal-konto.

Når en kunde vælger PayPal-linket i en salgsfaktura eller et salgsordredokument, vises servicesiden for deres PayPal-konto med betalingsoplysningerne for salget. Kunden kan derefter betale fakturaen som andre PayPal-betalinger.

Hvis du vil aktivere debitorbetalinger via PayPal, skal du gøre følgende:

1. Konfigurer PayPal Payments Standard som en betalingstjeneste i vinduet **Betalingstjenester**.
2. Vælg PayPal Payments Standard i feltet **Betalingstjeneste** i salgsdokumentet.

PayPal Payments Standard-tjenesten er installeret som en udvidelse til Dynamics NAV og klar til at blive aktiveret. Du kan finde flere oplysninger i [Tilpasse Dynamics NAV ved hjælp af udvidelser](ui-extensions.md).

## <a name="to-enable-the-paypal-payments-standard-service"></a>Sådan aktiveres tjenesten PayPal Payments Standard
1. I øverste højre hjørne skal du vælge ikonet **Søg efter side eller rapport**, **Betalingstjenester** og derefter vælge det relaterede link.  
2. I vinduet **Betalingstjenester** skal du vælge handlingen **Ny**.
3. Vælg **PayPal Standard**, og luk derefter vinduet.
4. I vinduet **Betalingstjenester** skal du vælge handlingen **Konfigurer**.
5. Udfyld felterne efter behov. Vælg et felt for at læse en kort beskrivelse af det eller et link til flere oplysninger.

    **Bemærk**: Marker afkrydsningsfeltet **Medtag altid på dokumenter**, hvis hyperlinket til PayPal-betalingstjenesten skal altid være synlig på salgsdokumenter, hvor betaling gennem PayPal er aktiveret.

6. Luk vinduet.

## <a name="to-select-paypal-payments-standard-on-a-sales-invoice"></a>Sådan vælges PayPal Payments Standard på en salgsfaktura
1. På startsiden skal du vælge handlingen **Salgsfakturaer**.
2. Åbn den salgsfaktura, du vil aktivere PayPal-betalinger for.
3. I feltet **Betalingstjeneste** skal du vælge PayPal Payments Standard.

**Bemærk**: Feltet **Betalingstjeneste** er kun synligt, hvis PayPal Payments Standard-tjenesten er aktiveret.   

## <a name="see-also"></a>Se også  
[Konfigurere salg](sales-setup-sales.md)  
[Administrere salg](sales-manage-sales.md)  
[Tilpasse Dynamics NAV ved hjælp af udvidelser](ui-extensions.md)

