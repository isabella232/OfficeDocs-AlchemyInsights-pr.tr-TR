---
title: SharePoint çevrimiçi bir site oluşturmak
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 9ab06cbd1648da31d8a04e61c237a2326b4bbe93
ms.sourcegitcommit: f856d46a325c517fc29d935c27f21b77c4219e66
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/24/2019
ms.locfileid: "35199293"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="5b2c9-102">Şablonları kullanarak SharePoint sitesi oluşturmak</span><span class="sxs-lookup"><span data-stu-id="5b2c9-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="5b2c9-103">SharePoint site şablonları, belirli bir iş gereksinimini tasarlanmış önceden oluşturulmuş tanımlardır.</span><span class="sxs-lookup"><span data-stu-id="5b2c9-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="5b2c9-104">Daha fazla bilgi için bkz: [farklı türde SharePoint siteleri oluşturmak için şablonları kullanma](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="5b2c9-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="5b2c9-105">İşte bazı yaygın sorunlar/çözümleri kaydetme bir Site veya liste ile ilgili bir şablon olarak Sharepoint çevrimiçi.</span><span class="sxs-lookup"><span data-stu-id="5b2c9-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="5b2c9-106">**Site/liste şablonu Kaydet'i eksik veya kullanılabilir değil**</span><span class="sxs-lookup"><span data-stu-id="5b2c9-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="5b2c9-107">Yöneticiler, şablon özellikleri etkinleştirmek için özel komut dosyasına izin gerekir.</span><span class="sxs-lookup"><span data-stu-id="5b2c9-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="5b2c9-108">Ayrıntılı adımlar için bkz: örnekler ve dikkat edilmesi gereken noktalar</span><span class="sxs-lookup"><span data-stu-id="5b2c9-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="5b2c9-109">İzin verme veya özel komut dosyası engelleme</span><span class="sxs-lookup"><span data-stu-id="5b2c9-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="5b2c9-110">Şablon komut olarak Kaydet site desteklenmez ve SharePoint Server Yayımlama altyapısını kullanan sitelerde sorunlara neden olabilir.</span><span class="sxs-lookup"><span data-stu-id="5b2c9-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="5b2c9-111">**Site şablonu oluşturulamıyor veya düzgün çalışmıyor**</span><span class="sxs-lookup"><span data-stu-id="5b2c9-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="5b2c9-112">Şablon [özelliği](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) eksik ve etkinleştirmeniz gerekmez.</span><span class="sxs-lookup"><span data-stu-id="5b2c9-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="5b2c9-113">Özelliği geçerli site koleksiyonunda etkinleştirmek kullanılabilir değilse, site şablonu site oluşturmak için kullanamazsınız.</span><span class="sxs-lookup"><span data-stu-id="5b2c9-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="5b2c9-114">Bu site şablonu oluşturulmasını engelleyebilir gibi herhangi bir liste veya kitaplık 5000 öğeleri [Liste görünümü sınırı eşiği](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) aşarsa denetleyin.</span><span class="sxs-lookup"><span data-stu-id="5b2c9-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="5b2c9-115">Site çok fazla kaynak kullanıyor olabilir ve bu nedenle site şablonu 50 MB sınırı aşıyor.</span><span class="sxs-lookup"><span data-stu-id="5b2c9-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="5b2c9-116">Arama sütunu kullanan bir listeden veri görüntüleme sorunları vardır.</span><span class="sxs-lookup"><span data-stu-id="5b2c9-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="5b2c9-117">Daha fazla bilgi için bkz: [SharePoint çevrimiçi doğru arama listesinden verileri şablonu tarafından oluşturulan liste görüntülenmeyecek](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span><span class="sxs-lookup"><span data-stu-id="5b2c9-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>

<span data-ttu-id="5b2c9-118">Yaygın sorunlar ve çözümleri hakkında daha ayrıntılı bilgi için lütfen [site şablonları oluşturma ve kullanma](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)denetleyin.</span><span class="sxs-lookup"><span data-stu-id="5b2c9-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



