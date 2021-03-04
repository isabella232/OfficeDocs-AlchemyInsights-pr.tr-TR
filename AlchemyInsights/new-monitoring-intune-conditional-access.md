---
title: Intune Koşullu Erişimini İzleme
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/03/2021
ms.locfileid: "50428310"
---
# <a name="monitor-intune-conditional-access"></a><span data-ttu-id="7ce0e-102">Intune Koşullu Erişimini İzleme</span><span class="sxs-lookup"><span data-stu-id="7ce0e-102">Monitor Intune Conditional Access</span></span>

<span data-ttu-id="7ce0e-103">Koşullu erişimle hedef alan kullanıcılar, kuruma erişim gereksinimlerini karşılamıyorsa bir bildirim e-postası alırlar.</span><span class="sxs-lookup"><span data-stu-id="7ce0e-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="7ce0e-104">Bu sorunu çözmek için aşağıdaki çözümlerden birini veya birden fazlasını öneririz:</span><span class="sxs-lookup"><span data-stu-id="7ce0e-104">To resolve, we recommend one or more of the following solutions:</span></span>

1. <span data-ttu-id="7ce0e-105">Cihazın kayıtlı olduğu varsayiliyorsa, kullanıcıya Şirket Portalı uygulamasına gidip cihazın Şirket Portalı'nda görüntülendiğinden emin olması önerin.</span><span class="sxs-lookup"><span data-stu-id="7ce0e-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="7ce0e-106">Bunu yoksa, kullanıcının cihazı kaydetmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="7ce0e-106">If it doesn't, the user must enroll the device.</span></span>
1. <span data-ttu-id="7ce0e-107">Azure portalında **Intune Cihaz**  >  **uyumluluğu'ne gidin.**</span><span class="sxs-lookup"><span data-stu-id="7ce0e-107">In the Azure portal go to **Intune** > **Device compliance**.</span></span> 
1. <span data-ttu-id="7ce0e-108">Kullanıcının cihazı uyumlu olarak işaretlenirken cihaz uyumluluk raporlarınızı görüntülemek için, monitör altında **Cihaz** **uyumluluğu'ne tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="7ce0e-108">To view your device compliance report to verify that the user's device is marked as compliant, under **Monitor**, click **Device compliance**.</span></span>
1. <span data-ttu-id="7ce0e-109">Azure portalında **Intune Cihaz**  >  **uyumluluğu'ne gidin.**</span><span class="sxs-lookup"><span data-stu-id="7ce0e-109">In the Azure portal go to **Intune** > **Device compliance**.</span></span> <span data-ttu-id="7ce0e-110">**Yönet'in altında İlkeler'e** **tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="7ce0e-110">Under **Manage,** click **Policies**.</span></span> <span data-ttu-id="7ce0e-111">Uyumluluk ilkeleri listesinde, kullanıcı cihazınıza bir profilin atandığı doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="7ce0e-111">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="7ce0e-112">Profil atanmamışsa, Intune cihazın uyumluluk durumunu onaylamaz.</span><span class="sxs-lookup"><span data-stu-id="7ce0e-112">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
1. <span data-ttu-id="7ce0e-113">Kullanıcının koşullu erişim atamalarını düzenleyin.</span><span class="sxs-lookup"><span data-stu-id="7ce0e-113">Edit the user's conditional access assignment.</span></span>
1. <span data-ttu-id="7ce0e-114">Azure portalında **Intune** Koşullu erişim İlkelerine gidin, listeden bir ilke seçin ve Kullanıcılar  >    >  ve **gruplar'a tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="7ce0e-114">In the Azure portal, navigate to **Intune** > **Conditional access** > **Policies**, select a policy from the list, and click **Users and groups**.</span></span>
1. <span data-ttu-id="7ce0e-115">Belirli bir ilkeyi birine hedeflemek için, bu ilkeyi Ekle **listesine ekleyin.**</span><span class="sxs-lookup"><span data-stu-id="7ce0e-115">To target a certain policy at someone, add them to the **Include list**.</span></span> <span data-ttu-id="7ce0e-116">Bir kişinin ilkeden atlanmış olduğundan emin olmak için, bu kişiyi Dışla **listesine ekleyin.**</span><span class="sxs-lookup"><span data-stu-id="7ce0e-116">To ensure that a person is omitted from the policy, add them to the **Exclude list**.</span></span>

<span data-ttu-id="7ce0e-117">**Yararlı bağlantılar:**</span><span class="sxs-lookup"><span data-stu-id="7ce0e-117">**Helpful links:**</span></span>

- [<span data-ttu-id="7ce0e-118">Cihaz uyumluluğuna genel bakış</span><span class="sxs-lookup"><span data-stu-id="7ce0e-118">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)
- [<span data-ttu-id="7ce0e-119">CA sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="7ce0e-119">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [<span data-ttu-id="7ce0e-120">Sorun giderme ilkesi</span><span class="sxs-lookup"><span data-stu-id="7ce0e-120">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [<span data-ttu-id="7ce0e-121">Intune cihaz uyumluluğunu izleme</span><span class="sxs-lookup"><span data-stu-id="7ce0e-121">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> <span data-ttu-id="7ce0e-122">Bu adımlar yalnızca Azure Active Directory özelliği Koşullu Erişim sorunlarını gidermek için yararlıdır.</span><span class="sxs-lookup"><span data-stu-id="7ce0e-122">These steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="7ce0e-123">Ayrıca, Exchange ilkesiyle e-posta erişimini engelleyen bir cihazı karantinaya almak da mümkündür.</span><span class="sxs-lookup"><span data-stu-id="7ce0e-123">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="7ce0e-124">Exchange cihaz yönetimi hakkında daha fazla bilgiyi burada [**bulunabilir.**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))</span><span class="sxs-lookup"><span data-stu-id="7ce0e-124">More information on Exchange device management can be found [**here**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span></span>
