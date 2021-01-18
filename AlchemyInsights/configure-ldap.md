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
# <a name="configure-ldap"></a>LDAP yapılandırma

LDAP yapılandırmak için aşağıdakileri yapın:

1. [Azure portalında](https://aka.ms/aadds-health)etki alanınızın sağlığını denetleyin.
1. Geçerli bir Azure AD aboneliği olduğundan ve Azure AD etki alanı Hizmetleri 'nin etkinleştirildiğinden emin olun.
1. Güvenli LDAP 'ı etkinleştirmek için gereken sertifika, güvenilir bir genel sertifika yetkilisinden alınmalı veya otomatik olarak imzalanan bir sertifika olmalıdır.
1. Sertifikanın gerekli [talimatları](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)takip edin.

**Geçersiz sertifika**
1. Sertifikayı yenilemek için, yeni sertifika oluşturmak ve yeniden karşıya yüklemek [için aşağıdaki adımları izleyin.](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)
1. Azure Active Directory etki alanı Hizmetleri 'ndeki Güvenli LDAP uyarıları ile ilgili bilinen sorunları çözmek için [LDAP uyarılarını çözme](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)bölümüne bakın.
