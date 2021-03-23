---
title: Azure AD Kimlik Doğrulama ve Yetkilendirme (AADSTS) hata kodlarını giderme
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9800"
- "9005744"
ms.openlocfilehash: 14555dfcb1406fd3a3977012393714a713ff80dc
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037842"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a>Azure AD Kimlik Doğrulama ve Yetkilendirme (AADSTS) hata kodlarını giderme

AAD kimlik doğrulama ve yetkilendirme hata kodlarını (AADSTS) çözmek için, aşağıdaki önerilen adımları uygulayın:

1. **Uygulamanıza hata kodlarını işleme**

- **OAuth2.0 spec**, hata yanıtının hata kısmını kullanarak kimlik doğrulaması sırasında hataların nasıl işlil olduğu https://tools.ietf.org/html/rfc6749#section-5.2 konusunda yol gösterir.

    - **hata:** Oluşan hata türlerini sınıflandırmak ve hatalara tepki olarak kullanılmalıdır.
    - Hata **alanında** çeşitli olası değerler vardır; belirli hatalar ve tepki verme hakkında daha fazla bilgi için protokol belge bağlantıları ve OAuth 2.0 özellikleri gözden geçirebilirsiniz.

- İşte örnek bir hata yanıtı:
```
{
  "error": "invalid_scope",
  "error_description": "AADSTS70011: The provided value for the input parameter 'scope' is not 
valid. The scope https://example.contoso.com/activity.read is not valid.\r\nTrace ID: 255d1aef- 8c98-452f-ac51-23d051240864\r\nCorrelation ID: fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7\r\nTimestamp: 2016-01-09 02:02:12Z",
  "error_codes": [
    70011
  ],
  "timestamp": "2016-01-09 02:02:12Z",
  "trace_id": "255d1aef-8c98-452f-ac51-23d051240864",
  "correlation_id": "fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7", 
  "error_uri":"https://login.microsoftonline.com/error?code=70011"
}
```
2. **Geçerli hata kodu bilgilerini arama**

- Hata kodları ve iletileri değişebilir. En güncel bilgiler için, AADSTS hata açıklamalarını, düzeltmelerini ve önerilen bazı geçici https://login.microsoftonline.com/error çözümleri bulmak için sayfaya bakın.
- Ayrıca, Azure AD Kimlik Doğrulaması ve yetkilendirme hata kodları makalesinde listelenen [AADSTS](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) hata kodlarını arayabilir [ve sorunlarını giderebilirsiniz.](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application)

3. **Yardım Al**

- [Geliştiriciler için destek](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) ve yardım seçenekleri - Belgelerimizde yer alan bir sorunun çözümünde bir soruya yanıta veya yardıma ihtiyacınız varsa, uzmanlardan yardım için ulaşmanın zamanı geldi. Bu makalede, Microsoft kimlik platformuyla tümleştirilmiş uygulamalar geliştirirken sorularınıza yanıt almak için çeşitli öneriler bulabilirsiniz.








