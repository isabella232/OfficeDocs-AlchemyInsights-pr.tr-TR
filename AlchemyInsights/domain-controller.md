---
title: Etki alanı denetleyicisi
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901317"
---
# <a name="domain-controller"></a><span data-ttu-id="72a7f-102">Etki alanı denetleyicisi</span><span class="sxs-lookup"><span data-stu-id="72a7f-102">Domain controller</span></span>

<span data-ttu-id="72a7f-103">**AAD etkinleştirilemiyor-DS veya dağıtım başarısız oluyor**</span><span class="sxs-lookup"><span data-stu-id="72a7f-103">**Unable to enable AAD-DS or deployment is failing**</span></span>

<span data-ttu-id="72a7f-104">Azure AD etki alanı hizmeti 'nin (AAD-DS) etkinleştirilmemiş veya dağıtılmadığı sorunu çözmek için aşağıdaki adımları uygulayın:</span><span class="sxs-lookup"><span data-stu-id="72a7f-104">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="72a7f-105">Var olan bir sanal ağı kullanıyorsanız, portalda AAD-DS 'de eşitleme yapmak için gereken bağlantı noktalarını engelleyen kurallar için NSG 'inizi denetleyin https://aka.ms/aadds-networking .</span><span class="sxs-lookup"><span data-stu-id="72a7f-105">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="72a7f-106">Bu sorun giderme kılavuzunda, hata iletinizin yanıtlanmadığını denetleyin  https://aka.ms/aadds-troubleshoot-enable .</span><span class="sxs-lookup"><span data-stu-id="72a7f-106">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="72a7f-107">Azure AD etki alanı Hizmetleri 'ni yeni bir sanal ağda dağıtmayı deneyin.</span><span class="sxs-lookup"><span data-stu-id="72a7f-107">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="72a7f-108">[Azure AD etki alanı Hizmetleri oluşturmaya yönelik öğretici](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance)'de sağlanan AAD-DS 'yi dağıtmaya yönelik Başlarken Kılavuzunu izleyin.</span><span class="sxs-lookup"><span data-stu-id="72a7f-108">Follow the Getting Started guide on how to deploy AAD-DS, which is available at [Tutorial to Create Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="72a7f-109">Azure AD etki alanı Hizmetleri 'ni dağıtma konusunda sorun yaşıyorsanız, bir kez daha çalışmanızı öğrenmenize yardımcı olacak genel hataları çözmek için [Azure AD etki alanı Hizmetleri sorunlarını giderme](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="72a7f-109">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="72a7f-110">**AAD devre dışı bırakılamıyor-DS**</span><span class="sxs-lookup"><span data-stu-id="72a7f-110">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="72a7f-111">AAD-DS duraklatılamıyor.</span><span class="sxs-lookup"><span data-stu-id="72a7f-111">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="72a7f-112">Yönetilen etki alanınızı kullanmayı durdurmak istiyorsanız, silinmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="72a7f-112">If you wish to stop using your managed domain, it must be deleted.</span></span>

<span data-ttu-id="72a7f-113">Sorunlarla karşılaşırsanız, yaygın hata iletilerini ve daha fazla işlem yapmanıza yardımcı olacak ilgili sorun giderme adımları için [, bkz.](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot)</span><span class="sxs-lookup"><span data-stu-id="72a7f-113">If you run into issues, to resolve common error messages and for associated troubleshooting steps to help you get things running again, see [Troubleshoot Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).</span></span>
