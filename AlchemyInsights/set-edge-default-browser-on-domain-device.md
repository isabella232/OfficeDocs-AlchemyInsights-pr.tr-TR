---
title: Etki alanına katılmış bir cihazda Microsoft Edge'i varsayılan tarayıcı olarak ayarlama
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: f51a455ea15b7bd92f548f2c1717be9888b43d07
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491875"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-domain-joined-device"></a><span data-ttu-id="ebb6a-102">Etki alanına katılmış bir cihazda Microsoft Edge'i varsayılan tarayıcı olarak ayarlama</span><span class="sxs-lookup"><span data-stu-id="ebb6a-102">Set Microsoft Edge as the default browser on a domain-joined device</span></span>

<span data-ttu-id="ebb6a-103">Microsoft Edge'i varsayılan tarayıcı olarak ayarlayın:</span><span class="sxs-lookup"><span data-stu-id="ebb6a-103">Set Microsoft Edge as the default browser:</span></span> 

1. <span data-ttu-id="ebb6a-104">[Varsayılan bir ilişkilendirme yapılandırma dosyası oluşturun ve dosyayı](https://go.microsoft.com/fwlink/?linkid=2132437) yerel olarak veya ağ paylaşımında depolar.</span><span class="sxs-lookup"><span data-stu-id="ebb6a-104">[Create a default associations configuration file](https://go.microsoft.com/fwlink/?linkid=2132437) and store it locally or on a network share.</span></span>

1. <span data-ttu-id="ebb6a-105">Grup İlkesi düzenleyicisini açın ve ardından Bilgisayar Yapılandırması Yönetim Şablonları  >    >  **Windows Bileşenleri Dosya**  >  **Gezgini'ne gidin.**</span><span class="sxs-lookup"><span data-stu-id="ebb6a-105">Open the Group Policy editor, and then go to **Computer Configuration** > **Administrative Templates** > **Windows Components** > **File Explorer**.</span></span>

1. <span data-ttu-id="ebb6a-106">Varsayılan **ilişkilendirme yapılandırma dosyasını ayarla'ya seçin.**</span><span class="sxs-lookup"><span data-stu-id="ebb6a-106">Select **Set a default associations configuration file**.</span></span>

1. <span data-ttu-id="ebb6a-107">İlke **ayarını ve** ardından Etkin'i **seçin.**</span><span class="sxs-lookup"><span data-stu-id="ebb6a-107">Select **Policy setting**, and then select **Enabled**.</span></span>

1. <span data-ttu-id="ebb6a-108">**Seçenekler'in** altında, varsayılan ilişkilendirme yapılandırma dosyanızı girin ve Tamam'ı **seçin.**</span><span class="sxs-lookup"><span data-stu-id="ebb6a-108">Under **Options**, enter the location of your default associations configuration file, and then select **OK**.</span></span>
