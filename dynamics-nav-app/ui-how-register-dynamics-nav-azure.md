---
title: "Sådan registreres Dynamics NAV på Azure Management-portalen"
author: edupont04
manager: edupont
ms.author: edupont
ms.custom: na
ms.date: 11/15/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: d41b96ab5807402a342991d5c5bc2d672db09e2f
ms.contentlocale: da-dk
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-register-dynamics-nav-in-the-azure-management-portal"></a>Sådan registreres Dynamics NAV på Azure Management-portalen
Hvis du vil bruge tjenester, der er baseret på Microsoft Azure, skal du registrere Dynamics NAV på Azure Management-portalen. Udvidelsen [Salgs- og lagerprognose](ui-extensions-sales-forecast.md) kræver eksempelvis, at du angiver en API-nøgle og URI'et for API og andre tjenester kræver tilsvarende oplysninger. Hvor finder du disse oplysninger?

Du kan bruge vejledningen **Konfigurere Azure Management-portal** til at registrere Dynamics NAV på Azure Management-porten og hente de oplysninger, du skal bruge for at benytte tjenester, f.eks udvidelsen Salgs- og lagerprognose, Power BI, Office 365 osv. Du skal kun registrere dig på Azure Management-portalen én gang, og du skal være en administrator eller superbruger i Dynamics NAV.

Formålet med registreringen er, at Dynamics NAV og den tjeneste, som du vil oprette forbindelse til, skal kende oplysningerne for Azure Active Directory (Azure AD) for hinanden.

## <a name="to-register-dynamics-nav-in-the-azure-management-portal"></a>Sådan registreres Dynamics NAV på Azure Management-portalen
1. Log ind på Azure-administrationsportalen på [https://portal.azure.com](https://portal.azure.com). Hvis du ikke kender Azure-administrationsportalen, kan du finde vejledning i [Azure-dokumentationsbiblioteket](https://azure.microsoft.com/en-us/documentation/articles).
2. I venstre navigationsrude skal du vælge **Flere tjenester** og derefter vælge **Appregistreringer**.
3. Vælg **Tilføj** i den øverste menu, og udfyld derefter feltet **Opret rude** i felterne med følgende oplysninger:
    - **Navn**: Angiv et navn til Dynamics NAV-løsningen, f.eks *Dynamics NAV*.
    - **Programtype**: Vælg **Webapp*/API**.
    - **URL-adresse til pålogning**: Angiv URL-adressen til Dynamics NAV-browserklienten, f.eks *https://MyServer:8080/DynamicsNAV/WebClient/OAuthLanding.htm*.
        Filen OAuthLanding.htm hjælper med at administrere udveksling af data mellem Dynamics NAV og andre tjenester via Azure AD.
4. Vælg knappen **Opret**.
    Dette tilføjer Dynamics NAV til ruden **Appregistreringer**, så du kan nu føje indstillinger til den.
5. I listen **Appregistreringer** skal du vælge den nye app. Hvis ruden **Indstillinger** ikke åbnes, vil du få vist en handling til at åbne **Indstillinger**.
6. I ruden **Indstillinger** i sektionen **API-adgang** skal du vælge **Nøgler**.
7. I ruden **Nøgler** skal du angive en beskrivelse, og hvornår du vil lade nøgle udløbe, og derefter vælge **Gem**.
8. Kopier den genererede nøgle til en midlertidig lokation - du skal bruge den i næste procedure.
9. I sektionen **API-adgang** skal du vælge **Krævede tilladelser**.
    - Tilføj uddelegerede tilladelser for at få vist alle rapporter fra Power BI-tjenester
    - Tilføj uddelegerede tilladelser for at logge på og læse brugerprofil for Windows Azure Active Directory
    - Gentag for andre tjenester, du vil give adgang til Dynamics NAV
10. Luk ruden **Indstillinger**, og i ruden **Essentials** skal du derefter kopiere værdien for **Progam-id** til en midlertidig lokation.

Du har nu registreret Dynamics NAV på Azure Management-portalen, du har givet adgang til de relevante tjenester, og du har hentet de oplysninger, der er nødvendige i Dynamics NAV.  

## <a name="to-add-the-information-to-dynamics-nav"></a>Sådan føjes oplysninger til Dynamics NAV
1. I øverste højre hjørne skal du vælge ikonet **Søg efter side eller rapport**, angive **Konfiguration af guiden Azure AD-installation** og derefter vælge det relaterede link.
2. I guiden skal du vælge **Næste**.
3. I feltet **Klient-id** skal du angive det indhold, som du tidligere har kopieret fra feltet **Program-id**.
4. I feltet **Hemmelig nøgle** skal du angive det indhold, som du tidligere har kopieret fra ruden **Nøgler**.
5. Vælg **Næste**. Medmindre du får vist en fejlmeddelelse, er proceduren nu fuldført.

Din Dynamics NAV er registreret og klar til at oprette forbindelse til tjenester såsom Cortana Intelligence og Power BI.

## <a name="see-also"></a>Se også
[Salgs- og lagerprognose](ui-extensions-sales-forecast.md)  
[Konfigurere din Dynamics NAV](setup.md)  

