---
title: Access services emeklilik
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 8886d7a6fad49e942e17f6a2f3c98542f87aae0b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36495771"
---
# <a name="access-services-retirement"></a><span data-ttu-id="b7fcb-102">Access services emeklilik</span><span class="sxs-lookup"><span data-stu-id="b7fcb-102">Access services retirement</span></span>

<span data-ttu-id="b7fcb-103">Biz başlangıçta Mart 2017'de MC97576 duyurulan ve geçen yıl iletişim kurmak devamı olarak Access Services Office 365 ' emekli.</span><span class="sxs-lookup"><span data-stu-id="b7fcb-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="b7fcb-104">Sonraki aşama bu işlem SharePoint listelerini, alttaki veri deposu olarak kullanan Access Web veritabanları kaldırılması olacaktır.</span><span class="sxs-lookup"><span data-stu-id="b7fcb-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="b7fcb-105">**Nasıl bu beni etkiler mi?**</span><span class="sxs-lookup"><span data-stu-id="b7fcb-105">**How does this affect me?**</span></span>

<span data-ttu-id="b7fcb-106">Haziran 2019 başlayarak, biz yeni Access veritabanlarında SharePoint çevrimiçi oluşturulmasını durdurmak ve hizmet ve kalan tüm apps aşağı tarafından Nisan 2020 kapatmak.</span><span class="sxs-lookup"><span data-stu-id="b7fcb-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="b7fcb-107">**Bu değişikliğe hazırlanmak için ne yapmalıyım?**</span><span class="sxs-lookup"><span data-stu-id="b7fcb-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="b7fcb-108">Kuruluşunuzun Access web veritabanları için bir geçiş planı oluşturmak için önerilir.</span><span class="sxs-lookup"><span data-stu-id="b7fcb-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="b7fcb-109">Yöneticileri [SharePoint erişimi app tarayıcı](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) siteleri kullanarak erişim apps envanterini elde etmek için kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b7fcb-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="b7fcb-110">Access web veritabanları veri taşımak için birkaç yolu vardır:</span><span class="sxs-lookup"><span data-stu-id="b7fcb-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="b7fcb-111">Yerel bir Access veritabanına alma (. Olmayan ACCDB) veya Excel dosyası.</span><span class="sxs-lookup"><span data-stu-id="b7fcb-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="b7fcb-112">Microsoft PowerApps web ve mobil aygıtlar için kod içermeyen iş çözümleri oluşturmak için alternatif bir platform olarak araştırma öneririz.</span><span class="sxs-lookup"><span data-stu-id="b7fcb-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>