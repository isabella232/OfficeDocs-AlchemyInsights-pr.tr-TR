---
title: Şirket içi çoklu oturum açma (SSO) sorunlarını giderme
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9370"
- "9004357"
ms.openlocfilehash: a8d14b12bfb3b02da0468eee70af26344465a2a2
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816346"
---
# <a name="troubleshoot-seamless-single-sign-on-sso-for-on-premises"></a><span data-ttu-id="b7cd0-102">Şirket içi çoklu oturum açma (SSO) sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="b7cd0-102">Troubleshoot Seamless Single Sign-on (SSO) for on-premises</span></span>

<span data-ttu-id="b7cd0-103">Sorunsuz Çoklu Oturum Açma (SSO) sorunlarını çözmek için aşağıdaki adımları uygulayın:</span><span class="sxs-lookup"><span data-stu-id="b7cd0-103">To resolve Seamless Single Sign-on (SSO) issues, perform the following steps:</span></span>

<span data-ttu-id="b7cd0-104">**AZUREADSSO bilgisayar hesabının Kerberos şifre çözme anahtarını nasıl kullanabilirim?**</span><span class="sxs-lookup"><span data-stu-id="b7cd0-104">**How can I roll over the Kerberos decryption key of the AZUREADSSO computer account?**</span></span>

<span data-ttu-id="b7cd0-105">Kerberos şifre çözme anahtarını en az 30 günde bir tekrarlamanizi kesinlikle öneririz.</span><span class="sxs-lookup"><span data-stu-id="b7cd0-105">We highly recommend that you roll over the Kerberos decryption key at least every 30 days.</span></span> <span data-ttu-id="b7cd0-106">Bunu el ile yapmak için [Bkz. Kerberos şifre çözme anahtarları nasıl yuvarlanur?](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#)</span><span class="sxs-lookup"><span data-stu-id="b7cd0-106">To do this manually, see [How to roll over Kerberos decryption keys](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#).</span></span>

<span data-ttu-id="b7cd0-107">**Sorunsuz SSO'ya yapılandırma**</span><span class="sxs-lookup"><span data-stu-id="b7cd0-107">**Configure Seamless SSO**</span></span>

<span data-ttu-id="b7cd0-108">Sorunsuz SSO'nun dağıtımı için Azure Active Directory Sorunsuz Çoklu Oturum Açma: Hızlı [Başlangıç'ta adımları izleyin.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys)</span><span class="sxs-lookup"><span data-stu-id="b7cd0-108">To deploy Seamless SSO, follow the steps in [Azure Active Directory Seamless Single Sign-On: Quickstart](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys).</span></span>

<span data-ttu-id="b7cd0-109">**Danışma**</span><span class="sxs-lookup"><span data-stu-id="b7cd0-109">**Advisory**</span></span>

- <span data-ttu-id="b7cd0-110">[Azure Active Directory Sorunsuz Çoklu](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) Oturum Açma: Sık sorulan sorular - Bu makalede, Azure Active Directory Sorunsuz Çoklu Oturum Açma (Sorunsuz SSO) hakkında sık Sign-On soruların yanıtlarını bulabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b7cd0-110">[Azure Active Directory Seamless Single Sign-On: Frequently asked questions](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) - In this article, we address frequently asked questions about Azure Active Directory Seamless Single Sign-On (Seamless SSO).</span></span> <span data-ttu-id="b7cd0-111">Yeni içeriği denetlemeye devam.</span><span class="sxs-lookup"><span data-stu-id="b7cd0-111">Keep checking back for new content.</span></span>
- <span data-ttu-id="b7cd0-112">[Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) - Bu makalede, Sorunsuz SSO hakkında özellik istekleri yapma veya teknik sorular sorma hakkında bilgi sağlanmaktadır.</span><span class="sxs-lookup"><span data-stu-id="b7cd0-112">[Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) - This article provides information on how to make feature requests or ask technical questions about Seamless SSO.</span></span>

<span data-ttu-id="b7cd0-113">**Sorun giderme**</span><span class="sxs-lookup"><span data-stu-id="b7cd0-113">**Troubleshoot**</span></span>

<span data-ttu-id="b7cd0-114">[Azure Active Directory Sorunsuz Çoklu](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) Oturum Açma sorunlarını giderme - Bu makale, Azure Active Directory (Azure AD) Sorunsuz Çoklu Oturum Açma (Sorunsuz SSO) ile ilgili sık karşılaşılan sorunlar hakkında Sign-On bilgileri bu makalede bulabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b7cd0-114">[Troubleshoot Azure Active Directory Seamless Single Sign-On](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) - This article helps you find troubleshooting information about common problems regarding Azure Active Directory (Azure AD) Seamless Single Sign-On (Seamless SSO).</span></span>







