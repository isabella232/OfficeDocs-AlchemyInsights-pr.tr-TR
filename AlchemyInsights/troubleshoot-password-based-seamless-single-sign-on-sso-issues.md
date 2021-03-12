---
title: Parola Tabanlı Sorunsuz Çoklu Oturum Açma (SSO) sorunlarını giderme
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
- "9004357"
- "9374"
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714890"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a><span data-ttu-id="f1d76-102">Parola Tabanlı Sorunsuz Çoklu Oturum Açma (SSO) sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="f1d76-102">Troubleshoot Password-based Seamless Single Sign-on (SSO) issues</span></span>

<span data-ttu-id="f1d76-103">Parola tabanlı SSO'nun temellerini öğrenmek için Azure [Active Directory ile Parola tabanlı kimlik doğrulamasına bakın.](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)</span><span class="sxs-lookup"><span data-stu-id="f1d76-103">To learn the fundamentals of password-based SSO, see [Password-based authentication with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).</span></span>

<span data-ttu-id="f1d76-104">**Parola tabanlı SSO'nun yapılandırılması**</span><span class="sxs-lookup"><span data-stu-id="f1d76-104">**Configure Password-based SSO**</span></span>

1. <span data-ttu-id="f1d76-105">[Parola tabanlı çoklu oturum açma ayarlarını yapılandırma](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) - Bu makale, parola tabanlı SSO seçeneği hakkında daha fazla ayrıntıya gider.</span><span class="sxs-lookup"><span data-stu-id="f1d76-105">[Configure password-based single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) - This article goes into more detail about the password-based SSO option.</span></span> <span data-ttu-id="f1d76-106">Ekley istediğiniz uygulama özel yapılandırma gerektiriyorsa ve parola tabanlı SSO kullanıyorsanız, bu makale tam size göredir.</span><span class="sxs-lookup"><span data-stu-id="f1d76-106">If the application you're adding requires custom configuration and you need to use password-based SSO, then this article is for you.</span></span>
2. <span data-ttu-id="f1d76-107">[Uygulama öncesi uygulamalar için parola tabanlı çoklu](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) oturum açma ayarlarını yapılandırma - Uygulama Ara Sunucusu çeşitli çoklu oturum açma modlarını destekler.</span><span class="sxs-lookup"><span data-stu-id="f1d76-107">[Configure password-based single sign on for on-prem apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) - Application Proxy supports several single sign-on modes.</span></span> <span data-ttu-id="f1d76-108">Parola tabanlı oturum açma, kimlik doğrulaması için kullanıcı adı/parola bileşimi kullanan uygulamalara yöneliktir.</span><span class="sxs-lookup"><span data-stu-id="f1d76-108">Password-based sign-on is intended for applications that use a username/password combination for authentication.</span></span> <span data-ttu-id="f1d76-109">Uygulamanız için parola tabanlı oturum açma yapılandırıldığında, kullanıcılarının şirket içi uygulamada bir kez oturum açmaları gerekir.</span><span class="sxs-lookup"><span data-stu-id="f1d76-109">When you configure password-based sign-on for your application, your users have to sign in to the on-premises application once.</span></span> <span data-ttu-id="f1d76-110">Bundan sonra, Azure Active Directory oturum açma bilgilerini depolar ve kullanıcılarınız uzaktan erişse uygulamaya otomatik olarak sağlar.</span><span class="sxs-lookup"><span data-stu-id="f1d76-110">After that, Azure Active Directory stores the sign-in information and automatically provides it to the application when your users access it remotely.</span></span>
    - <span data-ttu-id="f1d76-111">Uygulama Ara Sunucusu ile uygulamanızı zaten yayımlanmış ve test edilmiş olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="f1d76-111">You should already have published and tested your app with Application Proxy.</span></span> <span data-ttu-id="f1d76-112">Yoksa, Azure AD [Application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) Proxy'lerini kullanarak Uygulamaları yayımla'daki adımları izleyin ve ardından uygulama öncesi uygulamalar için parola tabanlı SSO yapılandırmanıza devam edin.</span><span class="sxs-lookup"><span data-stu-id="f1d76-112">If not, follow the steps in [Publish applications using Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) then continue your configuration of password-based SSO for on-prem apps.</span></span>

<span data-ttu-id="f1d76-113">Parola tabanlı SSO sorunlarını gidermek için Bkz. [Azure AD'de](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) parola tabanlı çoklu oturum açma sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="f1d76-113">To troubleshoot password-based SSO, see [Troubleshoot password-based single sign-on in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span></span>
