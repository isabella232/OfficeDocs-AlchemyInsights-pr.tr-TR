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
ms.openlocfilehash: 900d5f250846e9a7046f72156c150f4970d91d5ad94cb7fc054952228f4bf257
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54026242"
---
# <a name="missing-emails-in-quarantine"></a>Karantinada e-postalar eksik"

Yöneticiler bu [iletileri görüntüde veya sürümde ilebilir veya silebilir.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

Güvenlik ve Uyumluluk & açmak için, [https://protection.office.com](https://protection.office.com/) gidin. Karantina sayfasını doğrudan açmak için, [https://protection.office.com/quarantine](https://protection.office.com/quarantine) gidin.  

Aşağıdaki değerlere göre arama yapabilirsiniz:  

- **İleti Kimliği:** İletinin genel benzersiz tanımlayıcısıdır. Listeden bir ileti seçersiniz,  **görüntülenen**  Ayrıntılar açılır bölmesinde  **İleti**  Kimliği değeri gösterilir. Yöneticiler, iletileri ve [karşılık gelen](/microsoft-365/security/office-365-security/message-trace-scc) İleti Kimliği değerlerini bulmak için ileti izleme kullanabilir.
- **Gönderen e-posta** adresi: Tek bir gönderenin e-posta adresi.
- **Alıcı e-posta** adresi: Tek bir alıcının e-posta adresi.
- **Konu:** İletinin konusunun tamamını kullanın. Arama büyük/harfe duyarlı değildir.

Arama ölçütlerini girdikten sonra, sonuçları filtrelemek ![ için Yenile ](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  düğmesini Yenile'yi tıklatın.

Karantinada iletileri ve dosyaları görüntülemek ve yönetmek için kullanabileceğiniz cmdlet'ler:
- [Delete-QuarantineMessage](/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](/powershell/module/exchange/preview-quarantinemessage): Bu cmdlet'in yalnızca iletilere yönelik olduğunu, SharePoint Online, OneDrive İş veya Office 365 için Microsoft Defender'dan gelen kötü amaçlı yazılım dosyalarına yönelik Teams.
- [Release-QuarantineMessage](/powershell/module/exchange/release-quarantinemessage)