---
title: Parola eşitlemesi sorun giderme
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: edd4f68466296f72c2dc0bafda45e6749d62d942
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732530"
---
# <a name="troubleshoot-password-synchronization"></a>Parola eşitlemesi sorun giderme

Azure AD Connect sürümü 1.1.614.0 veya sonraki sürümle hiçbir parolanın eşitlenmediği sorunları gidermek için:
  
1. Azure AD Connect sunucunuzda **Yönetici olarak Çalıştır** seçeneğiyle yeni bir Windows PowerShell oturumu açın.

2. **Set-ExecutionPolicy RemoteSigned** veya **Set-ExecutionPolicy Sınırsız**çalıştırın.

3. Azure AD Bağlantısı sihirbazını başlatın.

4. **Ek Görevler** sayfasına gidin, **Sorun Giderme'yi**seçin ve **İleri'yi**tıklatın.

5. Sorun Giderme sayfasında, **PowerShell'deki sorun giderme menüsünü başlatmak için Başlat'ı** tıklatın.

6. Ana menüde **Sorun Giderme Parola Eşitlemesi'ni**seçin.

7. Alt menüde **Parola Eşitlemesi'ni**seçin hiç çalışmıyor.

**Sorun giderme görevinin sonuçlarını anlama**
  
Sorun giderme görevi aşağıdaki denetimleri gerçekleştirir:
  
- Azure AD kiracınız için parola eşitleme özelliğinin etkin olduğunu doğrular.

- Azure AD Connect sunucusunun hazırlama modunda olmadığını doğrular.

- Varolan her şirket içi Active Directory bağlayıcısı için (varolan bir Active Directory ormanına karşılık gelir):

- 
  - Parola eşitleme özelliğinin etkin olduğunu doğrular.

  - Windows Application Event günlüklerinde parola eşitleme sinyali olaylarını arar.

  - Şirket içi Active Directory bağlayıcısı altındaki her Active Directory etki alanı için:

  - Etki alanına Azure AD Connect sunucusundan erişilebildiğini doğrular.

  - Şirket içi Active Directory bağlayıcısı tarafından kullanılan Active Directory Domain Services (AD DS) hesaplarının parola eşitleme için gereken doğru kullanıcı adı, parola ve izinlere sahip olduğunu doğrular.

Parola eşitleme sorununa yardımcı olmak için Azure [AD Connect eşitlemeyle Sorun Giderme Parola senkronizasyonu'na](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization)bakın.
  