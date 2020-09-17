---
title: SharePoint kitaplığını ağ sürücüsüne eşleştirme
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
ms.assetid: 4b8245c3-a179-4524-ae83-0c22d539c202
ms.openlocfilehash: 9115a3ab8d1234127a95628a9a49679ef06f6d39
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806203"
---
# <a name="map-a-sharepoint-library-to-a-network-drive"></a><span data-ttu-id="7d1a2-102">SharePoint kitaplığını ağ sürücüsüne eşleştirme</span><span class="sxs-lookup"><span data-stu-id="7d1a2-102">Map a SharePoint library to a network drive</span></span>

<span data-ttu-id="7d1a2-103">Kitaplığın ağ sürücüsü olarak eşlenmesi geçicidir ve yalnızca Internet Explorer ile desteklenir.</span><span class="sxs-lookup"><span data-stu-id="7d1a2-103">Mapping a library as a network drive is temporary and supported only through Internet Explorer.</span></span> <span data-ttu-id="7d1a2-104">Oturum zaman aşımına uğramak için, zaman zaman SharePoint sitesini Internet Explorer 'da açmalı ve oturum **açmış kalmak** seçeneğini seçmelisiniz.</span><span class="sxs-lookup"><span data-stu-id="7d1a2-104">You must occasionally open the SharePoint site in Internet Explorer and select **Stay signed in** to prevent the session from expiring.</span></span> <span data-ttu-id="7d1a2-105">Bunun yerine, [SharePoint dosyalarını](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88) </a> [isteğe bağlı dosyalar](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e)sağlayan yeni OneDrive eşitleme istemcisiyle eşitleyin.</span><span class="sxs-lookup"><span data-stu-id="7d1a2-105">Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e).</span></span> <span data-ttu-id="7d1a2-106">Yerel depolama alanı kullanmadan OneDrive 'daki tüm dosyalarınıza erişin.</span><span class="sxs-lookup"><span data-stu-id="7d1a2-106">Access all your files in OneDrive without using local storage space.</span></span>

<span data-ttu-id="7d1a2-107">[Yeni OneDrive eşitleme istemcisini kullanmak](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)yerine bir sürücüyü eşlemeyi seçerseniz, aşağıdaki makalede verilen adımları uyguladığınızdan emin olun.</span><span class="sxs-lookup"><span data-stu-id="7d1a2-107">If you choose to map a drive instead of [using the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88), ensure you follow the steps in the article below.</span></span> 


<span data-ttu-id="7d1a2-108">**Eşlenen ağ sürücüleriyle ilgili yapılandırma ve sorunları giderme**</span><span class="sxs-lookup"><span data-stu-id="7d1a2-108">**How to configure and troubleshoot mapped network drives**</span></span>


<span data-ttu-id="7d1a2-109">SharePoint 'te bağlanılan [ağ sürücüleriyle Ilgili sorun giderme](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="7d1a2-109">See [Troubleshoot mapped network drives that connect to SharePoint Onlines](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span></span>

<span data-ttu-id="7d1a2-110">Not: Windows 8 veya Windows 7 ile Internet Explorer 10 kullanıyorsanız ve bir sürücüyü eşleştirirken **erişim reddedildi** veya **yola** erişim izni alıyorsanız, bu sorunu çözmek için [Bu düzeltmeyi](https://support.microsoft.com/help/2846960) yükleyin.</span><span class="sxs-lookup"><span data-stu-id="7d1a2-110">NOTE:  If you use Internet Explorer 10 with Windows 8 or Windows 7, and receive **Access denied** or **Path is not accessible** when mapping a drive, install [this hotfix](https://support.microsoft.com/help/2846960) to resolve this problem.</span></span> 
