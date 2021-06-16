---
title: Active Directory eşitli değil
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
- "9001688"
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 0da512379e5a2f6ccb773e18c465e545c0660560
ms.sourcegitcommit: e42bb24c9bae1d0df8c49c424d2aa5e7466703ac
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/14/2021
ms.locfileid: "52930995"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="36c9d-102">Active Directory eşitli değil</span><span class="sxs-lookup"><span data-stu-id="36c9d-102">Active Directory not syncing</span></span>

<span data-ttu-id="36c9d-103">"Yakın zamanda eşitleme yok" gibi eşitleme hataları alıyorsanız veya Office yönetim portalında dizin eşitleme durumunun "Son eşitleme 3 gün önce" olarak açıklanmış olduğunu fark ederseniz, AADConnect'in yanlış ayarları veya eşitlemeyi gerçekleştirmek için yetersiz izinleri olabilir.</span><span class="sxs-lookup"><span data-stu-id="36c9d-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="36c9d-104">Hızlı ayarları kullanarak AADConnect'in yeniden yüklenmesi sorunu hızla çözebilir:</span><span class="sxs-lookup"><span data-stu-id="36c9d-104">Reinstalling AADConnect by using express settings might resolve the issue quickly:</span></span>

1. <span data-ttu-id="36c9d-105">[AADConnect'in en son sürümünü indirin.](https://go.microsoft.com/fwlink/?LinkId=615771)</span><span class="sxs-lookup"><span data-stu-id="36c9d-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="36c9d-106">[Hızlı yükleme yönergelerini izleyin.](/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="36c9d-106">[Follow the instructions for express installation](/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="36c9d-107">Azure AD Connect, Windows Server 2012 veya sonraki sürümlerde yüklü olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="36c9d-107">Azure AD Connect must be installed on Windows Server 2012 or later.</span></span> <span data-ttu-id="36c9d-108">Etki alanına katılmış olması gereken bu sunucu, etki alanı denetleyicisi veya üye sunucu olabilir.</span><span class="sxs-lookup"><span data-stu-id="36c9d-108">This server must be domain joined and may be a domain controller or a member server.</span></span> <span data-ttu-id="36c9d-109">Azure AD Önkoşullarının tam listesi Bağlan önkoşulları için Azure [AD](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)Önkoşulları'Bağlan.</span><span class="sxs-lookup"><span data-stu-id="36c9d-109">For a full list of Azure AD Connect requirements and pre-requisites, review [Prerequisites for Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).</span></span>

<span data-ttu-id="36c9d-110">AADConnect hizmet hesapları hakkında daha fazla bilgi için bkz. [Azure AD Bağlan: Hesaplar ve izinler.](/azure/active-directory/hybrid/reference-connect-accounts-permissions)</span><span class="sxs-lookup"><span data-stu-id="36c9d-110">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
