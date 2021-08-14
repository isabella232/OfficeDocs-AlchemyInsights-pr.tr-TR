---
title: Paylaşılan posta kutusu oluşturulurken ara sunucu adresi hatası
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: 7c15d5db5445fbe4c3ec22878f180f48d2da4f90369f2e6f223916646eb19c12
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54062928"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>Posta kutusu veya başka bir e-posta etkinleştirilmiş nesne oluşturulurken proxy adresi hatası

E-posta özelliği etkin bir nesne (posta kutusu, paylaşılan posta kutusu vb.) oluşturmaya çalıştınız ve ""SMTP:alias@domain.com" ara sunucu adresi zaten kullanılıyor..." hatasını alırsanız, seçtiğiniz e-posta adresi zaten kuruluşta e-posta özelliği olan başka bir nesne tarafından kullanılıyordur.
  
Bu e-posta adresini içeren kullanıcı, grup, paylaşılan posta kutusunu veya ortak klasörü bulmanız ve silmeniz veya e-posta adresini değiştirmeniz gerekir. Ardından, serbest e-posta adresiyle yeni bir e-posta özellikli nesne oluşturabilirsiniz. Bunu bulmak için Giriş sayfasında Ara'ya tıklayın. Ayrıca, aramak için Exchange Online PowerShell komutunu da kullanabilirsiniz:

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
Var olan e-posta adresini silmek istemiyorsanız, oluşturmakta istediğiniz yeni nesne için yeni bir e-posta adresi seçin.
  