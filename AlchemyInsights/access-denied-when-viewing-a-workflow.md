---
title: Iş akışını görüntülerken erişim reddedildi
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 710775e8b2dee98969df7a4c8410a3e61181aaf6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688822"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="a1664-102">Iş akışını görüntülerken erişim reddedildi</span><span class="sxs-lookup"><span data-stu-id="a1664-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="a1664-103">SharePoint grubuna e-posta göndermeyi deneyen SharePoint 2013 Iş akışları, SharePoint grubunun üyeliği herkes olarak ayarlanmamışsa "erişim reddedildi" hata iletisiyle başarısız olabilir.</span><span class="sxs-lookup"><span data-stu-id="a1664-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="a1664-104">**Bu sorunu çözmek için aşağıdaki adımları uygulayın:**</span><span class="sxs-lookup"><span data-stu-id="a1664-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="a1664-105">Herkesin SharePoint grubunun üyelerini görmesine izin verin.</span><span class="sxs-lookup"><span data-stu-id="a1664-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="a1664-106">SharePoint grubunu e-postanın Kime veya bilgi satırından kaldırın.</span><span class="sxs-lookup"><span data-stu-id="a1664-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="a1664-107">Üyelik görünürlüğü SharePoint grubu için değiştirilenemediyseniz, kime veya BILGI satırına kullanıcıları açık olarak ekleyin.</span><span class="sxs-lookup"><span data-stu-id="a1664-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="a1664-108">Daha fazla ayrıntı görüntülemek için lütfen [HTTP _vti_bin yetkisi](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409)</span><span class="sxs-lookup"><span data-stu-id="a1664-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  