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
ms.openlocfilehash: 7926ff9ebbd54969fb5b3ae5d909baffe96a4292
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/26/2020
ms.locfileid: "44493421"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: Politikalar beklendiği gibi davranmıyor

Azure Bilgi Koruması: Beklendiği gibi davranamayan ilkeler, çeşitli ilke sorunları için önerilen yönergeler için aşağıdakilere bakın:

1. Görsel işaretlerle ilgili sorunlar yaşıyorsanız, lütfen [görsel işaretlerin ne zaman uygulandığını](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)gözden geçirin.
2. Otomatik etiketleme ile ilgili sorunlar yaşıyorsanız, lütfen [Azure Bilgi Koruması için otomatik ve önerilen sınıflandırma için koşulları nasıl yapılandırabileceğinizi](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) ve [hassas bilgi türlerinin neleri aradığını](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)gözden geçirin.
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

