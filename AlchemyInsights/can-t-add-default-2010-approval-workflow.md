---
title: Varsayılan ekleyemezsiniz 2010 onay iş akışı
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2060c9a1-e714-4d93-925e-629c82c35986
ms.openlocfilehash: 758b0339b842478f9609eb716b5b4ddab6579c80
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29494215"
---
# <a name="cant-add-default-2010-approval-workflow"></a>Varsayılan ekleyemezsiniz 2010 onay iş akışı

Bir Microsoft SharePoint site koleksiyonu (örneğin, "onay - SharePoint 2010") genel olarak yeniden kullanılabilir bir iş akışı bir liste veya kitaplığa ekleyemezsiniz.
  
Bu sorunu gidermek için şu adımları izleyin: 
  
1. Kök Web sitesinin site koleksiyonunun SharePoint Designer 2013'de açın.
  
2. **Site nesneleri**altında **iş akışı**seçin. 
  
3. **İş akışları** Şerit'in **Yeni** bölümünde, **Yeniden kullanılabilir iş akışı**seçin. 
  
4. **Yeniden kullanılabilir iş akışı Oluştur** formunda, adı girin * **Repair2010***. **Platform türü**, **SharePoint 2010 iş akışını**seçin ve sonra **Tamam**' ı seçin. 
  
5. **İş akışı** Şerit **Kaydet** bölümünde **Yayımlama**seçin. 
  
6. **Genel olarak yayınlama** **iş akışı** Şerit **Yönet** bölümünde seçin. Görüntülenen onay iletişim kutusunda **Tamam**' ı seçin. 
  
7. Bir web tarayıcısında site koleksiyonunun kök Web sitesi bulun ve sonra **Site ayarlarını** erişim \> **Site koleksiyonu özellikleri**. Daha sonra **iş akışı** özelliğini Değiştir: 
  
· Özellik *etkinleştirildi* , **etkinliğini,** tıklatın ve ardından **Etkinleştir**' i tıklatın. 
  
· Bu özellik *devre dışı* ise, **Etkinleştir**' i tıklatın. 
  
Daha fazla bilgi için lütfen aşağıdaki [makaleye](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)bakın.
  

