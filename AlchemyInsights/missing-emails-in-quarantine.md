---
title: Karantinada e-postalar eksik
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 43f9a1f03084bf9adab706b3f77eff1d1db888ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831754"
---
# <a name="missing-emails-in-quarantine"></a>Karantinada e-postalar eksik"

Yöneticiler bu [iletileri görüntüde veya sürümde ilebilir veya silebilir.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Güvenlik ve Uyumluluk & açmak için, [https://protection.office.com](https://protection.office.com/) gidin. Karantina sayfasını doğrudan açmak için, [https://protection.office.com/quarantine](https://protection.office.com/quarantine) gidin.  

Aşağıdaki değerlere göre arama yapabilirsiniz:  

- **İleti Kimliği:** İletinin genel benzersiz tanımlayıcısıdır. Listeden bir ileti seçersiniz,  **görüntülenen**  Ayrıntılar açılır bölmesinde  **İleti**  Kimliği değeri gösterilir. Yöneticiler, iletileri ve [karşılık gelen](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) İleti Kimliği değerlerini bulmak için ileti izleme kullanabilir.
- **Gönderen e-posta** adresi: Tek bir gönderenin e-posta adresi.
- **Alıcı e-posta** adresi: Tek bir alıcının e-posta adresi.
- **Konu:** İletinin konusunun tamamını kullanın. Arama büyük/harfe duyarlı değildir.

Arama ölçütlerini girdikten sonra, sonuçları filtrelemek ![ için Yenile ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  düğmesini Yenile'yi tıklatın.  

Karantinada iletileri ve dosyaları görüntülemek ve yönetmek için kullanabileceğiniz cmdlet'ler:
- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Bu cmdlet'in yalnızca iletilere yönelik olduğunu unutmayın; SharePoint Online, OneDrive İş veya Teams için ATP'den gelen kötü amaçlı yazılım dosyaları için değildir.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)