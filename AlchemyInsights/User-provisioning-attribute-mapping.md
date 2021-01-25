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
# <a name="user-provisioning-attribute-mapping"></a>Kullanıcı tarafından sağlanan öznitelik eşlemesi

1. Bilinen öznitelik eşleme sorunlarını gidermek için, [öznitelik eşlemelerine](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings)bakın. 
2. Microsoft Azure Active Directory (AD), Salesforce, G Suite ve diğerleri gibi üçüncü taraf SaaS uygulamalarına Kullanıcı sağlama desteği sağlar. Üçüncü taraf SaaS uygulaması için Kullanıcı sağlamayı etkinleştirirseniz, Azure Portal öznitelik değerlerini öznitelik eşlemeleri aracılığıyla denetler. Varsayılan öznitelik eşlemelerini özelleştirmeyi öğrenmek için, [Azure Active Directory 'de SaaS uygulamaları için Kullanıcı hazırlama öznitelik eşlemeleri özelleştirme](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes)konusuna bakın.
    - SaaS uygulaması Kullanıcı sağlama hakkında daha fazla bilgi edinmek için [Azure AD 'de otomatik SaaS uygulaması Kullanıcı sağlama nedir?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning) 
3. Kullanıcı sağlaması için öznitelik eşlemelerini özelleştirirken, eşlemek istediğiniz özniteliğin kaynak öznitelik listesinde görünmeyeceğini fark edebilirsiniz. [Active Directory 'nizde şirket Içi Active Directory 'Den Azure AD 'ye eşitleme bir uygulama makalesine kaynak olarak eşitleme](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) işlemi, eksik özniteliği ŞIRKET içi ad 'DAN Azure AD 'ye eşitleyerek nasıl ekleyeceğinizi gösterir.
