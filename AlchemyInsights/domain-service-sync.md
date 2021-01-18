---
title: Etki alanı hizmeti eşitlemesi
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "7922"
- "7921"
ms.openlocfilehash: b35d3a402bc08a27a818209385c5666b901fa524
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885560"
---
# <a name="domain-service-synchronization"></a><span data-ttu-id="236ac-102">Etki alanı hizmeti eşitlemesi</span><span class="sxs-lookup"><span data-stu-id="236ac-102">Domain service synchronization</span></span>

<span data-ttu-id="236ac-103">Azure Active Directory etki alanı Hizmetleri (Azure AD DS) yönetilen etki alanındaki nesneler ve kimlik bilgileri, etki alanı içinde yerel olarak veya Azure Active Directory (Azure AD) kiracısından eşitlenebilir.</span><span class="sxs-lookup"><span data-stu-id="236ac-103">Objects and credentials in an Azure Active Directory Domain Services (Azure AD DS) managed domain can either be created locally within the domain, or synchronized from an Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="236ac-104">İlk kez Azure AD DS 'yi dağıtırken, Azure AD 'den nesneleri çoğaltmaya yönelik otomatik tek yönlü eşitleme yapılandırılır ve başlatılır.</span><span class="sxs-lookup"><span data-stu-id="236ac-104">When you first deploy Azure AD DS, an automatic one-way synchronization is configured and initiated to replicate the objects from Azure AD.</span></span> <span data-ttu-id="236ac-105">Bu tek yönlü eşitleme, Azure AD DS yönetilen etki alanını Azure AD 'deki değişikliklerle güncel tutmak için arka planda çalışmaya devam eder.</span><span class="sxs-lookup"><span data-stu-id="236ac-105">This one-way synchronization continues to run in the background to keep the Azure AD DS managed domain up-to-date with any changes from Azure AD.</span></span> <span data-ttu-id="236ac-106">Azure AD DS 'den Azure AD 'ye geri eşitleme yapılmaz.</span><span class="sxs-lookup"><span data-stu-id="236ac-106">No synchronization occurs from Azure AD DS back to Azure AD.</span></span>

<span data-ttu-id="236ac-107">Azure Active Directory etki alanı hizmeti eşitlemesi hakkında daha fazla bilgi için bkz: [etki alanı hizmeti eşitleme](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).</span><span class="sxs-lookup"><span data-stu-id="236ac-107">For more details on Azure Active Directory domain service synchronization, see [Domain Service Synchronization](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).</span></span> 
