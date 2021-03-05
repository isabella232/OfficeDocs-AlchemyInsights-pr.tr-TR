---
title: Öznitelik vecoping filtresiyle ilgili sorun
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482925"
---
# <a name="problem-with-attribute-and-scoping-filter"></a><span data-ttu-id="01ab3-102">Öznitelik vecoping filtresiyle ilgili sorun</span><span class="sxs-lookup"><span data-stu-id="01ab3-102">Problem with attribute and scoping filter</span></span>

<span data-ttu-id="01ab3-103">**UPN değerlerinin çakışması sorunu**</span><span class="sxs-lookup"><span data-stu-id="01ab3-103">**Issue with conflicting UPN values**</span></span>

<span data-ttu-id="01ab3-104">The Workday to AD User Provisioning Workday to AD User Provisioning, **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique** hata iletisini gösterir.</span><span class="sxs-lookup"><span data-stu-id="01ab3-104">The Workday to AD User Provisioning Workday to AD User Provisioning shows error message **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span></span> <span data-ttu-id="01ab3-105">Ekleme/değiştirme için sağlanan UPN değeri orman genelinde benzersiz bir değer olduğundan işlem başarısız oldu.</span><span class="sxs-lookup"><span data-stu-id="01ab3-105">The operation failed because UPN value provided for addition/modification is not unique forest-wide.</span></span> <span data-ttu-id="01ab3-106">Hata Ayrıntıları: **CONSTRAINT_ATT_TYPE - userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="01ab3-106">Error Details: **CONSTRAINT_ATT_TYPE - userPrincipalName**.</span></span>

<span data-ttu-id="01ab3-107">Workday bağlayıcısı AD kullanıcı hesabını oluştururken ayarlamaya çalıştığı **userPrincipalName** değeri, hedef AD etki alanında zaten var.</span><span class="sxs-lookup"><span data-stu-id="01ab3-107">The **userPrincipalName** value that Workday connector is trying to set when creating the AD user account already exists in the target AD domain.</span></span> <span data-ttu-id="01ab3-108">Bu, (1) kullanıcının zaten var olduğunu ve kullanıcı için eşleşen kimlik denetiminin başarısız olduğunu veya (2) UPN oluşturma kuralının çakışan bir değer üreterek bunu ima eder.</span><span class="sxs-lookup"><span data-stu-id="01ab3-108">This implies that either (1) the user already exists and the matching ID check failed for the user or (2) the UPN generation rule generated a conflicting value.</span></span>

<span data-ttu-id="01ab3-109">Önerilen çözüm adımları:</span><span class="sxs-lookup"><span data-stu-id="01ab3-109">Here are the suggested resolution steps:</span></span>

<span data-ttu-id="01ab3-110">Kullanıcı zaten varsa ve eşleşen kimlik denetimi İşGünü hesabını Active Directory hesabına bağlayamamışsa, hem İşGünü'deki hem de AD'deki eşleşen kimlik özniteliğinin (normalde çalışanKimsi) tam eşleşmesi olup olduğunu kontrol edin. </span><span class="sxs-lookup"><span data-stu-id="01ab3-110">If the user already exists and the matching ID check failed to link the Workday account to Active Directory account, then check if the matching ID attribute (typically **employeeID**) in both Workday and AD have an exact match.</span></span> <span data-ttu-id="01ab3-111">Eşleşmesi yoksa, bu sorunun düzeltilecek bir veri sorunudur.</span><span class="sxs-lookup"><span data-stu-id="01ab3-111">If they don't have a match, it is a data issue that needs to be fixed.</span></span> <span data-ttu-id="01ab3-112">Örneğin, İşGünü'nin ÇalışanKimlikKimlikKimsi 001052 ve AD'de 1052 ise, sağlama altyapısı iki hesabı bağamaz ve zaten var olan bir kullanıcıyı oluşturmayı dener.</span><span class="sxs-lookup"><span data-stu-id="01ab3-112">For example, if the EmployeeID in Workday is 001052 and in AD it is 1052, then the provisioning engine will fail to link the two accounts and will try to create a user that already exists.</span></span> <span data-ttu-id="01ab3-113">Bu durumda çözüm, AD'de **ÇalışanKimlik** değerini baştaki sıfırları içerecek şekilde değiştirmek ve bunu 001052 yapmaktır.</span><span class="sxs-lookup"><span data-stu-id="01ab3-113">The solution in this case is to change the **EmployeeID** value in AD to include the leading zeros to make it 001052.</span></span>
<span data-ttu-id="01ab3-114">UPN oluşturan ifade benzersiz bir değer oluşturamazsa, her zaman benzersiz bir değer oluşturmak için **SelectUniqueValue** de-duplication işlevini kullanmayı göz önünde bulundurabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="01ab3-114">If the UPN-generating expression is not generating a unique value, consider using the de-duplication function **SelectUniqueValue** to generate a unique value each time.</span></span>

