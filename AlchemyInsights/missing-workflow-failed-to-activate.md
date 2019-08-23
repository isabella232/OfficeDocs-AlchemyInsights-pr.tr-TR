---
title: İş akışı eksik etkinleştirilemedi
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 44fd3c2d1e8b278b47c0fde6d48c7cbcbaa5c324
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36543945"
---
# <a name="missing-workflow-failed-to-activate"></a>İş akışı eksik etkinleştirilemedi

Bir Microsoft SharePoint site koleksiyonu (örneğin, "onay - SharePoint 2010") genel olarak yeniden kullanılabilir bir iş akışı bir liste veya kitaplığa ekleyemezsiniz.
  
Bu sorunu gidermek için şu adımları izleyin: 
  
1. Kök Web sitesinin site koleksiyonunun SharePoint Designer 2013'de açın.
  
2. **Site nesneleri**altında **iş akışı**seçin. 
  
3. **İş akışları** Şerit'in **Yeni** bölümünde, **Yeniden kullanılabilir iş akışı**seçin. 
  
4. **Yeniden kullanılabilir iş akışı Oluştur** formunda, adı girin ** *Repair2010* **. **Platform türü**, **SharePoint 2010 iş akışı**' nı tıklatın ve sonra **Tamam**' ı tıklatın. 
  
1. **İş akışı** Şerit **Kaydet** bölümünde **Yayımlama**seçin. 
  
2. **Genel olarak yayınlama** **iş akışı** Şerit **Yönet** bölümünde seçin. Görüntülenen onay iletişim kutusunda **Tamam**' ı seçin. 
  
3. Bir web tarayıcısında site koleksiyonunun kök Web sitesi bulun ve sonra **Site ayarlarını** erişim \> **Site koleksiyonu özellikleri**. Daha sonra **iş akışı** özelliğini Değiştir: 
  
· Özellik *etkinleştirildi* , **etkinliğini,** tıklatın ve ardından **Etkinleştir**' i tıklatın. 
  
· Bu özellik *devre dışı* ise, **Etkinleştir**' i tıklatın. 
  
Daha fazla bilgi için lütfen aşağıdaki [makaleye](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)bakın.
  

