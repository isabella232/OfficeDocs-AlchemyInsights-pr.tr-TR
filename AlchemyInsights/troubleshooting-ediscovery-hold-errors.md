---
title: eBulma içerirken oluşan hataları giderme
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52676286"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a>eBulma içerirken oluşan hataları giderme

eBulma 10 ile ilgili sorunlar mı yaşıyorsunuz? Göz önünde bulundurarak en iyi yöntemlerden bazıları:

- Tutma dağılımı durumunu kontrol edin.  Durum, Kapalı **(Beklemede) veya** **Kapalı (Beklemede)** ise, dağıtımın tamamlanması için beklemede bekleyin.
- eBulma güncelleştirmelerini her işlemde ilkeyi tekrar tekrar güncelleştirmek yerine tek bir toplu istekte birleştirin.
- Güvenlik Set-CaseHoldPolicy <policyname> Uyumluluk Merkezi Powershell'de -RetryDistribution'i çalıştırın. Ayrıntılar için güvenlik ve [Bağlan Merkezi PowerShell& e bakın.](/powershell/exchange/connect-to-scc-powershell)

Bu ayarları denetleme adımları ve eBulma tutma sorunlarını azaltmaya ve çözmeye yönelik en iyi diğer yöntemler için bkz. [eBulma tutma hatalarını giderme.](/microsoft-365/compliance/hold-distribution-errors)
Sık karşılaşılan diğer eBulma sorunlarını giderme hakkında daha fazla bilgi için bkz. Yaygın eBulma sorunlarını araştırma, giderme [ve çözme.](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)
