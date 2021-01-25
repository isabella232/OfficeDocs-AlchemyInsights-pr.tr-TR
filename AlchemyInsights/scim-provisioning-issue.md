---
title: YAPıŞTıRMA sorunu
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
- "7854"
- "9004348"
ms.openlocfilehash: aa5b4cbb99cb1a5a323b39101766bea55fd49064
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949951"
---
# <a name="scim-provisioning-issue"></a><span data-ttu-id="ce02b-102">YAPıŞTıRMA sorunu</span><span class="sxs-lookup"><span data-stu-id="ce02b-102">SCIM provisioning issue</span></span>

<span data-ttu-id="ce02b-103">Otomatik sağlama, kullanıcıların erişmesi gereken bulut uygulamalarında Kullanıcı kimlikleri ve roller oluşturmaya başvurur.</span><span class="sxs-lookup"><span data-stu-id="ce02b-103">Automatic provisioning refers to creating user identities and roles in the cloud applications that users need access to.</span></span> <span data-ttu-id="ce02b-104">Kullanıcı kimlikleri oluşturmanın yanı sıra, otomatik sağlama, kullanıcı kimliklerinin bakım ve kaldırılmasını, durum veya rol değişikliği olarak içerir.</span><span class="sxs-lookup"><span data-stu-id="ce02b-104">In addition to creating user identities, automatic provisioning includes the maintenance and removal of user identities as status or roles change.</span></span> <span data-ttu-id="ce02b-105">Dağıtıma başlamadan önce, Azure Active Directory (AD) hazırlamanın nasıl çalıştığını öğrenmek ve yapılandırma önerilerini öğrenmek için [sağlama Işleminin nasıl çalıştığını](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works) gözden geçirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="ce02b-105">Before you start a deployment, you can review [How provisioning works](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works) to learn how Azure Active Directory (AD) provision works, and get configuration recommendations.</span></span>

<span data-ttu-id="ce02b-106">Uygulama geliştiricisi olarak, uygulamanız ve Azure AD arasındaki Kullanıcı ve grupların otomatik olarak sağlanması için etki alanları arası kimlik yönetimi (SCıM) Kullanıcı yönetimi API 'sini kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="ce02b-106">As an application developer, you can use the System for Cross-Domain Identity Management (SCIM) user management API to enable automatic provisioning of users and groups between your application and Azure AD.</span></span> <span data-ttu-id="ce02b-107">[Derleme uç noktası oluştur ve Azure AD makalesinde Kullanıcı sağlamasını yapılandırma](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) , BIR SCIM uç noktası oluşturma</span><span class="sxs-lookup"><span data-stu-id="ce02b-107">The [Build a SCIM endpoint and configure user provisioning with Azure AD](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) article describes how to build an SCIM endpoint and integrate it with the Azure AD provisioning service.</span></span>



