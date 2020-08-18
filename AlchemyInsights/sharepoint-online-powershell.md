---
title: SharePoint Online PowerShell
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
- "9000266"
- "1867"
ms.openlocfilehash: 300c07e7f0010eae2bd4fe893ece9d09aab93ba5
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786909"
---
# <a name="sharepoint-online-powershell"></a>SharePoint Online PowerShell

SharePoint Online 'da PowerShell veya betiklerle mı çalışıyorsunuz? Daha fazla bilgi için aşağıdaki bağlantıları ziyaret edin.
- [SharePoint Online Yönetim Kabuğu ile çalışmaya başlama](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [SPO PowerShell 'e çok faktörlü kimlik doğrulaması (MFA) ile bağlanma](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [SharePoint modelleri ve uygulamaları (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) , SPO 'e yönelik karmaşık yönetim eylemleri gerçekleştirmenize olanak sağlayan bir PowerShell komutları kitaplığı içerir.

> [!NOTE]
> - SPO Yönetim Kabuğu ile bağlantı sorunları yaşıyorsanız, en son sürüme güncelleştirildiğinden emin olun ve *"Import-Module Microsoft. online. SharePoint. PowerShell"* kullanarak [modülü yeniden içeri aktarmayı](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) deneyin.
> - İstemci tarafı nesne modeli komut dosyalarını çalıştırmaya çalışıyorsanız, yerel makinenizde [SharePoint Online Istemci BILEŞENLERI SDK](https://www.microsoft.com/download/details.aspx?id=42038) 'ya sahip olmanız gerekir.
> - PowerShell 'den betikleri çalıştırırken sorun yaşıyorsanız, PowerShell 'i yönetici olarak çalıştırmayı ve [Yürütme ilkesini](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)değiştirmeyi düşünebilirsiniz.