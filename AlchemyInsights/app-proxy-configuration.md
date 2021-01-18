---
title: Uygulama proxy yapılandırması
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7800"
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885531"
---
# <a name="app-proxy-configuration"></a><span data-ttu-id="c6527-102">Uygulama proxy yapılandırması</span><span class="sxs-lookup"><span data-stu-id="c6527-102">App Proxy Configuration</span></span>

1. <span data-ttu-id="c6527-103">Şirket içi uygulamalarınızı buluta göstermek için Azure AD 'de bir uygulama proxy uygulaması yapılandırmayı öğrenmek için, [uygulama proxy uygulaması yapılandırma](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="c6527-103">To understand how to configure an Application Proxy application within Azure AD to expose your on-premises applications to the cloud, see [How to configure an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span></span>
2. <span data-ttu-id="c6527-104">Çoklu oturum açma (SSO), kullanıcılarınızın birden çok kez kimlik doğrulamadan bir uygulamaya erişmesine olanak tanır.</span><span class="sxs-lookup"><span data-stu-id="c6527-104">Single sign-on (SSO) allows your users to access an application without authenticating multiple times.</span></span> <span data-ttu-id="c6527-105">Tek kimlik doğrulamanın Bulutta Azure Active Directory karşısında gerçekleşmesini sağlar ve hizmet veya bağlayıcının, uygulamadaki ek kimlik doğrulama sorunlarını tamamlaması için kullanıcıyı taklit etmesine olanak tanır.</span><span class="sxs-lookup"><span data-stu-id="c6527-105">It allows the single authentication to occur in the cloud, against Azure Active Directory, and allows the service or Connector to impersonate the user to complete any additional authentication challenges from the application.</span></span> <span data-ttu-id="c6527-106">Daha fazla bilgi edinmek için, [uygulama proxy uygulamasında çoklu oturum açmayı yapılandırma](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="c6527-106">To learn more, see [How to configure single sign-on to an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span></span>
3. <span data-ttu-id="c6527-107">Yeni uygulama proxy uygulaması oluştururken sık karşılaşılan sorunları gidermek için [Bu makaleyi](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) kullanın.</span><span class="sxs-lookup"><span data-stu-id="c6527-107">Use [this article](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) to troubleshoot common issues people face when creating a new application proxy application.</span></span>
4. <span data-ttu-id="c6527-108">Uygulamanıza arka uç kimlik doğrulamayı ayarlarken sorun yaşıyorsanız, [uygulama ara sunucusunun Kerberos kısıtlı temsilci yapılandırmalarını gidermeniz](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) veya sorununuzu çözmek Için [uygulamayı pingaccess ile yapılandırma](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) konusunda rehberlik izlemeniz gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="c6527-108">If you are having a problem setting up back-end authentication to your application you may need to [Troubleshoot Kerberos constrained delegation configurations for Application Proxy](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) or follow guidance on [configuring application with PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) to resolve your issue.</span></span>
