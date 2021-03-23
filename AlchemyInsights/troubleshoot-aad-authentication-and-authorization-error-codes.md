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
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a><span data-ttu-id="d04c9-102">Azure AD Kimlik Doğrulama ve Yetkilendirme (AADSTS) hata kodlarını giderme</span><span class="sxs-lookup"><span data-stu-id="d04c9-102">Troubleshoot Azure AD Authentication and Authorization (AADSTS) error codes</span></span>

<span data-ttu-id="d04c9-103">AAD kimlik doğrulama ve yetkilendirme hata kodlarını (AADSTS) çözmek için, aşağıdaki önerilen adımları uygulayın:</span><span class="sxs-lookup"><span data-stu-id="d04c9-103">To resolve AAD authentication and authorization error codes (AADSTS), perform the following recommended steps:</span></span>

1. <span data-ttu-id="d04c9-104">**Uygulamanıza hata kodlarını işleme**</span><span class="sxs-lookup"><span data-stu-id="d04c9-104">**Handling error codes in your application**</span></span>

- <span data-ttu-id="d04c9-105">**OAuth2.0 spec**, hata yanıtının hata kısmını kullanarak kimlik doğrulaması sırasında hataların nasıl işlil olduğu https://tools.ietf.org/html/rfc6749#section-5.2 konusunda yol gösterir.</span><span class="sxs-lookup"><span data-stu-id="d04c9-105">The **OAuth2.0 spec**, https://tools.ietf.org/html/rfc6749#section-5.2, provides guidance on how to handle errors during authentication using the error portion of the error response.</span></span>

    - <span data-ttu-id="d04c9-106">**hata:** Oluşan hata türlerini sınıflandırmak ve hatalara tepki olarak kullanılmalıdır.</span><span class="sxs-lookup"><span data-stu-id="d04c9-106">**error**: An error code string that can be used to classify types of errors that occur, and should be used to react to errors.</span></span>
    - <span data-ttu-id="d04c9-107">Hata **alanında** çeşitli olası değerler vardır; belirli hatalar ve tepki verme hakkında daha fazla bilgi için protokol belge bağlantıları ve OAuth 2.0 özellikleri gözden geçirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d04c9-107">The **error** field has several possible values - review the protocol documentation links and OAuth 2.0 specs for more information about specific errors and how to react to them.</span></span>

- <span data-ttu-id="d04c9-108">İşte örnek bir hata yanıtı:</span><span class="sxs-lookup"><span data-stu-id="d04c9-108">Here is a sample error response:</span></span>
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
2. <span data-ttu-id="d04c9-109">**Geçerli hata kodu bilgilerini arama**</span><span class="sxs-lookup"><span data-stu-id="d04c9-109">**Lookup current error code information**</span></span>

- <span data-ttu-id="d04c9-110">Hata kodları ve iletileri değişebilir.</span><span class="sxs-lookup"><span data-stu-id="d04c9-110">Error codes and messages are subject to change.</span></span> <span data-ttu-id="d04c9-111">En güncel bilgiler için, AADSTS hata açıklamalarını, düzeltmelerini ve önerilen bazı geçici https://login.microsoftonline.com/error çözümleri bulmak için sayfaya bakın.</span><span class="sxs-lookup"><span data-stu-id="d04c9-111">For the most current information, see the https://login.microsoftonline.com/error page to find AADSTS error descriptions, fixes, and some suggested workarounds.</span></span>
- <span data-ttu-id="d04c9-112">Ayrıca, Azure AD Kimlik Doğrulaması ve yetkilendirme hata kodları makalesinde listelenen [AADSTS](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) hata kodlarını arayabilir [ve sorunlarını giderebilirsiniz.](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application)</span><span class="sxs-lookup"><span data-stu-id="d04c9-112">You can also search for and troubleshoot [AADSTS error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) listed in the article [Azure AD Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).</span></span>

3. <span data-ttu-id="d04c9-113">**Yardım Al**</span><span class="sxs-lookup"><span data-stu-id="d04c9-113">**Get Help**</span></span>

- <span data-ttu-id="d04c9-114">[Geliştiriciler için destek](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) ve yardım seçenekleri - Belgelerimizde yer alan bir sorunun çözümünde bir soruya yanıta veya yardıma ihtiyacınız varsa, uzmanlardan yardım için ulaşmanın zamanı geldi.</span><span class="sxs-lookup"><span data-stu-id="d04c9-114">[Support and help options for developers](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) - If you need an answer to a question or help in solving a problem not covered in our documentation, it might be time to reach out to experts for help.</span></span> <span data-ttu-id="d04c9-115">Bu makalede, Microsoft kimlik platformuyla tümleştirilmiş uygulamalar geliştirirken sorularınıza yanıt almak için çeşitli öneriler bulabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d04c9-115">This article provides several suggestions for getting answers to your questions as you develop apps that integrate with the Microsoft identity platform.</span></span>








