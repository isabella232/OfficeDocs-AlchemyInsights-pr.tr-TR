---
title: Bing'de Microsoft Arama için arka plan hizmetini kaldırma
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816341"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a><span data-ttu-id="ddd99-102">Bing'de Microsoft Arama için arka plan hizmetini kaldırma</span><span class="sxs-lookup"><span data-stu-id="ddd99-102">Remove the background service for Microsoft Search in Bing</span></span>

<span data-ttu-id="ddd99-103">Bing'de Microsoft Arama'nın arka plan hizmetini kaldırmak için aşağıdaki çözümlerini deneyin:</span><span class="sxs-lookup"><span data-stu-id="ddd99-103">To remove the background service for Microsoft Search in Bing, you can try the following remedies:</span></span>

1. <span data-ttu-id="ddd99-104">Özgün arama alt yapısı ayarlarına geri dönmek için aşağıdaki işlemi yapın:</span><span class="sxs-lookup"><span data-stu-id="ddd99-104">To revert to the original search engine settings, do the following things:</span></span>

    <span data-ttu-id="ddd99-105">a.</span><span class="sxs-lookup"><span data-stu-id="ddd99-105">a.</span></span> <span data-ttu-id="ddd99-106">**Bing'i varsayılan arama motorunuz olarak kullan [iki durumlu düğmeyi](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) kapatın.**</span><span class="sxs-lookup"><span data-stu-id="ddd99-106">Switch the **Use Bing as your default search engine [toggle](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) Off**.</span></span>

    <span data-ttu-id="ddd99-107">b.</span><span class="sxs-lookup"><span data-stu-id="ddd99-107">b.</span></span> <span data-ttu-id="ddd99-108">[Microsoft 365 yönetim merkezine gidin](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) ve kuruluşta bulunan tüm kullanıcıları etkileyen ayarın temizlerini seçin.</span><span class="sxs-lookup"><span data-stu-id="ddd99-108">[Go to the Microsoft 365 admin center](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) and clear the setting that affects all users in your organization.</span></span>

2. <span data-ttu-id="ddd99-109">Tek bir cihazdan arka plan hizmetini kaldırmak için aşağıdaki görevleri yapın:</span><span class="sxs-lookup"><span data-stu-id="ddd99-109">To remove the background service from an individual device, do the following tasks:</span></span>

    <span data-ttu-id="ddd99-110">a.</span><span class="sxs-lookup"><span data-stu-id="ddd99-110">a.</span></span> <span data-ttu-id="ddd99-111">Programlar **ve Özellikler > Denetim > Seçin.**</span><span class="sxs-lookup"><span data-stu-id="ddd99-111">Choose **Control Panel > Programs > Programs and Features**.</span></span>

    <span data-ttu-id="ddd99-112">b.</span><span class="sxs-lookup"><span data-stu-id="ddd99-112">b.</span></span> <span data-ttu-id="ddd99-113">Yüklü programlar **listesinin altındaki Bing'de Microsoft** Arama'ya sağ tıklayın ve sonra Kaldır'a **tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="ddd99-113">Right-click **Microsoft Search in Bing** under the list of installed programs, and then click **Uninstall**.</span></span>

3. <span data-ttu-id="ddd99-114">Arka plan hizmetini kurumdaki birden çok cihazdan kaldırmak için, yönetici olarak oturum açın ve betikte aşağıdaki komutu çalıştırın:</span><span class="sxs-lookup"><span data-stu-id="ddd99-114">To remove the background service from multiple devices in your organization, log in as an administrator and run the following command in a script:</span></span> 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
