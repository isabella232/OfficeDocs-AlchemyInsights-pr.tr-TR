---
title: Koşullu Erişimi İzleme
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708694"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="36152-102">Exchange için Koşullu Erişimi İzleme</span><span class="sxs-lookup"><span data-stu-id="36152-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="36152-103">Koşullu erişimle hedef alan kullanıcılar, kuruma erişim gereksinimlerini karşılamıyorsa bir bildirim e-postası alırlar.</span><span class="sxs-lookup"><span data-stu-id="36152-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="36152-104">Bu sorunu çözmek için aşağıdaki çözümlerden birini veya birden fazlasını öneririz:</span><span class="sxs-lookup"><span data-stu-id="36152-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="36152-105">Cihazın kayıtlı olduğu varsayiliyorsa, kullanıcıya Şirket Portalı uygulamasına gidip cihazın Şirket Portalı'nda görüntülendiğinden emin olması önerin.</span><span class="sxs-lookup"><span data-stu-id="36152-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="36152-106">Bunu yoksa, kullanıcının cihazı kaydetmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="36152-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="36152-107">Azure portalında Intune'a > uyumluluğuna gidin.</span><span class="sxs-lookup"><span data-stu-id="36152-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="36152-108">İzleme'nin altında Cihaz uyumluluğu'ne tıklayın.</span><span class="sxs-lookup"><span data-stu-id="36152-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="36152-109">Kullanıcının cihazı uyumlu olarak işaretlenir doğrulamak için cihaz uyumluluk raporlarınızı görüntüleme.</span><span class="sxs-lookup"><span data-stu-id="36152-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="36152-110">Azure portalında Intune'a > uyumluluğuna gidin.</span><span class="sxs-lookup"><span data-stu-id="36152-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="36152-111">Yönet'in altında İlkeler'e tıklayın.</span><span class="sxs-lookup"><span data-stu-id="36152-111">Under Manage, click Policies.</span></span> <span data-ttu-id="36152-112">Uyumluluk ilkeleri listesinde, kullanıcı cihazınıza bir profilin atandığı doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="36152-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="36152-113">Profil atanmamışsa, Intune cihazın uyumluluk durumunu onaylamaz.</span><span class="sxs-lookup"><span data-stu-id="36152-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="36152-114">Kullanıcının koşullu erişim atamalarını düzenleyin.</span><span class="sxs-lookup"><span data-stu-id="36152-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="36152-115">Azure portalında **Intune Koşullu erişim**  >  **İlkeleri'ne**  >  **gidin.**</span><span class="sxs-lookup"><span data-stu-id="36152-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="36152-116">Listeden bir ilke seçin.</span><span class="sxs-lookup"><span data-stu-id="36152-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="36152-117">Kullanıcılar ve gruplar'a tıklayın.</span><span class="sxs-lookup"><span data-stu-id="36152-117">Click Users and groups.</span></span>
4. <span data-ttu-id="36152-118">Belirli bir ilkeyi birine hedeflemek için, bu ilkeyi Ekle listesine ekleyin.</span><span class="sxs-lookup"><span data-stu-id="36152-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="36152-119">Bir kişinin ilkeden atlanmış olduğundan emin olmak için, bu kişiyi Dışla listesine ekleyin.</span><span class="sxs-lookup"><span data-stu-id="36152-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="36152-120">Yararlı bağlantılar:</span><span class="sxs-lookup"><span data-stu-id="36152-120">Helpful links:</span></span>

[<span data-ttu-id="36152-121">Cihaz uyumluluğuna genel bakış</span><span class="sxs-lookup"><span data-stu-id="36152-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="36152-122">CA sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="36152-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="36152-123">Sorun giderme ilkesi</span><span class="sxs-lookup"><span data-stu-id="36152-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="36152-124">Intune cihaz uyumluluğunu izleme</span><span class="sxs-lookup"><span data-stu-id="36152-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="36152-125">Not: Bu adımlar yalnızca Azure Active Directory özelliği Koşullu Erişim sorunlarını gidermek için yararlıdır.</span><span class="sxs-lookup"><span data-stu-id="36152-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="36152-126">Ayrıca, Exchange ilkesiyle e-posta erişimini engelleyen bir cihazı karantinaya almak da mümkündür.</span><span class="sxs-lookup"><span data-stu-id="36152-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="36152-127">Exchange cihaz yönetimi hakkında daha fazla bilgiyi [burada]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) bulunabilir.</span><span class="sxs-lookup"><span data-stu-id="36152-127">More information on Exchange device management can be found [here](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141).</span></span>
