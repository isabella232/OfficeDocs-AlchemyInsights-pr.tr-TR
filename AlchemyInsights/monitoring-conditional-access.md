---
title: Koşullu erişim izleme
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 06307b57475e8828e6d4e5e01625d5100576f12b
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29494183"
---
# <a name="monitoring-conditional-access"></a><span data-ttu-id="03c37-102">Koşullu erişim izleme</span><span class="sxs-lookup"><span data-stu-id="03c37-102">Monitoring Conditional Access</span></span>

<span data-ttu-id="03c37-p101">Kuruluşunuzun erişim gereksinimlerini karşılamıyorsa koşullu erişim ile hedeflenen kullanıcılara bildirim e-posta alacaksınız. Çözmek için aşağıdakilerden birini veya daha fazlasını aşağıdaki çözümleri öneririz:</span><span class="sxs-lookup"><span data-stu-id="03c37-p101">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements. To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="03c37-p102">Aygıt için kaydı kabul edilir, kullanıcı şirket Portal app için gidin ve şirket portalda göründüğünden emin olun önerin. Seçili değilse, kullanıcı aygıtı kaydetmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="03c37-p102">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal. If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="03c37-p103">Azure portalda gitmek için **Intune \> aygıt uyumluluğu**. **Aygıt uyumluluğu**altında **İzleyicisi'ni** tıklatın. Kullanıcının aygıt uyumlu olarak işaretlendiğini doğrulamak için aygıt uyumluluğu raporu görüntüleyin.</span><span class="sxs-lookup"><span data-stu-id="03c37-p103">In the Azure portal go to **Intune \> Device compliance**. Under **Monitor** click **Device compliance**. View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="03c37-p104">Azure portalda gitmek için **Intune \> aygıt uyumluluğu**. **Yönet**altında **ilkeleri**' ni tıklatın. Uyumluluk ilkeler listesinde bir profil, kullanıcının aygıta atanmış olduğunu doğrulayın. Profil atanırsa, Intune aygıtın uyum durumu onaylamak mümkün olmayacak.</span><span class="sxs-lookup"><span data-stu-id="03c37-p104">In the Azure portal go to **Intune \> Device compliance**. Under **Manage**, click **Policies**. In the list of compliance policies, verify that a profile is assigned to your user's device. If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="03c37-114">Kullanıcının koşullu erişim atama düzenleyin.</span><span class="sxs-lookup"><span data-stu-id="03c37-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="03c37-115">Azure portalda gitmek için **Intune \> koşullu erişim \> ilkeler**</span><span class="sxs-lookup"><span data-stu-id="03c37-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="03c37-116">Bir ilkeyi listeden seçin.</span><span class="sxs-lookup"><span data-stu-id="03c37-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="03c37-117">**Kullanıcılar ve gruplar'ı** tıklatın.</span><span class="sxs-lookup"><span data-stu-id="03c37-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="03c37-p105">Belirli bir ilke birisi olarak hedeflemek için **ekleme** listesine ekleyin. Bir kişinin ilkesinden atlanır sağlamak için **dışlama** listesine ekleyin.</span><span class="sxs-lookup"><span data-stu-id="03c37-p105">To target a certain policy at someone, add them to the **Include** list. To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="03c37-120">Daha fazla bilgi: [Monitör koşullu erişim aygıtları nasıl](https://docs.microsoft.com/en-us/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="03c37-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/en-us/intune/conditional-access-exchange-monitor)</span></span>
  

