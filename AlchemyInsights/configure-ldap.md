---
title: LDAP'yi yapılandırma
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
ms.openlocfilehash: 3f1f9728cdcfbe5676e5afc45b2afe82836fed9c8907df3559ac7daec21194ed
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090432"
---
# <a name="configure-ldap"></a>LDAP'yi yapılandırma

LDAP'yi yapılandırmak için şunları yapın:

1. Azure portalda etki alanınız durumunu [kontrol edin.](https://aka.ms/aadds-health)
1. Geçerli bir Azure AD aboneliğinin kullanılabilir olduğundan ve Azure AD Etki Alanı Hizmetleri'nin etkinleştirildiğinden emin olun.
1. Güvenli LDAP'yi etkinleştirmek için gereken sertifika güvenilir bir genel sertifika yetkiliden alın olmalı veya otomatik olarak imzalanan bir sertifika olmalı.
1. Sertifikanın gerekli yönergelere uygun olduğundan emin [olun.](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)

**Geçersiz Sertifika**
1. Sertifikayı yenilemek için, adımları izleyin ve yeni sertifika oluşturun ve yeniden yükleyin: [LDAP'yi yapılandırma.](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)
1. Azure Active Directory Etki Alanı Hizmetleri'nin Güvenli LDAP uyarılarında bilinen sorunu çözmek için [BKZ. LDAP uyarılarını çözme.](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)
