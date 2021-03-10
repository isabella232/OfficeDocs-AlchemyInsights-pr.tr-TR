---
title: SAML imzalama sertifikası sorunlarını giderme
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694453"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a>SAML imzalama sertifika sorunlarını giderme

SAML İmzalama sertifika sorununu çözmek için, aşağıdaki önerilen adımları uygulayın:

1. SSO'u destekleyen bir kurumsal uygulama eklerken Azure, SAML İmzalama sertifikası olarak adlandırılan [bir sertifika üretir.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications) Bu sertifikanın son kullanma tarihi 3 yıldır. Sertifikanın son kullanma tarihini değiştirmek için bkz. Federasyon sertifikanız için son kullanma tarihini özelleştirme ve yeni [bir sertifikaya teslim edin.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate)
2. Azure, uygulama tarafından istenen SAML belirteçlerini imzalamak ve başarılı bir SSO için bu sertifikayı uygulamaya göndermek için kullanır. Bunun tamamlanması için Azure portaldan sertifikayı indirin ve SSO işlemini tamamlamak için uygulama satıcısına gönderin.

Bu işlem tamamlandıktan sonra, uygulama bu sertifikaya güvenir ve bu sertifikayla imzalanan tüm SAML belirteçleri uygulama tarafından kabul edilir.

3. Bu sertifikanın süresi dolsa, yeni bir sertifika oluşturun, bunu uygulama satıcısına güncelleştirin ve Azure tarafında etkin hale kurun. Daha fazla bilgi için [bkz. Süresi yakında dolacak olan bir sertifikayı yenileme.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire)

> [!NOTE]
> Sertifikanın süresi dolsa, kullanıcı engellanmaz.

4. [Geçerli sertifikanın süresi dolmadan önce](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) bildirimleri almak için bir e-posta adresi ekleyin.

> [!NOTE]
> 4. Adım isteğe bağlı bir adımdır.

5. Bir uygulamanın SAML sertifika imzalama seçeneklerini ve sertifika imzalama algoritmasını değiştirebilirsiniz. Daha fazla bilgi için [bkz. Sertifika imzalama seçeneklerini ve imzalama algoritmasını değiştirme.](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)

