---
title: Konuk kullanıcı sorunlarını giderme
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004358"
- "7822"
ms.openlocfilehash: 9e6030919721b4c0805a26ca45d365f31d88894e86ea08225f47576e7d152047
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939399"
---
# <a name="troubleshoot-guest-user-issues"></a>Konuk kullanıcı sorunlarını giderme

1. Uygulamalara konuk erişimini yönetme kılavuzu için bkz. [Azure AD erişim incelemeleriyle konuk erişimini yönetme.](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews)
1. [Azure portalında](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal)dizininize konuk kullanıcı ekleme: Bu hızlı başlangıçta, Azure portalı aracılığıyla Azure AD dizininize yeni bir konuk kullanıcı ekli bir konuk kullanıcı ekersiniz, davet gönderir ve konuk kullanıcının davet kullanım işleminin nasıl göründüğünü görebilirler.
1. [PowerShell ile konuk](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell)kullanıcı ekleme: Bu hızlı başlangıç olarak, Azure kiracınıza bir konuk New-AzureADMSInvitation kullanıcı eklemek için Hızlı Başlangıç komutunu kullanacağız.
1. Azure portalında veya PowerShell kullanarak Azure Active Directory'daki (Azure AD) kurumsal uygulamalara kullanıcı ve grup atamayı öğrenmek için bkz. Azure Active Directory'te bir uygulama için kullanıcı [atamayı yönetme.](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal) 
1. Azure Active Directory (Azure AD) B2B işbirliği, Azure AD ile tümleştirilmiş çoğu uygulamayla birlikte çalışır. Bu [makalede,](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)Azure AD B2B ile kullanmak üzere bazı popüler SaaS uygulamalarını yapılandırma yönergelerini size adım adım göstereceğiz.
1. İş ortağı kuruluşlardan konuk kullanıcıları Azure AD'nize davet etmek için Azure Active Directory (Azure AD) B2B işbirliği özelliklerini kullanan bir kuruluş olarak, artık bu B2B kullanıcılarının şirket içi uygulamalara erişmelerini sebilirsiniz. Bu şirket içi uygulamalar, Kerberos kısıtlanmış temsilcisiyle (KCD) SAML tabanlı kimlik doğrulama veya Tümleşik Windows Kimlik Doğrulaması (IWA) kullanabilir. Daha fazla bilgi için [bkz. Azure AD'de B2B kullanıcılarına şirket içi uygulamalarınıza erişim izni verilmesi.](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises)
1. [Azure AD B2B işbirliğini kullanarak bulut kaynaklarına yerel olarak yönetilen iş ortağı hesaplarına erişim iznini nasıl ver ola öğrenin.](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)