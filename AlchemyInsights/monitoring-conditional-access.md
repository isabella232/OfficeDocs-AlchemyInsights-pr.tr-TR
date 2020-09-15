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
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702923"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="b9190-102">Exchange için koşullu erişimi izleme</span><span class="sxs-lookup"><span data-stu-id="b9190-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="b9190-103">Koşullu erişimle hedeflenen kullanıcılar kuruluşunuzun erişim gereksinimlerini karşılamıyorsa bildirim e-postası alır.</span><span class="sxs-lookup"><span data-stu-id="b9190-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="b9190-104">Sorunu çözmek için, aşağıdaki çözümlerden bir veya daha fazlasını öneririz:</span><span class="sxs-lookup"><span data-stu-id="b9190-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="b9190-105">Cihazın kayıtlı olduğu kabul ediyorsanız, kullanıcının Şirket Portalı uygulamasına gitmesini ve şirket portalında göründüğünü doğrulamasını tavsiye edin.</span><span class="sxs-lookup"><span data-stu-id="b9190-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="b9190-106">Yoksa, Kullanıcı cihazı kaydetmelidir.</span><span class="sxs-lookup"><span data-stu-id="b9190-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="b9190-107">Azure portalında **Intune \> cihaz uyumu**'na gidin.</span><span class="sxs-lookup"><span data-stu-id="b9190-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="b9190-108">**Monitör** altında **cihaz uyumluluğu**'nı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="b9190-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="b9190-109">Cihazın uyumluluk raporunuzu görüntülemek için, kullanıcının cihazının uyumlu olduğunu doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="b9190-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="b9190-110">Azure portalında **Intune \> cihaz uyumu**'na gidin.</span><span class="sxs-lookup"><span data-stu-id="b9190-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="b9190-111">**Yönet**altında, **ilkeler**'e tıklayın.</span><span class="sxs-lookup"><span data-stu-id="b9190-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="b9190-112">Uyumluluk ilkeleri listesinde, kullanıcının cihazına bir profilin atandığını doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="b9190-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="b9190-113">Atanmış profil yoksa, Intune cihazın uyumluluk durumunu doğrulayamayacaktır.</span><span class="sxs-lookup"><span data-stu-id="b9190-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="b9190-114">Kullanıcının koşullu erişim atamasını düzenleyin.</span><span class="sxs-lookup"><span data-stu-id="b9190-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="b9190-115">Azure portalında **Intune \> koşullu erişim \> ilkelerine** git</span><span class="sxs-lookup"><span data-stu-id="b9190-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="b9190-116">Listeden bir ilke seçin</span><span class="sxs-lookup"><span data-stu-id="b9190-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="b9190-117">**Kullanıcılar ve gruplar** 'ı tıklatın</span><span class="sxs-lookup"><span data-stu-id="b9190-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="b9190-118">Belirli bir ilkeyi bir başkasından hedeflemek için bunları **ekleme listesine ekleyin** .</span><span class="sxs-lookup"><span data-stu-id="b9190-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="b9190-119">Bir kişinin ilkeden atlandığından emin olmak için bunları **dışlama** listesine ekleyin.</span><span class="sxs-lookup"><span data-stu-id="b9190-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="b9190-120">Daha fazla bilgi: [koşullu erişim aygıtlarını izleme](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="b9190-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

