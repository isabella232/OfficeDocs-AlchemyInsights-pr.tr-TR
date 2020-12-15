---
title: Office 'in önceki MSI sürümlerini kaldırma
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003886"
- "6940"
ms.openlocfilehash: 26ab610cb204149536bd23c830a1b8558892a7c0
ms.sourcegitcommit: c033720921cb9a06b9560eedef4f1935e69a846b
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/15/2020
ms.locfileid: "49680779"
---
# <a name="remove-prior-msi-versions-of-office"></a><span data-ttu-id="72ea0-102">Office 'in önceki MSI sürümlerini kaldırma</span><span class="sxs-lookup"><span data-stu-id="72ea0-102">Remove prior MSI versions of Office</span></span>

<span data-ttu-id="72ea0-103">Office 365 ProPlus 'ı yüklemeden önce Office 'in önceki Windows Installer (MSI) sürümlerini kaldırmanızı tavsiye ediyorum.</span><span class="sxs-lookup"><span data-stu-id="72ea0-103">I recommend removing prior Windows Installer (MSI) versions of Office before installing Office 365 ProPlus.</span></span> <span data-ttu-id="72ea0-104">Bunu şöyle yapabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="72ea0-104">Here's how to do this:</span></span>

1. <span data-ttu-id="72ea0-105">Office 'i yüklemek için MSI kullandıysanız Office 'i kaldırmak için Office dağıtım aracı 'nı (ODT) kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="72ea0-105">If you used MSI to install Office, you can use the Office Deployment Tool (ODT) to uninstall Office.</span></span> <span data-ttu-id="72ea0-106">**configuration.xml** dosyanızda removemsi öğesini kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="72ea0-106">You can use the RemoveMSI element in your **configuration.xml** file.</span></span>
1. <span data-ttu-id="72ea0-107">Bu makaledeki yönergeleri izleyin: [Office 365 güvenlik & Uyumluluk Merkezi.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="72ea0-107">Follow the instruction in this article: [Office 365 Security & Compliance Center.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span></span>