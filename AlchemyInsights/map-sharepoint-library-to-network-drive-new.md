---
title: SharePoint kitaplığını ağ sürücüsüyle eşle
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 4b8245c3-a179-4524-ae83-0c22d539c202
ms.openlocfilehash: ab1b9a0a7e9f9cd2ffabfb2b5af75401d13207a9
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049177"
---
# <a name="map-a-sharepoint-library-to-a-network-drive"></a><span data-ttu-id="27d91-102">SharePoint kitaplığını ağ sürücüsüyle eşle</span><span class="sxs-lookup"><span data-stu-id="27d91-102">Map a SharePoint library to a network drive</span></span>

<span data-ttu-id="27d91-103">Kitaplığı ağ sürücüsü olarak eşleme geçicidir ve yalnızca Internet Explorer aracılığıyla desteklenir.</span><span class="sxs-lookup"><span data-stu-id="27d91-103">Mapping a library as a network drive is temporary and supported only through Internet Explorer.</span></span> <span data-ttu-id="27d91-104">Oturumun süresinin dolmasını önlemek için zaman zaman Internet Explorer'da SharePoint sitesini açmanız ve **oturumda oturumda oturumda kal** seçeneğini seçmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="27d91-104">You must occasionally open the SharePoint site in Internet Explorer and select **Stay signed in** to prevent the session from expiring.</span></span> <span data-ttu-id="27d91-105">Bunun yerine, SharePoint dosyalarını [Isteğe Bağlı Dosyalar](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e)sağlayan [yeni OneDrive eşitleme istemcisiyle](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88) </a> eşitleyin.</span><span class="sxs-lookup"><span data-stu-id="27d91-105">Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e).</span></span> <span data-ttu-id="27d91-106">Yerel depolama alanı kullanmadan OneDrive'daki tüm dosyalarınıza erişin.</span><span class="sxs-lookup"><span data-stu-id="27d91-106">Access all your files in OneDrive without using local storage space.</span></span>

<span data-ttu-id="27d91-107">[Yeni OneDrive eşitleme istemcisini kullanmak](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)yerine bir sürücüyü eşlemeyi seçerseniz, aşağıdaki makaledeki adımları izlediğinizi sağlayın.</span><span class="sxs-lookup"><span data-stu-id="27d91-107">If you choose to map a drive instead of [using the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88), ensure you follow the steps in the article below.</span></span> 


<span data-ttu-id="27d91-108">**Eşlenen ağ sürücülerini yapılandırma ve sorun giderme**</span><span class="sxs-lookup"><span data-stu-id="27d91-108">**How to configure and troubleshoot mapped network drives**</span></span>


<span data-ttu-id="27d91-109">[Bkz. SharePoint Onlines'a bağlanan eşlenmiş ağ sürücüleri.](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives)</span><span class="sxs-lookup"><span data-stu-id="27d91-109">See [Troubleshoot mapped network drives that connect to SharePoint Onlines](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span></span>

<span data-ttu-id="27d91-110">NOT: Windows 8 veya Windows 7 ile Internet Explorer 10 kullanıyorsanız ve **Access reddedildi** alıyorsanız veya bir sürücü eşleme yaparken Yol **erişilebilir değil,** bu sorunu gidermek için [bu düzeltmeyi](https://support.microsoft.com/help/2846960) yükleyin.</span><span class="sxs-lookup"><span data-stu-id="27d91-110">NOTE:  If you use Internet Explorer 10 with Windows 8 or Windows 7, and receive **Access denied** or **Path is not accessible** when mapping a drive, install [this hotfix](https://support.microsoft.com/help/2846960) to resolve this problem.</span></span> 
