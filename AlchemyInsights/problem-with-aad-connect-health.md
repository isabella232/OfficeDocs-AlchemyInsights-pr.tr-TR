---
title: AAD Bağlan Health ile ilgili sorun
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004649"
- "8427"
ms.openlocfilehash: 82cfcc6132549b52278b174fce3173f5566268864a207882a4dd639cb8024ee3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923772"
---
# <a name="problem-with-aad-connect-health"></a>AAD Bağlan Health ile ilgili sorun

- İşlemleri gerçekleştirme yetkiniz olduğundan emin olmak. Genel Yöneticilerin varsayılan olarak erişimi vardır. Ayrıca, Katılımcıya kayıt [izni temsilci olarak rol](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) tabanlı erişim denetimi de kullanabilirsiniz.
- Gerekli uç noktaların etkinleştirildiğinden ve güvenlik duvarı nedeniyle engellenmildiğinden emin olun. Ayrıntılar için gereksinimlere [bakın.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)
- Kayıt, ağ katmanı tarafından SSL incelemesine tabi olan giden iletişim nedeniyle başarısız olabilir.
- Azure AD veya Azure AD için bildirim ayarlarını doğruladıktan emin Bağlan olun. Lütfen ayarınızı gözden geçirin. Bu [kılavuz,](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) Azure AD veya Azure AD için bildirim ayarlarını ve durum bildirimlerini Bağlan yardımcı olabilir.
- AAD Eşitleme raporunu oluşturma ve Bağlan hakkında daha fazla bilgi edinmek için, bkz. [Nesne düzeyi eşitleme raporu](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).

AAD Bağlan durum uyarılarını gidermek için [AAD Bağlan](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) Durum verisi freshness uyarıları için sorun giderme kılavuzunu izleyin ve sık sorulan sorular için bkz. Genel [AAD Bağlan Durum yükleme soruları.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)
