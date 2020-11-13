---
title: SharePoint veya OneDrive 'da öğeler silinemiyor
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: db45aa8df40484fdcda7c430f1ca27482a1dd4ce
ms.sourcegitcommit: a9415f3ae8c7ba267b5134bcbdc1e070cea41a0f
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/12/2020
ms.locfileid: "49019603"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="74729-102">Öğeler silinemiyor</span><span class="sxs-lookup"><span data-stu-id="74729-102">Unable to delete items</span></span>

- <span data-ttu-id="74729-103">Bekletme ilkeleri bunun nedeni, bu soruna neden olan ilgili tutmayı devre dışı bırakmanız veya dışarıda bırakmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="74729-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="74729-104">Bekletme ilkesi veya tutma kaldırıldıktan sonra, değişikliğin geçerlilik kazanması 24 saate kadar sürebilir.</span><span class="sxs-lookup"><span data-stu-id="74729-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="74729-105">Öğede [bekletme ilkesi](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) ayarı olmadığından emin olun.</span><span class="sxs-lookup"><span data-stu-id="74729-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="74729-106">Site depolama sınırını aşmış olabilir, [site kotasını](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) artırıp öğeyi silin.</span><span class="sxs-lookup"><span data-stu-id="74729-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

- <span data-ttu-id="74729-107">Öğenin başka bir kullanıcıya [teslim](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) kullanılmadığından emin olun.</span><span class="sxs-lookup"><span data-stu-id="74729-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="74729-108">Son olarak, Yöneticiler, Stubborn öğelerini silmeye zorlama gibi karmaşık yönetim eylemlerini gerçekleştirmenize olanak sağlayan bir PowerShell komutları kitaplığı içeren [SharePoint modellerini ve uygulamalarını](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) kullanabilir.</span><span class="sxs-lookup"><span data-stu-id="74729-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="74729-109">PNP dosyasını kaldırma</span><span class="sxs-lookup"><span data-stu-id="74729-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="74729-110">PNP klasörünü kaldırma</span><span class="sxs-lookup"><span data-stu-id="74729-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="74729-111">PNP listesi öğesini kaldır</span><span class="sxs-lookup"><span data-stu-id="74729-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="74729-112">PNP listesini kaldır</span><span class="sxs-lookup"><span data-stu-id="74729-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="74729-113">PNP alanı (sütun) kaldırma</span><span class="sxs-lookup"><span data-stu-id="74729-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)