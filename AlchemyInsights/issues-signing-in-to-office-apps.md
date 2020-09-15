---
title: Microsoft 365 uygulamalarında oturum açma sorunları
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: 7d2cfd437bb55804c3b9263428833c10d5caaa47
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695343"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Microsoft 365 uygulamalarını düzeltme "Maalesef kuruluşunuzdaki başka bir hesap zaten oturum açmış" iletisi

Bu hatayı düzeltmek için aşağıdakileri deneyin:

- **İş veya okul**> Windows ayarlarını kullanarak, etkilenen hesap dışında tüm iş hesaplarını kaldırın.
- Windows kimlik bilgileri Yöneticisi 'Ni kullanarak [Office kimlik bilgilerini temizleyin](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) .<br/>
    **Not:** Office 2016 için kayıt defteri yolları 16,0 olarak değiştirilmiştir. (Örn: \Software\Microsoft\Office\16.0\Common\Identity\)
- Bir Office uygulamasını açın, **Dosya**  >  **hesabı**  >  **oturumu**kapat 'ı seçin. Ardından geçerli bir lisansla Kullanıcı hesabı kullanarak oturum açın. Ayrıntılı bilgi için bkz. [Office’te Hesaplar](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Mac için bkz. [Office Mac 2016 uygulamasında oturum açılamıyor](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Daha fazla bilgi için, [Office 'te "Üzgünüz, kuruluşunuzdaki başka bir hesap zaten bu bilgisayarda oturum açtı"](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)başlığına bakın.