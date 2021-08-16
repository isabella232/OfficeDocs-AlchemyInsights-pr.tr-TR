---
title: Günlükler ve Raporlama
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004331"
- "7727"
ms.openlocfilehash: 03d77c17622a1aac5ecb035bb5b73efdbbfe5e6b141e6b266eef8783f612c8b2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54067032"
---
# <a name="logs-and-reporting"></a>Günlükler ve Raporlama

[Azure Active Directory hakkında SSS](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) soruları, SSS Azure Active Directory (Azure AD) raporlama hakkında sık sorulan soruların yanıtlarını verir. Daha fazla bilgi için [bkz. Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports)

**Denetim ile ilgili sorunları giderme**

1. Bazı denetim etkinliklerini görmede sorun ediyorsanız ve eksik Etkinlik bu listede yer [alıyorsa](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities)lütfen destek bileti dosyalayın.
2. Kiracınıza ilişkin Denetim günlüklerini görmede sorun ediyorsanız lütfen bir destek bileti dosya edin.
3. Denetim etkinlikleriniz Azure Portal'da hemen gösteriliyorsa, [](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) gecikme süresi belgelenmiş gecikme süresini aşarsa gecikme bilgilerimize bakın ve destek bileti olarak dosya edin.
4. [Azure AD Etkinlik Günlüklerini Bekletme](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention)
5. Seçtiğiniz tarih aralığı için tüm denetimi görmüyorsanız Azure portaldan en çok 250.000 satır (en son oturum açma bilgilerine göre sıralanmış) indirebilirsiniz. Daha fazla bilgi için [bkz. Denetim etkinlikleri indirme.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report)

**Oturum Açma ile ilgili sorunları giderme**

1. Son 30 günlük verileri, yalnızca kiracınız için bir Azure AD Premium (P1 veya P2) lisansınız varsa görebilirsiniz.
2. Oturum açma, yalnızca kiracı Azure AD Premium kullanılabilir. Ücretsiz veya Temel lisanslı kiracılarda kullanılamaz.
3. Kiracınız Premium P1 lisansına sahipse ve oturum açmaları görmüyorsanız, gecikme [](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) süresi bilgilerimize göz atın ve gecikme süresi belgelenmiş gecikme süresini aşarsa destek bileti olarak dosya edin.
4. Seçtiğiniz tarih aralığı için tüm oturum açmaları görmüyorsanız Azure portaldan en çok 250.000 satır indirebilirsiniz (en son oturum açma bilgilerine göre sıralanmış). Daha fazla bilgi için [bkz. Oturum açma etkinlikleri indirme](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities).

**Güvenlik Raporları Sorunlarını Giderme (Risk altında Bayrakla İşaretlenen Kullanıcılar, Riskli Oturum Açma)**

1. [Risk güvenliği raporu için bayrakla işaretlenmiş kullanıcılar](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-user-at-risk)
2. [Azure Active Directory portalında risky sign-ins report](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risky-sign-ins)
3. [Azure Active Directory olaylarını geri almak](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risk-events)
