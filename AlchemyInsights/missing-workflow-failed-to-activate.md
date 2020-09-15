---
title: Eksik Iş akışı etkinleştirilemedi
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 604dc770c5c14ded6a8de1cec9e311b03b69f094
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667106"
---
# <a name="missing-workflow-failed-to-activate"></a>Eksik Iş akışı etkinleştirilemedi

Microsoft SharePoint site koleksiyonunda, bir liste veya kitaplığa genel olarak kullanılabilen bir iş akışı ("onay-SharePoint 2010" gibi) ekleyemezsiniz.
  
Bu sorunu çözmek için aşağıdaki adımları izleyin: 
  
1. SharePoint Designer 2013 'da site koleksiyonunun kök Web sitesini açın.
  
2. **Site nesneleri**altında, **iş akışları**'nı seçin. 
  
3. **Iş akışları** şeridinin **Yeni** bölümünde, yeniden **kullanılabilir iş akışı**'nı seçin. 
  
4. Yeniden **kullanılabilir Iş akışı oluştur** formunda * * *Repair2010* * * adını girin. **Platform türü**için **SharePoint 2010 iş akışı**'nı ve sonra **Tamam**'ı tıklatın. 
  
1. **Iş akışı** şeridinin **Kaydet** bölümünde **Yayımla**'yı seçin. 
  
2. **Iş akışı** şeridinin **Yönet** bölümünde, **genel olarak Yayımla**'yı seçin. Görüntülenen onay iletişim kutusunda **Tamam 'ı**seçin. 
  
3. Web tarayıcısında, site koleksiyonunun kök Web sitesini bulun ve **site ayarları** \> **site koleksiyonu özelliklerine**erişin. Ardından, **Iş akışları** özelliğini değiştirin: 
  
· Özellik  *etkinleştirilirse*  , **devre dışı bırak** 'ı ve ardından **Etkinleştir**'i tıklatın. 
  
· Özellik  *devre dışı*  bırakılmışsa **Etkinleştir**'i tıklatın. 
  
Daha fazla bilgi için lütfen aşağıdaki [makaleye](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)bakın.
  

