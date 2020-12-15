---
title: Microsoft Edge (Kmuum) için Google Chrome uzantıları
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
ms.openlocfilehash: 2a20f258cbcbca7c8db4e38c52464fefb1b6f39d
ms.sourcegitcommit: 38c87ed786dda7181562492d5d2e7ef0e18e0cab
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678978"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a><span data-ttu-id="1dd69-102">Microsoft Edge (Kmuum) için Google Chrome uzantıları</span><span class="sxs-lookup"><span data-stu-id="1dd69-102">Port Google Chrome extensions to Microsoft Edge (Chromium)</span></span>

<span data-ttu-id="1dd69-103">[Microsoft Edge (Kmıum) Için Google Chrome uzantıları bağlantı noktası](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension)kullanımı kolaydır.</span><span class="sxs-lookup"><span data-stu-id="1dd69-103">It's easy to [port Google Chrome extensions to Microsoft Edge (Chromium)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension).</span></span> <span data-ttu-id="1dd69-104">Çoğu durumda, bu uzantıları Microsoft Edge 'de çalıştırmak için yalnızca en az değişiklik gereklidir.</span><span class="sxs-lookup"><span data-stu-id="1dd69-104">In most cases, only minimal changes are needed to run these extensions on Microsoft Edge.</span></span>

<span data-ttu-id="1dd69-105">Google Chrome tarafından desteklenen uzantı API 'Leri ve bildirim anahtarları Microsoft Edge ile kod uyumludur.</span><span class="sxs-lookup"><span data-stu-id="1dd69-105">The extension APIs and manifest keys supported by Google Chrome are code-compatible with Microsoft Edge.</span></span> <span data-ttu-id="1dd69-106">Bununla birlikte, Microsoft Edge, dahili uzantılar Chrome. gcm, Chrome. Identity. getAccounts, Chrome. Identity. getAuthToken ve Chrome. InstanceId.</span><span class="sxs-lookup"><span data-stu-id="1dd69-106">However, Microsoft Edge does not support the extension APIs chrome.gcm, chrome.identity.getAccounts, chrome.identity.getAuthToken, and chrome.instanceID.</span></span>