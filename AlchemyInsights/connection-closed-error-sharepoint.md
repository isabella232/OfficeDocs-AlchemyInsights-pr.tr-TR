---
title: Bağlantının temel alınan kapalı SharePoint
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10802"
- "9006390"
ms.openlocfilehash: 1b4f336f389eb6fd81ac2ca40e6047184cc4c1bf
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317716"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a>Hatada "Temel bağlantı kapatıldı" SharePoint

2013'te "Temel bağlantı kapatıldı" hatasını alıyorsanız SharePoint BU, TLS 1.0/1.1'in kullanım dışı olmasıyla ilgili olabilir. Daha fazla bilgi için şu makalelere bakın:

- [Office 365 ve Office 365 GCC'de TLS 1.2'ye hazırlanma](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [İstemcinin TLS 1.2 desteği yoksa kimlik doğrulama hataları oluşur](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Windows'da WinHTTP'da varsayılan güvenli protokol olarak TLS 1.1 ve TLS 1.2'yi etkinleştirmek Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Kullanıcılar 7. Windows varsa, [7.](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)ve 7. Windows TLS Şifreleme Paketlerini Windows olun.