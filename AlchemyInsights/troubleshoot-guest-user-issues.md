---
title: Konuk Kullanıcı sorunlarını giderme
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
ms.openlocfilehash: 0f2a10b918fee067b167ab58ac2544a89e0c8ea1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901593"
---
# <a name="troubleshoot-guest-user-issues"></a>Konuk Kullanıcı sorunlarını giderme

1. Uygulamalara konuk erişimini yönetme konusunda rehberlik için, [Azure AD erişimi incelemelerle konuk erişimini yönetme](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews)konusuna bakın.
1. [Azure portalında dizine Konuk kullanıcıları ekleme](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal): Bu hızlı başlangıç bölümünde, Azure Portal kullanarak Azure AD dizinine yeni bir Konuk Kullanıcı eklersiniz, bir davet gönderilir ve Konuk Kullanıcı daveti ödeme işleminin nasıl göründüğünü görebilirsiniz.
1. [PowerShell ile Konuk Kullanıcı ekleme](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell): Bu hızlı başlangıç bölümünde, Azure kiracınıza bir Konuk Kullanıcı eklemek için New-AzureADMSInvitation komutunu kullanırsınız.
1. Azure Active Directory 'de veya PowerShell kullanarak Azure Active Directory 'de (Azure AD) kurumsal uygulamalara Kullanıcı ve grup atamayı öğrenmek için [Azure Active Directory 'de bir uygulama için Kullanıcı atamasını yönetme](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal)bölümüne bakın. 
1. Azure Active Directory (Azure AD) B2B işbirliği, Azure AD ile bütünleşen uygulamaların çoğunda çalışır. Bu [makalede](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps), Azure AD B2B ile kullanım için bazı popüler SaaS uygulamalarını yapılandırma yönergelerini gözden geçirin.
1. Azure Active Directory (Azure AD) B2B işbirliği özelliklerini kullanan bir kuruluş olarak, Konuk kullanıcılarını iş ortağı Kuruluşlarınıza davet etme Şirket içi bu uygulamalar, SAML tabanlı kimlik doğrulamayı veya Kerberos kısıtlı temsilci (KCD) ile tümleşik Windows kimlik doğrulamasını (ıWA) kullanabilir. Daha fazla bilgi için, [Şirket içi uygulamalarınıza Azure AD erişimi 'NDE B2B kullanıcıları verme](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises)bölümüne bakın.
1. [Azure AD B2B işbirliği kullanarak bulut kaynaklarına yerel olarak yönetilen iş ortağı hesaplarının erişimine nasıl izin](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)vereceğinizi öğrenin.