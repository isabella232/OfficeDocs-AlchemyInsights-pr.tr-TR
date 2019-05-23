---
title: SharePoint veya OneDrive öğeler silinemiyor
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 21d7b928fade48a6729c120e6ea33b16dafe799e
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057792"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="b9b78-102">Öğeler silinemiyor</span><span class="sxs-lookup"><span data-stu-id="b9b78-102">Unable to delete items</span></span>

<span data-ttu-id="b9b78-103">Öğeleri silme sorunlar yaşıyorsunuz?</span><span class="sxs-lookup"><span data-stu-id="b9b78-103">Having issues deleting items?</span></span>

- <span data-ttu-id="b9b78-104">Her zaman öğeyi silmek veya öğeyi kaldırmak bir [site koleksiyonu yöneticisi](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) denemesinde bulunması için [uygun izinlere](https://docs.microsoft.com/en-us/sharepoint/default-sharepoint-groups) sahip olduğunuzdan emin olun.</span><span class="sxs-lookup"><span data-stu-id="b9b78-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/en-us/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="b9b78-105">Olmadığını bir [bekletme ilkesi](https://docs.microsoft.com/en-us/office365/securitycompliance/retention-policies) ayarı öğede emin olun.</span><span class="sxs-lookup"><span data-stu-id="b9b78-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/en-us/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="b9b78-106">Öğeyi başka bir kullanıcı [kullanıma](https://support.office.com/en-us/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) değil emin olun.</span><span class="sxs-lookup"><span data-stu-id="b9b78-106">Ensure the item is not [checked out](https://support.office.com/en-us/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="b9b78-107">Son olarak, yöneticilerin geçeceğinizi öğeleri silme gibi karmaşık yönetimi eylemleri gerçekleştirmenize olanak sağlayan komutlar zorla PowerShell kitaplığını içeren [SharePoint desenleri ve yöntemler](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b9b78-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span> 
- [<span data-ttu-id="b9b78-108">PNP dosyasını kaldırın.</span><span class="sxs-lookup"><span data-stu-id="b9b78-108">Remove PNP File</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="b9b78-109">PNP klasörünü kaldırma</span><span class="sxs-lookup"><span data-stu-id="b9b78-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="b9b78-110">PNP liste öğesi Kaldır</span><span class="sxs-lookup"><span data-stu-id="b9b78-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="b9b78-111">PNP listesini Kaldır</span><span class="sxs-lookup"><span data-stu-id="b9b78-111">Remove PNP List</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="b9b78-112">PNP alan (sütun) Kaldır</span><span class="sxs-lookup"><span data-stu-id="b9b78-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)