---
title: AıP 'den MıP/Birleşik etiketleme 'ye Uyumluluk Merkezi 'nde geçiş
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
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674346"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>AıP 'den MıP/Birleşik etiketleme 'ye Uyumluluk Merkezi 'nde geçiş

Bir IP etiketlerinden, güvenlik ve Uyumluluk Merkezi 'nde Birleşik etiketleme 'a geçmek için aşağıdakileri yapın:

**Azure portalında korumayı etkinleştirme**

1. Şimdiye kadar yapmadıysanız, yeni bir tarayıcı penceresi açın ve [Azure portalında oturum açın](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal). **Azure bilgi koruması** dikey öğesine gidin. Örneğin, hub menüsünde **tüm hizmetler** 'e tıklayın ve filtre kutusuna **bilgileri** yazmaya başlayın. **Azure bilgi koruması**'nı seçin. Daha önce Azure Information Protection Blade 'e erişmediniz, bu dikey pencereyi portala eklemek için bir kerelik [ek adımlara](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) bakın. Azure Information Protection Blade 'i açmak için, [Azure Information Protection Premium planı](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) veya hak yönetimi Içeren bir Office 365 planınız olmalıdır. Bu aboneliklerden birine sahipseniz ancak geçerli bir aboneliğin bulunamadığını belirten bir ileti görürseniz, [Microsoft destek 'e başvurun](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) veya standart destek kanallarınız kullanın.

2. **Yönet** menüsü seçeneklerini bulun ve **koruma etkinleştirme**'yi seçin. **Etkinleştir**'i tıklatın ve sonra eyleminizi onaylayın. Etkinleştirme tamamlandığında bilgi çubuğunda **etkinleştirme başarıyla tamamlandı**görüntülenir.

**Azure bilgi koruması etiketlerini Office 365 güvenlik & Uyumluluk Merkezi 'ne geçirme**

1. Genel yönetici izni olan bir kullanıcı olarak oturum açtığınızdan emin olun.

2. **Azure bilgi koruması** dikey öğesine gidin.

3. **Yönet** menüsü seçeneğinden **Birleşik etiketleme**'yi seçin.

4. **Azure Information Protection-Birleşik etiketleme** dikey 'da **Etkinleştir** 'i tıklatın ve çevrimiçi yönergeleri izleyin.

**Not**: güvenlik & Uyumluluk Merkezi geçişini etkinleştirmeden önce uygun izinlere sahip olduğunuzu doğrulayın. Daha fazla bilgi için şu makalelere bakın:

1. [Azure bilgi koruması 'nı yapılandırmak veya başka yöneticilere temsilci seçmek için genel yönetici olmanız mı gerekiyor?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Güvenlik & Uyumluluk Merkezi 'ne geçtikten sonra yönetim rolleriyle ilgili önemli bilgiler.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Güvenlik ve Uyumluluk Merkezi 'ne ASııP ile Birleşik etiketleme arasında geçiş hakkında daha fazla bilgi [için bkz.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)
