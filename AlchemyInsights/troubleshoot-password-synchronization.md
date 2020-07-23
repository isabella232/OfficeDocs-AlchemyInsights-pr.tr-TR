---
title: Parola eşitlemesi sorun giderme
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387897"
---
# <a name="troubleshoot-password-synchronization"></a>Parola eşitlemesi sorun giderme

Parola eşitleme sorunlarını gidermek için, parolaların neden eşitlenmediğini belirlemek için bu AAD Connect sorun giderme görevini kullanarak başlayın. Başlamak için [doğrudan eşitle'yi yönet'e](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement)gidin.  

1. Azure AD Connect sunucunuzda yeni bir Windows PowerShell oturumu açın ve **Yönetici olarak Çalıştır** seçeneğini belirleyin.

2. Set-ExecutionPolicy RemoteSigned veya Set-ExecutionPolicy Sınırsız çalıştırın.

3. Azure AD Bağlantısı sihirbazını başlatın.

4. Sonraki Sorun **Giderme**> Ek Görevler sayfasına  >  **Next**gidin.

5. PowerShell sorun giderme menüsünü açmak için **Başlat'ı** seçin.

6. **Sorun Giderme Parola Eşitleme'yi**seçin.

    Sorun genellikle bir parolabelirli bir kullanıcı hesabı için senkronize değildir.

    **Notlar** Son başarılı parola eşitleme bir süre önce yse parola eşitleme başarısız olur.

Parola eşitleme sorununa yardımcı olmak için Azure [AD Connect eşitlemeyle Sorun Giderme parola karma senkronizasyonu'na](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)bakın.