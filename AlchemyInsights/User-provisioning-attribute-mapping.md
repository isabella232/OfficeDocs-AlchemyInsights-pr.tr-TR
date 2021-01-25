---
title: Kullanıcı tarafından sağlanan öznitelik eşlemesi
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7851"
- "9004348"
ms.openlocfilehash: 8bbf554c533d960a304901d7cbb492b87e9bec71
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949899"
---
# <a name="user-provisioning-attribute-mapping"></a><span data-ttu-id="20827-102">Kullanıcı tarafından sağlanan öznitelik eşlemesi</span><span class="sxs-lookup"><span data-stu-id="20827-102">User-provisioning attribute mapping</span></span>

1. <span data-ttu-id="20827-103">Bilinen öznitelik eşleme sorunlarını gidermek için, [öznitelik eşlemelerine](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings)bakın.</span><span class="sxs-lookup"><span data-stu-id="20827-103">To troubleshoot known attribute-mapping issues, see [Attribute mappings](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span></span> 
2. <span data-ttu-id="20827-104">Microsoft Azure Active Directory (AD), Salesforce, G Suite ve diğerleri gibi üçüncü taraf SaaS uygulamalarına Kullanıcı sağlama desteği sağlar.</span><span class="sxs-lookup"><span data-stu-id="20827-104">Microsoft Azure Active Directory (AD) provides support for user provisioning to third-party SaaS applications such as Salesforce, G Suite and others.</span></span> <span data-ttu-id="20827-105">Üçüncü taraf SaaS uygulaması için Kullanıcı sağlamayı etkinleştirirseniz, Azure Portal öznitelik değerlerini öznitelik eşlemeleri aracılığıyla denetler.</span><span class="sxs-lookup"><span data-stu-id="20827-105">If you enable user provisioning for a third-party SaaS application, the Azure portal controls its attribute values through attribute-mappings.</span></span> <span data-ttu-id="20827-106">Varsayılan öznitelik eşlemelerini özelleştirmeyi öğrenmek için, [Azure Active Directory 'de SaaS uygulamaları için Kullanıcı hazırlama öznitelik eşlemeleri özelleştirme](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="20827-106">To learn how to customize the default attribute-mappings, see [Customize user provisioning attribute-mappings for SaaS applications in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span></span>
    - <span data-ttu-id="20827-107">SaaS uygulaması Kullanıcı sağlama hakkında daha fazla bilgi edinmek için [Azure AD 'de otomatik SaaS uygulaması Kullanıcı sağlama nedir?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span><span class="sxs-lookup"><span data-stu-id="20827-107">To learn more about SaaS app user provisioning, see [What is automated SaaS app user provisioning in Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span></span> 
3. <span data-ttu-id="20827-108">Kullanıcı sağlaması için öznitelik eşlemelerini özelleştirirken, eşlemek istediğiniz özniteliğin kaynak öznitelik listesinde görünmeyeceğini fark edebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="20827-108">When customizing attribute-mappings for user provisioning, you might find that the attribute you want to map doesn't appear in the Source attribute list.</span></span> <span data-ttu-id="20827-109">[Active Directory 'nizde şirket Içi Active Directory 'Den Azure AD 'ye eşitleme bir uygulama makalesine kaynak olarak eşitleme](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) işlemi, eksik özniteliği ŞIRKET içi ad 'DAN Azure AD 'ye eşitleyerek nasıl ekleyeceğinizi gösterir.</span><span class="sxs-lookup"><span data-stu-id="20827-109">The [Sync an attribute from your on-premises Active Directory to Azure AD for provisioning to an application](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) article shows you how to add the missing attribute by synchronizing it from your on-premises AD to Azure AD.</span></span>
