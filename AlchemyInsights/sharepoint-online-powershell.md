---
title: SharePoint Online PowerShell
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
ms.openlocfilehash: d90b60de72cf87a56e3b7f6a792708693f31af00
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770859"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="b22cd-102">SharePoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="b22cd-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="b22cd-103">SharePoint Online 'da PowerShell veya betiklerle mı çalışıyorsunuz?</span><span class="sxs-lookup"><span data-stu-id="b22cd-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="b22cd-104">Daha fazla bilgi için aşağıdaki bağlantıları ziyaret edin.</span><span class="sxs-lookup"><span data-stu-id="b22cd-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="b22cd-105">SharePoint Online Yönetim Kabuğu ile çalışmaya başlama</span><span class="sxs-lookup"><span data-stu-id="b22cd-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="b22cd-106">SPO PowerShell 'e çok faktörlü kimlik doğrulaması (MFA) ile bağlanma</span><span class="sxs-lookup"><span data-stu-id="b22cd-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="b22cd-107">[SharePoint modelleri ve uygulamaları (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) , SPO 'e yönelik karmaşık yönetim eylemleri gerçekleştirmenize olanak sağlayan bir PowerShell komutları kitaplığı içerir.</span><span class="sxs-lookup"><span data-stu-id="b22cd-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="b22cd-108">SPO Yönetim Kabuğu ile bağlantı sorunları yaşıyorsanız, en son sürüme güncelleştirildiğinden emin olun ve *"Import-Module Microsoft. online. SharePoint. PowerShell"* kullanarak [modülü yeniden içeri aktarmayı](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) deneyin.</span><span class="sxs-lookup"><span data-stu-id="b22cd-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="b22cd-109">İstemci tarafı nesne modeli komut dosyalarını çalıştırmaya çalışıyorsanız, yerel makinenizde [SharePoint Online Istemci BILEŞENLERI SDK](https://www.microsoft.com/download/details.aspx?id=42038) 'ya sahip olmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="b22cd-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="b22cd-110">PowerShell 'den betikleri çalıştırırken sorun yaşıyorsanız, PowerShell 'i yönetici olarak çalıştırmayı ve [Yürütme ilkesini](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)değiştirmeyi düşünebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b22cd-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>