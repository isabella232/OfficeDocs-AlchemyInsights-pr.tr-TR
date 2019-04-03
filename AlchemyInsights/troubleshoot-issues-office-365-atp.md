---
title: İle Office 365 Gelişmiş tehdit Koruması (ATP) sorunlarını giderme
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: dbdfe2ddcc4afd4477f66ffd060ddb7093af8fd6
ms.sourcegitcommit: 601aec31e6556286fe5e0fd62827a037cbb6fe17
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/02/2019
ms.locfileid: "31031128"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a>Office 365 KM ile ilgili sorunları giderme

- **E-posta ileti teslimi ile bildirim gecikmeleri**? ATP güvenli ekler ilkelerinizi dinamik teslim seçeneğini kullanmayı deneyin. Kötü amaçlı dosyaları alıcılar korurken bu e-posta iletisi teslim gecikmelerini önler.
- **Yanlış pozitif durumlar rapor ya da yanlış negatifler istiyor musunuz**? Dosyanızı analiz için göndermek için bu bağlantıyı kullanın:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)
- **Kuruluşunuzdaki kişiler arasında gönderilen e-posta için güvenli bağlantılar ATP koruma etkinleştirmek biliyor muydunuz**? İzleyeceğiniz adımlar:
    1. Git https://protection.office.comve oturum açın.
    2. **Tehdit Yönetimi**Git > **ilke** > **Güvenli bağlantılar**.
    3. **Belirli alıcılar için geçerli ilkeleri**altında Düzenle (veya ekleyin) bir ilke.
    4. **Kuruluş içinde gönderilen iletilere uygula güvenli bağlantıları**seçin.
    5. İlkeniz kaydedin ve yaklaşık 30 dakika boyunca yaptığınız değişiklikler, datacenter üzerinden kendi şekilde çalışmanıza olanak sağlar.
- ATP ile ilgili daha fazla yardım almak için bkz: [Office 365 Gelişmiş tehdit koruması](https://docs.microsoft.com/office365/securitycompliance/office-365-atp).