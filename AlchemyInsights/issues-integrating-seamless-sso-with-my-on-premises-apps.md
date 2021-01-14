---
title: Şirket içi uygulamalarınızla kesintisiz SSO 'yu tümleştirmeyle ilgili sorunlar
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 785d7f842031c1056ec6868376f253439919a3ab
ms.sourcegitcommit: 227a949a6ae49cc52c7fdcef2f9fd202c746169d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/13/2021
ms.locfileid: "49868770"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a><span data-ttu-id="7daac-102">Şirket içi uygulamalarınızla kesintisiz SSO 'yu tümleştirmeyle ilgili sorunlar</span><span class="sxs-lookup"><span data-stu-id="7daac-102">Issues with integrating Seamless SSO with my on-premises apps</span></span>

<span data-ttu-id="7daac-103">Şirket içi uygulamalarla kesintisiz SSO 'yu tümleştirmeyle ilgili sorunları gidermek için aşağıdakileri yapın:</span><span class="sxs-lookup"><span data-stu-id="7daac-103">To troubleshoot issues with integrating Seamless SSO with on-premises applications, do the following:</span></span>

<span data-ttu-id="7daac-104">**Önerilen adımlar**</span><span class="sxs-lookup"><span data-stu-id="7daac-104">**Recommended steps**</span></span>

1. <span data-ttu-id="7daac-105">**Uygulama ara sunucusu aracılığıyla çoklu oturum açma** için bir **Şirket içi uygulama** yapılandırmak üzere, [uygulama proxy 'si Ile çoklu oturum açma için parola](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)oluşturma konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="7daac-105">To configure an **on-premises application** for **single sign-on through Application Proxy**, see [Password vaulting for single sign-on with Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).</span></span>
1. <span data-ttu-id="7daac-106">**Uygulama proxy 'si sorunlarını giderme**: uygulama proxy bağlayıcıları 'nın doğru yapılandırılıp yapılandırılmadığını belirlemek Için, [uygulama ara](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)</span><span class="sxs-lookup"><span data-stu-id="7daac-106">**Troubleshooting Application Proxy issues**: we recommend that you start with reviewing the troubleshooting flow, [Debug Application Proxy Connector issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), to determine if Application Proxy connectors are configured correctly.</span></span> <span data-ttu-id="7daac-107">Uygulamaya bağlanma konusunda hala sorun yaşıyorsanız, [uygulama proxy 'si uygulama sorunlarını ayıklamada](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps)sorun giderme adımlarını izleyin.</span><span class="sxs-lookup"><span data-stu-id="7daac-107">If you're still having trouble connecting to the application, follow the troubleshooting steps in [Debug Application Proxy application issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps).</span></span> <span data-ttu-id="7daac-108">[CORS sorunlarını](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) aşağıdaki tarayıcı hata ayıklama araçlarını kullanarak tanımlayabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="7daac-108">You can [identify CORS issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) by using the following browser debug tools:</span></span>
    1. <span data-ttu-id="7daac-109">Tarayıcıyı başlatın ve Web uygulamasına gidin.</span><span class="sxs-lookup"><span data-stu-id="7daac-109">Launch the browser and browse to the web app.</span></span>
    1. <span data-ttu-id="7daac-110">Debug konsolunu görüntülemek için **F12** tuşuna basın.</span><span class="sxs-lookup"><span data-stu-id="7daac-110">Press **F12** to bring up the debug console.</span></span>
    1. <span data-ttu-id="7daac-111">İşlemi yeniden oluşturmaya çalışın ve konsol iletisini gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="7daac-111">Try to reproduce the transaction, and review the console message.</span></span> <span data-ttu-id="7daac-112">CORS ihlaliyle ilgili bir konsol hatası veriyor.</span><span class="sxs-lookup"><span data-stu-id="7daac-112">A CORS violation produces a console error about origin.</span></span>
    1. <span data-ttu-id="7daac-113">Uygulamanızın kimlik doğrulaması için login.microsoftonline.com 'a yönlendirdiği ve erişim belirtecinin süresi dolduğunda bazı CORS sorunları çözülebilir.</span><span class="sxs-lookup"><span data-stu-id="7daac-113">Some CORS issues can't be resolved, such as when your app redirects to login.microsoftonline.com to authenticate, and the access token expires.</span></span> <span data-ttu-id="7daac-114">CORS çağrısı başarısız olur.</span><span class="sxs-lookup"><span data-stu-id="7daac-114">The CORS call then fails.</span></span> <span data-ttu-id="7daac-115">Bu senaryo için geçici bir çözüm olan erişim belirtecinin kullanım süresini uzatmak, kullanıcının oturumu sırasında süresinin dolmasını önleyecek şekilde.</span><span class="sxs-lookup"><span data-stu-id="7daac-115">A workaround for this scenario is to extend the lifetime of the access token, to prevent it from expiring during a user’s session.</span></span> <span data-ttu-id="7daac-116">Bunu yapma hakkında daha fazla bilgi için [Microsoft Identity platformunda yapılandırılabilir belirteç ömürleri](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="7daac-116">For more information about how to do this, see [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="7daac-117">**Önerilen belgeler**</span><span class="sxs-lookup"><span data-stu-id="7daac-117">**Recommended documents**</span></span>

- [<span data-ttu-id="7daac-118">Uygulama proxy uygulamasında çoklu oturum açmayı yapılandırma</span><span class="sxs-lookup"><span data-stu-id="7daac-118">How to configure single sign-on to an Application Proxy application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [<span data-ttu-id="7daac-119">Uygulama proxy 'Si ile şirket içi uygulamalar için SAML tekli oturum açma</span><span class="sxs-lookup"><span data-stu-id="7daac-119">SAML single sign-on for on-premises applications with Application Proxy</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [<span data-ttu-id="7daac-120">Azure Active Directory uygulama proxy CORS sorunlarını anlama ve çözme</span><span class="sxs-lookup"><span data-stu-id="7daac-120">Understand and solve Azure Active Directory Application Proxy CORS issues</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [<span data-ttu-id="7daac-121">Uygulama proxy 'Si için Kerberos kısıtlı temsilci yapılandırmalarında sorun giderme</span><span class="sxs-lookup"><span data-stu-id="7daac-121">Troubleshoot Kerberos constrained delegation configurations for Application Proxy</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)