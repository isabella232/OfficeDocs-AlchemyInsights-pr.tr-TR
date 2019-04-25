---
title: Koşullu erişim izleme
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 756c5e98ed3e9cedd0152b5747ea6bf1ed31778e
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32418489"
---
# <a name="monitoring-conditional-access"></a><span data-ttu-id="87715-102">Koşullu erişim izleme</span><span class="sxs-lookup"><span data-stu-id="87715-102">Monitoring Conditional Access</span></span>

<span data-ttu-id="87715-103">Kuruluşunuzun erişim gereksinimlerini karşılamıyorsa koşullu erişim ile hedeflenen kullanıcılara bildirim e-posta alacaksınız.</span><span class="sxs-lookup"><span data-stu-id="87715-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="87715-104">Çözmek için aşağıdakilerden birini veya daha fazlasını aşağıdaki çözümleri öneririz:</span><span class="sxs-lookup"><span data-stu-id="87715-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="87715-105">Aygıt için kaydı kabul edilir, kullanıcı şirket Portal app için gidin ve şirket portalda göründüğünden emin olun önerin.</span><span class="sxs-lookup"><span data-stu-id="87715-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="87715-106">Seçili değilse, kullanıcı aygıtı kaydetmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="87715-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="87715-107">Azure portalda gitmek için **Intune \> aygıt uyumluluğu**.</span><span class="sxs-lookup"><span data-stu-id="87715-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="87715-108">**Aygıt uyumluluğu**altında **İzleyicisi'ni** tıklatın.</span><span class="sxs-lookup"><span data-stu-id="87715-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="87715-109">Kullanıcının aygıt uyumlu olarak işaretlendiğini doğrulamak için aygıt uyumluluğu raporu görüntüleyin.</span><span class="sxs-lookup"><span data-stu-id="87715-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="87715-110">Azure portalda gitmek için **Intune \> aygıt uyumluluğu**.</span><span class="sxs-lookup"><span data-stu-id="87715-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="87715-111">**Yönet**altında **ilkeleri**' ni tıklatın.</span><span class="sxs-lookup"><span data-stu-id="87715-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="87715-112">Uyumluluk ilkeler listesinde bir profil, kullanıcının aygıta atanmış olduğunu doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="87715-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="87715-113">Profil atanırsa, Intune aygıtın uyum durumu onaylamak mümkün olmayacak.</span><span class="sxs-lookup"><span data-stu-id="87715-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="87715-114">Kullanıcının koşullu erişim atama düzenleyin.</span><span class="sxs-lookup"><span data-stu-id="87715-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="87715-115">Azure portalda gitmek için **Intune \> koşullu erişim \> ilkeler**</span><span class="sxs-lookup"><span data-stu-id="87715-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="87715-116">Bir ilkeyi listeden seçin.</span><span class="sxs-lookup"><span data-stu-id="87715-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="87715-117">**Kullanıcılar ve gruplar'ı** tıklatın.</span><span class="sxs-lookup"><span data-stu-id="87715-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="87715-118">Belirli bir ilke birisi olarak hedeflemek için **ekleme** listesine ekleyin.</span><span class="sxs-lookup"><span data-stu-id="87715-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="87715-119">Bir kişinin ilkesinden atlanır sağlamak için **dışlama** listesine ekleyin.</span><span class="sxs-lookup"><span data-stu-id="87715-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="87715-120">Daha fazla bilgi: [Monitör koşullu erişim aygıtları nasıl](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="87715-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

