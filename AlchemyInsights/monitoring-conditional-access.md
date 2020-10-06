---
title: Koşullu erişimi izleme
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
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366448"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="82f33-102">Exchange için koşullu erişimi izleme</span><span class="sxs-lookup"><span data-stu-id="82f33-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="82f33-103">Koşullu erişimle hedeflenen kullanıcılar kuruluşunuzun erişim gereksinimlerini karşılamıyorsa bildirim e-postası alır.</span><span class="sxs-lookup"><span data-stu-id="82f33-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="82f33-104">Sorunu çözmek için, aşağıdaki çözümlerden bir veya daha fazlasını öneririz:</span><span class="sxs-lookup"><span data-stu-id="82f33-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="82f33-105">Cihazın kayıtlı olduğu kabul ediyorsanız, kullanıcının Şirket Portalı uygulamasına gitmesini ve şirket portalında göründüğünü doğrulamasını tavsiye edin.</span><span class="sxs-lookup"><span data-stu-id="82f33-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="82f33-106">Yoksa, Kullanıcı cihazı kaydetmelidir.</span><span class="sxs-lookup"><span data-stu-id="82f33-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="82f33-107">Azure portalında cihaz uyumluluğu > Intune 'a gidin.</span><span class="sxs-lookup"><span data-stu-id="82f33-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="82f33-108">Monitör altında cihaz uyumluluğu 'nı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="82f33-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="82f33-109">Cihazın uyumluluk raporunuzu görüntülemek için, kullanıcının cihazının uyumlu olduğunu doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="82f33-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="82f33-110">Azure portalında cihaz uyumluluğu > Intune 'a gidin.</span><span class="sxs-lookup"><span data-stu-id="82f33-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="82f33-111">Yönet altında, Ilkeler 'e tıklayın.</span><span class="sxs-lookup"><span data-stu-id="82f33-111">Under Manage, click Policies.</span></span> <span data-ttu-id="82f33-112">Uyumluluk ilkeleri listesinde, kullanıcının cihazına bir profilin atandığını doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="82f33-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="82f33-113">Atanmış profil yoksa, Intune cihazın uyumluluk durumunu doğrulayamayacaktır.</span><span class="sxs-lookup"><span data-stu-id="82f33-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="82f33-114">Kullanıcının koşullu erişim atamasını düzenleyin.</span><span class="sxs-lookup"><span data-stu-id="82f33-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="82f33-115">Azure portalında **Intune**  >  **koşullu erişim**  >  **ilkelerine**gidin.</span><span class="sxs-lookup"><span data-stu-id="82f33-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="82f33-116">Listeden bir ilke seçin.</span><span class="sxs-lookup"><span data-stu-id="82f33-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="82f33-117">Kullanıcılar ve gruplar 'ı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="82f33-117">Click Users and groups.</span></span>
4. <span data-ttu-id="82f33-118">Belirli bir ilkeyi bir başkasından hedeflemek için bunları ekleme listesine ekleyin.</span><span class="sxs-lookup"><span data-stu-id="82f33-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="82f33-119">Bir kişinin ilkeden atlandığından emin olmak için bunları dışlama listesine ekleyin.</span><span class="sxs-lookup"><span data-stu-id="82f33-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="82f33-120">Faydalı bağlantılar:</span><span class="sxs-lookup"><span data-stu-id="82f33-120">Helpful links:</span></span>

[<span data-ttu-id="82f33-121">Cihaz uyumuna genel bakış</span><span class="sxs-lookup"><span data-stu-id="82f33-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="82f33-122">Sorun giderme CA</span><span class="sxs-lookup"><span data-stu-id="82f33-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="82f33-123">Sorun giderme ilkesi</span><span class="sxs-lookup"><span data-stu-id="82f33-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="82f33-124">Intune cihaz uyumluluğunu izleme</span><span class="sxs-lookup"><span data-stu-id="82f33-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="82f33-125">Not: Bu adımlar yalnızca Azure Active Directory özelliğinin koşullu erişimi sorunlarını gidermede yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="82f33-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="82f33-126">Exchange ilkesiyle e-posta erişimini engelleyen bir cihaz karantinaya alınabilir.</span><span class="sxs-lookup"><span data-stu-id="82f33-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="82f33-127">Exchange cihazı yönetimi hakkında daha fazla bilgiyi [burada](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>)bulabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="82f33-127">More information on Exchange device management can be found [here](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).</span></span>
