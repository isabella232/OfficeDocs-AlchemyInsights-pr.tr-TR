---
title: Parola eşitleme sorunlarını giderme
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: c71fce8621057093d23891c26f7b0285fdc8b9ed
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28318168"
---
# <a name="troubleshoot-password-synchronization"></a>Parola eşitleme sorunlarını giderme

Hiçbir parola Azure AD Connect sürüm 1.1.614.0 ile eşitlenen veya üstü olduğu sorunları gidermek için:
  
1. **Yönetici olarak çalıştır** seçeneğiyle Azure AD Bağlan sunucunuzdaki yeni bir Windows PowerShell oturumu açın. 
    
2. **Set-ExecutionPolicy RemoteSigned** veya **Set-ExecutionPolicy sınırsız**çalıştırın. 
    
3. Azure AD Bağlan Sihirbazı'nı başlatın.
    
4. Gidin ** ek görevler ** sayfa, select ** giderme **, **İleri**' yi tıklatın. 
    
5. Sorun giderme sayfasında PowerShell **sorun giderme işlemlerine başlamak için Başlat** menüsünü tıklatın. 
    
6. Ana menüde, **Parola eşitleme sorunlarını giderme**seçin. 
    
7. **Parola Eşitleme hiç çalışmıyor**alt menüde seçin. 
    
 **Sorun giderme Görev sonuçlarını anlamak**
  
Sorun giderme görev aşağıdaki denetimleri gerçekleştirir:
  
- Parola eşitleme özelliği, Azure AD Kiracı için etkin olduğunu doğrular.
    
- Azure AD Connect server hazırlama modu içinde olmadığını doğrular.
    
- (Varolan bir Active Directory ormanına karşılık gelir) her varolan yerinde Active Directory Bağlayıcısı için:
    
- 
  - Parola eşitleme özelliği etkin olduğunu doğrular.
    
  - Parola eşitleme sinyali olaylar Windows uygulama olay günlüklerine arar.
    
  - Her Active Directory etki alanı için Active Directory Bağlayıcısı yerinde altında:
    
  - Etki alanı AD Bağlan Azure sunucudan ulaşılabilir olduğunu doğrular.
    
  - Şirket içi Active Directory Bağlayıcısı tarafından kullanılan Active Directory etki alanı Hizmetleri (AD DS) hesap doğru kullanıcı adı, parola ve parola eşitleme için gereken izinlere sahip olduğunu doğrular.
    
Parola eşitleme sorunlarını giderme hakkında daha fazla yardım için bkz: [eşitleme Azure AD Connect ile parola eşitleme sorunlarını giderme](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).
  

