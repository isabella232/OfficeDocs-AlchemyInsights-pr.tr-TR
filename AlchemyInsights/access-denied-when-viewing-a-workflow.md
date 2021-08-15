---
title: İş Akışı görüntülerken erişim reddedildi
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 2b076ec5dca070555ce51b88631fb6bd619ed9269e59ccc799b23b8b95547c16
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955221"
---
# <a name="access-denied-when-viewing-a-workflow"></a>İş Akışı görüntülerken erişim reddedildi

SharePoint grubuna e-posta göndermeye çalışan SharePoint 2013 İş Akışları, SharePoint grubunun üyeliği Herkes olarak ayarlanmazsa "Erişim Reddedildi" hata iletisiyle başarısız olabilir.
  
 **Bu sorunu çözmek için şu adımları izleyin:**
  
 1. Grup üyelerini herkesin görmelerine izin SharePoint.
  
 2. E SharePoint e veya Bilgi satırına gelen Kullanıcı Grubu'nda grubu kaldırın.
  
 3. Üyelik görünürlüğü bir grup için değiştirilenene kadar kullanıcıları To veya Bilgi SharePoint ekleyin.
  
Diğer ayrıntıları görüntülemek için lütfen [HTTP Yetkisiz /_vti_bin/client.svc/sp.utilities.utility.SendEmail adresine bakın.](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409)
  