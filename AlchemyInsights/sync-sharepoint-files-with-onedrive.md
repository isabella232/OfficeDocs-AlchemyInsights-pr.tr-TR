---
title: SharePoint Online’daki “Explorer ile Aç” sorunlarını giderme
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 8/7/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: 21a0c193b752342d47189dda73d171249153f7fc
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050833"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="98dfd-102">SharePoint Online’daki “Explorer ile Aç” sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="98dfd-102">Troubleshoot “Open with Explorer” issues in SharePoint Online</span></span>

<span data-ttu-id="98dfd-103">Gezgin ile Aç komutu, SharePoint sitesini barındıran sunucudaki klasör yapısını görüntüleyen yerel bir Windows Gezgini örneğini açar.</span><span class="sxs-lookup"><span data-stu-id="98dfd-103">The Open with Explorer command opens a local instance of Windows Explorer that displays the folder structure on the server that hosts the SharePoint site.</span></span> <span data-ttu-id="98dfd-104">Bununla birlikte, dosyalarınıza yerel erişim sağladığından ve en iyi performansı sunduğundan [İsteğe Bağlı Dosyalar](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) sağlayan [yeni OneDrive eşitleme istemcisiyle SharePoint dosyalarını eşitlemenizi](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> öneririz.</span><span class="sxs-lookup"><span data-stu-id="98dfd-104">This being said, we recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>


<span data-ttu-id="98dfd-105">Yeni OneDrive eşitleme istemcisi yerine Gezgin görünümünü kullanmayı seçtiyseniz şu makalelerde verilen adımları ve en iyi yöntemleri izlediğinizden emin olun:</span><span class="sxs-lookup"><span data-stu-id="98dfd-105">If you chose to use Explorer view instead of using the new OneDrive sync client, make sure you follow the steps and best practices in the following articles:</span></span>

- [<span data-ttu-id="98dfd-106">SharePoint Online’daki sorunları gidermek için ”Gezgin ile Aç” komutunu kullanma</span><span class="sxs-lookup"><span data-stu-id="98dfd-106">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer)

- [<span data-ttu-id="98dfd-107">Gezgin ile Aç’ı kullanarak kitaplık dosyalarını kopyalama veya taşıma</span><span class="sxs-lookup"><span data-stu-id="98dfd-107">Copy or move library files by using Open with Explorer</span></span>](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)

> [!Note]  
> <span data-ttu-id="98dfd-108">**Gezgin ile Aç** düğmesi yeni kitaplık deneyiminde gösterilmez.</span><span class="sxs-lookup"><span data-stu-id="98dfd-108">The **Open with Explorer** button doesn't appear in the new library experience.</span></span> <span data-ttu-id="98dfd-109">Sağ üst kısımdaki **Görünüm** açılan listesini seçin (geçerli görünümünüze bağlı olarak açılan listenin adı değişir) ve sonra da **Dosya Gezgini’nde Görünüm**’e tıklayın.</span><span class="sxs-lookup"><span data-stu-id="98dfd-109">Select the **View** drop-down in the upper right (the name of the drop-down changes depending on your current view), and then select **View in File Explorer**.</span></span>
>
 ><span data-ttu-id="98dfd-110">SharePoint'in Gezgin ile Aç komutu ActiveX denetimlerini kullanır, bu nedenle yalnızca Internet Explorer 10 veya 11’de desteklenir.</span><span class="sxs-lookup"><span data-stu-id="98dfd-110">SharePoint Open with Explorer uses ActiveX controls, so it's only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="98dfd-111">Explorer ile Aç komutu Windows’da Microsoft Edge, Google Chrome, Mozilla Firefox ile veya Mac platformunda çalışmaz.</span><span class="sxs-lookup"><span data-stu-id="98dfd-111">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="98dfd-112">Bu nedenle Gezgin Görünümü seçeneği soluk görünebilir.</span><span class="sxs-lookup"><span data-stu-id="98dfd-112">Due to this reason, the Explorer View option may be grayed out.</span></span>
>
> - <span data-ttu-id="98dfd-113">[SharePoint şerit düğmeleri neden kullanılamıyor veya soluk görüntüleniyor?](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca)</span><span class="sxs-lookup"><span data-stu-id="98dfd-113">[Why SharePoint ribbon buttons are unavailable or grayed out](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span></span>
  

