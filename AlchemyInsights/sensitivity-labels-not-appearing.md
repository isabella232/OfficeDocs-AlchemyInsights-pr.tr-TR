---
title: Duyarlılık etiketleri görünmüyor
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 67719380aea0481f96c03fa591542e8e5a6e6993
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048672"
---
# <a name="sensitivity-labels-not-appearing"></a><span data-ttu-id="80e45-102">Duyarlılık etiketleri görünmüyor</span><span class="sxs-lookup"><span data-stu-id="80e45-102">Sensitivity labels not appearing</span></span>

<span data-ttu-id="80e45-103">Duyarlılık etiketleri, hassas içeriğinizi sınıflandırmanıza ve korumanıza yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="80e45-103">Sensitivity labels allow you to classify and help protect your sensitive content.</span></span> <span data-ttu-id="80e45-104">Microsoft 365 uyumluluk merkezi, Microsoft 365 güvenlik merkezi veya Office 365 Güvenlik & Uyumluluk Merkezi'nde Sınıflandırma > Duyarlılığı etiketleri altında oluşturulabilirler.</span><span class="sxs-lookup"><span data-stu-id="80e45-104">They can be created in the Microsoft 365 compliance center, Microsoft 365 security center, or Office 365 Security & Compliance Center under Classification > Sensitivity labels.</span></span> <span data-ttu-id="80e45-105">Bu özellik hakkında daha fazla bilgi edinmek için [duyarlılık etiketlerine genel bakış](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels)bölümüne bakın.</span><span class="sxs-lookup"><span data-stu-id="80e45-105">To learn more about this feature, see [Overview of sensitivity labels](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels).</span></span>

<span data-ttu-id="80e45-106">Duyarlılık etiketlerinizi yapılandırmış ancak Office uygulamalarında görünmüyorsa aşağıdakileri kontrol edin:</span><span class="sxs-lookup"><span data-stu-id="80e45-106">If you configured your sensitivity labels but they aren't appearing in the Office apps, check the following:</span></span>

- <span data-ttu-id="80e45-107">Duyarlılık etiketinin istediğiniz kullanıcılara ve gruplara [yayımlandığını](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do) doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="80e45-107">Confirm that the sensitivity label has been [published](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do) to the users and groups that you want.</span></span>

- <span data-ttu-id="80e45-108">Kullanıcının duyarlılık etiketlerini destekleyen bir uygulama kullandığını doğrulayın - [belgenizde duyarlılık etiketlerini](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?ad=US&ui=en-US&rs=en-US#bkmk_whereavailable)görün.</span><span class="sxs-lookup"><span data-stu-id="80e45-108">Confirm that the user is using an app that supports sensitivity labels - see [sensitivity labels in your document](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?ad=US&ui=en-US&rs=en-US#bkmk_whereavailable).</span></span>

- <span data-ttu-id="80e45-109">Azure Bilgi [Koruması etiketlerini geçiriyorsanız,](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels) [burada](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)listelenen hususlara dikkat edin.</span><span class="sxs-lookup"><span data-stu-id="80e45-109">If you're [migrating Azure Information Protection labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), be aware of the considerations listed [here](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span></span>

- <span data-ttu-id="80e45-110">Veri kaybı önleme (DLP) desteği: Şu anda, Yalnızca saklama etiketleri DLP ilkelerinde koşul olarak kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="80e45-110">Data loss prevention (DLP) support: Currently, only retention labels can be used as a condition in DLP policies.</span></span>  <span data-ttu-id="80e45-111">DLP ilkesindeki duyarlılık etiketleri için destek henüz mevcut değil, ancak üzerinde çalışıyoruz.</span><span class="sxs-lookup"><span data-stu-id="80e45-111">Support for sensitivity labels in a DLP policy is not available yet but we're working on it.</span></span>

- <span data-ttu-id="80e45-112">Bir duyarlılık etiketinde şifreleme etkinleştirildiğinde, aşağıdakileri seçebilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="80e45-112">When encryption is enabled on a sensitivity label, you can choose either to:</span></span>
    - <span data-ttu-id="80e45-113">İzinleri şimdi atama</span><span class="sxs-lookup"><span data-stu-id="80e45-113">Assign permissions now</span></span>
    - <span data-ttu-id="80e45-114">Kullanıcıların izin atamasına izin verme</span><span class="sxs-lookup"><span data-stu-id="80e45-114">Let users assign permissions</span></span>


<span data-ttu-id="80e45-115">Olası sorunlar hakkında daha fazla bilgi için, [duyarlılık etiketleri ile bilinen sorunlara](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc)bakın.</span><span class="sxs-lookup"><span data-stu-id="80e45-115">For more information on possible issues, see [Known issues with sensitivity labels](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span></span>