<span data-ttu-id="01ab3-115">**İşGünü'nde AD Kullanıcı Sağlama, AD kullanıcı hesabı için yönetici öznitelik değeri ayarlanmıyor**</span><span class="sxs-lookup"><span data-stu-id="01ab3-115">**Workday to AD User Provisioning does not set manager attribute value for AD user account**</span></span>

<span data-ttu-id="01ab3-116">İşGünü'nde AD Kullanıcı Hazırlama işi, AD kullanıcı **hesapları** için yönetici öznitelik değerini ayar çalışmıyor.</span><span class="sxs-lookup"><span data-stu-id="01ab3-116">The Workday to AD User Provisioning job is not setting the **manager** attribute value for AD user accounts.</span></span> <span data-ttu-id="01ab3-117">Bu davranış görülürken iki olası senaryo vardır:</span><span class="sxs-lookup"><span data-stu-id="01ab3-117">There are two possible scenarios when this behavior is seen:</span></span>

1. <span data-ttu-id="01ab3-118">İşGünü'nde yönetici ilgili AD Kullanıcı hesabına çözüm bulunamaz, çünkü yönetici kapsamda değildir.</span><span class="sxs-lookup"><span data-stu-id="01ab3-118">The manager in Workday cannot be resolved to a corresponding AD User account because the manager is not in scope.</span></span>
2. <span data-ttu-id="01ab3-119">Birden **çok AD etki alanı** senaryosunda, İşGünü'nde yönetici kullanıcıyla aynı etki alanında değildir.</span><span class="sxs-lookup"><span data-stu-id="01ab3-119">In a **multiple AD domains** scenario, the manager in Workday is not present in the same domain as the user.</span></span>

<span data-ttu-id="01ab3-120">Sorunu çözmek için şu adımları deneyin:</span><span class="sxs-lookup"><span data-stu-id="01ab3-120">Try these steps to resolve the issue:</span></span>

1. <span data-ttu-id="01ab3-121">Kapsam filtreleme filtrelerini tanımladıysanız, önce yöneticinin kapsam içinde olup olduğunu ve kapsam kapsamının kapsamının tamamlandığı yan tümcesini kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="01ab3-121">If you have defined scoping filters, first check if the manager is in scope and that it satisfies the scoping clause.</span></span> <span data-ttu-id="01ab3-122">Yönetici kapsam filtrelemesini karşılayana kadar filtreyi değiştirerek, yöneticinin sağlama işlemi kapsamında da yer alamayacak şekilde filtreyi değiştirmesini sağlar.</span><span class="sxs-lookup"><span data-stu-id="01ab3-122">If the manager does not satisfy the scoping filter, change the filter so that the manager is also in scope of the provisioning operation.</span></span>
2. <span data-ttu-id="01ab3-123">Birden çok AD etki alanınız varsa, bağlayıcının etki alanı yöneticisi başvurularını çözememeyle ilgili bilinen bir sınırlaması vardır.</span><span class="sxs-lookup"><span data-stu-id="01ab3-123">If you have multiple AD domains, then the connector has a known limitation of inability to resolve cross-domain manager references.</span></span>

<span data-ttu-id="01ab3-124">Otomatik sağlama için iş günü yapılandırma hakkında daha fazla ayrıntı için öğreticiye bakın: Otomatik kullanıcı [sağlama için İşGünü'ne yapılandırma.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)</span><span class="sxs-lookup"><span data-stu-id="01ab3-124">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>













