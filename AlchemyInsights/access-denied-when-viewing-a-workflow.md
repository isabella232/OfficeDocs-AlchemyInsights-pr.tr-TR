---
title: Bir iş akışı görüntülerken erişim engellendi
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: cced887b03876eef527e0166a5a3c9be4b553029
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29494644"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="d952f-102">Bir iş akışı görüntülerken erişim engellendi</span><span class="sxs-lookup"><span data-stu-id="d952f-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="d952f-103">SharePoint grubu üyeliğini herkese ayarlanmamışsa SharePoint 2013 SharePoint grubuna bir e-posta göndermeye iş akışları bir "Erişim reddedildi" hata iletisiyle başarısız olabilir.</span><span class="sxs-lookup"><span data-stu-id="d952f-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="d952f-104">**Bu sorunu gidermek için şu adımları uygulayın:**</span><span class="sxs-lookup"><span data-stu-id="d952f-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="d952f-105">Herkes SharePoint grubunun üyelerini görmek izin verir.</span><span class="sxs-lookup"><span data-stu-id="d952f-105">Allow everybody to see the members of the SharePoint group.</span></span> 
  
 2. <span data-ttu-id="d952f-106">SharePoint grubunu kaldırmak Kime veya bilgi satırındaki e-posta.</span><span class="sxs-lookup"><span data-stu-id="d952f-106">Remove the SharePoint group from the To or CC line of the email.</span></span> 
  
 3. <span data-ttu-id="d952f-107">Kime veya bilgi Kullanıcıları açıkça eklemek için SharePoint grup üyeliği görünürlüğü değiştirilemez, satır.</span><span class="sxs-lookup"><span data-stu-id="d952f-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span> 
  
<span data-ttu-id="d952f-108">Görüntülemek için daha fazla ayrıntı lütfen [/_vti_bin/client.svc/sp.utilities.utility.SendEmail yetkisiz HTTP ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409)için başvurun.</span><span class="sxs-lookup"><span data-stu-id="d952f-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  

