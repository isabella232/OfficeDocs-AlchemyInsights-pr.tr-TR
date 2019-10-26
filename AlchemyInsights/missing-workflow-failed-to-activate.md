---
title: Eksik İş Akışı Etkinleştirilemede Başarısız Oldu
ms.author: pebaum
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: f03d7e1441465050c4b0608f4100f217b183d2e2
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/25/2019
ms.locfileid: "36753816"
---
# <a name="missing-workflow-failed-to-activate"></a>Eksik İş Akışı Etkinleştirilemede Başarısız Oldu

Microsoft SharePoint site koleksiyonunda, bir listeye veya kitaplıka genel olarak yeniden kullanılabilir bir iş akışı ("Onay - SharePoint 2010" gibi) ekemezsiniz.
  
Bu sorunu gidermek için aşağıdaki adımları izleyin: 
  
1. SharePoint Designer 2013'te site koleksiyonunun kök web sitesini açın.
  
2. **Site Nesneleri** **altında, İş Akışları'nı**seçin. 
  
3. **İş Akışları** şeridinin **Yeni** bölümünde, Yeniden Kullanılabilir **İş Akışı'nı**seçin. 
  
4. Yeniden **Kullanılabilir İş Akışı Oluştur** formuna ** *Repair2010* **adını girin. **Platform Türü**için **SharePoint 2010 İş Akışı'nı**tıklatın ve ardından **Tamam'ı**tıklatın. 
  
1. **İş Akışı** şeridinin **Kaydet** bölümünde **Yayımla'yı**seçin. 
  
2. **İş Akışı** şeridinin **Yönet** bölümünde, Genel **Olarak Yayımla'yı**seçin. Görünen onay iletişim kutusunda **Tamam'ı**seçin. 
  
3. Bir web tarayıcısında, site koleksiyonunun kök web sitesini bulun ve **ardından Site Ayarları** \> **Site Toplama Özelliklerine**erişin. Ardından, İş **Akışları** özelliğini geçişe: 
  
· Özellik *Etkinleştirildiyse,* **Devre Dışı bırak'ı** tıklatın ve sonra **Etkinleştir'i**tıklatın. 
  
· Özellik Devre *Dışı* bırakılırsa, **Etkinleştir'i**tıklatın. 
  
Daha fazla bilgi için lütfen aşağıdaki [makaleye](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)bakın.
  

