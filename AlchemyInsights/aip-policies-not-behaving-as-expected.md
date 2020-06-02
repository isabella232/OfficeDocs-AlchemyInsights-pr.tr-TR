---
title: 'AIP: Politikalar beklendiği gibi davranmıyor'
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
- "4780"
ms.openlocfilehash: 527556fcb02525eb88ea992c38a2ddfcba6f9453
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506578"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: Politikalar beklendiği gibi davranmıyor

Azure Bilgi Koruması: Beklendiği gibi davranamayan ilkeler, çeşitli ilke sorunları için önerilen yönergeler için aşağıdakilere bakın:

1. Görsel işaretlerle ilgili sorunlar yaşıyorsanız, lütfen [görsel işaretlerin ne zaman uygulandığını](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)gözden geçirin.
2. Otomatik etiketleme ile ilgili sorunlar yaşıyorsanız, lütfen [Azure Bilgi Koruması için otomatik ve önerilen sınıflandırma için koşulları nasıl yapılandırabileceğinizi](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) ve [hassas bilgi türlerinin neleri aradığını](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)gözden geçirin.
3. Yerel/Pfile korumasıyla ilgili sorunlar yaşıyorsanız, lütfen [Dosya API yapılandırması'nı](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)gözden geçirin.
4. Doğru şekilde yapılandırılmamış kapsamlı ilkeler kullanıp kullanmadığınızı kontrol edin: [Kapsamlı ilkeleri kullanarak belirli kullanıcılar için Azure Bilgi Koruması ilkesini yapılandırma.](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)
5. Etiketli bir belge iliştirirken otomatik etiketleme Outlook için çalışmıyorsa, DRMEncryptProperty'in burada açıklandığı gibi tanımlanmadığını doğrulayın: [Güvenlik için IRM kayıt defteri ayarları.](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)

Sorun yaşamaya devam ediyorsanız, lütfen Azure Bilgi Koruması istemci günlüklerini toplayın ve dışa aktarılan günlükleri bu bilete takın.

1. Office belgesini açın veya Outlook'ta yeni bir e-posta oluşturun.
2. **Koruma/Duyarlılık**  >  **Yardım ve geri bildirim'i**tıklatın.
3. **Günlükleri Dışa**Aktar'ı tıklatın.
4. Günlükleri seçtiğiniz konuma kaydedin ve bu hizmet isteğine takın.

Ek kaynaklar:

- [Azure Bilgi Koruması için görsel işaretler için etiket nasıl yapılandırılabilen](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Azure Bilgi Koruması belgelerini gözden geçirin](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Office uygulamalarında duyarlılık etiketlerini kullanma](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

