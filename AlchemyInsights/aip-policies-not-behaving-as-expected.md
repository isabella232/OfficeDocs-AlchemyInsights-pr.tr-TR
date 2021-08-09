---
title: 'AIP: İlkeler beklendiği gibi değil'
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
- "4780"
ms.openlocfilehash: 90448bf57297ce59ba222efd1927b5de588bfbfdb1206b6403764d7f43fed690
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934313"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: İlkeler beklendiği gibi değil

Azure Information Protection: İlkeler beklendiği gibi değil, çeşitli ilke sorunlarıyla ilgili önerilen yönergeler için aşağıdakilere bakın:

1. Görsel işaretlerle ilgili sorun ediyorsanız, lütfen Görsel işaretler [uygulandığında yazıyı gözden geçirin.](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)
2. Otomatik etiketlemeyle ilgili sorunlar ediyorsanız, lütfen [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) için otomatik ve önerilen sınıflandırma koşullarını yapılandırma ve Hassas bilgi türlerinin ne için arama yaptığını gözden geçirme [.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
3. Yerel/Pfile korumasıyla ilgili sorunlar ediyorsanız, lütfen Dosya [API yapılandırmasında gözden geçirmeyi unutmayın.](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)
4. Düzgün yapılandırılmamış kapsamda ilkeleri olup olmadığını denetleyin: Kapsamı olan ilkeleri kullanarak belirli kullanıcılar için Azure Information Protection ilkesi [nasıl yapılandırılır?](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)
5. Etiketli bir belge eklerken Outlook etiketleme çalışmıyorsa DRMEncryptProperty'in burada açıklandığı gibi tanımlanmamış olduğunu doğrulayın: Güvenlik için [IRM](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)kayıt defteri ayarları .

Hala sorun yaşıyorsanız, lütfen Azure Information Protection istemci günlüklerini toplayın ve dışarı aktarma günlüklerini bu bilete iliştirin.

1. Office'da bir belge açın veya e-posta Outlook.
2. **Koru/Duyarlılık Yardımı ve geri**  >  **bildirim'e tıklayın.**
3. Günlükleri Dışarı **Aktar 'a tıklayın.**
4. Günlükleri tercih konumunuzla kaydedin ve bunları bu hizmet isteğine iliştirin.

Ek kaynaklar:

- [Azure Information Protection'da görsel işaretlere uygun etiketi yapılandırma](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Azure Information Protection belgelerini gözden geçirme](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Microsoft 365 Microsoft 365 kullanma](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

