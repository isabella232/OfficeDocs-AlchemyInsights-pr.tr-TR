---
title: Microsoft Edge 'in Microsoft Defender Application Guard desteği
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49584007"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a>Microsoft Edge 'in Microsoft Defender Application Guard desteği

Windows 10 ve Microsoft Edge için tasarlanan Application Guard, kullanıcının güvenilmeyen bir sitede, ana bilgisayar işletim sisteminden ayrılan yalıtılmış, Hyper-V etkinleştirilmiş bir kapsayıcının içinden gezinmesini sağlayan donanım yalıtımı yaklaşımı kullanır.

Kuruluş Yöneticisi güvenilen Web sitelerinin, bulut kaynaklarının ve iç ağların listesini tanımlar. Kullanıcı listede bulunmayan bir siteyi ziyaret ettiğinde, Microsoft Edge siteyi kapsayıcıda açar. Bu, site zararlı olmaya devam etmiyorsa, ana bilgisayarın korumalı kalması ve saldırganın kurumsal verilere kullanılamayacağı anlamına gelir.

Kapsayıcıdaki uzantıların yüklemesi, Microsoft Edge sürüm 81 itibariyle desteklenir ve bir ilkeyle denetlenebilir. ExtensionInstallForcelist ilkesinde kullanılan updateURL adresi, Application Guard tarafından kullanılan ağ yalıtımı ilkelerine nötr kaynak olarak eklenmelidir.

Daha fazla bilgi için [Microsoft Defender Application Guard Için Microsoft Edge desteği](https://go.microsoft.com/fwlink/?linkid=2134229)konusuna bakın.
