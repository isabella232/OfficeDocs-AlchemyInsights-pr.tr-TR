---
title: 2010 Onay İş Akışı eklenemiyor
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: f40716dd399fe7bea1b606cd725676268dc0a66d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582867"
---
# <a name="unable-to-add-2010-approval-workflow"></a>2010 Onay İş Akışı eklenemiyor

Microsoft SharePoint site koleksiyonunda, bir listeye veya kitaplıka genel olarak yeniden kullanılabilir bir iş akışı ("Onay - SharePoint 2010" gibi) ekemezsiniz.
  
Bu sorunu gidermek için aşağıdaki adımları izleyin: 
  
1. SharePoint Designer 2013'te site koleksiyonunun kök web sitesini açın.
  
2. **Site Nesneleri** **altında, İş Akışları'nı**seçin. 
  
3. **İş Akışları** şeridinin **Yeni** bölümünde, Yeniden Kullanılabilir **İş Akışı'nı**seçin. 
  
4. Yeniden **Kullanılabilir İş Akışı Oluştur** formuna ** *Repair2010* **adını girin. **Platform Türü**için **SharePoint 2010 İş Akışı'nı**tıklatın ve ardından **Tamam'ı**tıklatın. 
  
1. **İş Akışı** şeridinin **Kaydet** bölümünde **Yayımla'yı**seçin. 
  
2. **İş Akışı** şeridinin **Yönet** bölümünde, Genel **Olarak Yayımla'yı**seçin. Görünen onay iletişim kutusunda **Tamam'ı**seçin. 
  
3. Bir web tarayıcısında, site koleksiyonunun kök web sitesini bulun ve **ardından Site Ayarları** Site Toplama Özelliklerine erişin. \> **Site Collection Features** **İş Akışları** özelliğini geçişe: 
  
· Özellik *Etkinleştirildiyse,* **Devre Dışı bırak'ı** tıklatın ve sonra **Etkinleştir'i**tıklatın. 
  
· Özellik Devre *Dışı* bırakılırsa, **Etkinleştir'i**tıklatın. 
  
Daha fazla bilgi için lütfen aşağıdaki [makaleye](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)bakın.
  

