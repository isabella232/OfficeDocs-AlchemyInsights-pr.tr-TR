---
title: Karantinada eksik e-postalar
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569563"
---
# <a name="missing-emails-in-quarantine"></a>Karantinada eksik e-postalar"

Yöneticiler [bu iletileri görüntüleyebilir, yayınlayabilir veya silebilir.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Güvenlik & Uyumluluk Merkezi'ni açmak [https://protection.office.com](https://protection.office.com/) için. Karantina sayfasını doğrudan açmak [https://protection.office.com/quarantine](https://protection.office.com/quarantine) için.  

Aşağıdaki değerlere göre arama yapabilirsiniz:  

- **İleti Kimliği**: İletinin genel olarak benzersiz tanımlayıcısı. Listede bir ileti seçerseniz, **İleti Kimliği** değeri görünen **Ayrıntılar** uçuş bölmesinde görünür. Yöneticiler iletileri ve karşılık gelen İleti Kimliği değerlerini bulmak için [ileti izleme](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) sini kullanabilir.
- **Gönderen e-posta adresi**: Tek bir gönderenin e-posta adresi.
- **Alıcı nın e-posta adresi**: Tek bir alıcının e-posta adresi.
- **Konu**: İletinin tüm konusunu kullanın. Arama büyük/küçük harf duyarlı değildir.

Arama ölçütlerini girdikten ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) sonra, sonuçları filtrelemek için**Yenile** düğmesini tıklatın.  

İletileri ve dosyaları karantinada görüntülemek ve yönetmek için kullandığınız cmdletler şunlardır:
- [Sil-KarantinaMesajı](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Dışa Aktarma-KarantinaMesajı](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-KarantinaMesajı](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Önizleme-Karantina Mesajı](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Bu cmdlet'in SharePoint Online, OneDrive for Business veya Teams için ATP'den gelen kötü amaçlı yazılım dosyaları için değil, yalnızca mesajlar için olduğunu unutmayın.
- [Yayın-KarantinaMesajı](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)