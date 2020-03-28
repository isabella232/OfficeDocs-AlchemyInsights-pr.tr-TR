---
title: SharePoint’te siteyi kalıcı olarak silme
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: 263317339d965d173a5a038fa006e0ce6f8476cc
ms.sourcegitcommit: da04e79b6072321caa16a6ceea6eb5f15de22394
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/25/2020
ms.locfileid: "42955233"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a><span data-ttu-id="1f10c-102">SharePoint’te siteyi kalıcı olarak silme</span><span class="sxs-lookup"><span data-stu-id="1f10c-102">Permanently delete a site in SharePoint</span></span>

<span data-ttu-id="1f10c-103">Silinen sitenin URL’sini yeniden kullanmak (siteyi yeniden oluşturmak) veya artık kullanımda olmadığından siteyi kalıcı olarak silmek için Yeni SharePoint Yönetim Merkezi’nden **Kalıcı Olarak Sil**’i kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="1f10c-103">To reuse a URL from a deleted site (to recreate a site), or to permanently delete a site because it's no longer in use, you can use **Permanently Delete** from the New SharePoint Admin Center.</span></span> 

1. <span data-ttu-id="1f10c-104">[Yeni SharePoint yönetim merkezinin Silinen siteler sayfasına](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) gidin ve kuruluşunuzda yönetim izinleri olan bir hesapla oturum açın.</span><span class="sxs-lookup"><span data-stu-id="1f10c-104">Go to the [Deleted sites page of the new SharePoint admin center](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) and sign in with an account that has admin permissions for your organization.</span></span> 

2. <span data-ttu-id="1f10c-105">Sol sütunda bir site seçin.</span><span class="sxs-lookup"><span data-stu-id="1f10c-105">In the left column, select a site.</span></span> 

3. <span data-ttu-id="1f10c-106">**Kalıcı Olarak Sil**’e tıklayın.</span><span class="sxs-lookup"><span data-stu-id="1f10c-106">Click **Permanently Delete**.</span></span> 

<span data-ttu-id="1f10c-107">**Not**: Grup bağlantılı siteler Yeni SharePoint Yönetim Merkezi’nden kalıcı olarak silinemez.</span><span class="sxs-lookup"><span data-stu-id="1f10c-107">**Note**: Group-connected sites cannot be permanently deleted from the New SharePoint Admin Center.</span></span> <span data-ttu-id="1f10c-108">Bunun yerine [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) kullanılmalıdır.</span><span class="sxs-lookup"><span data-stu-id="1f10c-108">[Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) will need to be used instead.</span></span>  

<span data-ttu-id="1f10c-109">Daha fazla bilgi için bkz. [Siteyi kalıcı olarak silme](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="1f10c-109">For more info, see [Permanently delete a site](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span></span> 
