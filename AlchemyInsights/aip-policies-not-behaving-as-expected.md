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
ms.openlocfilehash: 7baa010cc0b18b5d2a295623639fabf2bc5f88ec
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821647"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="f1242-102">AIP: İlkeler beklendiği gibi değil</span><span class="sxs-lookup"><span data-stu-id="f1242-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="f1242-103">Azure Information Protection: İlkeler beklendiği gibi değil, çeşitli ilke sorunlarıyla ilgili önerilen yönergeler için aşağıdakilere bakın:</span><span class="sxs-lookup"><span data-stu-id="f1242-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="f1242-104">Görsel işaretlerle ilgili sorun ediyorsanız, lütfen Görsel işaretler [uygulandığında yazıyı gözden geçirin.](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)</span><span class="sxs-lookup"><span data-stu-id="f1242-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="f1242-105">Otomatik etiketlemeyle ilgili sorunlar ediyorsanız, lütfen [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) için otomatik ve önerilen sınıflandırma koşullarını yapılandırma ve Hassas bilgi türlerinin ne için arama yaptığını gözden geçirme [.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="f1242-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="f1242-106">Yerel/Pfile korumasıyla ilgili sorunlar ediyorsanız, lütfen Dosya [API yapılandırmasında gözden geçirmeyi unutmayın.](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)</span><span class="sxs-lookup"><span data-stu-id="f1242-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="f1242-107">Düzgün yapılandırılmamış kapsamda ilkeleri olup olmadığını denetleyin: Kapsamı olan ilkeleri kullanarak belirli kullanıcılar için Azure Information Protection ilkesi [nasıl yapılandırılır?](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)</span><span class="sxs-lookup"><span data-stu-id="f1242-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="f1242-108">Etiketli bir belge eklerken Outlook'ta otomatik etiketleme çalışmıyorsa, DRMEncryptProperty'in burada açıklandığı gibi tanımlanmamış olduğunu doğrulayın: Güvenlik için [IRM](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)kayıt defteri ayarları .</span><span class="sxs-lookup"><span data-stu-id="f1242-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="f1242-109">Hala sorun yaşıyorsanız, lütfen Azure Information Protection istemci günlüklerini toplayın ve dışarı aktarma günlüklerini bu bilete iliştirin.</span><span class="sxs-lookup"><span data-stu-id="f1242-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="f1242-110">Bir Office belgesi açın veya Outlook'ta yeni e-posta oluşturun.</span><span class="sxs-lookup"><span data-stu-id="f1242-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="f1242-111">**Koru/Duyarlılık Yardımı ve geri**  >  **bildirim'e tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="f1242-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="f1242-112">Günlükleri Dışarı **Aktar 'a tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="f1242-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="f1242-113">Günlükleri tercih konumunuzla kaydedin ve bunları bu hizmet isteğine iliştirin.</span><span class="sxs-lookup"><span data-stu-id="f1242-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="f1242-114">Ek kaynaklar:</span><span class="sxs-lookup"><span data-stu-id="f1242-114">Additional resources:</span></span>

- [<span data-ttu-id="f1242-115">Azure Information Protection'da görsel işaretlere uygun etiketi yapılandırma</span><span class="sxs-lookup"><span data-stu-id="f1242-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="f1242-116">Azure Information Protection belgelerini gözden geçirme</span><span class="sxs-lookup"><span data-stu-id="f1242-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="f1242-117">Microsoft 365 uygulamalarına duyarlılık etiketleri kullanma</span><span class="sxs-lookup"><span data-stu-id="f1242-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

