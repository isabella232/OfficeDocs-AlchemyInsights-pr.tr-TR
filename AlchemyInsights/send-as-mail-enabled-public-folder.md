---
title: EXO 'da posta olarak etkin ortak klasör olarak gönder
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: ed62c6d7db0ae532f806ce4fdc48f42623bcd545
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/13/2020
ms.locfileid: "48462076"
---
# <a name="sendas-mail-enabled-public-folder"></a><span data-ttu-id="00dc8-102">SendAs mail etkin ortak klasör</span><span class="sxs-lookup"><span data-stu-id="00dc8-102">SendAs Mail Enabled Public Folder</span></span>

<span data-ttu-id="00dc8-103">Aşağıdaki örnek, Kullanıcı Jason posta etkin ortak klasörü için "Farklı Gönder" izinlerini atar.</span><span class="sxs-lookup"><span data-stu-id="00dc8-103">The following example assigns "Send As" permissions for the mail-enabled public folder NewPF1 to the user Jason.</span></span>

<span data-ttu-id="00dc8-104">Add-RecipientPermission-IDENTITY ' NewPF1 '-güvenilen "Jason"-AccessRights ' SendAs '</span><span class="sxs-lookup"><span data-stu-id="00dc8-104">Add-RecipientPermission -Identity 'NewPF1' -Trustee "Jason" -AccessRights 'SendAs'</span></span>

<span data-ttu-id="00dc8-105">Ayrıntılı sözdizimi ve parametre bilgileri için [posta etkinleştirilmiş ortak klasörler için "Farklı Gönder" veya "adına Gönder" izinlerinin](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs)bakın.</span><span class="sxs-lookup"><span data-stu-id="00dc8-105">For detailed syntax and parameter information see [Assign "Send As" or "Send on Behalf" permissions for mail-enabled public folders](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).</span></span>

