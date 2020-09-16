---
title: SharePoint Online 'da site oluşturma
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732264"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="135aa-102">Şablonları kullanarak SharePoint siteleri oluşturma</span><span class="sxs-lookup"><span data-stu-id="135aa-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="135aa-103">Siteyi şablon olarak kaydetme özelliği modern Iletişimde veya ekip sitelerinde desteklenmez.</span><span class="sxs-lookup"><span data-stu-id="135aa-103">The ability to save a site as a template is not supported with modern Communication or Team Sites.</span></span> <span data-ttu-id="135aa-104">Şablonları kullanma hakkında daha fazla bilgi için [, SharePoint sitesini şablon olarak kaydetme, indirme ve karşıya yükleme](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template)bölümüne bakın.</span><span class="sxs-lookup"><span data-stu-id="135aa-104">For more information about using templates see [Save, download and upload a SharePoint site as a template](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span></span>

<span data-ttu-id="135aa-105">SharePoint Online 'da bir site veya listeyi şablon olarak kaydetme ile ilgili bazı yaygın sorun/çözümleri aşağıda bulabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="135aa-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="135aa-106">**Site/liste şablonunu Kaydet düğmesi kullanılamıyor veya yok**</span><span class="sxs-lookup"><span data-stu-id="135aa-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="135aa-107">Yöneticilerin şablon özelliklerini etkinleştirmesi için özel komut dosyasına Izin vermesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="135aa-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="135aa-108">Ayrıntılı adımlar için, örnekler ve hususlar</span><span class="sxs-lookup"><span data-stu-id="135aa-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="135aa-109">Özel Betik</span><span class="sxs-lookup"><span data-stu-id="135aa-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="135aa-110">Siteyi şablon olarak Kaydet komutu desteklenmediğinden SharePoint Server yayımlama altyapısını kullanan sitelerde sorunlara neden olabilir.</span><span class="sxs-lookup"><span data-stu-id="135aa-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="135aa-111">**Site şablonu oluşturulamıyor veya düzgün çalışmıyor**</span><span class="sxs-lookup"><span data-stu-id="135aa-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="135aa-112">Şablonda bir [özellik](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) eksik olabilir ve etkinleştirilmeyecektir.</span><span class="sxs-lookup"><span data-stu-id="135aa-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="135aa-113">Özellik geçerli site koleksiyonunda etkinleştirme için kullanılamıyorsa site şablonunu kullanarak site oluşturmaya kullanamazsınız.</span><span class="sxs-lookup"><span data-stu-id="135aa-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="135aa-114">Herhangi bir liste veya kitaplıkta 5000 öğelerinin [liste görünümü sınırı eşiğini](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) aşmadığını denetleyin, bu da bir site şablonunun oluşturulmasını engelleyebilir.</span><span class="sxs-lookup"><span data-stu-id="135aa-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="135aa-115">Site çok fazla kaynak kullanıyor olabilir ve bu nedenle site şablonu 50 MB sınırını aşıyor.</span><span class="sxs-lookup"><span data-stu-id="135aa-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="135aa-116">Arama sütunu kullanan bir listeden verileri görüntülerken sorun çıktı.</span><span class="sxs-lookup"><span data-stu-id="135aa-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="135aa-117">Daha fazla bilgi için, [şablon tarafından oluşturulan liste, SharePoint Online 'daki doğru arama listesinden verileri görüntülemez](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="135aa-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="135aa-118">Sık karşılaşılan sorunlar ve çözümleri hakkında daha ayrıntılı bilgi için lütfen [site şablonlarını oluşturma ve kullanma](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)seçeneğini işaretleyin.</span><span class="sxs-lookup"><span data-stu-id="135aa-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



