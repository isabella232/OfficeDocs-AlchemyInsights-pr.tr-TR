---
title: LDAP yapılandırma
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
- "9004394"
- "7923"
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885581"
---
# <a name="configure-ldap"></a><span data-ttu-id="4b995-102">LDAP yapılandırma</span><span class="sxs-lookup"><span data-stu-id="4b995-102">Configure LDAP</span></span>

<span data-ttu-id="4b995-103">LDAP yapılandırmak için aşağıdakileri yapın:</span><span class="sxs-lookup"><span data-stu-id="4b995-103">To configure LDAP, do the following:</span></span>

1. <span data-ttu-id="4b995-104">[Azure portalında](https://aka.ms/aadds-health)etki alanınızın sağlığını denetleyin.</span><span class="sxs-lookup"><span data-stu-id="4b995-104">Check your domain’s health on the [Azure portal](https://aka.ms/aadds-health).</span></span>
1. <span data-ttu-id="4b995-105">Geçerli bir Azure AD aboneliği olduğundan ve Azure AD etki alanı Hizmetleri 'nin etkinleştirildiğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="4b995-105">Ensure a valid Azure AD subscription is available and Azure AD Domain Services has been enabled.</span></span>
1. <span data-ttu-id="4b995-106">Güvenli LDAP 'ı etkinleştirmek için gereken sertifika, güvenilir bir genel sertifika yetkilisinden alınmalı veya otomatik olarak imzalanan bir sertifika olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="4b995-106">The certificate required to enable secure LDAP must be obtained from a trusted public certification authority or be a self-signed certificate.</span></span>
1. <span data-ttu-id="4b995-107">Sertifikanın gerekli [talimatları](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)takip edin.</span><span class="sxs-lookup"><span data-stu-id="4b995-107">Ensure the certificate follows the required [guidelines](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).</span></span>

<span data-ttu-id="4b995-108">**Geçersiz sertifika**</span><span class="sxs-lookup"><span data-stu-id="4b995-108">**Invalid Certificate**</span></span>
1. <span data-ttu-id="4b995-109">Sertifikayı yenilemek için, yeni sertifika oluşturmak ve yeniden karşıya yüklemek [için aşağıdaki adımları izleyin.](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="4b995-109">To renew a certificate, follow the steps to create a new certificate and reupload: [Configure LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
1. <span data-ttu-id="4b995-110">Azure Active Directory etki alanı Hizmetleri 'ndeki Güvenli LDAP uyarıları ile ilgili bilinen sorunları çözmek için [LDAP uyarılarını çözme](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)bölümüne bakın.</span><span class="sxs-lookup"><span data-stu-id="4b995-110">To resolve known issue with Secure LDAP alerts in Azure Active directory Domain Services, see [Resolve LDAP alerts](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
