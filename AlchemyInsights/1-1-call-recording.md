---
title: 1:1 arama kaydı
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733869"
---
# <a name="11-call-recording"></a><span data-ttu-id="c1d5b-102">1:1 arama kaydı</span><span class="sxs-lookup"><span data-stu-id="c1d5b-102">1:1 call recording</span></span>

<span data-ttu-id="c1d5b-103">Yöneticilerin, kullanıcıların 1:1 arama kaydetmelerine izin vermeye devam etmek için hemen harekete geçleri gerekir.</span><span class="sxs-lookup"><span data-stu-id="c1d5b-103">Administrators need to take action now to continue allowing users to Record 1:1 calls.</span></span>
 
<span data-ttu-id="c1d5b-104">12 Nisan 2021'den itibaren, yeni bir Teams Arama İlkesi *seçeneği AllowCloudRecordingForCalls'u zorlamaya başlayacağız.*</span><span class="sxs-lookup"><span data-stu-id="c1d5b-104">Beginning April 12, 2021, we will start enforcing a new Teams Calling Policy option *AllowCloudRecordingForCalls*.</span></span> 

<span data-ttu-id="c1d5b-105">Şu anda 1:1 arama kaydı özellikleri, Teams Toplantı *İlkeleri'nin AllowCloudRecording* seçeneği tarafından denetlenmektedir.</span><span class="sxs-lookup"><span data-stu-id="c1d5b-105">Currently 1:1 call recording capabilities are controlled by the *AllowCloudRecording* option in Teams Meeting Policies.</span></span> <span data-ttu-id="c1d5b-106">Kullanıcılarının Teams Toplantıları kaydetmesine izin veriliyorsa, bire bir aramaları da kaydedebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="c1d5b-106">If your users are allowed to record Teams Meetings they can also record 1:1 calls.</span></span>

<span data-ttu-id="c1d5b-107">Tüm kullanıcıların bire bir arama kaydetmelerini engellemeyi tercih ederseniz herhangi bir işlem yapmaya gerek yok.</span><span class="sxs-lookup"><span data-stu-id="c1d5b-107">If you prefer to block all users from recording 1:1 calls, you do not need to take any action.</span></span> <span data-ttu-id="c1d5b-108">*AllowCloudRecordingForCalls* arama ilkesi seçeneği varsayılan $False kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="c1d5b-108">*AllowCloudRecordingForCalls* calling policy option will be $False by default.</span></span>

<span data-ttu-id="c1d5b-109">Bu değişiklik, şu İleti Merkezi Gönderisinde belgelenmektedir: [(Güncelleştirildi) 1:1](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) Arama kaydı ilkesine giriş Teams Arama İlkesi Seçeneğini ayarlamak için [Teams PowerShell'i kullanasınız.](https://docs.microsoft.com/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="c1d5b-109">This change is documented in the following Message Center Post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) To set the Teams Calling Policy Option you must use [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span></span>

<span data-ttu-id="c1d5b-110">**Bire bir aramalarda** arama kaydını etkinleştirmek için: Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span><span class="sxs-lookup"><span data-stu-id="c1d5b-110">**To enable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span></span>

<span data-ttu-id="c1d5b-111">**Bire bir aramalarda** arama kaydını devre dışı bırakmak için: Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span><span class="sxs-lookup"><span data-stu-id="c1d5b-111">**To disable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span></span>

