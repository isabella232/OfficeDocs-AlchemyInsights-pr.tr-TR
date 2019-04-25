---
title: 1332 - OWA gelen kutusu kuralları bir posta kutusu için yürütülen değil
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1332
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: c0b221b5335254bd0f1eb4b258efa6946376ca12
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32372580"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="3d5ac-102">Gelen kutusu kuralı beklendiği gibi çalışmıyor</span><span class="sxs-lookup"><span data-stu-id="3d5ac-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="3d5ac-103">Aşağıdaki ayarları doğrulayın:</span><span class="sxs-lookup"><span data-stu-id="3d5ac-103">Verify the following settings:</span></span>

- <span data-ttu-id="3d5ac-104">Bir ileti, iletilen veya yanıtlanan dayanarak otomatik olarak gelen kutusu kuralları üzerinde yalnızca bir kez yeniden yönlendirilebilir.</span><span class="sxs-lookup"><span data-stu-id="3d5ac-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="3d5ac-105">Bir yeniden yönlendirme kuralı (bir gelen kutusu kuralı veya posta akışı kuralı, bir aktarım kuralı olarak da bilinir) en çok on iletme alıcıların iletiye ekleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="3d5ac-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="3d5ac-106">[Günlük, taşıma ve gelen kutusu kuralı sınırlarını](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)daha fazla bilgi için bkz.</span><span class="sxs-lookup"><span data-stu-id="3d5ac-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="3d5ac-107">Gelen Kutusu kuralları diğer günlük kaydı posta kutusunun üzerinde çalışmaz.</span><span class="sxs-lookup"><span data-stu-id="3d5ac-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="3d5ac-108">[Diğer günlük kaydı posta kutusu](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)posta kutusu diğer günlük kaydı hakkında daha fazla bilgi için bkz.</span><span class="sxs-lookup"><span data-stu-id="3d5ac-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="3d5ac-109">Bu sorunları gidermek için bkz: [KB 2829319](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="3d5ac-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="3d5ac-110">Yukarıdaki sorunlar uygulamazsanız, Microsoft Support sorunu üst düzeye iletmeden önce gelen kutusu kuralı Tanılama raporunu çalıştırın:</span><span class="sxs-lookup"><span data-stu-id="3d5ac-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="3d5ac-111">Web'de Outlook'taki posta kutusunu açın ve **Ayarlar** ' ı tıklatın \> **seçenekleri** \> **Düzenle e-posta** \> **Gelen Kutusu kuralları**.</span><span class="sxs-lookup"><span data-stu-id="3d5ac-111">Open the mailbox in Outlook on the web, and click **Settings** \> **Options** \> **Organize email** \> **Inbox rules**.</span></span>

2. <span data-ttu-id="3d5ac-112">Sayfanın alt kısmında, **kurallarınızın bir tanılama raporu oluşturmak için burayı tıklatın çalışıyorsanız değil'i**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="3d5ac-112">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
