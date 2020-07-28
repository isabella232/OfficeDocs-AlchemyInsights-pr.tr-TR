---
title: Intune'dan aygıt pini/parola sıfırlama
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1278"
- "6700008"
ms.openlocfilehash: fd3bb957b0da22dfab5a9988a82e398757e12ee5
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440096"
---
# <a name="device-pinpassword-reset-from-intune"></a><span data-ttu-id="32525-102">Intune'dan aygıt pini/parola sıfırlama</span><span class="sxs-lookup"><span data-stu-id="32525-102">Device pin/password reset from Intune</span></span>

<span data-ttu-id="32525-103">Parolayı Kaldır eylemini kullanarak bir parolayı kaldırabilir veya kullanıcıyı iOS veya Android çalıştıran bir aygıt için Intune'da yeni bir parola oluşturmaya zorlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="32525-103">You can remove a passcode or force a user to create a new passcode in Intune for a device running iOS or Android by using the Remove Passcode action.</span></span>

<span data-ttu-id="32525-104">Yalnızca belirli işletim sistemi türleri ve iş profili türleri bu eylemi destekler.</span><span class="sxs-lookup"><span data-stu-id="32525-104">Only specific operating system types and work profile types support this action.</span></span>

<span data-ttu-id="32525-105">Desteklenen platformlar ve sıfırlama parola eyleminin nasıl tetiklenilen hakkında ayrıntılı bilgi için [Intune'da bir aygıt parolasını sıfırla veya kaldır'](https://docs.microsoft.com/intune/device-passcode-reset)a bakın.</span><span class="sxs-lookup"><span data-stu-id="32525-105">For details about supported platforms and how to trigger the reset passcode action, see [Reset or remove a device passcode in Intune](https://docs.microsoft.com/intune/device-passcode-reset).</span></span>

<span data-ttu-id="32525-106">Windows 10 Mobile işletim sistemini çalıştıran aygıtlarda Pin Sıfırlama eylemini kullanarak varolan bir pimi yeni bir değere sıfırlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="32525-106">You can reset an existing pin to a new value using the Pin Reset action on devices running the Windows 10 Mobile operating system.</span></span> <span data-ttu-id="32525-107">Bu, kullanıcının aygıtın kilidini açmasını ve uygun şekilde yeni bir pin ayarlamasını sağlar.</span><span class="sxs-lookup"><span data-stu-id="32525-107">This allows the user to unlock the device and set a new pin as appropriate.</span></span> <span data-ttu-id="32525-108">Daha fazla bilgi için bkz: [Intune'u kullanarak Windows aygıtlarında parolayı sıfırla.](https://docs.microsoft.com/intune/device-windows-pin-reset)</span><span class="sxs-lookup"><span data-stu-id="32525-108">For more info, see [Reset the passcode on Windows devices using Intune](https://docs.microsoft.com/intune/device-windows-pin-reset).</span></span>