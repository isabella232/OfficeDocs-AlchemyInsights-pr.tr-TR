---
title: Office uygulamaları için oturum açma sorunları
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: de0a1b78724db9a8e93d8d599ce3b503abcb86e2
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938373"
---
# <a name="fixing-the-office-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Office apps "Üzgünüm, kuruluşunuzda başka bir hesaptan zaten imzalanmış" iletisini çözme

Bu hatayı düzeltmek için aşağıdakileri deneyin:

- Windows ayarları > **erişim iş veya Okul**kullanarak etkilenen hesabı dışındaki tüm çalışma hesapları kaldırın.
- Windows kimlik bilgileri yöneticisini kullanarak [Office açık kimlik bilgileri](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) .<br/>
    **Not:** Office 2016 için kayıt defteri yolları için 16.0 değişti. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Bir Office uygulamasını açın, **Dosya** > **Hesap** > **Oturumu Kapat**. Sonra geçerli bir lisansa bir kullanıcı hesabı kullanarak oturum açın. Ayrıntılı bilgi için bkz: [Office hesapları](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Mac için bkz: [Mac app için bir Office 2016'da oturum açamıyorsunuz](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Daha fazla bilgi için bkz: ["Üzgünüm, kuruluşunuzda başka bir hesaptan zaten imzalanan bu bilgisayar üzerinde" Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).