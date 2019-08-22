---
title: Bir iş akışı görüntülerken erişim engellendi
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 53bd9285e49e220f880eea21923f261302003127
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36495843"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="60c26-102">Bir iş akışı görüntülerken erişim engellendi</span><span class="sxs-lookup"><span data-stu-id="60c26-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="60c26-103">SharePoint grubu üyeliğini herkese ayarlanmamışsa SharePoint 2013 SharePoint grubuna bir e-posta göndermeye iş akışları bir "Erişim reddedildi" hata iletisiyle başarısız olabilir.</span><span class="sxs-lookup"><span data-stu-id="60c26-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="60c26-104">**Bu sorunu gidermek için şu adımları uygulayın:**</span><span class="sxs-lookup"><span data-stu-id="60c26-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="60c26-105">Herkes SharePoint grubunun üyelerini görmek izin verir.</span><span class="sxs-lookup"><span data-stu-id="60c26-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="60c26-106">SharePoint grubunu kaldırmak Kime veya bilgi satırındaki e-posta.</span><span class="sxs-lookup"><span data-stu-id="60c26-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="60c26-107">Kime veya bilgi Kullanıcıları açıkça eklemek için SharePoint grup üyeliği görünürlüğü değiştirilemez, satır.</span><span class="sxs-lookup"><span data-stu-id="60c26-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="60c26-108">Görüntülemek için daha fazla ayrıntı lütfen [/_vti_bin/client.svc/sp.utilities.utility.SendEmail yetkisiz HTTP](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409)için başvurun.</span><span class="sxs-lookup"><span data-stu-id="60c26-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  