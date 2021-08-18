---
title: SharePoint kitaplığını ağ sürücüsüne eşleme
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
ms.openlocfilehash: 741d22c4231886b385b0bc2361e429929ef58f4b84d56e51186f129fc5d07921
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57901608"
---
# <a name="map-a-sharepoint-library-to-a-network-drive"></a>SharePoint kitaplığını ağ sürücüsüne eşleme

Ağ sürücüsüne eşlemek yerine, SharePoint Files On-Demand sağlayan OneDrive eşitleme istemcisini kullanarak eşitlenin. Yerel depolama alanı olmadan OneDrive tüm dosyalarınıza erişin. Daha fazla bilgi için [bkz. SharePoint](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88) ve Teams dosyaları bilgisayarınızla eşitleme ve OneDrive Için Files [On-Demand ile diskte yer Windows 10.](https://support.microsoft.com/office/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e)

Yeni sürücü istemcisini kullanmak yerine bir sürücüyü [eşlemeyi OneDrive eşitleme](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88)şu adımları izle mutlaka kullanın:

- [SharePoint Online'a bağlanan eşlenmiş ağ sürücülerinin sorunlarını giderme](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives)

- [İstemcinin TLS 1.2 desteğine sahip olmayan kimlik doğrulama hataları oluşur](https://docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support#network-drive-mapped-to-a-sharepoint-library)  

**NOT:** Internet Explorer 10 Windows 8 veya Windows 7 kullanıyorsanız ve bir sürücüyü eşlerken **Access**  reddedildi veya Yol erişilebilir değil hatasını alırsanız, bu düzeltmeyi yükleyerek bu sorunu [giderin.](https://support.microsoft.com/topic/error-when-you-open-a-sharepoint-document-library-in-windows-explorer-or-map-a-network-drive-to-the-library-after-you-install-internet-explorer-10-96e640ba-059f-9b09-bb91-2a0319ee8b1d)