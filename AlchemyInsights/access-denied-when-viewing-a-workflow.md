---
title: İş Akışını görüntülerken erişim engellendi
ms.author: pebaum
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 4ca65583fbd98867026e9e3cc8f36fe38798aa85
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/15/2019
ms.locfileid: "36747768"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="3bf4e-102">İş Akışını görüntülerken erişim engellendi</span><span class="sxs-lookup"><span data-stu-id="3bf4e-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="3bf4e-103">SharePoint grubuna e-posta göndermeye çalışan SharePoint 2013 SharePoint grubunun üyeliği Herkes olarak ayarlanmazsa "Erişim Reddedildi" hata iletisiyle başarısız olabilir.</span><span class="sxs-lookup"><span data-stu-id="3bf4e-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="3bf4e-104">**Bu sorunu gidermek için şu adımları yapın:**</span><span class="sxs-lookup"><span data-stu-id="3bf4e-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="3bf4e-105">Herkesin SharePoint grubunun üyelerini görmesine izin verin.</span><span class="sxs-lookup"><span data-stu-id="3bf4e-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="3bf4e-106">E-postanın To veya CC satırından SharePoint grubunu kaldırın.</span><span class="sxs-lookup"><span data-stu-id="3bf4e-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="3bf4e-107">SharePoint grubu için üyelik görünürlüğü değiştirilemiyorsa, kullanıcıları Açıkça To veya CC satırına ekleyin.</span><span class="sxs-lookup"><span data-stu-id="3bf4e-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="3bf4e-108">Daha fazla bilgi için lütfen [http yetkisiz /_vti_bin/client.svc/sp.utilities.utility.SendEmail adresine](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409)bakın.</span><span class="sxs-lookup"><span data-stu-id="3bf4e-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  