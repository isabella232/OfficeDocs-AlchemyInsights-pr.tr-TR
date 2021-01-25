---
title: API Izinleri ve Izin
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974997"
---
# <a name="api-permissions-and-consent"></a><span data-ttu-id="30e18-102">API izinleri ve izin</span><span class="sxs-lookup"><span data-stu-id="30e18-102">API permissions and consent</span></span>

<span data-ttu-id="30e18-103">Microsoft Identity platform ile birleşen uygulamalar, kullanıcıların ve yöneticilerin verilere nasıl erişilebileceğini denetler.</span><span class="sxs-lookup"><span data-stu-id="30e18-103">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="30e18-104">Yetkilendirme modelinin uygulaması Microsoft Identity platform uç noktasında güncelleştirilmiştir.</span><span class="sxs-lookup"><span data-stu-id="30e18-104">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint.</span></span> <span data-ttu-id="30e18-105">Bir uygulamanın Microsoft Identity platformuyla etkileşimde bulunma şeklini değiştirir.</span><span class="sxs-lookup"><span data-stu-id="30e18-105">It changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="30e18-106">[Microsoft Identity platform Endpoint 'Daki izinler ve izinler](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) , bu yetkilendirme modelinin temel kavramlarını, kapsamlar, izinler ve izin dahil olmak üzere kapsar.</span><span class="sxs-lookup"><span data-stu-id="30e18-106">[Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) covers the basic concepts of this authorization model, including scopes, permissions, and consent.</span></span>

<span data-ttu-id="30e18-107">[Azure Active Directory (Azure AD) izin çatısı](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) , çok kiracılı web ve yerel istemci uygulamalarını geliştirmeyi kolaylaştırır.</span><span class="sxs-lookup"><span data-stu-id="30e18-107">The [Azure Active Directory (Azure AD) consent framework](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) makes it easy to develop multi-tenant web and native client applications.</span></span> <span data-ttu-id="30e18-108">Bu uygulamalar, uygulamanın kaydettirildiği bir Azure AD kiracısından Kullanıcı hesaplarıyla oturum açmaya olanak tanır.</span><span class="sxs-lookup"><span data-stu-id="30e18-108">These applications allow sign-in by user accounts from an Azure AD tenant that's different from the one where the application is registered.</span></span> <span data-ttu-id="30e18-109">Ayrıca, kendi Web API 'larınızın yanı sıra Microsoft Graph API (Microsoft 365 'de Azure AD, Intune ve hizmetlere erişmek için, diğer Microsoft Hizmetleri ' API 'Leri gibi Web API 'Lerine de erişmeyi gerektirebilir.</span><span class="sxs-lookup"><span data-stu-id="30e18-109">They may also need to access web APIs such as the Microsoft Graph API (to access Azure AD, Intune, and services in Microsoft 365) and other Microsoft services' APIs, in addition to your own web APIs.</span></span>

