---
title: Uyumluluk Merkezi'nde AIP'den MIP/Birleşik Etiketleme'ye geçiş
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
- "9002278"
- "5114"
ms.openlocfilehash: 12f5f5c46edd7918618c55a8a1905f3b28643092
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825391"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="421ab-102">Uyumluluk Merkezi'nde AIP'den MIP/Birleşik Etiketleme'ye geçiş</span><span class="sxs-lookup"><span data-stu-id="421ab-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="421ab-103">Güvenlik ve Uyumluluk Merkezi'nde AIP etiketlerinden Birleşik Etiketleme'ye geçiş yapmak için şunları yapın:</span><span class="sxs-lookup"><span data-stu-id="421ab-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="421ab-104">**Azure portaldan korumayı etkinleştirme**</span><span class="sxs-lookup"><span data-stu-id="421ab-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="421ab-105">Henüz açmadısanız yeni bir tarayıcı penceresi açın ve [Azure portalında oturum açın.](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="421ab-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="421ab-106">**Azure Information Protection blade'a** gidin.</span><span class="sxs-lookup"><span data-stu-id="421ab-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="421ab-107">Örneğin, hub menüsünde Tüm **hizmetler'e tıklayın ve** Filtre **kutusuna Bilgi** yazmaya başlayın.</span><span class="sxs-lookup"><span data-stu-id="421ab-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="421ab-108">**Azure Information Protection öğesini seçin.**</span><span class="sxs-lookup"><span data-stu-id="421ab-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="421ab-109">Azure Information Protection blade'e daha önce erişemediysanız [](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) bu blade'i portala eklemek için tek seferlik ek adımlara bakın.</span><span class="sxs-lookup"><span data-stu-id="421ab-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="421ab-110">Azure Information Protection blade'i açmak için, [bir Azure Information Protection Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) planınız veya Hak Yönetimi içeren bir Office 365 planınız olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="421ab-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="421ab-111">Bu aboneliklerden birini kullanıyorsanız ancak geçerli bir aboneliğin buluna olmadığını haber veren bir ileti görüyorsanız [Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) Desteği'ne başvurun veya standart destek kanallarınızı kullanın.</span><span class="sxs-lookup"><span data-stu-id="421ab-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="421ab-112">Yönet menü **seçeneklerini** bulun ve Koruma **etkinleştirme'yi seçin.**</span><span class="sxs-lookup"><span data-stu-id="421ab-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="421ab-113">**Etkinleştir'e** tıklayın ve ardından eyleminizi onaylayın.</span><span class="sxs-lookup"><span data-stu-id="421ab-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="421ab-114">Etkinleştirme tamamlandığında, bilgi çubuğunda Etkinleştirme başarıyla **tamamlandı olarak görüntülenir.**</span><span class="sxs-lookup"><span data-stu-id="421ab-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="421ab-115">**Azure Information Protection etiketlerini Office 365 Güvenlik ve Uyumluluk & geçirme**</span><span class="sxs-lookup"><span data-stu-id="421ab-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="421ab-116">Genel Yönetici izni olan bir kullanıcı olarak oturum açtığınızdan emin olun.</span><span class="sxs-lookup"><span data-stu-id="421ab-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="421ab-117">**Azure Information Protection blade'a** gidin.</span><span class="sxs-lookup"><span data-stu-id="421ab-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="421ab-118">Yönet menü **seçeneğinden** Birleşik **etiketleme'yi seçin.**</span><span class="sxs-lookup"><span data-stu-id="421ab-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="421ab-119">Azure **Information Protection - Birleşik etiketleme blade'inde** Etkinleştir'e **tıklayın** ve çevrimiçi yönergeleri izleyin.</span><span class="sxs-lookup"><span data-stu-id="421ab-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="421ab-120">**Not:** Güvenlik ve Uyumluluk Merkezi Geçişi'ne etkinleştirmeden önce uygun izinlere & doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="421ab-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="421ab-121">Daha fazla bilgi için şu makalelere bakın:</span><span class="sxs-lookup"><span data-stu-id="421ab-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="421ab-122">Azure Information Protection'i yapılandırmak için genel yönetici mi olmak gerekiyor yoksa diğer yöneticilere temsilci de kullanabilir miyim?</span><span class="sxs-lookup"><span data-stu-id="421ab-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="421ab-123">Güvenlik ve Uyumluluk Merkezi'ne katıldıktan sonra yönetim rolleri & bilgiler.</span><span class="sxs-lookup"><span data-stu-id="421ab-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="421ab-124">Güvenlik ve Uyumluluk Merkezi'ne Birleşik Etiketleme için AIP geçişi hakkında daha fazla bilgi için bkz. [Etiketleri geçirme](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span><span class="sxs-lookup"><span data-stu-id="421ab-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
