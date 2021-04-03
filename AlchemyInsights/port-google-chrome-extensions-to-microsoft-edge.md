---
title: Microsoft Edge'e (Chromium) Google Chrome uzantıları bağlantı noktası
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004032"
- "7102"
- "8297"
- "9004617"
ms.openlocfilehash: 1c71d74d01c1e38e4c7789aea2c0b43701b3a5de
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505304"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a><span data-ttu-id="3fbb3-102">Microsoft Edge'e (Chromium) Google Chrome uzantıları bağlantı noktası</span><span class="sxs-lookup"><span data-stu-id="3fbb3-102">Port Google Chrome extensions to Microsoft Edge (Chromium)</span></span>

<span data-ttu-id="3fbb3-103">Google Chrome uzantılarını [Microsoft Edge'e (Chromium) kolayca](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension)taşınabilir.</span><span class="sxs-lookup"><span data-stu-id="3fbb3-103">It's easy to [port Google Chrome extensions to Microsoft Edge (Chromium)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension).</span></span> <span data-ttu-id="3fbb3-104">Çoğu durumda, bu uzantıları Microsoft Edge'de çalıştırmak için yalnızca az değişiklik gereklidir.</span><span class="sxs-lookup"><span data-stu-id="3fbb3-104">In most cases, only minimal changes are needed to run these extensions on Microsoft Edge.</span></span>

<span data-ttu-id="3fbb3-105">Google Chrome tarafından desteklenen uzantı API'leri ve bildirim anahtarları Microsoft Edge ile kodla uyumludur.</span><span class="sxs-lookup"><span data-stu-id="3fbb3-105">The extension APIs and manifest keys supported by Google Chrome are code-compatible with Microsoft Edge.</span></span> <span data-ttu-id="3fbb3-106">Bununla birlikte, Microsoft Edge API'ler chrome.obm, chrome.identity.getAccounts, chrome.identity.getAuthToken ve chrome.instanceID uzantılarını desteklemez.</span><span class="sxs-lookup"><span data-stu-id="3fbb3-106">However, Microsoft Edge does not support the extension APIs chrome.gcm, chrome.identity.getAccounts, chrome.identity.getAuthToken, and chrome.instanceID.</span></span>