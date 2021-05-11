---
title: Konfiguration af arbejdsgangsnotifikationer
description: "Mange arbejdsgangssvar vedrører notifikationer til en bruger om, at der er forekommet en hændelse, som brugeren skal reagere på. F.eks. på kan hændelsen på ét arbejdsgangstrin være, at bruger 1 anmoder om godkendelse af en ny post, og svaret er, at der er sendt en notifikation til bruger 2, godkenderen. På næste arbejdsgangstrin kan hændelsen være, at bruger 2 godkender posten, og svaret er, at der er sendt en notifikation til bruger 3 om at påbegynde en relateret behandling af den godkendte post. For trin i arbejdsgangen, der vedrører godkendelse, er hver notifikation knyttet til en godkendelsespost."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 2c3e64a5d343bad026ba5417f18861ef6417dae3
ms.contentlocale: da-dk
ms.lasthandoff: 10/16/2017

---
# <a name="setting-up-workflow-notifications"></a>Konfiguration af arbejdsgangsnotifikationer
Mange arbejdsgangssvar vedrører notifikationer til en bruger om, at der er forekommet en hændelse, som brugeren skal reagere på. F.eks. på kan hændelsen på ét arbejdsgangstrin være, at bruger 1 anmoder om godkendelse af en ny post, og svaret er, at der er sendt en notifikation til bruger 2, godkenderen. På næste arbejdsgangstrin kan hændelsen være, at bruger 2 godkender posten, og svaret er, at der er sendt en notifikation til bruger 3 om at påbegynde en relateret behandling af den godkendte post. For trin i arbejdsgangen, der vedrører godkendelse, er hver notifikation knyttet til en godkendelsespost. Du kan finde flere oplysninger i [Workflow](across-workflow.md).  

> [!NOTE]  
>  Den generiske version af [!INCLUDE[d365fin](includes/d365fin_md.md)] understøtter notifikationer som mail og som interne noter.  

> [!IMPORTANT]  
>  Alle arbejdsgangsnotifikationer sendes via en opgavekø. Kontrollér, at opgaven kommer i kø i løsningen. Du kan finde flere oplysninger i [Brug af opgavekøer til at planlægge opgaver](admin-job-queues-schedule-tasks.md).

Du konfigurerer forskellige aspekter af arbejdsgangsnotifikationer følgende steder:  

1.  For godkendelsesarbejdsgange konfigurerer du modtagerne af arbejdsgangsnotifikationer ved at udfylde en linje i vinduet **Konfiguration af godkendelsesbruger** for hver bruger, der indgår i arbejdsprocessen. Hvis f.eks. bruger 2 angives i feltet **Godkender-id** på linjen for bruger 1, sendes notifikationen for godkendelsesanmodningen til bruger 1. Du kan finde flere oplysninger i [Fremgangsmåde: Konfigurere godkendelsesbrugere](across-how-to-set-up-approval-users.md)  
2.  Du kan konfigurere, hvornår og hvordan brugere får arbejdsgangsnotifikationer, ved at udfylde vinduet **Notifikationsplan** for hver bruger i arbejdsgangen. Du kan finde flere oplysninger i [Fremgangsmåde: Angive, hvornår og hvordan notifikationer modtages](across-how-to-specify-when-and-how-to-receive-notifications.md).  
3.  Du konfigurerer det generelle indhold og layout for notifikationer, herunder notifikationer om forfaldne arbejdsgangssvar, ved at konfigurere notifikationsskabeloner i vinduet **Notifikationsskabeloner**. Du kan bruge de standardskabeloner, der er leveret sammen med [!INCLUDE[d365fin](includes/d365fin_md.md)].  
4.  Du konfigurerer det specifikke indhold og de specifikke regler for en arbejdsgangsnotifikation, når du opretter den pågældende arbejdsgang. Det gør du ved at vælge indstillinger i vinduet **Indstillinger for workflowrespons** for det arbejdsgangssvar, der repræsenterer notifikationen. Du kan finde flere oplysninger i trin 9 i [Fremgangsmåde: Oprette arbejdsgange](across-how-to-create-workflows.md).  

## <a name="see-also"></a>Se også  
 [Fremgangsmåde: Konfigurere godkendelsesbrugere](across-how-to-set-up-approval-users.md)   
 [Fremgangsmåde: Oprette brugere til arbejdsgange](across-how-to-set-up-workflow-users.md)   
 [Fremgangsmåde: Angive, hvornår og hvordan notifikationer modtages](across-how-to-specify-when-and-how-to-receive-notifications.md)   
 [Fremgangsmåde: Oprette arbejdsgange](across-how-to-create-workflows.md)   
 [Fremgangsmåde: Administrere notifikationsskabeloner](across-how-to-manage-notification-templates.md)   
 [Du kan bruge opgavekøer til at planlægge opgaver](admin-job-queues-schedule-tasks.md)   
 [Fremgangsmåde: Konfigurere mail](madeira-how-setup-email.md)   
 [Gennemgang: Opsætning og brug af workflow for godkendelse af køb](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md)   
 [Workflow](across-workflow.md)   

