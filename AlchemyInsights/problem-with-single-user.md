---
title: Tek kullanıcıyla ilgili sorun
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430358"
---
# <a name="problem-with-single-user"></a><span data-ttu-id="8fd74-102">Tek kullanıcıyla ilgili sorun</span><span class="sxs-lookup"><span data-stu-id="8fd74-102">Problem with single user</span></span>

- <span data-ttu-id="8fd74-103">Hizmet, kullanıcıyı henüz değerlendirme fırsatı olmadı diye kullanıcıya sağlanmadı.</span><span class="sxs-lookup"><span data-stu-id="8fd74-103">The user may not have been provisioned because the service hasn't had a chance to evaluate the user yet.</span></span> <span data-ttu-id="8fd74-104">Hazırlamanın ne kadar sürece sürecesi ile ilgili kılavuzu ve sağlama yapılandırma sayfasındaki ilerleme çubuğunu gözden geçirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="8fd74-104">Review the guidance for how long provisioning takes as well as the progress bar on the provisioning configuration page.</span></span> <span data-ttu-id="8fd74-105">Ek ayrıntılar bölümünde belirtilen sabit durum kullanıcının oluşturulma/güncelleştirilmeden/silinmeden önce geliyorsa, kullanıcıyı henüz değerlendirmedik demektir.</span><span class="sxs-lookup"><span data-stu-id="8fd74-105">If the steady state specified in the additional details section is before the date the user was created/updated/deleted, it means we have not evaluated the user yet.</span></span> <span data-ttu-id="8fd74-106">Bu senaryoda, yapacak en iyi şey sağlama hizmetinin bitip bitimini beklemektir.</span><span class="sxs-lookup"><span data-stu-id="8fd74-106">In this scenario, the best thing to do is wait for the provisioning service to finish.</span></span>

  - <span data-ttu-id="8fd74-107">Hizmetimizin yalnızca kaynak sistem (Bulut İk) kullanıcıya yapılan değişikliklerden haberdar olduğunu unutmayın.</span><span class="sxs-lookup"><span data-stu-id="8fd74-107">Note that our service is only aware of changes to a user in the source system (Cloud HR).</span></span> <span data-ttu-id="8fd74-108">Azure AD'nin değişikliği algılaması ve Active Directory'ye akışı için kaynak sistemde geçerli bir değişiklik olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="8fd74-108">There has to be a valid change in the source system for Azure AD to detect the change and flow it into Active Directory.</span></span>
- <span data-ttu-id="8fd74-109">Sağlama hizmeti kullanıcıyı değerlendirdi ve sağlanmaz olarak belirledi:</span><span class="sxs-lookup"><span data-stu-id="8fd74-109">Provisioning service evaluated the user and determined it should not be provisioned:</span></span>
  - <span data-ttu-id="8fd74-110">Özniteliği temel alan bircoping filtresi ayardıysanız, kullanıcının belirttiğiniz ölçütlere uygun olduğundan emin olur.</span><span class="sxs-lookup"><span data-stu-id="8fd74-110">If you have set an attribute based scoping filter, ensure that the user meets the criteria that you have specified.</span></span>
  - <span data-ttu-id="8fd74-111">Kullanıcılar zaten hedef sistemde bulunuyorsa ve kullanıcının durumu kaynak ve hedef eşleşmede bulunuyorsa, başka bir işlemde yer almayacağız.</span><span class="sxs-lookup"><span data-stu-id="8fd74-111">If users already exist in the target system and the state of the user in the source and target match, we won't take any further action.</span></span>
- <span data-ttu-id="8fd74-112">Sağlama hizmeti, kullanıcıya sağlamayı denendi ve başarısız oldu.</span><span class="sxs-lookup"><span data-stu-id="8fd74-112">Provisioning service attempted to provision the user and it failed.</span></span> <span data-ttu-id="8fd74-113">Bu senaryolar için, sağlama günlüklerinin sorun giderme ve öneriler sekmesini gözden geçirebilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="8fd74-113">For these scenarios, review the troubleshooting and recommendations tab of the provisioning logs:</span></span>
  - <span data-ttu-id="8fd74-114">Şirket içi Active Directory'de veya Azure AD'de kullanıcıda gerekli bir öznitelik eksik olabilir.</span><span class="sxs-lookup"><span data-stu-id="8fd74-114">A required attribute on the user might be missing in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="8fd74-115">Örneğin, userPrincipalName veya sAMAccountName oluşturma kuralları doğru değeri oluşturmaz.</span><span class="sxs-lookup"><span data-stu-id="8fd74-115">For example, the userPrincipalName or sAMAccountName generation rules are not generating the right value.</span></span>
  - <span data-ttu-id="8fd74-116">Eşleşen öznitelik (genellikle employeeId) şirket içi Active Directory'de veya Azure AD'de benzersiz bir kullanıcıyla çözümlenemmektedir.</span><span class="sxs-lookup"><span data-stu-id="8fd74-116">The matching attribute (usually employeeId) is not resolving to a unique user in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="8fd74-117">Örneğin, AD'de aynı çalışankimsi olan iki kullanıcı vardır ve hizmet aynı kaynak girdi için yinelenen hedef girdileri belirten bir hata kodu döndürür.</span><span class="sxs-lookup"><span data-stu-id="8fd74-117">For example, there are two users with the same employeeId in AD and the service returns an error code indicate duplicate target entries for the same source entry.</span></span>

<span data-ttu-id="8fd74-118">Tek bir kullanıcının ve grupların günlüklerini gözden geçirmek için bkz. Belirli bir kullanıcıyla ilgili [bir sorunun sağlama günlüklerini gözden geçirme.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)</span><span class="sxs-lookup"><span data-stu-id="8fd74-118">To review logs for single user and groups, see [Review the provisioning logs for an issue with a specific user](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span></span>
