---
title: Intune ilkeleri ve profilleri oluşturma
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1064"
- "6700005"
ms.openlocfilehash: af8f1a3dfaccaca52f187f387274d63b22631b2d
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704662"
---
# <a name="creating-intune-policy-and-profiles"></a><span data-ttu-id="7a7a8-102">Intune ilkesi ve profilleri oluşturma</span><span class="sxs-lookup"><span data-stu-id="7a7a8-102">Creating Intune policy and profiles</span></span>

<span data-ttu-id="7a7a8-103">Intune'da, farklı şeyler yapacak ilkeler ve profiller oluşturabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="7a7a8-103">In Intune, you can create policies and profiles that do different things.</span></span>

- <span data-ttu-id="7a7a8-104">**Kayıt profilleri:** Cihazlarınızı platforma göre önceden yapılandırma, kullanıcı yakınlıklarını etkinleştirme, çok faktörlü kimlik doğrulamasını kullanma ve daha fazlası.</span><span class="sxs-lookup"><span data-stu-id="7a7a8-104">**Enrollment profiles**: Preconfigure your devices by platform, enable user affinity, use multi-factor authentication, and more.</span></span>

  <span data-ttu-id="7a7a8-105">[Cihaz kaydı nedir ve](https://docs.microsoft.com/intune/device-enrollment) [Android,](https://docs.microsoft.com/intune/android-enroll) [iOS,](https://docs.microsoft.com/intune/ios-enroll) [macOS](https://docs.microsoft.com/intune/macos-enroll)ve [Windows](https://docs.microsoft.com/intune/windows-enrollment-methods) için kayıt profilleri oluşturmak iyi bir kaynaktır.</span><span class="sxs-lookup"><span data-stu-id="7a7a8-105">[What is device enrollment](https://docs.microsoft.com/intune/device-enrollment), and create enrollment profiles for [Android](https://docs.microsoft.com/intune/android-enroll), [iOS](https://docs.microsoft.com/intune/ios-enroll), [macOS](https://docs.microsoft.com/intune/macos-enroll), and [Windows](https://docs.microsoft.com/intune/windows-enrollment-methods) are good resources.</span></span>

- <span data-ttu-id="7a7a8-106">**Uyumluluk ilkeleri:** Cihazların uyumlu olması için izlemesi gereken kuralları ve ayarları tanımlayın.</span><span class="sxs-lookup"><span data-stu-id="7a7a8-106">**Compliance policies**: Define the rules and settings that devices must follow to be compliant.</span></span> <span data-ttu-id="7a7a8-107">Ayrıca, cihazları izlemek ve kullanıcılara uyumluluk dışı durumu bildirmek için uyumluluk ilkelerini de kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="7a7a8-107">You can also use compliance policies to monitor devices, and notify users of non-compliance.</span></span>

  <span data-ttu-id="7a7a8-108">Cihaz uyumluluk [ilkeleriyle çalışmaya başlama.](https://docs.microsoft.com/intune/device-compliance-get-started)</span><span class="sxs-lookup"><span data-stu-id="7a7a8-108">Get started with [device compliance policies](https://docs.microsoft.com/intune/device-compliance-get-started).</span></span>
- <span data-ttu-id="7a7a8-109">**Koşullu erişim ilkeleri:** Giriş koşullarına bağlı olarak kuruluş kaynaklarının güvenliğini sağlama.</span><span class="sxs-lookup"><span data-stu-id="7a7a8-109">**Conditional access policies**: Help secure organizational resources, depending on conditions that you enter.</span></span> <span data-ttu-id="7a7a8-110">Örneğin, uyumlu olmayan cihazlar için, e-postaya ve SharePoint'e erişimi kısıtlamak için koşullu erişimi kullanın.</span><span class="sxs-lookup"><span data-stu-id="7a7a8-110">For example, for devices that aren't compliant, use conditional access to restrict access to email and SharePoint.</span></span>

  <span data-ttu-id="7a7a8-111">[Koşullu erişim nedir ve](https://docs.microsoft.com/intune/conditional-access) [koşullu erişimi kullanmanın yaygın yolları,](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use) kullanmaya başlamanız için iyi kaynaklardır.</span><span class="sxs-lookup"><span data-stu-id="7a7a8-111">[What is conditional access](https://docs.microsoft.com/intune/conditional-access) and [common ways to use conditional access](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use) are good resources to get started.</span></span>

- <span data-ttu-id="7a7a8-112">**Yapılandırma profilleri:** E-posta ayarları dahil olmak üzere cihazlarda özellikleri ve ayarları yönetin, WiFi ağı ekleyin, yerleşik şablonları kullanın, iOS ve macOS cihaz özelliklerini kontrol edin ve daha fazlasını yapın.</span><span class="sxs-lookup"><span data-stu-id="7a7a8-112">**Configuration profiles**: Manage features and settings on devices, including email settings, add a WiFi network, use built-in templates, control iOS and macOS device features, and more.</span></span>

  <span data-ttu-id="7a7a8-113">Cihaz yapılandırma [profillerini başlatabilirsiniz.](https://docs.microsoft.com/intune/device-profiles)</span><span class="sxs-lookup"><span data-stu-id="7a7a8-113">Get started at [device configuration profiles](https://docs.microsoft.com/intune/device-profiles).</span></span>

<span data-ttu-id="7a7a8-114">Yararlı bağlantılar:</span><span class="sxs-lookup"><span data-stu-id="7a7a8-114">Helpful links:</span></span>

- [<span data-ttu-id="7a7a8-115">Intune'da cihaz ilkeleri ve profilleriyle ilgili sık sorulan sorular, sorunlar ve çözünürlükler</span><span class="sxs-lookup"><span data-stu-id="7a7a8-115">Common questions, issues, and resolutions with device policies and profiles in Intune</span></span>](https://docs.microsoft.com/intune/device-profile-troubleshoot)

- [<span data-ttu-id="7a7a8-116">Intune'da ilke ve profil sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="7a7a8-116">Troubleshoot policies and profiles in Intune</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)
