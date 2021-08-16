---
title: Uyumluluk Merkezi'nde AIP'den MIP/Birleşik Etiketleme'ye geçiş
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 378c3f58f77db8b23682432c942cd4f9c3a392651ca6564528a635724ad66a25
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54000386"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Uyumluluk Merkezi'nde AIP'den MIP/Birleşik Etiketleme'ye geçiş

Güvenlik ve Uyumluluk Merkezi'nde AIP etiketlerinden Birleşik Etiketleme'ye geçiş yapmak için şunları yapın:

**Azure portaldan korumayı etkinleştirme**

1. Henüz açmadısanız yeni bir tarayıcı penceresi açın ve [Azure portalında oturum açın.](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal) **Azure Information Protection blade'a** gidin. Örneğin, hub menüsünde Tüm **hizmetler'e tıklayın ve** Filtre **kutusuna Bilgi** yazmaya başlayın. **Azure Information Protection öğesini seçin.** Azure Information Protection blade'e daha önce erişemediysanız [](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) bu blade'i portala eklemek için tek seferlik ek adımlara bakın. Azure Information Protection blade'i açmak için, [Azure Information Protection Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) planınız veya Hak Yönetimi Office 365 içeren bir Office 365 planınız olması gerekir. Bu aboneliklerden birini kullanıyorsanız ancak geçerli bir aboneliğin buluna olmadığını haber veren bir ileti görüyorsanız [Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) Desteği'ne başvurun veya standart destek kanallarınızı kullanın.

2. Yönet menü **seçeneklerini** bulun ve Koruma **etkinleştirme'yi seçin.** **Etkinleştir'e** tıklayın ve ardından eyleminizi onaylayın. Etkinleştirme tamamlandığında, bilgi çubuğunda Etkinleştirme başarıyla **tamamlandı olarak görüntülenir.**

**Azure Information Protection etiketlerini Güvenlik ve uyumluluk Office 365'& geçirme**

1. Genel Yönetici izni olan bir kullanıcı olarak oturum açtığınızdan emin olun.

2. **Azure Information Protection blade'a** gidin.

3. Yönet menü **seçeneğinden** Birleşik **etiketleme'yi seçin.**

4. Azure **Information Protection - Birleşik etiketleme blade'inde** Etkinleştir'e **tıklayın** ve çevrimiçi yönergeleri izleyin.

**Not:** Güvenlik ve Uyumluluk Merkezi Geçişi'ne etkinleştirmeden önce uygun izinlere & doğrulayın. Daha fazla bilgi için şu makalelere bakın:

1. [Azure Information Protection'i yapılandırmak için genel yönetici mi olmak gerekiyor yoksa diğer yöneticilere temsilci de kullanabilir miyim?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Güvenlik ve Uyumluluk Merkezi'ne katıldıktan sonra yönetim rolleri & bilgiler.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Güvenlik ve Uyumluluk Merkezi'ne Birleşik Etiketleme için AIP geçişi hakkında daha fazla bilgi için bkz. [Etiketleri geçirme](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).
