---
title: Intune ile e-posta profillerini kullanma
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
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555758"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="93c34-102">Intune ile e-posta profillerini kullanma</span><span class="sxs-lookup"><span data-stu-id="93c34-102">Using email profiles with Intune</span></span>

<span data-ttu-id="93c34-103">Intune, birden çok aygıt platformunda yerel (yerleşik) e-posta istemcisi için e-posta profilleri oluşturmak ve dağıtmak için kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="93c34-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="93c34-104">Varolan profillerin varlığının nasıl işlendiği ve e-posta profillerinin nasıl kaldırılılabildiğini içeren bazı kısıtlamalar hakkında bilgi için [bkz.](https://docs.microsoft.com/intune/email-settings-configure)</span><span class="sxs-lookup"><span data-stu-id="93c34-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="93c34-105">Her cihaz platformu için e-posta profilleri nin nasıl oluşturulabildiğini hakkında daha fazla bilgi için bkz:</span><span class="sxs-lookup"><span data-stu-id="93c34-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="93c34-106">Intune'da e-posta, kimlik doğrulama ve senkronizasyon yapılandırmak için Android cihaz ayarları</span><span class="sxs-lookup"><span data-stu-id="93c34-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="93c34-107">Microsoft Intune'da iOS ve iPadOS aygıtları için e-posta ayarları ekleme</span><span class="sxs-lookup"><span data-stu-id="93c34-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="93c34-108">Windows Phone 8.1 çalıştıran aygıtlar için Microsoft Intune'daki e-posta profil ayarları</span><span class="sxs-lookup"><span data-stu-id="93c34-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="93c34-109">Microsoft Intune'da Windows 10 çalıştıran aygıtlar için e-posta profil ayarları</span><span class="sxs-lookup"><span data-stu-id="93c34-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="93c34-110">**Ortak eşitleme sorunu**</span><span class="sxs-lookup"><span data-stu-id="93c34-110">**Common syncing issue**</span></span>

<span data-ttu-id="93c34-111">**Android e-posta profilindeki bir KNOX, kullanıcı Kişileri, Takvim ve Görevler'in kullanıcı aygıtlarına senkronize olmasını engeller.**</span><span class="sxs-lookup"><span data-stu-id="93c34-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="93c34-112">Android KNOX e-posta profilindeki KNOX, yöneticiye, her biri etkin olarak ayarlayarak hangi içerik türlerinin cihazla senkronize edildiğine karar verme seçeneği sunar.</span><span class="sxs-lookup"><span data-stu-id="93c34-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="93c34-113">İçerik türlerinden herhangi birinin ayarı **yapılandırılmamış** (varsayılan) olarak ayarlanmışsa, bu içerik türü otomatik olarak eşitlenmez.</span><span class="sxs-lookup"><span data-stu-id="93c34-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="93c34-114">Kullanıcı doğrudan aygıtta istediği içerik türünü el ile etkinleştirebilir, ancak bu yapılandırma Intune ilke ayarı tarafından üzerine yazılır ve bu içerik türü için eşitleme durur.</span><span class="sxs-lookup"><span data-stu-id="93c34-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

