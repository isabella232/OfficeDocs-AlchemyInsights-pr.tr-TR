---
title: AAD etki alanı Hizmetleri ile sanal yapılandırma
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885653"
---
# <a name="virtual-configuration-with-aad-domain-services"></a><span data-ttu-id="ffbbf-102">AAD etki alanı Hizmetleri ile sanal yapılandırma</span><span class="sxs-lookup"><span data-stu-id="ffbbf-102">Virtual configuration with AAD domain services</span></span>

<span data-ttu-id="ffbbf-103">AAD etki alanı Hizmetleri ile sanal yapılandırma aşağıdaki adımları içerir:</span><span class="sxs-lookup"><span data-stu-id="ffbbf-103">Virtual configuration with AAD domain services involves the following steps:</span></span> 

1. <span data-ttu-id="ffbbf-104">Azure portalında etki alanınızın durumu denetleniyor https://aka.ms/aadds-health</span><span class="sxs-lookup"><span data-stu-id="ffbbf-104">Checking your domain’s health on the Azure portal https://aka.ms/aadds-health</span></span>
2. <span data-ttu-id="ffbbf-105">Portalınızdaki Azure AD etki alanı Hizmetleri 'nde eşitleme https://aka.ms/aadds-networking</span><span class="sxs-lookup"><span data-stu-id="ffbbf-105">Checking your NSG for rules that block ports needed to synchronize in Azure AD Domain Services on the portal https://aka.ms/aadds-networking</span></span>
3. <span data-ttu-id="ffbbf-106">Sanal ağınızın Azure AD etki alanı Hizmetleri-yönetilen etki alanınızla aynı Azure bölgesinde dağıtılmasını sağlama.</span><span class="sxs-lookup"><span data-stu-id="ffbbf-106">Ensuring that your virtual network is deployed in the same Azure Region as your Azure AD Domain Services-managed domain.</span></span>
4. <span data-ttu-id="ffbbf-107">Sanal ağda aynı etki alanı adına sahip bir etki alanınız olmadığından emin olma.</span><span class="sxs-lookup"><span data-stu-id="ffbbf-107">Ensuring you don’t have an existent domain with the same domain name available on the virtual network.</span></span>

<span data-ttu-id="ffbbf-108">AAD etki alanı Hizmetleri 'ni desteklemesi için Azure sanal ağında tasarım konusunda daha fazla ayrıntı için [sanal ağ dikkat](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="ffbbf-108">For more details on design consideration on Azure Virtual Network to support AAD domain services, see [Virtual Network Consideration](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span></span>

