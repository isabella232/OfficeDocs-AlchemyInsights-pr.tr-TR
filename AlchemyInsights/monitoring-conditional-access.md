---
title: Koşullu Erişimin İzlenmesi
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 8b76d58791408037b5704b421d7afa166e3ea0be
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713738"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="db6a2-102">Değişim için Koşullu Erişimin İzlenmesi</span><span class="sxs-lookup"><span data-stu-id="db6a2-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="db6a2-103">Koşullu erişim le hedeflenen kullanıcılar, kuruluşunuzun erişim gereksinimlerini karşılamadıkları takdirde bir bildirim e-postası alır.</span><span class="sxs-lookup"><span data-stu-id="db6a2-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="db6a2-104">Çözmek için, aşağıdaki çözümlerden birini veya birkaçını öneririz:</span><span class="sxs-lookup"><span data-stu-id="db6a2-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="db6a2-105">Cihazın kayıtlı olduğu varsayılsa, kullanıcıya Şirket Portalı uygulamasına gitmesini ve Şirket Portalı'nda göründüğünü doğrulamasını tavsiye edin.</span><span class="sxs-lookup"><span data-stu-id="db6a2-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="db6a2-106">Değilse, kullanıcı aygıtı kaydetmelidir.</span><span class="sxs-lookup"><span data-stu-id="db6a2-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="db6a2-107">Azure portalında **Intune \> Aygıt uyumluluğu'na**gidin.</span><span class="sxs-lookup"><span data-stu-id="db6a2-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="db6a2-108">**Monitör** altında **Aygıt uyumluluğu'na**tıklayın.</span><span class="sxs-lookup"><span data-stu-id="db6a2-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="db6a2-109">Kullanıcının aygıtının uyumlu olarak işaretlendiğini doğrulamak için cihazınızın uyumluluk raporunu görüntüleyin.</span><span class="sxs-lookup"><span data-stu-id="db6a2-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="db6a2-110">Azure portalında **Intune \> Aygıt uyumluluğu'na**gidin.</span><span class="sxs-lookup"><span data-stu-id="db6a2-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="db6a2-111">**Yönet**altında, **İlkeler'i**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="db6a2-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="db6a2-112">Uyumluluk ilkeleri listesinde, kullanıcınızın cihazına bir profil atandığını doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="db6a2-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="db6a2-113">Profil atanmamışsa, Intune aygıtın uyumluluk durumunu onaylayamayacaktır.</span><span class="sxs-lookup"><span data-stu-id="db6a2-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="db6a2-114">Kullanıcının koşullu erişim atamasını edin.</span><span class="sxs-lookup"><span data-stu-id="db6a2-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="db6a2-115">Azure portalında **Intune \> Koşullu \> erişim İlkeleri'ne** gidin</span><span class="sxs-lookup"><span data-stu-id="db6a2-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="db6a2-116">Listeden bir ilke seçin</span><span class="sxs-lookup"><span data-stu-id="db6a2-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="db6a2-117">**Kullanıcılar ve gruplar'ı** tıklatın</span><span class="sxs-lookup"><span data-stu-id="db6a2-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="db6a2-118">Belirli bir ilkeyi birine hedeflemek için, bu politikayı **Ekle** listesine ekleyin.</span><span class="sxs-lookup"><span data-stu-id="db6a2-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="db6a2-119">Bir kişinin ilkeden çıkarıldığından emin olmak için, bunları **Dışlayın** listesine ekleyin.</span><span class="sxs-lookup"><span data-stu-id="db6a2-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="db6a2-120">Daha fazla bilgi: [Koşullu Erişim aygıtları nasıl izlenir?](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="db6a2-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

