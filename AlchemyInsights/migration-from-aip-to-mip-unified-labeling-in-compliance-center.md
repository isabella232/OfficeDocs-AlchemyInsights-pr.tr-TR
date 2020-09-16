---
title: AıP 'den MıP/Birleşik etiketleme 'ye Uyumluluk Merkezi 'nde geçiş
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
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674346"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="704d1-102">AıP 'den MıP/Birleşik etiketleme 'ye Uyumluluk Merkezi 'nde geçiş</span><span class="sxs-lookup"><span data-stu-id="704d1-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="704d1-103">Bir IP etiketlerinden, güvenlik ve Uyumluluk Merkezi 'nde Birleşik etiketleme 'a geçmek için aşağıdakileri yapın:</span><span class="sxs-lookup"><span data-stu-id="704d1-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="704d1-104">**Azure portalında korumayı etkinleştirme**</span><span class="sxs-lookup"><span data-stu-id="704d1-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="704d1-105">Şimdiye kadar yapmadıysanız, yeni bir tarayıcı penceresi açın ve [Azure portalında oturum açın](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="704d1-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="704d1-106">**Azure bilgi koruması** dikey öğesine gidin.</span><span class="sxs-lookup"><span data-stu-id="704d1-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="704d1-107">Örneğin, hub menüsünde **tüm hizmetler** 'e tıklayın ve filtre kutusuna **bilgileri** yazmaya başlayın.</span><span class="sxs-lookup"><span data-stu-id="704d1-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="704d1-108">**Azure bilgi koruması**'nı seçin.</span><span class="sxs-lookup"><span data-stu-id="704d1-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="704d1-109">Daha önce Azure Information Protection Blade 'e erişmediniz, bu dikey pencereyi portala eklemek için bir kerelik [ek adımlara](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) bakın.</span><span class="sxs-lookup"><span data-stu-id="704d1-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="704d1-110">Azure Information Protection Blade 'i açmak için, [Azure Information Protection Premium planı](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) veya hak yönetimi Içeren bir Office 365 planınız olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="704d1-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="704d1-111">Bu aboneliklerden birine sahipseniz ancak geçerli bir aboneliğin bulunamadığını belirten bir ileti görürseniz, [Microsoft destek 'e başvurun](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) veya standart destek kanallarınız kullanın.</span><span class="sxs-lookup"><span data-stu-id="704d1-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="704d1-112">**Yönet** menüsü seçeneklerini bulun ve **koruma etkinleştirme**'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="704d1-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="704d1-113">**Etkinleştir**'i tıklatın ve sonra eyleminizi onaylayın.</span><span class="sxs-lookup"><span data-stu-id="704d1-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="704d1-114">Etkinleştirme tamamlandığında bilgi çubuğunda **etkinleştirme başarıyla tamamlandı**görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="704d1-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="704d1-115">**Azure bilgi koruması etiketlerini Office 365 güvenlik & Uyumluluk Merkezi 'ne geçirme**</span><span class="sxs-lookup"><span data-stu-id="704d1-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="704d1-116">Genel yönetici izni olan bir kullanıcı olarak oturum açtığınızdan emin olun.</span><span class="sxs-lookup"><span data-stu-id="704d1-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="704d1-117">**Azure bilgi koruması** dikey öğesine gidin.</span><span class="sxs-lookup"><span data-stu-id="704d1-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="704d1-118">**Yönet** menüsü seçeneğinden **Birleşik etiketleme**'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="704d1-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="704d1-119">**Azure Information Protection-Birleşik etiketleme** dikey 'da **Etkinleştir** 'i tıklatın ve çevrimiçi yönergeleri izleyin.</span><span class="sxs-lookup"><span data-stu-id="704d1-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="704d1-120">**Not**: güvenlik & Uyumluluk Merkezi geçişini etkinleştirmeden önce uygun izinlere sahip olduğunuzu doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="704d1-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="704d1-121">Daha fazla bilgi için şu makalelere bakın:</span><span class="sxs-lookup"><span data-stu-id="704d1-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="704d1-122">Azure bilgi koruması 'nı yapılandırmak veya başka yöneticilere temsilci seçmek için genel yönetici olmanız mı gerekiyor?</span><span class="sxs-lookup"><span data-stu-id="704d1-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="704d1-123">Güvenlik & Uyumluluk Merkezi 'ne geçtikten sonra yönetim rolleriyle ilgili önemli bilgiler.</span><span class="sxs-lookup"><span data-stu-id="704d1-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="704d1-124">Güvenlik ve Uyumluluk Merkezi 'ne ASııP ile Birleşik etiketleme arasında geçiş hakkında daha fazla bilgi [için bkz.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)</span><span class="sxs-lookup"><span data-stu-id="704d1-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
