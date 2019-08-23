---
title: Siteyi veya listeyi şablon olarak Kaydet
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: a74d14f1743b9a016346f7bf0943523b1ab21f91
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551651"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="c56d2-102">Siteyi veya listeyi şablon olarak Kaydet</span><span class="sxs-lookup"><span data-stu-id="c56d2-102">Save site or list as a template</span></span>

<span data-ttu-id="c56d2-103">SharePoint site şablonları, belirli bir iş gereksinimini tasarlanmış önceden oluşturulmuş tanımlardır.</span><span class="sxs-lookup"><span data-stu-id="c56d2-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="c56d2-104">Daha fazla bilgi için bkz: [farklı türde SharePoint siteleri oluşturmak için şablonları kullanma](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="c56d2-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="c56d2-105">İşte bazı yaygın sorunlar/çözümleri kaydetme bir Site veya liste ile ilgili bir şablon olarak SharePoint çevrimiçi.</span><span class="sxs-lookup"><span data-stu-id="c56d2-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="c56d2-106">**Site / şablonu düğmesi kullanılabilir ya da eksik listesidir**.</span><span class="sxs-lookup"><span data-stu-id="c56d2-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="c56d2-107">Yöneticiler, şablon özellikleri etkinleştirmek için özel komut dosyasına izin gerekir.</span><span class="sxs-lookup"><span data-stu-id="c56d2-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="c56d2-108">Ayrıntılı adımlar, örnekler ve dikkat edilmesi gereken noktalar için bkz: [izin ver veya özel komut dosyası engelleme](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="c56d2-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="c56d2-109">Şablon komut olarak Kaydet site desteklenmez ve SharePoint Server Yayımlama altyapısını kullanan sitelerde sorunlara neden olabilir.</span><span class="sxs-lookup"><span data-stu-id="c56d2-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="c56d2-110">**Site şablonu oluşturulamıyor veya düzgün çalışmıyor**</span><span class="sxs-lookup"><span data-stu-id="c56d2-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="c56d2-111">Şablon [özelliği](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) eksik ve etkinleştirmeniz gerekmez.</span><span class="sxs-lookup"><span data-stu-id="c56d2-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="c56d2-112">Özelliği geçerli site koleksiyonunda etkinleştirmek kullanılabilir değilse, site şablonu site oluşturmak için kullanamazsınız.</span><span class="sxs-lookup"><span data-stu-id="c56d2-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="c56d2-113">Bu site şablonu oluşturulmasını engelleyebilir gibi herhangi bir liste veya kitaplık 5000 öğeleri [Liste görünümü sınırı eşiği](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) aşarsa denetleyin.</span><span class="sxs-lookup"><span data-stu-id="c56d2-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="c56d2-114">Site çok fazla kaynak kullanıyor olabilir ve bu nedenle site şablonu 50 megabayt (MB) sınırını aşıyor.</span><span class="sxs-lookup"><span data-stu-id="c56d2-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="c56d2-115">Arama sütunu kullanan bir listeden veri görüntüleme sorunları vardır.</span><span class="sxs-lookup"><span data-stu-id="c56d2-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="c56d2-116">Daha fazla bilgi için bkz: [SharePoint çevrimiçi doğru arama listesinden verileri şablonu tarafından oluşturulan liste görüntülenmeyecek](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span><span class="sxs-lookup"><span data-stu-id="c56d2-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>


<span data-ttu-id="c56d2-117">Yaygın sorunlar ve çözümleri hakkında daha ayrıntılı bilgi için başvuru, [site şablonları oluşturma ve kullanma](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)Lütfen.</span><span class="sxs-lookup"><span data-stu-id="c56d2-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

