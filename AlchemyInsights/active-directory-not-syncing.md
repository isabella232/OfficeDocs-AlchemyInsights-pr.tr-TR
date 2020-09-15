---
title: Active Directory eşitlenmiyor
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
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697649"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="81142-102">Active Directory eşitlenmiyor</span><span class="sxs-lookup"><span data-stu-id="81142-102">Active Directory not syncing</span></span>

<span data-ttu-id="81142-103">"Son eşitleme yok" gibi eşitleme hataları alıyorsanız veya Office Admin portalında Dizin eşitleme durumunun "en son 3 gün önce eşitlendi" ifadesinin olduğunu fark ederseniz, "en fazla 3 gün önce eşitlendi</span><span class="sxs-lookup"><span data-stu-id="81142-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="81142-104">Hızlı ayarlar 'ı kullanarak AADConnect 'in yeniden yüklenmesi sorunu hemen çözebilir:</span><span class="sxs-lookup"><span data-stu-id="81142-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="81142-105">[AADConnect 'in en son sürümünü indirin](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="81142-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="81142-106">[Hızlı yükleme yönergelerini izleyin](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="81142-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="81142-107">AADConnect hizmet hesapları hakkında daha fazla bilgi için [Azure AD Connect: hesaplar ve izinler](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)bölümüne bakın.</span><span class="sxs-lookup"><span data-stu-id="81142-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
