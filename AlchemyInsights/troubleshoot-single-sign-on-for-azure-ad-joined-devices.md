---
title: Azure AD'ye Katılan Cihazlar için Çoklu oturum açma sorunlarını giderme
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "9327"
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037336"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a><span data-ttu-id="8045c-102">Azure AD'ye Katılan Cihazlar için Çoklu oturum açma sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="8045c-102">Troubleshoot Single-sign on for Azure AD Joined Devices</span></span>

<span data-ttu-id="8045c-103">Şirket içi Active Directory (AD) ortamınız varsa ve AD etki alanına katılmış bilgisayarlarınızı Azure AD'ye katılmak istiyorsanız, karma Azure AD birleştirmeyi yaparak bunu gerçekleştirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="8045c-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="8045c-104">[Nasıl Kullanılır: Karma Azure Active Directory birleştirme](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) uygulamanızı planlamak, ortamınıza karma bir Azure AD birleştirmesi uygulamayla ilgili adımlar sağlar.</span><span class="sxs-lookup"><span data-stu-id="8045c-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

<span data-ttu-id="8045c-105">Daha fazla bilgi için bkz. Şirket içi Single-Sign İş için Windows Hello kullanırken [Azure AD'ye katılmış cihazları yapılandırma.](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)</span><span class="sxs-lookup"><span data-stu-id="8045c-105">For more information, see [Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span></span>

<span data-ttu-id="8045c-106">**Birincil Yenileme Belirteci (PRT) sorunları**</span><span class="sxs-lookup"><span data-stu-id="8045c-106">**Primary Refresh Token (PRT) issues**</span></span>

<span data-ttu-id="8045c-107">Birincil Yenileme Belirteci (PRT), Windows 10, Windows Server 2016 ve sonraki sürümler, iOS ve Android cihazlarında Azure AD kimlik doğrulamasının önemli bir yapıdır.</span><span class="sxs-lookup"><span data-stu-id="8045c-107">A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="8045c-108">Bu, bu cihazlarda kullanılan uygulamalarda çoklu oturum açmayı (SSO) etkinleştirmek için Microsoft birinci taraf belirteç aracıları için özel olarak verilen bir JSON Web Belirtecidir (JWT).</span><span class="sxs-lookup"><span data-stu-id="8045c-108">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="8045c-109">Windows 10 cihazlarında BIR PRT'nin nasıl çıkarı, kullanılır ve korunarak nasıl korunmaktadır hakkında ayrıntılı bilgi için bkz. Birincil Yenileme [Belirteci nedir?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)</span><span class="sxs-lookup"><span data-stu-id="8045c-109">For details on how a PRT is issued, used, and protected on Windows 10 devices, see [What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="8045c-110">**WamDefaultSet: YES ve AzureADPrt: YES**</span><span class="sxs-lookup"><span data-stu-id="8045c-110">**WamDefaultSet: YES and AzureADPrt: YES**</span></span>

<span data-ttu-id="8045c-111">Bu alanlar, kullanıcının cihazda oturum a açması için Azure AD'de başarılı bir şekilde kimlik doğrulaması olup olmadığını gösterir.</span><span class="sxs-lookup"><span data-stu-id="8045c-111">These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="8045c-112">Değerler NO **ise,** bunun nedeni şu olabilir:</span><span class="sxs-lookup"><span data-stu-id="8045c-112">If the values are **NO**, it could be due to:</span></span>

- <span data-ttu-id="8045c-113">Kayıt sırasında cihazla ilişkilendirilmiş OLAN TPM'de hatalı depolama anahtarı (yükseltilmiş çalışırken KeySignTest'i kontrol edin)</span><span class="sxs-lookup"><span data-stu-id="8045c-113">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated)</span></span>
- <span data-ttu-id="8045c-114">Alternatif Oturum Açma Kimliği</span><span class="sxs-lookup"><span data-stu-id="8045c-114">Alternate Login ID</span></span>
- <span data-ttu-id="8045c-115">HTTP Proxy bulunamadı</span><span class="sxs-lookup"><span data-stu-id="8045c-115">HTTP Proxy not found</span></span>

<span data-ttu-id="8045c-116">dsregcmd komutunu kullanarak cihaz sorunlarını gidermek için [SSO durumuna bakın.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="8045c-116">To troubleshoot devices using the dsregcmd command, see [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>
