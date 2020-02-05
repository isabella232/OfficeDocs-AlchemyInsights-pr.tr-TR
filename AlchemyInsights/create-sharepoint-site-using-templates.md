---
title: SharePoint Online'da site oluşturma
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b9009fdbdc2a5e7443151446daade1685d2f5d45
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770443"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="9729b-102">Şablonları kullanarak SharePoint siteleri oluşturma</span><span class="sxs-lookup"><span data-stu-id="9729b-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="9729b-103">Bir siteyi şablon olarak kaydetme özelliği, modern İletişim veya Ekip Siteleri ile desteklenmez.</span><span class="sxs-lookup"><span data-stu-id="9729b-103">The ability to save a site as a template is not supported with modern Communication or Team Sites.</span></span> <span data-ttu-id="9729b-104">Şablonları kullanma hakkında daha fazla bilgi için, [SharePoint sitesini şablon olarak kaydet, indir ve yükleyin.](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template)</span><span class="sxs-lookup"><span data-stu-id="9729b-104">For more information about using templates see [Save, download and upload a SharePoint site as a template](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span></span>

<span data-ttu-id="9729b-105">Sharepoint Online'da bir Siteyi veya Listeyi şablon olarak kaydetmeyle ilgili bazı sık karşılaşılan sorunlar/çözümler aşağıda verilmiştir.</span><span class="sxs-lookup"><span data-stu-id="9729b-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="9729b-106">**Site/liste şablonu kaydet düğmesi kullanılamıyor veya eksik**</span><span class="sxs-lookup"><span data-stu-id="9729b-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="9729b-107">Yöneticilerin şablon özelliklerini etkinleştirmek için Özel Komut Dosyasına İzin Vermeleri gerekir.</span><span class="sxs-lookup"><span data-stu-id="9729b-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="9729b-108">Ayrıntılı adımlar, örnekler ve hususlar için bkz.</span><span class="sxs-lookup"><span data-stu-id="9729b-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="9729b-109">Özel komut dosyasına izin verme veya engelleme</span><span class="sxs-lookup"><span data-stu-id="9729b-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="9729b-110">Şablon komutu olarak kaydet sitesi desteklenmez ve SharePoint Server Yayımlama Altyapısını kullanan sitelerde sorunlara neden olabilir.</span><span class="sxs-lookup"><span data-stu-id="9729b-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="9729b-111">**Site şablonu oluşturulamıyor veya doğru çalışmıyor**</span><span class="sxs-lookup"><span data-stu-id="9729b-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="9729b-112">Şablon bir [özellik](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) eksik olabilir ve etkinleştirilmez.</span><span class="sxs-lookup"><span data-stu-id="9729b-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="9729b-113">Özellik geçerli site koleksiyonunda etkinleştirmek için kullanılamıyorsa, site şablonunu bir site oluşturmak için kullanamazsınız.</span><span class="sxs-lookup"><span data-stu-id="9729b-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="9729b-114">Herhangi bir liste veya kitaplık, bir site şablonunun oluşturulmasını engelleyebilir gibi 5000 öğe liste [görünümü sınır eşiği](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) aşAbilir olup olmadığını görmek için denetleyin.</span><span class="sxs-lookup"><span data-stu-id="9729b-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="9729b-115">Site çok fazla kaynak kullanıyor olabilir ve bu nedenle site şablonu 50 MB sınırını aşıyor.</span><span class="sxs-lookup"><span data-stu-id="9729b-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="9729b-116">Arama sütunu kullanan bir listeden veri görüntülemede sorunlar vardır.</span><span class="sxs-lookup"><span data-stu-id="9729b-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="9729b-117">Daha fazla bilgi için bkz: [Şablon tarafından oluşturulan liste SharePoint Online'da doğru arama listesinden veri görüntülemiyor.](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)</span><span class="sxs-lookup"><span data-stu-id="9729b-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="9729b-118">Sık karşılaşılan sorunlar ve çözümler hakkında daha ayrıntılı bilgi için lütfen [site şablonları oluştur ve bunları kullanın.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)</span><span class="sxs-lookup"><span data-stu-id="9729b-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



