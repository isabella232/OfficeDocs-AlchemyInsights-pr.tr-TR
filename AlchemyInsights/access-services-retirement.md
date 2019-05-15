---
title: Access services emeklilik
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 395dac6abf1562aa0da0b1d87eddd943affefc3f
ms.sourcegitcommit: b2c9202b94fa1ce73dbeb3e43b219ba07e46e7e3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/14/2019
ms.locfileid: "33973958"
---
# <a name="access-services-retirement"></a><span data-ttu-id="eb276-102">Access services emeklilik</span><span class="sxs-lookup"><span data-stu-id="eb276-102">Access services retirement</span></span>

<span data-ttu-id="eb276-103">Biz başlangıçta Mart 2017'de MC97576 duyurulan ve geçen yıl iletişim kurmak devamı olarak Access Services Office 365 ' emekli.</span><span class="sxs-lookup"><span data-stu-id="eb276-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="eb276-104">Sonraki aşama bu işlem SharePoint listelerini, alttaki veri deposu olarak kullanan Access Web veritabanları kaldırılması olacaktır.</span><span class="sxs-lookup"><span data-stu-id="eb276-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

## <a name="how-does-this-affect-me"></a><span data-ttu-id="eb276-105">Nasıl bu beni etkiler mi?</span><span class="sxs-lookup"><span data-stu-id="eb276-105">How does this affect me?</span></span>

<span data-ttu-id="eb276-106">Haziran 2019 başlayarak, biz yeni Access veritabanlarında SharePoint çevrimiçi oluşturulmasını durdurmak ve hizmet ve kalan tüm apps aşağı tarafından Nisan 2020 kapatmak.</span><span class="sxs-lookup"><span data-stu-id="eb276-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

## <a name="what-do-i-need-to-do-to-prepare-for-this-change"></a><span data-ttu-id="eb276-107">Bu değişikliğe hazırlanmak için ne yapmalıyım?</span><span class="sxs-lookup"><span data-stu-id="eb276-107">What do I need to do to prepare for this change?</span></span>

<span data-ttu-id="eb276-108">Kuruluşunuzun Access web veritabanları için bir geçiş planı oluşturmak için önerilir.</span><span class="sxs-lookup"><span data-stu-id="eb276-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="eb276-109">Yöneticileri [SharePoint erişimi app tarayıcı](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0) siteleri kullanarak erişim apps envanterini elde etmek için kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="eb276-109">Admins can use the [SharePoint Access app scanner](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0) to obtain an inventory of the Access apps that sites are using.</span></span> 

<span data-ttu-id="eb276-110">Access web veritabanları veri taşımak için birkaç yolu vardır:</span><span class="sxs-lookup"><span data-stu-id="eb276-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="eb276-111">Yerel bir Access veritabanına alma (. Olmayan ACCDB) veya Excel dosyası.</span><span class="sxs-lookup"><span data-stu-id="eb276-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="eb276-112">Microsoft PowerApps web ve mobil aygıtlar için kod içermeyen iş çözümleri oluşturmak için alternatif bir platform olarak araştırma öneririz.</span><span class="sxs-lookup"><span data-stu-id="eb276-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>