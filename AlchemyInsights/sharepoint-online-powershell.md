---
title: Sharepoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: b7580f0e609d21bdc13fc07fda0bfd15bdb7a7ca
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709090"
---
# <a name="sharepoint-online-powershell"></a>Sharepoint Online PowerShell

SharePoint Online'da PowerShell veya Betikler ile mi çalışıyorsunuz? Daha fazla bilgi için aşağıdaki bağlantıları ziyaret edin.
- [SharePoint Online Yönetim Kabuğu ile çalışmaya başlama](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [Çok faktörlü kimlik doğrulaması (MFA) ile SPO PowerShell'e bağlanma](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [SharePoint Desenler ve Yöntemleri (PnP),](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) SPO'ya karşı karmaşık yönetim eylemleri gerçekleştirmenizi sağlayan bir PowerShell komut kitaplığı içerir.

> [!NOTE]
> - SPO yönetim kabuğuna bağlanırken sorun paylaşıyorsanız, en son sürüme güncelleştirilmiş [](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) olduğundan emin olun ve *"Import-Module Microsoft.Online.SharePoint.PowerShell"* kullanarak modülü yeniden içeri aktarmayı deneyin.
> - İstemci tarafı nesne modeli betiklerini çalıştırmayı denıyorsanız, yerel makinenize [SharePoint Online İstemci](https://www.microsoft.com/download/details.aspx?id=42038) Bileşenleri SDK'sini yüklemiş olması gerekir.
> - PowerShell'den betikleri çalıştırmada sorun ediyorsanız, PowerShell'i Yönetici olarak çalıştırmayı ve Yürütme İlkesini değiştirmeyi [göz önünde bulundurabilirsiniz.](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)