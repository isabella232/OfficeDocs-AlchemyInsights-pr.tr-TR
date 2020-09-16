---
title: 'AıP: Ilkeler beklendiği gibi çalışmıyor'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663209"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AıP: Ilkeler beklendiği gibi çalışmıyor

Azure bilgi koruması: Ilkeler beklendiği gibi çalışmıyorsa, çeşitli ilke sorunları için önerilen yönergeler için aşağıdakilere bakın:

1. Görsel işaretlerle ilgili sorunlarınız varsa, lütfen [görsel Işaretlemeleri ne zaman uygulandığını](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)gözden geçirin.
2. Otomatik etiketleme ile ilgili sorun yaşıyorsanız, [Azure bilgi koruması için otomatik ve önerilen sınıflandırmaya yönelik koşulların nasıl yapılandırılacağını](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) ve [hassas bilgi türlerinin nasıl göründüğünü](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)gözden geçirin.
3. Yerel/Pfıle korumasıyla ilgili sorunlarınız varsa, lütfen [API yapılandırmasını](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)gözden geçirin.
4. Düzgün yapılandırılmamış kapsamlı ilkeler kullanıp kullanmıyorsanız, [kapsamlı ilkeler kullanarak belirli kullanıcılar Için Azure bilgi koruması ilkesini yapılandırma](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Etiketli bir belge eklerken otomatik etiketleme Outlook 'Ta çalışmıyorsa, DRMEncryptProperty 'in burada açıklandığı şekilde tanımlandığını doğrulayın: [güvenlik Için IRM kayıt defteri ayarları](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Hala sorun yaşıyorsanız, lütfen Azure bilgi koruması istemci günlüklerini ve verilen günlükleri bu biletye ekleyin.

1. Outlook 'ta bir Office belgesi açın veya yeni bir e-posta oluşturun.
2. **Korumak/duyarlılık**  >  **Yardımı ve görüşler**'e tıklayın.
3. **Günlükleri dışarı aktar**'a tıklayın.
4. Günlükleri seçtiğiniz konuma kaydedin ve bu hizmet isteğine ekleyin.

Ek kaynaklar:

- [Azure bilgi koruması için bir etiket yapılandırma](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Azure bilgi koruması belgelerini gözden geçirme](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Microsoft 365 uygulamalarında duyarlılık etiketlerini kullanma](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

