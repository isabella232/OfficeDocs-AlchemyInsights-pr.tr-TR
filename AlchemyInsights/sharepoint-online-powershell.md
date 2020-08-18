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
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="32553-102">SharePoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="32553-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="32553-103">SharePoint Online 'da PowerShell veya betiklerle mı çalışıyorsunuz?</span><span class="sxs-lookup"><span data-stu-id="32553-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="32553-104">Daha fazla bilgi için aşağıdaki bağlantıları ziyaret edin.</span><span class="sxs-lookup"><span data-stu-id="32553-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="32553-105">SharePoint Online Yönetim Kabuğu ile çalışmaya başlama</span><span class="sxs-lookup"><span data-stu-id="32553-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="32553-106">SPO PowerShell 'e çok faktörlü kimlik doğrulaması (MFA) ile bağlanma</span><span class="sxs-lookup"><span data-stu-id="32553-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="32553-107">[SharePoint modelleri ve uygulamaları (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) , SPO 'e yönelik karmaşık yönetim eylemleri gerçekleştirmenize olanak sağlayan bir PowerShell komutları kitaplığı içerir.</span><span class="sxs-lookup"><span data-stu-id="32553-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="32553-108">SPO Yönetim Kabuğu ile bağlantı sorunları yaşıyorsanız, en son sürüme güncelleştirildiğinden emin olun ve *"Import-Module Microsoft. online. SharePoint. PowerShell"* kullanarak [modülü yeniden içeri aktarmayı](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) deneyin.</span><span class="sxs-lookup"><span data-stu-id="32553-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="32553-109">İstemci tarafı nesne modeli komut dosyalarını çalıştırmaya çalışıyorsanız, yerel makinenizde [SharePoint Online Istemci BILEŞENLERI SDK](https://www.microsoft.com/download/details.aspx?id=42038) 'ya sahip olmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="32553-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="32553-110">PowerShell 'den betikleri çalıştırırken sorun yaşıyorsanız, PowerShell 'i yönetici olarak çalıştırmayı ve [Yürütme ilkesini](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)değiştirmeyi düşünebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="32553-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>