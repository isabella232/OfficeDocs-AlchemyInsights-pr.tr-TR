---
title: AAD Connect Health ile ilgili sorun
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
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50483123"
---
# <a name="problem-with-aad-connect-health"></a>AAD Connect Health ile ilgili sorun

- İşlem gerçekleştirmek için yetkiniz olduğundan emin olmak. Genel Yöneticilerin varsayılan olarak erişimi vardır. Buna ek olarak, Rol Tabanlı [Erişim Denetimi'i kullanarak Katılımcıya](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) kayıt iznini temsilci olarak devredebilirsiniz.
- Gerekli uç noktaların etkinleştirildiğinden ve güvenlik duvarı nedeniyle engellenmiş olduğundan emin olun. Ayrıntılar için gereksinimlere [bakın.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)
- Giden iletişim ağ katmanı tarafından SSL incelemesine tabi olduğu için kayıt başarısız olabilir.
- Azure AD Connect Health için bildirim ayarlarını doğruladıktan emin olun. Lütfen ayarınızı gözden geçirin. Bu [kılavuz,](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) Azure AD Connect durum bildirimleri için bildirim ayarlarını yapılandırmayı anlamanıza yardımcı olabilir.
- AAD Connect Durum eşitleme raporu ve nasıl indirildi hakkında daha fazla bilgi edinmek için, Nesne düzeyi [eşitleme raporuna bakın.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)

AAD Connect Health uyarılarının sorunlarını gidermek [için, AAD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) Health veri tazeliği uyarıları için sorun giderme kılavuzunu izleyin ve sık sorulan sorular için Genel AAD Connect Health yükleme [sorularına bakın.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)
