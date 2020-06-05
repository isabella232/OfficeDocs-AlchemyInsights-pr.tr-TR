---
title: Microsoft 365 uygulamalarında oturum açma sorunları
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
ms.openlocfilehash: e4f2fea5c2f368ae240614ee1f7bc729338dd75d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579957"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Microsoft 365 uygulamalarını düzeltme "Üzgünüz, kuruluşunuzdaki başka bir hesap zaten oturum açmış durumda" iletisi

Bu hatayı düzeltmek için aşağıdakileri deneyin:

- Windows Ayarları > **Access çalışmasını veya okul'u**kullanarak etkilenen hesap dışındaki tüm iş hesaplarını kaldırın.
- Windows Kimlik Bilgileri Yöneticisi'ni kullanarak [Office kimlik bilgilerini temizleyin.](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)<br/>
    **Not:** Office 2016'nın kayıt defteri yolları 16.0 olarak değiştirildi. (Ör. \Software\Microsoft\Office\16.0\Common\Identity\)
- Office uygulaması açın, **File**  >  **Dosya Hesabı**Oturum  >  **Aç'ı**seçin. Ardından geçerli bir lisansa sahip bir kullanıcı hesabı kullanarak oturum açın. Ayrıntılı bilgi için bkz. [Office’te Hesaplar](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Mac için bkz. [Office Mac 2016 uygulamasında oturum açılamıyor](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Daha fazla bilgi için [Bkz. "Üzgünüz, kuruluşunuzdan başka bir hesap zaten bu bilgisayarda oturum açmış" Office'te.](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)