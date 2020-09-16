---
title: Duyarlılık etiketleri görünmüyor
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 6a64e001be115c8e5553a0d8c97b8cb815922c69
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801204"
---
# <a name="sensitivity-labels-not-appearing"></a><span data-ttu-id="b61db-102">Duyarlılık etiketleri görünmüyor</span><span class="sxs-lookup"><span data-stu-id="b61db-102">Sensitivity labels not appearing</span></span>

<span data-ttu-id="b61db-103">Duyarlılık etiketleri hassas içeriğinizi sınıflandırmanıza ve korunmanıza olanak tanır.</span><span class="sxs-lookup"><span data-stu-id="b61db-103">Sensitivity labels allow you to classify and help protect your sensitive content.</span></span> <span data-ttu-id="b61db-104">Microsoft 365 Uyumluluk Merkezi, Microsoft 365 güvenlik merkezi veya Microsoft 365 güvenlik & Uyumluluk Merkezi 'nde sınıflandırma > duyarlılık etiketleri altında oluşturulabilir.</span><span class="sxs-lookup"><span data-stu-id="b61db-104">They can be created in the Microsoft 365 compliance center, Microsoft 365 security center, or Microsoft 365 security & Compliance Center under Classification > Sensitivity labels.</span></span> <span data-ttu-id="b61db-105">Bu özellik hakkında daha fazla bilgi edinmek için [duyarlılık etiketlerine genel bakış](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="b61db-105">To learn more about this feature, see [Overview of sensitivity labels](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).</span></span>

<span data-ttu-id="b61db-106">Duyarlılık etiketlerinizi yapılandırdıysanız ancak Microsoft 365 uygulamalarında görünmüyorsa, aşağıdakileri denetleyin:</span><span class="sxs-lookup"><span data-stu-id="b61db-106">If you configured your sensitivity labels but they aren't appearing in the Microsoft 365 apps, check the following:</span></span>

- <span data-ttu-id="b61db-107">Duyarlılık etiketinin, istediğiniz kullanıcı ve gruplara [yayımlandığını](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="b61db-107">Confirm that the sensitivity label has been [published](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) to the users and groups that you want.</span></span>

- <span data-ttu-id="b61db-108">Kullanıcının, duyarlılık etiketlerini destekleyen bir uygulamayı kullandığını doğrulayın- [belgenizdeki duyarlılık etiketlerine](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable)bakın.</span><span class="sxs-lookup"><span data-stu-id="b61db-108">Confirm that the user is using an app that supports sensitivity labels - see [sensitivity labels in your document](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).</span></span>

- <span data-ttu-id="b61db-109">[Azure Information Protection etiketlerini geçiriyorsanız](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), [burada](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)listelenen dikkat edilmesi gereken noktaları göz önünde bulundurun.</span><span class="sxs-lookup"><span data-stu-id="b61db-109">If you're [migrating Azure Information Protection labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), be aware of the considerations listed [here](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span></span>

- <span data-ttu-id="b61db-110">Veri kaybı önleme (DLP) desteği: şimdilik yalnızca bekletme etiketleri DLP ilkelerinde bir koşul olarak kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="b61db-110">Data loss prevention (DLP) support: Currently, only retention labels can be used as a condition in DLP policies.</span></span>  <span data-ttu-id="b61db-111">DLP ilkesindeki duyarlılık etiketleri desteği henüz kullanılamaz, ancak üzerinde çalışıyoruz.</span><span class="sxs-lookup"><span data-stu-id="b61db-111">Support for sensitivity labels in a DLP policy is not available yet but we're working on it.</span></span>

- <span data-ttu-id="b61db-112">Duyarlılık etiketinde şifreleme etkinleştirildiğinde şunları yapabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="b61db-112">When encryption is enabled on a sensitivity label, you can choose either to:</span></span>
    - <span data-ttu-id="b61db-113">İzinleri şimdi ata</span><span class="sxs-lookup"><span data-stu-id="b61db-113">Assign permissions now</span></span>
    - <span data-ttu-id="b61db-114">Kullanıcıların izin atamasına izin verme</span><span class="sxs-lookup"><span data-stu-id="b61db-114">Let users assign permissions</span></span>


<span data-ttu-id="b61db-115">Olası sorunlar hakkında daha fazla bilgi için [duyarlılık etiketleriyle Ilgili bilinen sorunlar](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="b61db-115">For more information on possible issues, see [Known issues with sensitivity labels](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span></span>