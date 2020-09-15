---
title: Karantinadaki e-postalar eksik
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673734"
---
# <a name="missing-emails-in-quarantine"></a>Karantinadaki e-postalar eksik "

Yöneticiler [Bu iletileri görüntüleyebilir, serbest bırakabilir veya silebilir.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Güvenlik & Uyumluluk Merkezi 'ni açmak için gidin [https://protection.office.com](https://protection.office.com/) . Karantina sayfasını doğrudan açmak için öğesine gidin [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Aşağıdaki değerlerle arama yapabilirsiniz:  

- **ILETI kimliği**: iletinin genel benzersiz tanımlayıcısı. Listeden bir ileti seçerseniz, görüntülenen **Ayrıntılar** açılır BÖLMESINDE **ileti kimliği** değeri görünür. Yöneticiler ileti [izlemeyi](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) kullanarak iletileri ve ılgılı ileti kimliği değerlerini bulabilir.
- **Gönderenin e-posta adresi**: tek bir gönderenin e-posta adresi.
- **Alıcının e-posta adresi**: tek bir alıcının e-posta adresi.
- **Konu**: iletinin tüm konusunu kullanın. Arama büyük/küçük harf duyarlı değildir.

Arama ölçütlerini girdikten sonra, ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) sonuçları filtrelemek için Yenile düğmesini**Yenile** 'yi tıklatın.  

İletileri ve karantinadaki dosyaları görüntülemek ve yönetmesi için kullandığınız cmdlet 'ler:
- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Dışarı aktarma-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Önizleme-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Bu cmdlet 'in yalnızca iletiler için olduğunu, SharePoint Online, OneDrive Iş veya ekiplerin ATP 'den kötü amaçlı yazılım dosyaları olmadığını unutmayın.
- [Sürüm karantinaya alır](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)