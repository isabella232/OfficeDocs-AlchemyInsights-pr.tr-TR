---
title: Intune ilkeleri ve profilleri oluşturma
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 05/07/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1064"
- "6700005"
ms.openlocfilehash: 11516232e7ad1fb1d54f07bccd31d586d5c04d42
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36514783"
---
# <a name="creating-intune-policy-and-profiles"></a><span data-ttu-id="c46df-102">Intune ilke ve profil oluşturma</span><span class="sxs-lookup"><span data-stu-id="c46df-102">Creating Intune policy and profiles</span></span>

<span data-ttu-id="c46df-103">Intune içinde ilkeleri ve farklı şeyler profilleri oluşturabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="c46df-103">In Intune, you can create policies and profiles that do different things.</span></span>

- <span data-ttu-id="c46df-104">**Kayıt profilleri**: aygıtlarınızın platformu tarafından önceden, kullanıcı benzeşimini etkinleştirmek, çok faktörlü kimlik doğrulama ve daha fazlasını kullanın.</span><span class="sxs-lookup"><span data-stu-id="c46df-104">**Enrollment profiles**: Preconfigure your devices by platform, enable user affinity, use multi-factor authentication, and more.</span></span>

  <span data-ttu-id="c46df-105">[Aygıt kayıt nedir](https://docs.microsoft.com/intune/device-enrollment), [Android](https://docs.microsoft.com/intune/android-enroll), [IOS](https://docs.microsoft.com/intune/ios-enroll), [macOS](https://docs.microsoft.com/intune/macos-enroll)için kayıt profilleri oluşturmak ve [iyi kaynakları pencerelerdir](https://docs.microsoft.com/intune/windows-enrollment-methods) .</span><span class="sxs-lookup"><span data-stu-id="c46df-105">[What is device enrollment](https://docs.microsoft.com/intune/device-enrollment), and create enrollment profiles for [Android](https://docs.microsoft.com/intune/android-enroll), [iOS](https://docs.microsoft.com/intune/ios-enroll), [macOS](https://docs.microsoft.com/intune/macos-enroll), and [Windows](https://docs.microsoft.com/intune/windows-enrollment-methods) are good resources.</span></span>

- <span data-ttu-id="c46df-106">**Uygunluk ilkeleri**: kurallar ve aygıtların uyumlu olması için izlemeniz gereken ayarları tanımlayın.</span><span class="sxs-lookup"><span data-stu-id="c46df-106">**Compliance policies**: Define the rules and settings that devices must follow to be compliant.</span></span> <span data-ttu-id="c46df-107">Uygunluk ilkeleri aygıtlarını izlemek için kullanın ve uyumu olmayan kullanıcılara bildirmek.</span><span class="sxs-lookup"><span data-stu-id="c46df-107">You can also use compliance policies to monitor devices, and notify users of non-compliance.</span></span>

  <span data-ttu-id="c46df-108">[Aygıt uyumluluğu ilkeleri](https://docs.microsoft.com/intune/device-compliance-get-started)ile başlayın.</span><span class="sxs-lookup"><span data-stu-id="c46df-108">Get started with [device compliance policies](https://docs.microsoft.com/intune/device-compliance-get-started).</span></span>
- <span data-ttu-id="c46df-109">**Koşullu erişim ilkeleri**: girdiğiniz koşullara bağlı olarak güvenli kuruluş kaynakları Yardım.</span><span class="sxs-lookup"><span data-stu-id="c46df-109">**Conditional access policies**: Help secure organizational resources, depending on conditions that you enter.</span></span> <span data-ttu-id="c46df-110">Örneğin, uyumlu olmayan aygıtlar için koşullu erişim için e-posta ve SharePoint erişimi kısıtlamak için kullanın.</span><span class="sxs-lookup"><span data-stu-id="c46df-110">For example, for devices that aren't compliant, use conditional access to restrict access to email and SharePoint.</span></span>

  <span data-ttu-id="c46df-111">[Koşullu erişim nedir](https://docs.microsoft.com/intune/conditional-access) ve [ortak bir koşullu erişim kullanma yöntemlerini](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use) kullanmaya başlamak için iyi kaynaklardır.</span><span class="sxs-lookup"><span data-stu-id="c46df-111">[What is conditional access](https://docs.microsoft.com/intune/conditional-access) and [common ways to use conditional access](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use) are good resources to get started.</span></span>

- <span data-ttu-id="c46df-112">**Yapılandırma profilleri**: özellikleri ve ayarları e-posta ayarları dahil olmak üzere aygıtlarda yönetmek, WiFi ağ eklemek, yerleşik şablonlar IOS ve macOS aygıt denetimi ve daha fazlasını kullanır.</span><span class="sxs-lookup"><span data-stu-id="c46df-112">**Configuration profiles**: Manage features and settings on devices, including email settings, add a WiFi network, use built-in templates, control iOS and macOS device features, and more.</span></span>

  <span data-ttu-id="c46df-113">[Aygıt yapılandırma profilleri](https://docs.microsoft.com/intune/device-profiles)başlayın.</span><span class="sxs-lookup"><span data-stu-id="c46df-113">Get started at [device configuration profiles](https://docs.microsoft.com/intune/device-profiles).</span></span>

<span data-ttu-id="c46df-114">Yararlı bağlantılar:</span><span class="sxs-lookup"><span data-stu-id="c46df-114">Helpful links:</span></span>

- [<span data-ttu-id="c46df-115">Ortak sorular, sorunlar ve aygıt ilkeleri ve Intune profilleri ile çözümler</span><span class="sxs-lookup"><span data-stu-id="c46df-115">Common questions, issues, and resolutions with device policies and profiles in Intune</span></span>](https://docs.microsoft.com/intune/device-profile-troubleshoot)

- [<span data-ttu-id="c46df-116">İlkeleri ve profillerini Intune sorun giderme</span><span class="sxs-lookup"><span data-stu-id="c46df-116">Troubleshoot policies and profiles in Intune</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
