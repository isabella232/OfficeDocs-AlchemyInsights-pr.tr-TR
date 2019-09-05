---
title: Siteyi veya listeyi şablon olarak kaydetme
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 1fe0a2f5bf65ef4e8cabf3d05a701c8eff966435
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752052"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="aa244-102">Siteyi veya listeyi şablon olarak kaydetme</span><span class="sxs-lookup"><span data-stu-id="aa244-102">Save site or list as a template</span></span>

<span data-ttu-id="aa244-103">SharePoint site şablonları, belirli bir iş gereksinimi etrafında tasarlanmış önceden oluşturulmuş tanımlardır.</span><span class="sxs-lookup"><span data-stu-id="aa244-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="aa244-104">Daha fazla bilgi için bkz. [Farklı SharePoint siteleri oluşturmak için şablonları kullanma.](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4)</span><span class="sxs-lookup"><span data-stu-id="aa244-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="aa244-105">SharePoint Online'da bir Siteyi veya Listeyi şablon olarak kaydetmeyle ilgili bazı sık karşılaşılan sorunlar/çözümler aşağıda verilmiştir.</span><span class="sxs-lookup"><span data-stu-id="aa244-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="aa244-106">**Site/liste şablonu kaydet düğmesi kullanılamıyor veya eksik.**</span><span class="sxs-lookup"><span data-stu-id="aa244-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="aa244-107">Yöneticilerin şablon özelliklerini etkinleştirmek için Özel Komut Dosyasına İzin Vermeleri gerekir.</span><span class="sxs-lookup"><span data-stu-id="aa244-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="aa244-108">Ayrıntılı adımlar, örnekler ve hususlar [için](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)bkz.</span><span class="sxs-lookup"><span data-stu-id="aa244-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="aa244-109">Şablon komutu olarak kaydet sitesi desteklenmez ve SharePoint Server Yayımlama Altyapısını kullanan sitelerde sorunlara neden olabilir.</span><span class="sxs-lookup"><span data-stu-id="aa244-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="aa244-110">**Site şablonu oluşturulamıyor veya doğru çalışmıyor**</span><span class="sxs-lookup"><span data-stu-id="aa244-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="aa244-111">Şablon bir [özellik](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) eksik olabilir ve etkinleştirilmez.</span><span class="sxs-lookup"><span data-stu-id="aa244-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="aa244-112">Özellik geçerli site koleksiyonunda etkinleştirmek için kullanılamıyorsa, site şablonunu bir site oluşturmak için kullanamazsınız.</span><span class="sxs-lookup"><span data-stu-id="aa244-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="aa244-113">Herhangi bir liste veya kitaplık, bir site şablonunun oluşturulmasını engelleyebilir gibi 5000 öğe liste [görünümü sınır eşiği](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) aşAbilir olup olmadığını görmek için denetleyin.</span><span class="sxs-lookup"><span data-stu-id="aa244-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="aa244-114">Site çok fazla kaynak kullanıyor olabilir ve bu nedenle site şablonu 50 megabayt (MB) sınırını aşıyor.</span><span class="sxs-lookup"><span data-stu-id="aa244-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="aa244-115">Arama sütunu kullanan bir listeden veri görüntülemede sorunlar vardır.</span><span class="sxs-lookup"><span data-stu-id="aa244-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="aa244-116">Daha fazla bilgi için bkz: [Şablon tarafından oluşturulan liste SharePoint Online'da doğru arama listesinden veri görüntülemiyor.](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)</span><span class="sxs-lookup"><span data-stu-id="aa244-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>


<span data-ttu-id="aa244-117">Sık karşılaşılan sorunlar ve çözümler hakkında daha ayrıntılı bilgi için lütfen başvuru, [Site şablonları oluşturun ve](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)kullanın.</span><span class="sxs-lookup"><span data-stu-id="aa244-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

