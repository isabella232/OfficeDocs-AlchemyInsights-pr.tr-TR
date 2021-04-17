---
title: Microsoft 365 uygulamalarına oturum açma sorunları
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: 8065a49c42953013ccfae9c5c1714d10ee0b4d49
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833095"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Microsoft 365 uygulamalarını düzeltme "Üzgünüz, kuruluşun başka bir hesabı zaten oturum açık" iletisi

Bu hatayı düzeltmek için aşağıdakileri deneyin:

- Etkilenen hesap hariç tüm iş hesaplarını, Windows Ayarları'> **Access iş veya okul hesabı ile kaldırın.**
- Windows [Kimlik Bilgileri Yöneticisi'ni](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) kullanarak Office kimlik bilgilerini temizleme.<br/>
    **Not:** Office 2016'nın kayıt defteri yolları 16.0 olarak değişti. (Örneğin: \Software\Microsoft\Office\16.0\Common\Identity\)
- Bir Office uygulamasını açın, Dosya **Hesabı Oturum**  >  **Açma'yi**  >  **seçin.** Ardından, geçerli bir lisansa sahip bir kullanıcı hesabı kullanarak oturum açın. Ayrıntılı bilgi için bkz. [Office’te Hesaplar](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Mac için bkz. [Office Mac 2016 uygulamasında oturum açılamıyor](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Daha fazla bilgi için [Office'te "Üzgünüz,](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)bu bilgisayarda kuruluştan başka bir hesap oturum alandı" bilgilerine bakın.