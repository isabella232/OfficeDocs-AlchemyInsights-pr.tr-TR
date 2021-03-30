---
title: Single-Sign Active Directory'ye katılmış cihazlar için daha fazla bilgi edinin
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405664"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a><span data-ttu-id="26783-102">Azure Active Directory'ye Katılan Cihazlar için çoklu oturum açma</span><span class="sxs-lookup"><span data-stu-id="26783-102">Single-sign on for Azure Active Directory Joined Devices</span></span>

<span data-ttu-id="26783-103">Şirket içi Active Directory (AD) ortamınız varsa ve AD etki alanına katılmış bilgisayarlarınızı Azure AD'ye katılmak istiyorsanız, karma Azure AD birleştirmeyi yaparak bunu gerçekleştirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="26783-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="26783-104">[Nasıl Kullanılır: Karma Azure Active Directory birleştirme](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) uygulamanızı planlamak, ortamınıza karma bir Azure AD birleştirmesi uygulamayla ilgili adımlar sağlar.</span><span class="sxs-lookup"><span data-stu-id="26783-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

[<span data-ttu-id="26783-105">İş için Windows Hello kullanarak Şirket İçi Single-Sign Için Azure AD'ye katılmış cihazları yapılandırma</span><span class="sxs-lookup"><span data-stu-id="26783-105">Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business</span></span>](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

<span data-ttu-id="26783-106">**Birincil Yenileme Belirteci (PRT) sorunları** Birincil Yenileme Belirteci (PRT), Windows 10, Windows Server 2016 ve sonraki sürümler, iOS ve Android cihazlarında Azure AD kimlik doğrulamasının önemli bir yapıdır.</span><span class="sxs-lookup"><span data-stu-id="26783-106">**Primary Refresh Token (PRT) issues** A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="26783-107">Bu, bu cihazlarda kullanılan uygulamalarda çoklu oturum açmayı (SSO) etkinleştirmek için Microsoft birinci taraf belirteç aracıları için özel olarak verilen bir JSON Web Belirtecidir (JWT).</span><span class="sxs-lookup"><span data-stu-id="26783-107">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="26783-108">[Birincil Yenileme Belirteci nedir?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)Windows 10 cihazlarında BIR PRT'nin nasıl çıkar, kullanılır ve korunarak nasıl korunduğla ilgili ayrıntılar sağlarız.</span><span class="sxs-lookup"><span data-stu-id="26783-108">[In What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), we will provide details on how a PRT is issued, used, and protected on Windows 10 devices.</span></span>

<span data-ttu-id="26783-109">**WamDefaultSet: YES ve AzureADPrt: YES** Bu alanlar, kullanıcının cihazda oturum a açması için Azure AD'de başarılı bir şekilde kimlik doğrulaması olup olmadığını gösterir.</span><span class="sxs-lookup"><span data-stu-id="26783-109">**WamDefaultSet: YES and AzureADPrt: YES** These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="26783-110">Değerler NO **ise,** son tarihi şu olabilir:</span><span class="sxs-lookup"><span data-stu-id="26783-110">If the values are **NO**, it could be due:</span></span>

- <span data-ttu-id="26783-111">Kayıt sırasında cihazla ilişkilendirilmiş OLAN TPM'de hatalı depolama anahtarı (yükseltilmiş çalışırken KeySignTest'i kontrol edin).</span><span class="sxs-lookup"><span data-stu-id="26783-111">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).</span></span>
- <span data-ttu-id="26783-112">Alternatif Oturum Açma Kimliği</span><span class="sxs-lookup"><span data-stu-id="26783-112">Alternate Login ID</span></span>
- <span data-ttu-id="26783-113">HTTP Proxy bulunamadı</span><span class="sxs-lookup"><span data-stu-id="26783-113">HTTP Proxy not found</span></span>

<span data-ttu-id="26783-114">dsregcmd komutunu kullanarak cihaz sorunlarını giderme - [SSO durumu](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="26783-114">Troubleshoot devices using the dsregcmd command - [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span></span>
