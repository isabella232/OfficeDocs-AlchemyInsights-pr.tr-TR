---
title: 401 Yetkisiz hata SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10935"
- "9001435"
ms.openlocfilehash: 8935f461aaf24cb100516311203ef642f5dbed931e472df944c1cd7e72a8cf4e
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57890286"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>401 Yetkisiz hata SharePoint

Bu hatanın TLS 1.0/1.1'i kullanımdan SharePoint'de "(401) Yetkisiz" hatasını alırsanız, bu hata TLS 1.0/1'in kullanımdan kullanılmasıyla ilgili olabilir. Daha fazla bilgi için bkz:

- [Office 365 ve Office 365 GCC'de TLS 1.2'ye hazırlanma](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [İstemcinin TLS 1.2 desteği yoksa kimlik doğrulama hataları oluşur](https://docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Windows'da WinHTTP'da varsayılan güvenli protokol olarak TLS 1.1 ve TLS 1.2'yi etkinleştirmek Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Kullanıcılar 7. Windows varsa, Windows [7'de TLS Şifreleme Paketlerini Windows olun.](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)