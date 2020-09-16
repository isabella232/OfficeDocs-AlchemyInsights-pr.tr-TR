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
ms.openlocfilehash: 9026beac824ebc3849241dbb534c27b00ef1d0eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47746779"
---
# <a name="creating-intune-policy-and-profiles"></a><span data-ttu-id="29fdb-102">Intune ilkesi ve profilleri oluşturma</span><span class="sxs-lookup"><span data-stu-id="29fdb-102">Creating Intune policy and profiles</span></span>

<span data-ttu-id="29fdb-103">Intune 'da farklı şeyler yapan ilkeler ve profiller oluşturabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="29fdb-103">In Intune, you can create policies and profiles that do different things.</span></span>

- <span data-ttu-id="29fdb-104">**Kayıt profilleri**: cihazlarınızı platforma göre önceden yapılandırın, Kullanıcı benzeşimini etkinleştirin, çok faktörlü kimlik doğrulaması kullanın ve daha fazlasını yapın.</span><span class="sxs-lookup"><span data-stu-id="29fdb-104">**Enrollment profiles**: Preconfigure your devices by platform, enable user affinity, use multi-factor authentication, and more.</span></span>

  <span data-ttu-id="29fdb-105">[Cihaz kaydı nedir](https://docs.microsoft.com/intune/device-enrollment)ve [Android](https://docs.microsoft.com/intune/android-enroll), [IOS](https://docs.microsoft.com/intune/ios-enroll), [MacOS](https://docs.microsoft.com/intune/macos-enroll)ve [Windows](https://docs.microsoft.com/intune/windows-enrollment-methods) için kayıt profilleri oluşturma iyi kaynaklardır.</span><span class="sxs-lookup"><span data-stu-id="29fdb-105">[What is device enrollment](https://docs.microsoft.com/intune/device-enrollment), and create enrollment profiles for [Android](https://docs.microsoft.com/intune/android-enroll), [iOS](https://docs.microsoft.com/intune/ios-enroll), [macOS](https://docs.microsoft.com/intune/macos-enroll), and [Windows](https://docs.microsoft.com/intune/windows-enrollment-methods) are good resources.</span></span>

- <span data-ttu-id="29fdb-106">**Uyumluluk ilkeleri**: cihazların uyumlu olması için izlenmesi gereken kuralları ve ayarları tanımlayın.</span><span class="sxs-lookup"><span data-stu-id="29fdb-106">**Compliance policies**: Define the rules and settings that devices must follow to be compliant.</span></span> <span data-ttu-id="29fdb-107">Ayrıca, uyumluluk ilkelerini, cihazları izlemek ve kullanıcıları uyumlu olmama durumunda bilgilendirmek için kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="29fdb-107">You can also use compliance policies to monitor devices, and notify users of non-compliance.</span></span>

  <span data-ttu-id="29fdb-108">[Cihaz uyumluluk ilkeleriyle](https://docs.microsoft.com/intune/device-compliance-get-started)çalışmaya başlayın.</span><span class="sxs-lookup"><span data-stu-id="29fdb-108">Get started with [device compliance policies](https://docs.microsoft.com/intune/device-compliance-get-started).</span></span>
- <span data-ttu-id="29fdb-109">**Koşullu erişim ilkeleri**: girdiğiniz koşullara bağlı olarak, kuruluş kaynaklarını güvenli hale getirme.</span><span class="sxs-lookup"><span data-stu-id="29fdb-109">**Conditional access policies**: Help secure organizational resources, depending on conditions that you enter.</span></span> <span data-ttu-id="29fdb-110">Örneğin, uyumlu olmayan cihazlarda e-posta ve SharePoint 'e erişimi kısıtlamak için koşullu erişimi kullanın.</span><span class="sxs-lookup"><span data-stu-id="29fdb-110">For example, for devices that aren't compliant, use conditional access to restrict access to email and SharePoint.</span></span>

  <span data-ttu-id="29fdb-111">Koşullu erişim ve [koşullu erişimi kullanmanın yaygın yolları](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use) [,](https://docs.microsoft.com/intune/conditional-access) başlamak için iyi kaynaklardır.</span><span class="sxs-lookup"><span data-stu-id="29fdb-111">[What is conditional access](https://docs.microsoft.com/intune/conditional-access) and [common ways to use conditional access](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use) are good resources to get started.</span></span>

- <span data-ttu-id="29fdb-112">**Yapılandırma profilleri**: e-posta ayarları, WiFi ağı ekleme, yerleşik şablonları kullanma, IOS ve MacOS cihaz özelliklerini denetleme ve daha fazlası gibi cihazlarda özellikleri ve ayarları yönetin.</span><span class="sxs-lookup"><span data-stu-id="29fdb-112">**Configuration profiles**: Manage features and settings on devices, including email settings, add a WiFi network, use built-in templates, control iOS and macOS device features, and more.</span></span>

  <span data-ttu-id="29fdb-113">[Cihaz yapılandırma profillerinde](https://docs.microsoft.com/intune/device-profiles)çalışmaya başlayın.</span><span class="sxs-lookup"><span data-stu-id="29fdb-113">Get started at [device configuration profiles](https://docs.microsoft.com/intune/device-profiles).</span></span>

<span data-ttu-id="29fdb-114">Faydalı bağlantılar:</span><span class="sxs-lookup"><span data-stu-id="29fdb-114">Helpful links:</span></span>

- [<span data-ttu-id="29fdb-115">Intune 'da cihaz ilkeleri ve profillerle ilgili sık sorulan sorular, sorunlar ve çözümler</span><span class="sxs-lookup"><span data-stu-id="29fdb-115">Common questions, issues, and resolutions with device policies and profiles in Intune</span></span>](https://docs.microsoft.com/intune/device-profile-troubleshoot)

- [<span data-ttu-id="29fdb-116">Intune 'da ilkeler ve profillerde sorun giderme</span><span class="sxs-lookup"><span data-stu-id="29fdb-116">Troubleshoot policies and profiles in Intune</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
