---
title: SharePoint veya OneDrive'daki öğeleri sileme
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 8647b65c52a782ca48ca58bb2700556db528796b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511996"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="9ac5b-102">Öğeleri sileme</span><span class="sxs-lookup"><span data-stu-id="9ac5b-102">Unable to delete items</span></span>

<span data-ttu-id="9ac5b-103">Bekletme ilkeleri buna neden olabilir, bu soruna neden olan ilgili tutmayı devre dışı bırakmak veya hariç tutmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="9ac5b-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="9ac5b-104">Bekletme ilkesi veya tutma kaldırıldıktan sonra, değişikliğin etkili olması 24 saat kadar sürebilir.</span><span class="sxs-lookup"><span data-stu-id="9ac5b-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="9ac5b-105">Öğeüzerinde [bekletme ilkesi](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) kurulumu olmadığından emin olun.</span><span class="sxs-lookup"><span data-stu-id="9ac5b-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="9ac5b-106">Site depolama sınırını aşmış, [site kotasını](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) artırmış ve öğeyi silmiş olabilir.</span><span class="sxs-lookup"><span data-stu-id="9ac5b-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="9ac5b-107">Öğenin başka bir kullanıcıya [kullanıma alınmadığından](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) emin olun.</span><span class="sxs-lookup"><span data-stu-id="9ac5b-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="9ac5b-108">Son olarak, yöneticiler, inatçı öğeleri zorla silme gibi karmaşık yönetim eylemleri gerçekleştirmenize olanak tanıyan PowerShell komutlarının kitaplığını içeren [SharePoint Desenleri ve Uygulamaları](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) 'nı (PnP) kullanabilir.</span><span class="sxs-lookup"><span data-stu-id="9ac5b-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="9ac5b-109">PNP dosyayı kaldırma</span><span class="sxs-lookup"><span data-stu-id="9ac5b-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="9ac5b-110">PNP Klasörünü Kaldırma</span><span class="sxs-lookup"><span data-stu-id="9ac5b-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="9ac5b-111">PNP Liste Öğeyi Kaldırma</span><span class="sxs-lookup"><span data-stu-id="9ac5b-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="9ac5b-112">PNP Listesini Kaldır</span><span class="sxs-lookup"><span data-stu-id="9ac5b-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="9ac5b-113">PNP Alanını Kaldırma (Sütun)</span><span class="sxs-lookup"><span data-stu-id="9ac5b-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)