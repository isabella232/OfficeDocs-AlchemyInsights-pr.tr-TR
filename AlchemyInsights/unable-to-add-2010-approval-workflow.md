---
title: 2010 onay Iş akışı eklenemiyor
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: aa61f1615b60d27cffad15f02f6ce5dbac1b607f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47699755"
---
# <a name="unable-to-add-2010-approval-workflow"></a>2010 onay Iş akışı eklenemiyor

Microsoft SharePoint site koleksiyonunda, bir liste veya kitaplığa genel olarak kullanılabilen bir iş akışı ("onay-SharePoint 2010" gibi) ekleyemezsiniz.
  
Bu sorunu çözmek için aşağıdaki adımları izleyin: 
  
1. SharePoint Designer 2013 'da site koleksiyonunun kök Web sitesini açın.
  
2. **Site nesneleri**altında, **iş akışları**'nı seçin. 
  
3. **Iş akışları** şeridinin **Yeni** bölümünde, yeniden **kullanılabilir iş akışı**'nı seçin. 
  
4. Yeniden **kullanılabilir Iş akışı oluştur** formunda * * *Repair2010* * * adını girin. **Platform türü**için **SharePoint 2010 iş akışı**'nı ve sonra **Tamam**'ı tıklatın. 
  
1. **Iş akışı** şeridinin **Kaydet** bölümünde **Yayımla**'yı seçin. 
  
2. **Iş akışı** şeridinin **Yönet** bölümünde, **genel olarak Yayımla**'yı seçin. Görüntülenen onay iletişim kutusunda **Tamam 'ı**seçin. 
  
3. Web tarayıcısında, site koleksiyonunun kök Web sitesini bulun ve **site ayarları** \> **site koleksiyonu özelliklerine**erişin. **Iş akışları** özelliğini değiştirme: 
  
· Özellik  *etkinleştirilirse*  , **devre dışı bırak** 'ı ve ardından **Etkinleştir**'i tıklatın. 
  
· Özellik  *devre dışı*  bırakılmışsa **Etkinleştir**'i tıklatın. 
  
Daha fazla bilgi için lütfen aşağıdaki [makaleye](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)bakın.
  

