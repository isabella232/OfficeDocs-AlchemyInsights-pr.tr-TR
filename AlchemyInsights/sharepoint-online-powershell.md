---
title: Sharepoint Online PowerShell
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
- "9000266"
- "1867"
ms.openlocfilehash: 839a70282b4dd619e9dbe8167ef0e409e468b1ad
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830602"
---
# <a name="sharepoint-online-powershell"></a>Sharepoint Online PowerShell

SharePoint Online'da PowerShell veya Betikler ile mi çalışıyorsunuz? Daha fazla bilgi için aşağıdaki bağlantıları ziyaret edin.
- [SharePoint Online Yönetim Kabuğu ile çalışmaya başlama](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [Multifactor Authentication (MFA) ile SPO PowerShell'e bağlanma](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [SharePoint Desenler ve Yöntemleri (PnP),](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) SPO üzerinde karmaşık yönetim eylemleri gerçekleştirmenizi sağlayan bir PowerShell komutları kitaplığı içerir.

> [!NOTE]
> - SPO yönetim kabuğuna bağlanırken sorun ediyorsanız, en son sürüme güncelleştirilmiş [](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) olduğundan emin olun ve *"Import-Module Microsoft.Online.SharePoint.PowerShell"* kullanarak modülü yeniden içeri aktarmayı deneyin.
> - İstemci tarafı nesne modeli betiklerini çalıştırmayı denıyorsanız, yerel makinenize [Sharepoint Online](https://www.microsoft.com/download/details.aspx?id=42038) İstemci Bileşenleri SDK'sini yüklemiş olması gerekir.
> - PowerShell'den betikleri çalıştırmada sorun ediyorsanız, PowerShell'i Yönetici olarak çalıştırmayı ve Yürütme İlkesini değiştirmeyi [göz önünde bulundurabilirsiniz.](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)