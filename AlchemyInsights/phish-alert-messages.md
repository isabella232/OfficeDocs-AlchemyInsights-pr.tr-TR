---
title: 2491 'Kimlik Avı Kiracı veya kullanıcı geçersiz kılma nedeniyle teslim edildi' ilkesinden gelen e-posta iletilerini uyarı
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 90b078147bbb1e60cba0a2de6e49a862469f93aa
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316378"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>'Kimlik Avı Kiracı veya kullanıcı geçersiz kılma nedeniyle teslim edildi' ilkesinden gelen e-posta iletilerini uyarı

Kiracı veya kullanıcı  geçersiz kılma nedeniyle Kimlik Avı Teslim Edildi adlı varsayılan bir uyarı ilkesi, Office 365 P1 ve P2 lisansları için Microsoft Defender'a sahip kuruluşlarda kullanılabilir. Bu uyarıyı aldıysanız, şu adımları araştırabilirsiniz:

1. Uyarı iletisinde, **Uyarıyı Görüntüle'ye** **tıklar ve** portalda Uyarılar Microsoft 365 Defender gidin.

2. İleti listesini görüntüleme veya İletileri **Explorer'da görüntüleme seçeneğini** **görmek için uyarıyı seçin.** Bu seçeneklerin her ikisi de sizi İleti Kimliğini içeren iletinin ayrıntılarına götürmektedir. Tehdit Gezgini bağlantısı, uyarı ölçütlerine uyan iletileri otomatik olarak filtrelemektedir. Threat Explorer'da tarih filtresini ayarlamanız gerekiyor olabilir.

Kimlik avı iletisi elle yapılandırılan geçersiz kılma nedeniyle teslim edildi:

- Kullanıcı tarafından ayarlanmış izin verilen bir gönderen veya etki alanı.
- İstenmeyen posta önleme ilkesinde yönetici tarafından ayarlanmış, izin verilen bir gönderen veya etki alanı.
- Bağlantı filtresi ilkesinde izin verilen IP adresi.
- İletilere izin verecek şekilde yapılandırılmış bir posta akışı kuralı (aktarım kuralı olarak da bilinir).

İletinin yanlışlıkla kimlik avı olarak işaret olmadığını inanıyorsanız, iletiyi Microsoft'a [bildirmesi](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission) için Yönetici gönderimi'ni kullanın.

Kullanıcılar, [Microsoft'a](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) ileti örnekleri göndermek için Rapor İletisi eklentisinde veya Rapor Kimlik Outlook eklentisinde kullanılabilir.
