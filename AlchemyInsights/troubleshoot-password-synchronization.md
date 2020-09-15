---
title: Parola eşitleme sorunlarını giderme
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
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664946"
---
# <a name="troubleshoot-password-synchronization"></a>Parola eşitleme sorunlarını giderme

Parola eşitleme sorunlarını gidermek için, bu AAD Connect sorun giderme görevini kullanarak parolaların neden eşitlenmediğine karar verin. Başlamak için [doğrudan Eşitlemeyi Yönet](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement)'e gidin.  

1. Azure AD Connect sunucunuzda yeni bir Windows PowerShell oturumu açın ve **yönetici olarak farklı** aç seçeneğini belirtin.

2. Set-ExecutionPolicy RemoteSigned veya set-ExecutionPolicy kısıtlanmaz.

3. Azure AD Connect Sihirbazı 'nı başlatın.

4. Sonraki görevler sayfasına **gidin >**  >  **sonraki**görevler sayfasına gidin.

5. PowerShell sorun giderme menüsünü açmak için **Başlat** 'ı seçin.

6. **Parola eşitleme sorunlarını giderme**'yi seçin.

    Bu sorun genellikle parolanın belirli bir kullanıcı hesabı için eşitlenmemesidir.

    **Notları** Son başarılı parola eşitleme işlemi biraz önce olmuşsa parola eşitlemesi başarısız olur.

Parola eşitleme sorunlarını gidermek için, [Azure AD Connect eşitlemesi ile parola karması eşitlemesi sorunlarını giderme](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)konusuna bakın.