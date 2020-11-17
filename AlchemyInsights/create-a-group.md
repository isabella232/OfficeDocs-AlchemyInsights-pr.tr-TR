---
title: Grup oluşturma
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/17/2020
ms.locfileid: "49089179"
---
# <a name="create-a-group"></a><span data-ttu-id="e44b8-102">Grup oluşturma</span><span class="sxs-lookup"><span data-stu-id="e44b8-102">Create a group</span></span>

<span data-ttu-id="e44b8-103">Bu konuda, Grup oluşturma açıklanmaktadır.</span><span class="sxs-lookup"><span data-stu-id="e44b8-103">This topic describes group creation.</span></span>

<span data-ttu-id="e44b8-104">**Grup oluşturma izni**</span><span class="sxs-lookup"><span data-stu-id="e44b8-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="e44b8-105">Yeni Grup oluşturma yetkiniz olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="e44b8-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="e44b8-106">Genel Yöneticiler, Azure portalında veya erişim panelinde grup oluşturmayı devre dışı bırakabilir.</span><span class="sxs-lookup"><span data-stu-id="e44b8-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="e44b8-107">Size yeni grup oluşturmak veya size uygun izinleri vermek için bir yöneticiye ihtiyacınız olabilir.</span><span class="sxs-lookup"><span data-stu-id="e44b8-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="e44b8-108">**Grup oluşturma izinlerini yönetme**</span><span class="sxs-lookup"><span data-stu-id="e44b8-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="e44b8-109">Genel Yöneticiler, Grup oluşturma izinlerini (güvenlikle ilgili nedenler için) veya Azure portalında veya erişim panelinde oluşturulmuş olan Office 365 gruplarını, tüm gruplardaki genel (Ayarlar) seçenekleri 365 belirleyerek, **Tüm gruplardaki**  >  **Genel (Ayarlar)**</span><span class="sxs-lookup"><span data-stu-id="e44b8-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="e44b8-110">Ayrıca, Azure Active Directory P1 Premium lisansına sahipseniz, Grup oluşturmayı kısıtlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="e44b8-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="e44b8-111">**Yeni Office 365 grubu üyeleri için hoş geldiniz bildirimini devre dışı bırakma**</span><span class="sxs-lookup"><span data-stu-id="e44b8-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="e44b8-112">Office 365 gruplarına eklenen kullanıcılara gönderilen hoş geldiniz bildirimi, **UnifiedGroupWelcomeMessageEnabled** .</span><span class="sxs-lookup"><span data-stu-id="e44b8-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="e44b8-113">Bu [ayarı hakkında](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)bilgi edinin.</span><span class="sxs-lookup"><span data-stu-id="e44b8-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

