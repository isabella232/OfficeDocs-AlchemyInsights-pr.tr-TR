---
title: SharePoint kitaplığı için bir ağ sürücüsüne
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 12/17/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 4b8245c3-a179-4524-ae83-0c22d539c202
ms.openlocfilehash: 7bb1f7d1b77ec5850109c9553ddfd894b3823946
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34754834"
---
# <a name="map-a-sharepoint-library-to-a-network-drive"></a><span data-ttu-id="9d440-102">SharePoint kitaplığı için bir ağ sürücüsüne</span><span class="sxs-lookup"><span data-stu-id="9d440-102">Map a SharePoint library to a network drive</span></span>

<span data-ttu-id="9d440-103">Kitaplık olarak bir ağ sürücüsünü eşleme geçici ve yalnızca Internet Explorer üzerinden desteklenen.</span><span class="sxs-lookup"><span data-stu-id="9d440-103">Mapping a library as a network drive is temporary and supported only through Internet Explorer.</span></span> <span data-ttu-id="9d440-104">Bazen, SharePoint sitesini Internet Explorer'da açın ve oturum zaman aşımına uğramasını önlemek için "Oturum Kal" seçmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="9d440-104">You must occasionally open the SharePoint site in Internet Explorer and select "Stay signed in" to prevent the session from expiring.</span></span> <span data-ttu-id="9d440-105">Bunun yerine, [Yeni OneDrive eşitleme istemcisi ile SharePoint dosyaları eşitleme](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88) </a> [Talep dosyaları](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e)sağlar.</span><span class="sxs-lookup"><span data-stu-id="9d440-105">Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e).</span></span> <span data-ttu-id="9d440-106">Tüm dosyalarınızı OneDrive yerel depolama alanını kullanmadan erişir.</span><span class="sxs-lookup"><span data-stu-id="9d440-106">Access all your files in OneDrive without using local storage space.</span></span>

<span data-ttu-id="9d440-107">[Yeni OneDrive eşitleme istemcisini kullanmak](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)yerine sürücüsüne seçerseniz, aşağıdaki makalede yer alan adımları izleyin emin olun.</span><span class="sxs-lookup"><span data-stu-id="9d440-107">If you choose to map a drive instead of[using the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88), ensure you follow the steps in the article below.</span></span> 


<span data-ttu-id="9d440-108">**Eşlenen ağ sürücülerine yazmalarını yapılandırma ve sorun giderme**</span><span class="sxs-lookup"><span data-stu-id="9d440-108">**How to configure and troubleshoot mapped network drives**</span></span>


- <span data-ttu-id="9d440-109">[Yapılandırmak ve eşleştirilmiş ağ sürücüleri ile ilgili sorunları giderme](https://support.office.com/article/troubleshoot-mapped-network-drives-that-connect-to-sharepoint-online-ef399c67-4578-4c3a-adbe-0b489084eabe?ui=en-US&amp;rs=en-US&amp;ad=US).</span><span class="sxs-lookup"><span data-stu-id="9d440-109">[Configure and to troubleshoot mapped network drives](https://support.office.com/article/troubleshoot-mapped-network-drives-that-connect-to-sharepoint-online-ef399c67-4578-4c3a-adbe-0b489084eabe?ui=en-US&amp;rs=en-US&amp;ad=US).</span></span>

<span data-ttu-id="9d440-110">Not: Internet Explorer 10 Windows 8 veya Windows 7'de "Erişim reddedildi" almak veya "Yol erişilemez" için bir sürücü varsa, bu sorunu gidermek için bu düzeltmeyi yükleyin.</span><span class="sxs-lookup"><span data-stu-id="9d440-110">NOTE:  For Internet Explorer 10 with Windows 8 or Windows 7 that receive "Access denied" or "Path is not accessible" when mapping a drive, install this hotfix to resolve this problem.</span></span> <span data-ttu-id="9d440-111">[SharePoint belge kitaplığı Windows Gezgini'nde açtığınızda veya Internet Explorer 10 yükledikten sonra kitaplık için bir ağ sürücüsüne hata](https://support.microsoft.com/help/2846960)Git.</span><span class="sxs-lookup"><span data-stu-id="9d440-111">Go to [Error when you open a SharePoint Document Library in Windows Explorer or map a network drive to the library after you install Internet Explorer 10](https://support.microsoft.com/help/2846960).</span></span>
