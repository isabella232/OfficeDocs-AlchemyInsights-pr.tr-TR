---
title: Intune ile koşullu erişim
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 5eec5982118b4f0246afadf2af219b2d5f32f95c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807679"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="74814-102">Intune ile koşullu erişim</span><span class="sxs-lookup"><span data-stu-id="74814-102">Conditional Access with Intune</span></span>

<span data-ttu-id="74814-103">Intune ile  **koşullu erişimi**  kullanmak için 3 adım gerekir:</span><span class="sxs-lookup"><span data-stu-id="74814-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="74814-104">Cihaz uyumlu olmadan önce karşılanması gereken ayarları tanımlamak için  **Uyumluluk ilkesi**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) oluşturun.</span><span class="sxs-lookup"><span data-stu-id="74814-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="74814-105">Örneğin, bir cihazın uyumlu kabul edilmeden önce en az 6 basamağı olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="74814-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="74814-106">Hangi kaynakların korunduğunu ve bu kaynaklara erişmek için hangi koşulların karşılanabileceğini tanımlayan bir **koşullu erişim ilkesi**  oluşturun.</span><span class="sxs-lookup"><span data-stu-id="74814-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="74814-107">[Örneğin,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  kurumsal e-postaya erişmeden önce bir cihazın uyumlu olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="74814-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="74814-108">Hem **uyumluluk ilkeleri**  hem de  **koşullu erişim ilkelerinin**  istenen kullanıcı gruplarını hedeflediğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="74814-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="74814-109">Bu, Azure Active Directory 'de belirli kullanıcı gruplarını oluşturmanız gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="74814-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="74814-110">**Faydalı bağlantılar:**</span><span class="sxs-lookup"><span data-stu-id="74814-110">**Helpful links:**</span></span>

[<span data-ttu-id="74814-111">Cihaz uyumuna genel bakış</span><span class="sxs-lookup"><span data-stu-id="74814-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="74814-112">Sorun giderme CA</span><span class="sxs-lookup"><span data-stu-id="74814-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="74814-113">Sorun giderme ilkesi</span><span class="sxs-lookup"><span data-stu-id="74814-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="74814-114">E-postayı uyumlu olmayan cihazlara erişimi önlemek için, her iki belgeyi de takip etmelisiniz:</span><span class="sxs-lookup"><span data-stu-id="74814-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="74814-115">EA kullanarak cihazlardan e-posta erişimini koruma</span><span class="sxs-lookup"><span data-stu-id="74814-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="74814-116">Outlook gibi modern kimlik doğrulama istemcileri kullanarak cihazlardan e-posta erişimini koruma</span><span class="sxs-lookup"><span data-stu-id="74814-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)