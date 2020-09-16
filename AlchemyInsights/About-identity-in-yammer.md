---
title: Yammer 'daki kimlik hakkında
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664190"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="1476b-102">Yammer 'daki kimlik hakkında</span><span class="sxs-lookup"><span data-stu-id="1476b-102">About identity in Yammer</span></span>

<span data-ttu-id="1476b-103">Tüm ağların, kimlikte ilgili sorunlardan kaçınmak için aşağıdaki adımları kullanmaları önerilir:</span><span class="sxs-lookup"><span data-stu-id="1476b-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="1476b-104">Azure AD 'deki kullanıcılar için Microsoft 365 hesapları hazırladıktan sonra, tüm kullanıcıların birincil Microsoft 365 hesabını kullanarak oturum açmasını sağlamak için Office 365 kimliği 'ni zorlayın.</span><span class="sxs-lookup"><span data-stu-id="1476b-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="1476b-105">Daha fazla bilgi için [Yammer kullanıcıları Için Office 365 kimlik](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="1476b-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="1476b-106">Birden çok Yammer ağını birleştirin.</span><span class="sxs-lookup"><span data-stu-id="1476b-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="1476b-107">Eski Yammer yapılandırmaları birden çok Yammer ağına tek bir kiracıya bağlanmasına olanak verir.</span><span class="sxs-lookup"><span data-stu-id="1476b-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="1476b-108">Daha fazla bilgi için bkz: [ağ geçişi-birden çok Yammer ağını birleştirme](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span><span class="sxs-lookup"><span data-stu-id="1476b-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="1476b-109">İsteğe bağlı olarak, Yammer lisansı yoksa kullanıcıların Yammer 'ı engellemesine gerek vardır.</span><span class="sxs-lookup"><span data-stu-id="1476b-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="1476b-110">Daha fazla bilgi için [Office 365 'Da Yammer kullanıcı lisanslarını yönetme](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="1476b-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="1476b-111">Son olarak, eski Yammer ağlarının Kullanıcı listesini denetleyin ve eski kullanıcıları askıya alın.</span><span class="sxs-lookup"><span data-stu-id="1476b-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="1476b-112">Silme işlemi geri alınamaz olduğundan kullanıcıları silmek yerine askıya almanız (devre dışı bırakmanız) tavsiye edilir.</span><span class="sxs-lookup"><span data-stu-id="1476b-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="1476b-113">Daha fazla bilgi için, [Office 365 'e bağlı ağlardaki Yammer kullanıcılarını denetleme](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) ve [kullanıcıları kaldırma](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="1476b-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="1476b-114">Yammer 'ı bu adımları kullanarak yapılandırarak, Yammer ağınızı Microsoft 365 için doğal mod için yapılandırmaya de hazırsınız.</span><span class="sxs-lookup"><span data-stu-id="1476b-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="1476b-115">Daha fazla bilgi için [Yammer ağınızı Microsoft 365 Için yerel mod Için yapılandırma](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode)bölümüne bakın.</span><span class="sxs-lookup"><span data-stu-id="1476b-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>