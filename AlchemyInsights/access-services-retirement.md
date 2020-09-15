---
title: Access Hizmetleri emekli
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 943066d5ac76c0630554ee724bbab9a94086fae4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698702"
---
# <a name="access-services-retirement"></a><span data-ttu-id="51928-102">Access Hizmetleri emekli</span><span class="sxs-lookup"><span data-stu-id="51928-102">Access services retirement</span></span>

<span data-ttu-id="51928-103">Başlangıçta 2017 Mart ' de duyuruluyor ve geçmiş yıl erişim Hizmetleri üzerinden iletişim kurmaya devam ediyor.</span><span class="sxs-lookup"><span data-stu-id="51928-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired.</span></span> <span data-ttu-id="51928-104">Bu işlemin sonraki aşaması, SharePoint listelerini temel aldığı veri deposu olarak kullanan Access Web veritabanlarının kaldırılması olacaktır.</span><span class="sxs-lookup"><span data-stu-id="51928-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="51928-105">**Bu, beni nasıl etkiler?**</span><span class="sxs-lookup"><span data-stu-id="51928-105">**How does this affect me?**</span></span>

<span data-ttu-id="51928-106">2019 Haziran 'da, SharePoint Online 'da yeni Access veritabanları oluşturulmasını durdururız ve hizmeti ve kalan uygulamaları 2020 Nisan tarafından kapatılacak.</span><span class="sxs-lookup"><span data-stu-id="51928-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="51928-107">**Bu değişikliğe hazırlanmak için ne yapmam gerekiyor?**</span><span class="sxs-lookup"><span data-stu-id="51928-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="51928-108">Kuruluşunuzun Access Web veritabanları için bir geçiş planı oluşturmanızı öneririz.</span><span class="sxs-lookup"><span data-stu-id="51928-108">We encourage you to create a transition plan for your organization's Access web databases.</span></span> <span data-ttu-id="51928-109">Yöneticiler, sitelerin kullandığı Access uygulamalarının envanterini almak için [SharePoint Access uygulaması tarayıcısını](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) kullanabilirler.</span><span class="sxs-lookup"><span data-stu-id="51928-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="51928-110">Access Web veritabanı verilerini geçirmek için birkaç yol vardır:</span><span class="sxs-lookup"><span data-stu-id="51928-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="51928-111">Yerel Access veritabanına (. ACCDB) veya Excel dosyasına gidin.</span><span class="sxs-lookup"><span data-stu-id="51928-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="51928-112">Ayrıca, Web ve mobil cihazlar için kod içermeyen iş çözümleri oluşturmaya yönelik alternatif bir platform olarak Microsoft PowerApps araştırmayı öneririz.</span><span class="sxs-lookup"><span data-stu-id="51928-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>