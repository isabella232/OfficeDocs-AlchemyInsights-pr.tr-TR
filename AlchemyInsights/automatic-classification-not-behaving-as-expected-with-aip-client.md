---
title: Otomatik sınıflandırma AIP istemcilerinde beklendiği gibi değil
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
- "9002266"
- "4373"
ms.openlocfilehash: b7ab09fe8430a54dacf2cd1ba076414a5f562541
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820918"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Otomatik sınıflandırma AIP istemcilerinde beklendiği gibi değil

Otomatik sınıflandırma beklendiği gibi değil, aşağıdaki önerilen yönergeleri kullanın:

1. Otomatik etiketlemeyle ilgili sorunlar ediyorsanız, bkz. [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) için otomatik ve önerilen sınıflandırma koşullarını yapılandırma ve Hassas bilgi türlerinin ne için [bakması gerekir.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
2. Düzgün yapılandırılmamış kapsamda ilkeleri olup olmadığını denetleyin: Kapsamı olan ilkeleri kullanarak belirli kullanıcılar için Azure Information Protection ilkesi [nasıl yapılandırılır?](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)
3. Etiketli bir belge eklerken Outlook'ta otomatik etiketleme çalışmıyorsa, burada açıklandığı gibi tanımlanmamış olduğunu doğrulayın: Güvenlik için `DRMEncryptProperty` [IRM kayıt defteri ayarları](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. Azure Information Protection [ilkeniz için yerleşik bilgi](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) türlerini kullandınız, içeriğinizin beklenen biçimle eşleni olduğunu doğrulayın.
5. Etiketin Otomatik veya Önerilen için uygun şekilde  **yapılandırıldığından emin olmak.** (**Otomatik** etiketleme tüm Microsoft 365 uygulamaları  için kullanılabilir, ancak Outlook dışında tüm Microsoft 365 uygulamaları için önerilir.)
6. Daha önce el ile etiketlenmiş veya daha önce daha önce daha yüksek bir sınıflandırmaya göre otomatik olarak etiketlenmiş belgeler ve e-postalar için otomatik sınıflandırma kullanılamaz.  Daha fazla bilgi için bkz. [Otomatik veya önerilen etiketler nasıl uygulanır?](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied)
7. Hala sorun yaşıyorsanız, lütfen Azure Information Protection istemci günlüklerini toplayın ve dışarı aktar alınan günlükleri destek biletinize iliştirin. Azure Information Protection günlüklerini dışarı aktarma:
    - Bir Office belgesi açın veya Outlook'ta yeni e-posta oluşturun.
    - **Koru/Duyarlılık Yardımı ve geri**  >  **bildirim'e tıklayın.**
    - Günlükleri Dışarı **Aktar 'a tıklayın.**
    - Günlükleri tercih konumunuzla kaydedin ve hizmet isteğinize iliştirin.

Ek bilgi için bkz:

- [Azure Information Protection için otomatik ve önerilen sınıflandırma koşullarını yapılandırma](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Azure Information Protection kullanan yaygın senaryolar için nasıl işlem kılavuzları](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Azure Information Protection belgelerini gözden geçirme](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Azure Information Protection aboneliklerini ve özelliklerini gözden geçirme](https://azure.microsoft.com/pricing/details/information-protection)
- [Azure Information Protection gereksinimleri](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Azure Information Protection hızlı başlangıç öğreticisi](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Azure Information Protection istemcisini indirin](https://www.microsoft.com/download/details.aspx?id=53018)
