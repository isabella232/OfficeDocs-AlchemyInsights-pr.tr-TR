---
title: Paylaşılan posta kutusu oluşturulurken proxy adresi hatası
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
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568310"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>Posta kutusu veya e-posta etkinleştirilmiş başka bir nesne oluşturulurken proxy adresi hatası

E-posta özelliği etkin bir nesne (posta kutusu, paylaşılan posta kutusu vb.) oluşturmayı denediy ve ""SMTP:alias@domain.com" ara sunucu adresi zaten kullanılıyor..." hatasını alırsanız, seçtiğiniz e-posta adresi zaten kuruluşta başka bir e-posta özelliği etkin nesne tarafından kullanılıyordur.
  
Bu e-posta adresini içeren kullanıcı, grup, paylaşılan posta kutusu veya ortak klasörü bulmalı ve silmeli veya e-posta adresini değiştirsin. Ardından, serbest e-posta adresine sahip yeni bir e-posta özelliği etkin nesne oluşturabilirsiniz. Bulmak için Giriş sayfasında Ara'ya tıklayın. Ayrıca, aramak için aşağıdaki Exchange Online PowerShell komutunu da kullanabilirsiniz:

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
Var olan e-posta adresini silmek istemiyorsanız, oluşturmakta olduğu yeni nesne için yeni bir e-posta adresi seçin.
  