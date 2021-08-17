---
title: Parola eşitlemesi sorunlarını giderme
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: cb782c0d1dc396ee7a9f016afb9629a2cdee93d52f5408b7a73e576e783ebc0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105798"
---
# <a name="troubleshoot-password-synchronization"></a>Parola eşitlemesi sorunlarını giderme

Parola eşitleme sorunlarını gidermek için, bu AAD'yi kullanarak Bağlan neden parolaların eşitleneme olmadığını belirlemek için sorun giderme görevine bakın. Başlamak için Doğrudan eşitlemeyi [yönet 'e gidin.](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement)  

1. Azure AD Windows PowerShell sunucunuzda yeni bir Bağlan oturum açın ve Yönetici Olarak **Çalıştır seçeneğini** belirleyin.

2. Run Set-ExecutionPolicy RemoteSigned veya Set-ExecutionPolicy Unrestricted.

3. Azure AD Ad Bağlan başlatın.

4. Sonraki Sorun Giderme'ye > **Görevler sayfasına**  >  **gidin.**

5. PowerShell **sorun** giderme menüsünü açmak için Başlat'ı seçin.

6. Parola **Eşitlemesi Sorunlarını Gider'i seçin.**

    Sorun genellikle parolanın belirli bir kullanıcı hesabı için eşitlenmez durumdadır.

    **Notlar** Parola eşitlemenin son başarılı olması için bir süre geçtiyseniz parola eşitleme başarısız olur.

Parola eşitlemesi sorunlarını gidermek için bkz. Azure AD ile parola [karması eşitlemesi sorunlarını Bağlan.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)