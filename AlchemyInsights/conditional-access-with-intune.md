---
title: Intune ile Koşullu Erişim
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 20ef8205431aad821419f2559be3402c8228d838
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704806"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="9e9c6-102">Intune ile Koşullu Erişim</span><span class="sxs-lookup"><span data-stu-id="9e9c6-102">Conditional Access with Intune</span></span>

<span data-ttu-id="9e9c6-103">**Intune** ile Koşullu Erişim'i kullanmak için 3 adım gerekir:</span><span class="sxs-lookup"><span data-stu-id="9e9c6-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="9e9c6-104">Cihazın uyumlu  **kabul edilene**  kadar karşılanmayacak ayarları tanımlamak için Uyumluluk İlkesi [(Android,](https://docs.microsoft.com/intune/compliance-policy-create-android)  [iOS,](https://docs.microsoft.com/intune/compliance-policy-create-ios)  [Windows)](https://docs.microsoft.com//intune/compliance-policy-create-windows)oluşturun.</span><span class="sxs-lookup"><span data-stu-id="9e9c6-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="9e9c6-105">Örneğin, bir cihazın uyumlu kabul edilene kadar en az 6 basamaklı bir pin'i olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="9e9c6-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="9e9c6-106">Korunan **kaynakları ve bu**  kaynaklara erişmek için hangi koşulların karşı korunmasını gerektir olacağını tanımlayan bir Koşullu Erişim İlkesi oluşturun.</span><span class="sxs-lookup"><span data-stu-id="9e9c6-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="9e9c6-107">[Örneğin, bir cihaz](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  kurumsal e-postaya erişmeden önce uyumlu olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="9e9c6-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="9e9c6-108">İstenen kullanıcı **gruplarına**  hem  **Uyumluluk İlkelerinin**  hem de Koşullu Erişim İlkelerinin hedefli olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="9e9c6-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="9e9c6-109">Bunun için Azure Active Directory'de belirli kullanıcı grupları oluşturulması gerekli olabilir.</span><span class="sxs-lookup"><span data-stu-id="9e9c6-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="9e9c6-110">**Yararlı bağlantılar:**</span><span class="sxs-lookup"><span data-stu-id="9e9c6-110">**Helpful links:**</span></span>

[<span data-ttu-id="9e9c6-111">Cihaz uyumluluğuna genel bakış</span><span class="sxs-lookup"><span data-stu-id="9e9c6-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="9e9c6-112">CA sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="9e9c6-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="9e9c6-113">Sorun giderme ilkesi</span><span class="sxs-lookup"><span data-stu-id="9e9c6-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="9e9c6-114">Uyumlu olmayan cihazlar tarafından E-postayı (Exchange Online) erişime karşı korumak için her iki belge de izlenmektedir:</span><span class="sxs-lookup"><span data-stu-id="9e9c6-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="9e9c6-115">EAS kullanarak cihazlardan e-posta erişimini koruma</span><span class="sxs-lookup"><span data-stu-id="9e9c6-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="9e9c6-116">Outlook gibi modern kimlik doğrulama istemcilerini kullanarak cihazlardan e-posta erişimini koruma</span><span class="sxs-lookup"><span data-stu-id="9e9c6-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)