---
title: Microsoft Edge'i Microsoft Intune'a ekleme
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8240"
- "9004604"
ms.openlocfilehash: d56c65910d1c2170d3e0ce9676e913663701db96
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194579"
---
# <a name="add-microsoft-edge-to-microsoft-intune"></a><span data-ttu-id="af14a-102">Microsoft Edge'i Microsoft Intune'a ekleme</span><span class="sxs-lookup"><span data-stu-id="af14a-102">Add Microsoft Edge to Microsoft Intune</span></span>

<span data-ttu-id="af14a-103">Windows 10 için Microsoft Edge'i dağıtmak, yapılandırmak, izlemek ve korumak için önce Microsoft Intune'a eklemeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="af14a-103">To be able to deploy, configure, monitor, and protect Microsoft Edge for Windows 10, you must first add it to Microsoft Intune.</span></span>

> [!IMPORTANT]
- <span data-ttu-id="af14a-104">Intune, Microsoft Edge 77 ve sonraki sürümleri destekler.</span><span class="sxs-lookup"><span data-stu-id="af14a-104">Intune supports Microsoft Edge 77 and later versions.</span></span>
- <span data-ttu-id="af14a-105">Intune, Microsoft Edge'in önceden var olan tüm yüklemelerini algılar.</span><span class="sxs-lookup"><span data-stu-id="af14a-105">Intune will detect any pre-existing installations of Microsoft Edge.</span></span>
- <span data-ttu-id="af14a-106">Microsoft Edge kullanıcı bağlamında yüklüyse, sistem yüklemesi kullanıcı bağlamında yüklemenin üzerine yazacak.</span><span class="sxs-lookup"><span data-stu-id="af14a-106">If Microsoft Edge is installed in user context, a system installation will overwrite the installation in user context.</span></span>
- <span data-ttu-id="af14a-107">Microsoft Edge sistem bağlamında yüklenirse, yükleme başarısı bildiriliyor.</span><span class="sxs-lookup"><span data-stu-id="af14a-107">If Microsoft Edge is installed in system context, the installation success will be reported.</span></span>
- <span data-ttu-id="af14a-108">Kullanıcı bağlamında tüm kanallar için önceden yüklenmiş Microsoft Edge 77 ve sonraki sürümlerin üzerine, sistem bağlamında Microsoft Edge yüklenmiş olarak yazılır.</span><span class="sxs-lookup"><span data-stu-id="af14a-108">Pre-installed Microsoft Edge 77 and later versions, for all channels in user context, will be overwritten with Microsoft Edge installed in system context.</span></span>

<span data-ttu-id="af14a-109">**Önkoşul**</span><span class="sxs-lookup"><span data-stu-id="af14a-109">**Prerequisite**</span></span>

<span data-ttu-id="af14a-110">Windows 10 sürüm 1709 veya sonraki sürümleri</span><span class="sxs-lookup"><span data-stu-id="af14a-110">Windows 10 version 1709 or later versions</span></span>

<span data-ttu-id="af14a-111">**Intune'a Edge ekleme adımları**</span><span class="sxs-lookup"><span data-stu-id="af14a-111">**Steps to add Edge to Intune**</span></span>

1. <span data-ttu-id="af14a-112">[Intune'da uygulamayı yapılandırma.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="af14a-112">[Configure the app in Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
2. <span data-ttu-id="af14a-113">[Uygulama bilgilerini yapılandırma.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="af14a-113">[Configure the app information](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
3. <span data-ttu-id="af14a-114">[Uygulama ayarlarını yapılandırma.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="af14a-114">[Configure the app settings](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
4. <span data-ttu-id="af14a-115">[Kapsam etiketlerini seçin (isteğe bağlı).](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="af14a-115">[Select the scope tags (optional)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
5. <span data-ttu-id="af14a-116">[Uygulamayı ekleyin.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="af14a-116">[Add the app](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>

<span data-ttu-id="af14a-117">Daha fazla yardım için Sorun [Giderme'ye bakın.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="af14a-117">For more help, see [Troubleshooting](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>




