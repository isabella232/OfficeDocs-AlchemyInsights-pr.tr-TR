---
title: Otomatik sınıflandırma AIP istemcisi ile beklendiği gibi davranmaz
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4373"
ms.openlocfilehash: 22eeb6ba32e4e943efa2495a477ff394f3c135db
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508396"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Otomatik sınıflandırma AIP istemcisi ile beklendiği gibi davranmaz

Otomatik sınıflandırma beklendiği gibi davranmıyorsa, aşağıdaki önerilen yönergeleri kullanın:

1. Otomatik etiketleme yle ilgili sorunlar yaşıyorsanız, [Azure Bilgi Koruması için otomatik ve önerilen sınıflandırma koşullarının nasıl yapılandırılabildiğini](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) ve hassas bilgi [türlerinin ne aradığına](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)bakın.
2. Doğru şekilde yapılandırılmamış kapsamlı ilkeler kullanıp kullanmadığınızı kontrol edin: [Kapsamlı ilkeleri kullanarak belirli kullanıcılar için Azure Bilgi Koruması ilkesini yapılandırma.](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)
3. Etiketli bir belge eklenirken otomatik etiketleme Outlook için çalışmıyorsa, `DRMEncryptProperty` burada açıklandığı gibi tanımlanmadığını doğrulayın: [Güvenlik için IRM kayıt defteri ayarları.](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)
4. Azure Bilgi Koruması politikanız için [yerleşik bilgi türlerini](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) kullandıysanız, içeriğinizin beklenen biçimle eşleştiğini doğrulayın.
5. Etiketin **Otomatik** veya **Önerilen**için uygun şekilde yapılandırıldığından doğrulayın. ( Tüm Office uygulamaları için**otomatik** etiketleme kullanılabilirken, **Önerilen** tüm Office uygulamaları Outlook hariç kullanılabilir.)
6. Daha önce el ile etiketlenmiş veya daha önce daha yüksek bir sınıflandırmayla otomatik olarak etiketlenmiş belgeler ve e-postalar için otomatik sınıflandırma kullanamazsınız.  Daha fazla bilgi için bkz: [Otomatik veya önerilen etiketler nasıl uygulanır.](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied)
7. Sorun yaşamaya devam ediyorsanız, lütfen Azure Bilgi Koruması istemci günlüklerini toplayın ve dışa aktarılan günlükleri destek biletinize takın. Azure Bilgi Koruması günlüklerini dışa aktarmak için:
    - Office belgesini açın veya Outlook'ta yeni bir e-posta oluşturun.
    - **Koruma/Duyarlılık**  >  **Yardım ve geri bildirim'i**tıklatın.
    - **Günlükleri Dışa**Aktar'ı tıklatın.
    - Günlükleri seçtiğiniz konuma kaydedin ve servis isteğinize takın.

Daha fazla bilgi için bkz:

- [Azure Bilgi Koruması için otomatik ve önerilen sınıflandırma için koşullar nasıl yapılandırılır?](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Azure Bilgi Koruması kullanan yaygın senaryolar için nasıl kullanılır kılavuzları](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Azure Bilgi Koruması belgelerini gözden geçirin](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Azure Bilgi Koruması aboneliklerini ve özelliklerini inceleyin](https://azure.microsoft.com/pricing/details/information-protection)
- [Azure Bilgi Koruması Gereksinimleri](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Azure Bilgi Koruması için hızlı başlangıç öğreticisi](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Azure Bilgi Koruması istemcisi indirin](https://www.microsoft.com/download/details.aspx?id=53018)
