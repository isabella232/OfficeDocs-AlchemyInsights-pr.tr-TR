---
title: Eksik İş Akışı Etkinleştirilemede Başarısız Oldu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 2598111005c219c398b63ca374e8e99348efc02c
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43762121"
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
  

