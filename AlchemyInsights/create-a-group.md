---
title: Grup oluşturma
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816392"
---
# <a name="create-a-group"></a><span data-ttu-id="cd994-102">Grup oluşturma</span><span class="sxs-lookup"><span data-stu-id="cd994-102">Create a group</span></span>

<span data-ttu-id="cd994-103">Bu konu başlığında grup oluşturma açıklanmıştır.</span><span class="sxs-lookup"><span data-stu-id="cd994-103">This topic describes group creation.</span></span>

<span data-ttu-id="cd994-104">**Grup Oluşturma İzni**</span><span class="sxs-lookup"><span data-stu-id="cd994-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="cd994-105">Yeni grup oluşturma yetkinizin olduğundan emin olmak.</span><span class="sxs-lookup"><span data-stu-id="cd994-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="cd994-106">Genel yöneticiler Azure portalda veya Erişim Masası'nda grup oluşturma özelliğini devre dışı bırakabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="cd994-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="cd994-107">Sizin için yeni grup oluşturmak veya size uygun izinleri vermek için bir yöneticiye ihtiyacınız olabilir.</span><span class="sxs-lookup"><span data-stu-id="cd994-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="cd994-108">**Grup oluşturma izinlerini yönetme**</span><span class="sxs-lookup"><span data-stu-id="cd994-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="cd994-109">Genel yöneticiler, Tüm gruplar Genel   >  **(Ayarlar)** içinde "Kullanıcılar Azure portallarında güvenlik grupları oluşturabilir" veya "Kullanıcılar Azure portallarında Office 365 grupları oluşturabilir" seçeneklerini seçerek (güvenlikle ilgili nedenlerle) Azure portalında veya Erişim Paneli'de oluşturulan Office 365 gruplarını yönetebilir.</span><span class="sxs-lookup"><span data-stu-id="cd994-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="cd994-110">Azure Active Directory P1 Premium lisansınız varsa, grup oluşturma seçeneğini kısıtlayan bir kullanıcı grubu da kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="cd994-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="cd994-111">**Yeni Office 365 grup üyeleri için karşılama bildirimini devre dışı bırakma**</span><span class="sxs-lookup"><span data-stu-id="cd994-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="cd994-112">Office 365 gruplarına eklenen kullanıcılara gönderilen karşılama bildirimi, Powershell'de **UnifiedGroupWelcomeMessageEnabled** değeri False olarak ayarlanabilir.</span><span class="sxs-lookup"><span data-stu-id="cd994-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="cd994-113">Bu ayar hakkında buradan bilgi [öğrenebilirsiniz.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="cd994-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

