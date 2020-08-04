---
title: Intune Wi-Fi profilleri
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555817"
---
# <a name="intune-wi-fi-profiles"></a><span data-ttu-id="13642-102">Intune Wi-Fi profilleri</span><span class="sxs-lookup"><span data-stu-id="13642-102">Intune Wi-Fi profiles</span></span>

<span data-ttu-id="13642-103">MDM istemcileri için Wi-Fi bağlantısının başarılı bir şekilde uygulanması, kurumsal Wi-Fi altyapısının gereksinimlerini yansıtan doğru şekilde dağıtılan bir profile bağlıdır.</span><span class="sxs-lookup"><span data-stu-id="13642-103">Successful implementation of Wi-Fi connectivity for MDM clients depends on a correctly deployed profile that reflects the requirements of the corporate Wi-Fi infrastructure.</span></span> <span data-ttu-id="13642-104">Araştırdığınız istemci platformları için uygun ayarları gözden geçirmek için bkz:</span><span class="sxs-lookup"><span data-stu-id="13642-104">To review the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="13642-105">Microsoft Intune'da Android çalıştıran cihazlar için Wi-Fi ayarları ekleme</span><span class="sxs-lookup"><span data-stu-id="13642-105">Add Wi-Fi settings for devices running Android in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android)

[<span data-ttu-id="13642-106">Microsoft Intune'da Android Enterprise'a özel ve tam olarak yönetilen cihazlar için Wi-Fi ayarları ekleme</span><span class="sxs-lookup"><span data-stu-id="13642-106">Add Wi-Fi settings for Android Enterprise dedicated and fully managed devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[<span data-ttu-id="13642-107">Microsoft Intune'da iOS ve iPadOS aygıtları için Wi-Fi ayarları ekleme</span><span class="sxs-lookup"><span data-stu-id="13642-107">Add Wi-Fi settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[<span data-ttu-id="13642-108">Intune'da Windows 10 ve sonraki aygıtlar için Wi-Fi ayarları ekleme</span><span class="sxs-lookup"><span data-stu-id="13642-108">Add Wi-Fi settings for Windows 10 and later devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[<span data-ttu-id="13642-109">Intune'daki Windows aygıtları için Wi-Fi ayarlarını alma</span><span class="sxs-lookup"><span data-stu-id="13642-109">Import Wi-Fi settings for Windows devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

<span data-ttu-id="13642-110">**Sık Karşılaşılan Sorunlar**</span><span class="sxs-lookup"><span data-stu-id="13642-110">**Common Issues**</span></span>

<span data-ttu-id="13642-111">**Wi-Fi profilinde belirtilen dağıtılmış sertifikaya bağlı bir Wi-Fi profili dağıtıyorum. Ancak, yapılandırma profilleri bir hata durumu gösteriyor.**</span><span class="sxs-lookup"><span data-stu-id="13642-111">**I'm deploying a Wi-Fi profile that is dependent on a deployed certificate specified in the Wi-Fi profile. However, the configuration profiles are showing an error status.**</span></span>

<span data-ttu-id="13642-112">Cihazınızın sertifikayı aldığından kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="13642-112">Check that your device received the certificate.</span></span>

1. <span data-ttu-id="13642-113">Intune'da **Tüm Aygıtlar'a** gidin ve aygıt > **Aygıtı'nı**seçin.</span><span class="sxs-lookup"><span data-stu-id="13642-113">In Intune, go to **All Devices** and select the device > **Device configuration**.</span></span>

2. <span data-ttu-id="13642-114">Beklenen tüm profillerin listelenmiş ve başarılı bir durumda olup olmadığını denetleyin.</span><span class="sxs-lookup"><span data-stu-id="13642-114">Check that all expected profiles are listed and in a successful state.</span></span>

3. <span data-ttu-id="13642-115">Android profili için, sertifika zincirinizde ara sertifikalar varsa, bunların Android cihazlara dağıtıldıklarından emin olun.</span><span class="sxs-lookup"><span data-stu-id="13642-115">For an Android profile, if you have intermediate certificates in your certificate chain, make sure they are deployed to Android devices.</span></span>

    <span data-ttu-id="13642-116">Sertifika durumunu kontrol etmek için **Aygıt yapılandırma**  >  **Profilleri**Android ara  >  **CA**  >  **Özellikleri**  >  **Güvenilir Sertifika'ya**gidin.</span><span class="sxs-lookup"><span data-stu-id="13642-116">To check the certificate status, go to **Device configuration** > **Profiles** > **Android intermediate CA** > **Properties** > **Trusted Certificate**.</span></span>

<span data-ttu-id="13642-117">Hataları görmeye devam ederseniz, yordamları ve sorun giderme bölümlerini gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="13642-117">If you continue to see errors, review the procedures and troubleshooting sections.</span></span> <span data-ttu-id="13642-118">Daha fazla bilgi için Microsoft [Intune ile sorun giderme SCEP sertifika profilleri için Genel Bakış'a](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)bakın.</span><span class="sxs-lookup"><span data-stu-id="13642-118">For more info, see [Overview for troubleshooting SCEP certificate profiles with Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span></span>

<span data-ttu-id="13642-119">**Bir cihaza Wi-Fi profili dağıttım. Intune başarılı olduğunu gösteriyor, ancak cihaz Wi-Fi'a bağlanmıyor.**</span><span class="sxs-lookup"><span data-stu-id="13642-119">**I deployed a Wi-Fi profile to a device. Intune is showing that it was successful, but the device is not connecting to the Wi-Fi.**</span></span>

<span data-ttu-id="13642-120">Başarılı bir durum, Intune'un profili yapılandırılmış olarak başarıyla dağıtmış olduğu anlamına gelir.</span><span class="sxs-lookup"><span data-stu-id="13642-120">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="13642-121">Ancak, bu yapılandırmalar ağınız ve/veya kimlik doğrulama gereksinimleriniz ile eşleşmeyebilir.</span><span class="sxs-lookup"><span data-stu-id="13642-121">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="13642-122">Bağlantı girişimi hakkında daha fazla bilgi için, altyapı ve kimlik doğrulama hizmetindeki (Wi-Fi Access noktası denetleyicisi ve NPS/Radius sunucusunda) günlükleri gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="13642-122">For more details about the attempted connection, review logs in the infrastructure and authentication service (on the Wi-Fi Access point controller and NPS/Radius server).</span></span> <span data-ttu-id="13642-123">Günlükleri toplamak ve incelemek için ağ altyapı ekibinizle veya üçüncü taraf Wi-Fi satıcısıyla çalışmanız gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="13642-123">You might have to work with your network infrastructure team, or the third-party Wi-Fi vendor, to gather and review logs.</span></span>