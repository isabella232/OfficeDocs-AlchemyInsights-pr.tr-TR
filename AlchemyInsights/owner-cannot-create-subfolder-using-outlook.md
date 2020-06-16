---
title: Sahibi Outlook kullanarak alt klasör oluşturamaz
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 2116bb837e4378ea29d7882df1d3010b3a4e0b1c
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/12/2020
ms.locfileid: "44749236"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Sahibi Outlook kullanarak alt klasör oluşturamaz

**Outlook'u kullanarak alt klasörler oluşturan ortak klasör sahiplerinin devam eden bir sorunu var. Sorun yakında giderilecektir.**

Bu arada, aşağıdaki geçici çözümlerden birini kullanın:

1. Sorun yalnızca masaüstü pencereleri için Outlook'u etkilediğiiçin alt klasörü oluşturmak için MAC için Outlook'u kullanın (tüm sürümler)
2. Yöneticiexo Shell veya EAC kullanarak alt klasörü oluşturma
3. Kullanıcıdaki VarsayılanKamuKlasörPosta Kutusu/EfektifKamuFolderMailbox'ı, soruna neden olan klasör için İçerik Posta Kutusu'ndan başka bir posta kutusuna değiştirme  
    - *Set-Posta Kutusu Kullanıcı1 VarsayılanKamuKlasörPosta Kutusu PubMBX3*
4. Bir saat bekleyin, outlook istemcisini yeniden başlatın