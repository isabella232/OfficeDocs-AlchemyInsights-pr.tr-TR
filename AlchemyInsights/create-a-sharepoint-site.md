---
title: SharePoint sitesi oluşturma
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: ac894195d847dfc009bc0b57647e1a474361f1c1
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/29/2019
ms.locfileid: "37769611"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="24fc4-102">SharePoint sitesi oluşturma</span><span class="sxs-lookup"><span data-stu-id="24fc4-102">Create a SharePoint site</span></span>

<span data-ttu-id="24fc4-103">SharePoint site oluşturma hakkında bilgi için aşağıdakileri görebilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="24fc4-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="24fc4-104">[Yeni SharePoint yönetici merkezindeki siteleri yönetme](https://docs.microsoft.com/sharepoint/manage-site-creation): Klasik bir sitenin veya Office 365 grubunu içermeyen bir ekip sitesinin nasıl oluşturulabildiğini içeren site oluşturma seçenekleri hakkında bilgi edinin.</span><span class="sxs-lookup"><span data-stu-id="24fc4-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="24fc4-105">[SharePoint'te bir ekip sitesi oluşturun](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): Ekip sitesi oluşturmayı öğrenin.</span><span class="sxs-lookup"><span data-stu-id="24fc4-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): Learn how to create a team site.</span></span>
- <span data-ttu-id="24fc4-106">[SharePoint Online'da bir iletişim sitesi oluşturun](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): İletişim sitesi oluşturmayı öğrenin.</span><span class="sxs-lookup"><span data-stu-id="24fc4-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="24fc4-107">[Yeni SharePoint yönetici merkezindeki siteleri yönetme](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): Klasik bir siteyi veya Office 365 grubunu içermeyen bir ekip sitesini nasıl oluşturacağız öğrenin.</span><span class="sxs-lookup"><span data-stu-id="24fc4-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
<span data-ttu-id="24fc4-108">**Ipuç -ları:**</span><span class="sxs-lookup"><span data-stu-id="24fc4-108">**Tips:**</span></span>
- <span data-ttu-id="24fc4-109">Varolan bir sitenin aynı URL'sini içeren bir site oluşturamazsınız.</span><span class="sxs-lookup"><span data-stu-id="24fc4-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="24fc4-110">Bir siteyi sildiyseniz ve URL'yi yeniden kullanmak istiyorsanız, silinen site **silinmiş sitelerin**altında hala var olabilir.</span><span class="sxs-lookup"><span data-stu-id="24fc4-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="24fc4-111">Silinen siteleri yönetmek için [bkz.](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site)</span><span class="sxs-lookup"><span data-stu-id="24fc4-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="24fc4-112">Powershell içeren bir siteyi tamamen kaldırmak [için, Kaldır-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet örneğine bakın.</span><span class="sxs-lookup"><span data-stu-id="24fc4-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="24fc4-113">Bazı kullanıcılar bir site oluşturamayabilir.</span><span class="sxs-lookup"><span data-stu-id="24fc4-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="24fc4-114">Bkz. [SharePoint Online'da site oluşturmayı yönet.](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="24fc4-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="24fc4-115">Sitenin beklenenden daha uzun süredir **Oluşturma'da** sıkışmış görünmesi mümkündür.</span><span class="sxs-lookup"><span data-stu-id="24fc4-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="24fc4-116">Bu sorunu ilk gördüğünüzden bu yana 24 saatten fazla zaman geçtiyse, lütfen bir destek bileti ni kaydedin.</span><span class="sxs-lookup"><span data-stu-id="24fc4-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="24fc4-117">Çoğu durumda, zaten bir çözüm üzerinde çalışıyoruz.</span><span class="sxs-lookup"><span data-stu-id="24fc4-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="24fc4-118">Lütfen bir çözümü tamamlamamız için bize en az 24 saat verin.</span><span class="sxs-lookup"><span data-stu-id="24fc4-118">Please give us at least 24 hours to complete a solution.</span></span>
- <span data-ttu-id="24fc4-119">Office 365 grubu içermeyen yeni bir ekip sitesi oluşturmanız gerekiyorsa,</span><span class="sxs-lookup"><span data-stu-id="24fc4-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


