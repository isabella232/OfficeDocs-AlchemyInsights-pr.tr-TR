---
title: Yammer kimlik hakkında
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 2c4c2c836d18d2ab45e2368e778c793277b18aa0
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148424"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="5c544-102">Yammer kimlik hakkında</span><span class="sxs-lookup"><span data-stu-id="5c544-102">About identity in Yammer</span></span>

<span data-ttu-id="5c544-103">Tüm ağların kimlikle ilgili sorunları önlemek için aşağıdaki adımları atması önerilir:</span><span class="sxs-lookup"><span data-stu-id="5c544-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="5c544-104">Tüm kullanıcıların birincil Microsoft 365 hesaplarını kullanarak oturum açmalarını sağlamak için Azure AD'deki kullanıcılar için Microsoft 365 hesaplarını verdikten sonra Office 365 kimliğini uygulayın.</span><span class="sxs-lookup"><span data-stu-id="5c544-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="5c544-105">Daha fazla bilgi için, [Yammer kullanıcıları için Office 365 kimliğini zorla'](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity)ya bakın.</span><span class="sxs-lookup"><span data-stu-id="5c544-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="5c544-106">Birden çok Yammer abunu birleştirin.</span><span class="sxs-lookup"><span data-stu-id="5c544-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="5c544-107">Eski Yammer yapılandırmaları, birden çok Yammer abunun bir kiracıya bağlanmasına izin verir.</span><span class="sxs-lookup"><span data-stu-id="5c544-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="5c544-108">Daha fazla bilgi için bkz: [Ağ geçişi - Birden çok Yammer ağlarını birleştirin.](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)</span><span class="sxs-lookup"><span data-stu-id="5c544-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="5c544-109">İsteğe bağlı olarak, Yammer'ın kullanıcıların lisansları yoksa Yammer'ı engellemesi için lisans lamayı zorlar.</span><span class="sxs-lookup"><span data-stu-id="5c544-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="5c544-110">Daha fazla bilgi için Office [365'teki Yammer kullanıcı lisanslarını yönet'e](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)bakın.</span><span class="sxs-lookup"><span data-stu-id="5c544-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="5c544-111">Son olarak, eski Yammer ağları için kullanıcı listesini denetleyin ve eski kullanıcıları askıya alın.</span><span class="sxs-lookup"><span data-stu-id="5c544-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="5c544-112">Silme geri alınamaz olduğundan, kullanıcıları siletmek yerine askıya almanız (devre dışı bırakmanız) önerilir.</span><span class="sxs-lookup"><span data-stu-id="5c544-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="5c544-113">Daha fazla bilgi için bkz: [Office 365'e bağlı ağlardaki Denetim Yammer kullanıcıları](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) ve [kullanıcıları kaldır.](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users)</span><span class="sxs-lookup"><span data-stu-id="5c544-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="5c544-114">Yammer'ı bu adımları kullanarak yapılandırarak, Yammer ağınızı Microsoft 365 için Yerel Mod için yapılandırmaya da hazır olacaksınız.</span><span class="sxs-lookup"><span data-stu-id="5c544-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="5c544-115">Daha fazla bilgi için, [Microsoft 365 için Yerel Mod için Yammer ağınızı yapılandırın' a](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode)bakın.</span><span class="sxs-lookup"><span data-stu-id="5c544-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>