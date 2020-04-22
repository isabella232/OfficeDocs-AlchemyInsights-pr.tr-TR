---
title: Erişim hizmetleri emeklilik
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 977bd5887ef58b328463a9befcd6b47ac55f5a85
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687278"
---
# <a name="access-services-retirement"></a><span data-ttu-id="8d266-102">Erişim hizmetleri emeklilik</span><span class="sxs-lookup"><span data-stu-id="8d266-102">Access services retirement</span></span>

<span data-ttu-id="8d266-103">İlk olarak MC97576'da, Mart 2017'de duyurduğumuz ve geçtiğimiz yıl içinde iletişim kurmaya devam ettiğimiz gibi Erişim Hizmetleri emekliye uymaktadır.</span><span class="sxs-lookup"><span data-stu-id="8d266-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired.</span></span> <span data-ttu-id="8d266-104">Bu işlemin bir sonraki aşaması, SharePoint listelerini temel veri depolama alanı olarak kullanan Access Web Veritabanlarının kaldırılması olacaktır.</span><span class="sxs-lookup"><span data-stu-id="8d266-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="8d266-105">**Bu beni nasıl etkiliyor?**</span><span class="sxs-lookup"><span data-stu-id="8d266-105">**How does this affect me?**</span></span>

<span data-ttu-id="8d266-106">Haziran 2019'dan itibaren SharePoint Online'da yeni Access veritabanları oluşturulmasını durduracağız ve hizmeti ve kalan uygulamaları Nisan 2020'ye kadar kapatacağız.</span><span class="sxs-lookup"><span data-stu-id="8d266-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="8d266-107">**Bu değişikliğe hazırlanmak için ne yapmam gerekiyor?**</span><span class="sxs-lookup"><span data-stu-id="8d266-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="8d266-108">Kuruluşunuzun Access web veritabanları için bir geçiş planı oluşturmanızı öneririz.</span><span class="sxs-lookup"><span data-stu-id="8d266-108">We encourage you to create a transition plan for your organization's Access web databases.</span></span> <span data-ttu-id="8d266-109">Yöneticiler, sitelerin kullandığı Access uygulamalarının envanterini almak için [SharePoint Access uygulama tarayıcısını](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) kullanabilir.</span><span class="sxs-lookup"><span data-stu-id="8d266-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="8d266-110">Access web veritabanları verilerini geçirmenin birkaç yolu vardır:</span><span class="sxs-lookup"><span data-stu-id="8d266-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="8d266-111">Yerel bir Access veritabanına aktarma (. ACCDB) veya bir Excel dosyasına.</span><span class="sxs-lookup"><span data-stu-id="8d266-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="8d266-112">Ayrıca, web ve mobil cihazlar için kodsuz iş çözümleri oluşturmak için Microsoft PowerApps'ı alternatif bir platform olarak keşfetmenizi öneririz.</span><span class="sxs-lookup"><span data-stu-id="8d266-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>