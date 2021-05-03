---
title: 7 makinede SharePoint Windows sorunları
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9006484"
- "11070"
ms.openlocfilehash: 787f0e713cc95b590bc494868d5098a25131ac56
ms.sourcegitcommit: d33ab8c73d8af51da782094fb8f8abf7626f4df3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52125521"
---
# <a name="issues-with-sharepoint-on-windows-7-machines"></a>7 makinede SharePoint Windows sorunları

SharePoint veya OneDrive üzerinde çalışırken Windows 7 makinede hata alırsanız, bunlar TLS 1.0/1.1'in kullanımdan kullanım dışı olmasıyla ilgili olabilir. Daha fazla bilgi için bkz.:

- [Office 365 ve Office 365 GCC'de TLS 1.2'ye hazırlanma](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- Windows 7 SP1/Windows 8 istemcilerinin TLS1.2'yi etkinleştirilmiş olması gerekir. Daha fazla bilgi için [bkz. İstemcinin TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support) desteğine sahip olmayan kimlik doğrulama hataları oluşuyor

- KB3140245 yükleyin ve kayıt defteri değerini oluşturun. Daha fazla bilgi için bkz. Windows'da WinHTTP'da varsayılan güvenli protokol olarak [TLS 1.1 ve TLS 1.2'yi](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392) etkinleştirmek için Windows

- Windows 7 SP1/Windows 8 istemcilerinin en son TLS şifreleme paketlerinin yüklü olduğundan emin olması gerekir. Daha fazla bilgi için [bkz. Microsoft Güvenlik Danışmanlığı 3042058.](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058) 


