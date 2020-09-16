---
title: 'AıP: Ilkeler beklendiği gibi çalışmıyor'
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
- "9002266"
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663209"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="826da-102">AıP: Ilkeler beklendiği gibi çalışmıyor</span><span class="sxs-lookup"><span data-stu-id="826da-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="826da-103">Azure bilgi koruması: Ilkeler beklendiği gibi çalışmıyorsa, çeşitli ilke sorunları için önerilen yönergeler için aşağıdakilere bakın:</span><span class="sxs-lookup"><span data-stu-id="826da-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="826da-104">Görsel işaretlerle ilgili sorunlarınız varsa, lütfen [görsel Işaretlemeleri ne zaman uygulandığını](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="826da-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="826da-105">Otomatik etiketleme ile ilgili sorun yaşıyorsanız, [Azure bilgi koruması için otomatik ve önerilen sınıflandırmaya yönelik koşulların nasıl yapılandırılacağını](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) ve [hassas bilgi türlerinin nasıl göründüğünü](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="826da-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="826da-106">Yerel/Pfıle korumasıyla ilgili sorunlarınız varsa, lütfen [API yapılandırmasını](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="826da-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="826da-107">Düzgün yapılandırılmamış kapsamlı ilkeler kullanıp kullanmıyorsanız, [kapsamlı ilkeler kullanarak belirli kullanıcılar Için Azure bilgi koruması ilkesini yapılandırma](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="826da-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="826da-108">Etiketli bir belge eklerken otomatik etiketleme Outlook 'Ta çalışmıyorsa, DRMEncryptProperty 'in burada açıklandığı şekilde tanımlandığını doğrulayın: [güvenlik Için IRM kayıt defteri ayarları](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="826da-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="826da-109">Hala sorun yaşıyorsanız, lütfen Azure bilgi koruması istemci günlüklerini ve verilen günlükleri bu biletye ekleyin.</span><span class="sxs-lookup"><span data-stu-id="826da-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="826da-110">Outlook 'ta bir Office belgesi açın veya yeni bir e-posta oluşturun.</span><span class="sxs-lookup"><span data-stu-id="826da-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="826da-111">**Korumak/duyarlılık**  >  **Yardımı ve görüşler**'e tıklayın.</span><span class="sxs-lookup"><span data-stu-id="826da-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="826da-112">**Günlükleri dışarı aktar**'a tıklayın.</span><span class="sxs-lookup"><span data-stu-id="826da-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="826da-113">Günlükleri seçtiğiniz konuma kaydedin ve bu hizmet isteğine ekleyin.</span><span class="sxs-lookup"><span data-stu-id="826da-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="826da-114">Ek kaynaklar:</span><span class="sxs-lookup"><span data-stu-id="826da-114">Additional resources:</span></span>

- [<span data-ttu-id="826da-115">Azure bilgi koruması için bir etiket yapılandırma</span><span class="sxs-lookup"><span data-stu-id="826da-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="826da-116">Azure bilgi koruması belgelerini gözden geçirme</span><span class="sxs-lookup"><span data-stu-id="826da-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="826da-117">Microsoft 365 uygulamalarında duyarlılık etiketlerini kullanma</span><span class="sxs-lookup"><span data-stu-id="826da-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

