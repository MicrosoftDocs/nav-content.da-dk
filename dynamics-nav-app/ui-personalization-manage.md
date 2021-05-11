---
title: Administrere tilpasning som administrator
description: "Få at vide, hvordan du kan tilpasse brugergrænsefladen, så den passer til din måde at arbejde på."
documentationcenter: 
author: jswymer
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 07/26/2017
ms.author: jswymer
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: e3d088c35efca4d62b7db1f0d44d5ef2958317d4
ms.contentlocale: da-dk
ms.lasthandoff: 10/16/2017

---
# <a name="managing-personalization-as-an-administrator"></a>Administrere tilpasning som administrator
Brugere kan tilpasse deres arbejdsområde, så det passer til deres egne præferencer. Som administrator kan du kan styre og administrere tilpasning ved at deaktivere brugernes mulighed for at tilpasse sider og ved at fjerne alle sidetilpasninger, som brugere har foretaget.

## <a name="disable-personalization-for-a-profile"></a>Deaktivere tilpasning for en profil
Du kan forhindre alle brugere, der tilhører en bestemt profil, i at tilpasse deres sider.
1.  Vælg ikonet ![Søg efter side eller rapport](media/ui-search/search_small.png "Ikonet Søg efter side eller rapport"), angiv **Profiler**, og vælg derefter det relaterede link.
2.  Vælg den profil på listen, der skal ændres.
3.  Markér afkrydsningsfeltet **Deaktiver tilpasning**, og vælg derefter knappen **OK**.

## <a name="clear-user-personalizations"></a>Fjern brugertilpasninger

Når sidetilpasninger fjernes, går siden tilbage til det oprindelige layout, før der blev foretaget nogen tilpasning. Tilpasninger, som brugere har foretaget af sider, kan fjernes på to måder: ved brug af siden **Slet brugertilpasning** side og ved brug af siden **Brugertilpasningskort**.

### <a name="clear-user-personalizations-by-using-the-delete-user-personalization-page"></a>Slette brugertilpasninger ved brug af siden Slet brugertilpasning

Siden **Slet brugertilpasning** giver dig mulighed for at slette tilpasning på side- eller brugerbasis.

1.  Vælg ikonet ![Søg efter side eller rapport](media/ui-search/search_small.png "Ikonet Søg efter side eller rapport"), angiv **Slet brugertilpasning**, og vælg derefter det relaterede link.

    Siden viser alle de sider, der er blevet tilpasset, og den bruger, de tilhører.

    >[!NOTE]
    > Afkrydsningsfeltet i kolonnen **Ældre tilpasning** angiver, at tilpasningen er udført udelukkende ved hjælp af [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)], og/eller den er foretaget i [!INCLUDE[nav_web_md](includes/nav_web_md.md)] forud for [!INCLUDE[navnow_md](includes/navnow_md.md)]. Brugere, som forsøger at tilpasse siderne ved hjælp af [!INCLUDE[nav_web_md](includes/nav_web_md.md)], er blokeret fra at gøre det, medmindre de vælger at låse siden op. Du kan finde flere oplysninger i [Derfor er en side spærret for tilpasning](ui-personalization-locked.md). Du kan finde yderligere oplysninger om tilpasning mellem [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] og [!INCLUDE[nav_web_md](includes/nav_web_md.md)], i [Arbejde med tilpasning mellem Dynamics NAV Windows- og webklinten](ui-personalization-overview.md#PersonalizationWinWeb).

2. Marker den post, du vil slette, og vælg derefter handlingen **Slet**.

    Brugerne vil se ændringerne, næste gang de logger på.

### <a name="clear-user-personalizations-by-using-the-user-personalization-card-page"></a>Slette brugertilpasninger ved brug af siden Brugertilpasningskort

Siden **Brugertilpasningskort** giver dig mulighed for at slette tilpasningen på alle sider for en specifik bruger. Det kræver skrivetilladelse til tabel 2000000072 **Profil**.

1.  Vælg ikonet ![Søg efter side eller rapport](media/ui-search/search_small.png "Ikonet Søg efter side eller rapport"), angiv **Brugertilpasning**, og vælg derefter det relaterede link.

    Siden **Brugertilpasning** viser alle brugere, der muligvis kan have personlige sider. Hvis du ikke kan finde en bruger på listen, betyder det, at vedkommende ikke har nogen tilpassede sider.

2. Vælg brugeren på listen, og vælg derefter handlingen **Rediger**.

3.  Under fanen **Handlinger** skal du vælge **Fjern tilpassede sider**.

    Brugerne vil se ændringerne, næste gang de logger på.

## <a name="see-also"></a>Se også
[Oversigt over tilpasning](ui-personalization-overview.md)  
[Tilpasse dit arbejdsområde](ui-personalization-user.md)  
[Arbejde med [!INCLUDE[navnow_md](includes/navnow_md.md)]](ui-work-product.md)  
[Fremgangsmåde: Ændre rollecentret](change-role.md)  
