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
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="fc76e-102">Sharepoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="fc76e-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="fc76e-103">SharePoint Online'da PowerShell veya Betikler ile mi çalışıyorsunuz?</span><span class="sxs-lookup"><span data-stu-id="fc76e-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="fc76e-104">Daha fazla bilgi için aşağıdaki bağlantıları ziyaret edin.</span><span class="sxs-lookup"><span data-stu-id="fc76e-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="fc76e-105">SharePoint Online Yönetim Kabuğu ile çalışmaya başlama</span><span class="sxs-lookup"><span data-stu-id="fc76e-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="fc76e-106">Çok faktörlü kimlik doğrulaması (MFA) ile SPO PowerShell'e bağlanma</span><span class="sxs-lookup"><span data-stu-id="fc76e-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="fc76e-107">[SharePoint Desenler ve Yöntemleri (PnP),](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) SPO'ya karşı karmaşık yönetim eylemleri gerçekleştirmenizi sağlayan bir PowerShell komut kitaplığı içerir.</span><span class="sxs-lookup"><span data-stu-id="fc76e-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="fc76e-108">SPO yönetim kabuğuna bağlanırken sorun paylaşıyorsanız, en son sürüme güncelleştirilmiş [](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) olduğundan emin olun ve *"Import-Module Microsoft.Online.SharePoint.PowerShell"* kullanarak modülü yeniden içeri aktarmayı deneyin.</span><span class="sxs-lookup"><span data-stu-id="fc76e-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="fc76e-109">İstemci tarafı nesne modeli betiklerini çalıştırmayı denıyorsanız, yerel makinenize [SharePoint Online İstemci](https://www.microsoft.com/download/details.aspx?id=42038) Bileşenleri SDK'sini yüklemiş olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="fc76e-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="fc76e-110">PowerShell'den betikleri çalıştırmada sorun ediyorsanız, PowerShell'i Yönetici olarak çalıştırmayı ve Yürütme İlkesini değiştirmeyi [göz önünde bulundurabilirsiniz.](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)</span><span class="sxs-lookup"><span data-stu-id="fc76e-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>