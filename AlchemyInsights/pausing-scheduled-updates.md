---
title: Zamanlanan güncelleştirmeleri duraklatma
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 9dc0f387cf63557e2a1f81ca8f3c3ca9998170ca
ms.sourcegitcommit: d1c51266e2890f61662f77dceea2ad0c88210015
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/30/2020
ms.locfileid: "46555993"
---
# <a name="pausing-scheduled-updates"></a><span data-ttu-id="5a40c-102">Zamanlanan güncelleştirmeleri duraklatma</span><span class="sxs-lookup"><span data-stu-id="5a40c-102">Pausing scheduled updates</span></span>

<span data-ttu-id="5a40c-103">Duraklatma komutu verildiğinde, aygıtlar komutu bir sonraki giriş lerine kadar işlemez.</span><span class="sxs-lookup"><span data-stu-id="5a40c-103">When a pause command is issued, devices don't process the command until the next time they check in to Intune.</span></span> <span data-ttu-id="5a40c-104">Bu nedenle, aygıtlarınızın aşağıdakileri olabilir:</span><span class="sxs-lookup"><span data-stu-id="5a40c-104">Because of this, your devices might have:</span></span>

- <span data-ttu-id="5a40c-105">Zamanlanan güncelleştirmeleri iadeden önce yükledi.</span><span class="sxs-lookup"><span data-stu-id="5a40c-105">Installed the scheduled updates prior to check-in.</span></span>
- <span data-ttu-id="5a40c-106">Duraklatma komutunu yayınladığınızda kapalı ydı.</span><span class="sxs-lookup"><span data-stu-id="5a40c-106">Been powered off when you issued the pause command.</span></span> <span data-ttu-id="5a40c-107">Bu durumda, aygıtlar açıkken, zamanlanmış güncelleştirmeleri iade den önce indirip yüklemiş olabilirler.</span><span class="sxs-lookup"><span data-stu-id="5a40c-107">In this case, when the devices were powered on, they might have downloaded and installed the scheduled updates prior to check-in.</span></span>