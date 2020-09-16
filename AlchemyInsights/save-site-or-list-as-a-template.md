---
title: Siteyi veya listeyi şablon olarak kaydetme
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 37ae727aa6dd6af94d0d833ce972aec413d90194
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727551"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="8fd17-102">Siteyi veya listeyi şablon olarak kaydetme</span><span class="sxs-lookup"><span data-stu-id="8fd17-102">Save site or list as a template</span></span>

<span data-ttu-id="8fd17-103">SharePoint site şablonları, belirli bir iş ihtiyacı etrafında tasarlanmış önceden oluşturulmuş tanımlardır.</span><span class="sxs-lookup"><span data-stu-id="8fd17-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="8fd17-104">Daha fazla bilgi için bkz: [şablonları kullanarak farklı türlerde SharePoint siteleri oluşturma](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="8fd17-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="8fd17-105">SharePoint Online 'da bir site veya listeyi şablon olarak kaydetme ile ilgili bazı yaygın sorun/çözümleri aşağıda bulabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="8fd17-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="8fd17-106">**Site/liste şablonunu Kaydet düğmesi kullanılamıyor veya yok**.</span><span class="sxs-lookup"><span data-stu-id="8fd17-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="8fd17-107">Yöneticilerin şablon özelliklerini etkinleştirmesi için özel komut dosyasına Izin vermesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="8fd17-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="8fd17-108">Ayrıntılı adımlar için, örnekler ve hususlar [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)</span><span class="sxs-lookup"><span data-stu-id="8fd17-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="8fd17-109">Siteyi şablon olarak Kaydet komutu desteklenmediğinden SharePoint Server yayımlama altyapısını kullanan sitelerde sorunlara neden olabilir.</span><span class="sxs-lookup"><span data-stu-id="8fd17-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="8fd17-110">**Site şablonu oluşturulamıyor veya düzgün çalışmıyor**</span><span class="sxs-lookup"><span data-stu-id="8fd17-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="8fd17-111">Şablonda bir [özellik](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) eksik olabilir ve etkinleştirilmeyecektir.</span><span class="sxs-lookup"><span data-stu-id="8fd17-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="8fd17-112">Özellik geçerli site koleksiyonunda etkinleştirme için kullanılamıyorsa site şablonunu kullanarak site oluşturmaya kullanamazsınız.</span><span class="sxs-lookup"><span data-stu-id="8fd17-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="8fd17-113">Herhangi bir liste veya kitaplıkta 5000 öğelerinin [liste görünümü sınırı eşiğini](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) aşmadığını denetleyin, bu da bir site şablonunun oluşturulmasını engelleyebilir.</span><span class="sxs-lookup"><span data-stu-id="8fd17-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="8fd17-114">Site çok fazla kaynak kullanıyor olabilir ve bu nedenle site şablonu 50 megabayt (MB) sınırını aşıyor.</span><span class="sxs-lookup"><span data-stu-id="8fd17-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="8fd17-115">Arama sütunu kullanan bir listeden verileri görüntülerken sorun çıktı.</span><span class="sxs-lookup"><span data-stu-id="8fd17-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="8fd17-116">Daha fazla bilgi için, [şablon tarafından oluşturulan liste, SharePoint Online 'daki doğru arama listesinden verileri görüntülemez](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="8fd17-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>


<span data-ttu-id="8fd17-117">Sık karşılaşılan sorunlar ve çözümler hakkında daha ayrıntılı bilgi için, [site şablonları oluşturma ve kullanma](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)konusuna başvurun.</span><span class="sxs-lookup"><span data-stu-id="8fd17-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

