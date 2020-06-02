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
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="7d60c-102">AIP: Politikalar beklendiği gibi davranmıyor</span><span class="sxs-lookup"><span data-stu-id="7d60c-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="7d60c-103">Azure Bilgi Koruması: Beklendiği gibi davranamayan ilkeler, çeşitli ilke sorunları için önerilen yönergeler için aşağıdakilere bakın:</span><span class="sxs-lookup"><span data-stu-id="7d60c-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="7d60c-104">Görsel işaretlerle ilgili sorunlar yaşıyorsanız, lütfen [görsel işaretlerin ne zaman uygulandığını](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="7d60c-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="7d60c-105">Otomatik etiketleme ile ilgili sorunlar yaşıyorsanız, lütfen [Azure Bilgi Koruması için otomatik ve önerilen sınıflandırma için koşulları nasıl yapılandırabileceğinizi](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) ve [hassas bilgi türlerinin neleri aradığını](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="7d60c-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>
3. <span data-ttu-id="7d60c-106">Yerel/Pfile korumasıyla ilgili sorunlar yaşıyorsanız, lütfen [Dosya API yapılandırması'nı](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="7d60c-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="7d60c-107">Doğru şekilde yapılandırılmamış kapsamlı ilkeler kullanıp kullanmadığınızı kontrol edin: [Kapsamlı ilkeleri kullanarak belirli kullanıcılar için Azure Bilgi Koruması ilkesini yapılandırma.](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)</span><span class="sxs-lookup"><span data-stu-id="7d60c-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="7d60c-108">Etiketli bir belge iliştirirken otomatik etiketleme Outlook için çalışmıyorsa, DRMEncryptProperty'in burada açıklandığı gibi tanımlanmadığını doğrulayın: [Güvenlik için IRM kayıt defteri ayarları.](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)</span><span class="sxs-lookup"><span data-stu-id="7d60c-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="7d60c-109">Sorun yaşamaya devam ediyorsanız, lütfen Azure Bilgi Koruması istemci günlüklerini toplayın ve dışa aktarılan günlükleri bu bilete takın.</span><span class="sxs-lookup"><span data-stu-id="7d60c-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="7d60c-110">Office belgesini açın veya Outlook'ta yeni bir e-posta oluşturun.</span><span class="sxs-lookup"><span data-stu-id="7d60c-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="7d60c-111">**Koruma/Duyarlılık**  >  **Yardım ve geri bildirim'i**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="7d60c-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="7d60c-112">**Günlükleri Dışa**Aktar'ı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="7d60c-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="7d60c-113">Günlükleri seçtiğiniz konuma kaydedin ve bu hizmet isteğine takın.</span><span class="sxs-lookup"><span data-stu-id="7d60c-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="7d60c-114">Ek kaynaklar:</span><span class="sxs-lookup"><span data-stu-id="7d60c-114">Additional resources:</span></span>

- [<span data-ttu-id="7d60c-115">Azure Bilgi Koruması için görsel işaretler için etiket nasıl yapılandırılabilen</span><span class="sxs-lookup"><span data-stu-id="7d60c-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="7d60c-116">Azure Bilgi Koruması belgelerini gözden geçirin</span><span class="sxs-lookup"><span data-stu-id="7d60c-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="7d60c-117">Office uygulamalarında duyarlılık etiketlerini kullanma</span><span class="sxs-lookup"><span data-stu-id="7d60c-117">Use sensitivity labels in Office apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

