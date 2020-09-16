---
title: E-posta profillerini Intune ile kullanma
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 92d91de5d369eb9d0ffde2580b75376035a6945b
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653308"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="58e38-102">E-posta profillerini Intune ile kullanma</span><span class="sxs-lookup"><span data-stu-id="58e38-102">Using email profiles with Intune</span></span>

<span data-ttu-id="58e38-103">Intune, birden çok cihaz platformunda yerel (yerleşik) e-posta istemcisi için e-posta profilleri oluşturmak ve dağıtmak için kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="58e38-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="58e38-104">Var olan profillerin nasıl işlendiği ve e-posta profillerinin nasıl kaldırılacağı dahil olmak üzere e-posta profilleriyle ilişkilendirilmiş kısıtlamaların bazıları hakkında bilgi için, [Intune kullanarak aygıtlara e-posta ayarları ekleme](https://docs.microsoft.com/intune/email-settings-configure)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="58e38-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="58e38-105">Her cihaz platformu için e-posta profili oluşturma hakkında daha fazla bilgi için bkz:</span><span class="sxs-lookup"><span data-stu-id="58e38-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="58e38-106">Intune 'da e-postayı, kimlik doğrulamayı ve eşitlemeyi yapılandırmak için Android cihaz ayarları</span><span class="sxs-lookup"><span data-stu-id="58e38-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="58e38-107">Microsoft Intune 'da iOS ve ıpados cihazları için e-posta ayarları ekleme</span><span class="sxs-lookup"><span data-stu-id="58e38-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="58e38-108">Windows Phone 8,1 çalıştıran cihazlarda Microsoft Intune 'da e-posta profili ayarları</span><span class="sxs-lookup"><span data-stu-id="58e38-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="58e38-109">Microsoft Intune 'da Windows 10 çalıştıran cihazların e-posta profili ayarları</span><span class="sxs-lookup"><span data-stu-id="58e38-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="58e38-110">**Yaygın eşitleme sorunu**</span><span class="sxs-lookup"><span data-stu-id="58e38-110">**Common syncing issue**</span></span>

<span data-ttu-id="58e38-111">**Android e-posta profilinde bir KNOX Kullanıcı kişilerinin, takvimin ve görevlerinin Kullanıcı aygıtlarına eşitlenmesini engeller.**</span><span class="sxs-lookup"><span data-stu-id="58e38-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="58e38-112">Android KNOX e-posta profilinde KNOX her biri etkin olarak ayarlanarak hangi içerik türlerinin cihaza eşitleneceğini belirleme seçeneğini belirtin.</span><span class="sxs-lookup"><span data-stu-id="58e38-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="58e38-113">İçerik türlerinden herhangi birinin ayarı **yapılandırılmazsa** (varsayılan olarak), bu içerik türü otomatik olarak eşitlenmez.</span><span class="sxs-lookup"><span data-stu-id="58e38-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="58e38-114">Bir kullanıcı doğrudan cihazda doğrudan cihazda istedikleri içerik türünü etkinleştirebilir, ancak bu yapılandırmanın Intune ilke ayarı tarafından üzerine yazılır ve eşitleme bu içerik türü için durdurulur.</span><span class="sxs-lookup"><span data-stu-id="58e38-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

