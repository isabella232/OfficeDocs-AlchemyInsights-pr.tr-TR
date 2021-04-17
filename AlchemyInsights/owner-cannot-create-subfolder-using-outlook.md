---
title: Sahip Outlook'u kullanarak alt klasör oluşturamaz
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836155"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="840de-102">Sahip Outlook'u kullanarak alt klasör oluşturamaz</span><span class="sxs-lookup"><span data-stu-id="840de-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="840de-103">**Ortak klasör sahiplerinin Outlook kullanarak alt klasör oluşturması sorunu devam ediyor. Sorun yakında giderilecek.**</span><span class="sxs-lookup"><span data-stu-id="840de-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="840de-104">Bu sırada, aşağıdaki geçici çözümlerden birini kullanın:</span><span class="sxs-lookup"><span data-stu-id="840de-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="840de-105">Alt klasörü oluşturmak için MAC için Outlook'u kullanın, bu sorun yalnızca Masaüstü için Outlook pencerelerini etkiler (tüm sürümler)</span><span class="sxs-lookup"><span data-stu-id="840de-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="840de-106">Yöneticinin EXO Shell veya EAC kullanarak alt klasör oluşturmasını</span><span class="sxs-lookup"><span data-stu-id="840de-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="840de-107">Kullanıcıda DefaultPublicFolderMailbox/EffectivePublicFolderMailbox'i, soruna neden olan klasörün İçerik Posta Kutusu'dan başka bir posta kutusuyla değiştirme</span><span class="sxs-lookup"><span data-stu-id="840de-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="840de-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="840de-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="840de-109">Bir saat bekleyin, Outlook istemcisini yeniden başlatın</span><span class="sxs-lookup"><span data-stu-id="840de-109">Wait for an hour, restart outlook client</span></span>