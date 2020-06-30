---
title: Intune ile Koşullu Erişim
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931456"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="23d89-102">Intune ile Koşullu Erişim</span><span class="sxs-lookup"><span data-stu-id="23d89-102">Conditional Access with Intune</span></span>

<span data-ttu-id="23d89-103">**Koşullu Erişimi** Intune ile kullanmak 3 adım gerektirir:</span><span class="sxs-lookup"><span data-stu-id="23d89-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="23d89-104">Aygıt **uyumlu** kabul edilmeden önce karşılanması gereken ayarları tanımlamak için bir Uyumluluk Politikası[(Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows)](https://docs.microsoft.com//intune/compliance-policy-create-windows)oluşturun.</span><span class="sxs-lookup"><span data-stu-id="23d89-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="23d89-105">Örneğin, bir aygıtın uyumlu kabul edilmeden önce en az 6 basamaklı bir iğneye sahip olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="23d89-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="23d89-106">Hangi kaynakların korunduğunu ve bu kaynaklara erişmek için hangi koşulların karşılanması gerektiğini tanımlayan **koşullu erişim ilkesi** oluşturun.</span><span class="sxs-lookup"><span data-stu-id="23d89-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="23d89-107">[Örneğin,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) bir aygıtın şirket e-postasına erişmeden önce uyumlu olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="23d89-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="23d89-108">Hem **Uyumluluk İlkeleri'nin** hem de **Koşullu Erişim İlkelerinin** istenilen kullanıcı gruplarına hedef olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="23d89-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="23d89-109">Bu, Azure Etkin Dizini'nde belirli kullanıcı grupları oluşturulmasını gerektirebilir.</span><span class="sxs-lookup"><span data-stu-id="23d89-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="23d89-110">**Yararlı bağlantılar:**</span><span class="sxs-lookup"><span data-stu-id="23d89-110">**Helpful links:**</span></span>

[<span data-ttu-id="23d89-111">Cihaz uyumluluğuna genel bakış</span><span class="sxs-lookup"><span data-stu-id="23d89-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="23d89-112">SORUN Giderme CA</span><span class="sxs-lookup"><span data-stu-id="23d89-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="23d89-113">Sorun giderme ilkesi</span><span class="sxs-lookup"><span data-stu-id="23d89-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="23d89-114">E-postayı (Çevrimiçi Exchange) uyumlu olmayan aygıtların erişiminden korumak için her iki belgeye de uyulmalıdır:</span><span class="sxs-lookup"><span data-stu-id="23d89-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="23d89-115">EAS kullanan cihazlardan e-posta erişimini koruma</span><span class="sxs-lookup"><span data-stu-id="23d89-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="23d89-116">Outlook gibi modern kimlik doğrulama istemcilerini kullanan aygıtlardan e-posta erişimini koruma</span><span class="sxs-lookup"><span data-stu-id="23d89-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)