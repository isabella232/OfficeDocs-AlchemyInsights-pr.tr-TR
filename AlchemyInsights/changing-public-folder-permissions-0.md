---
title: Ortak klasör izinlerini değiştirme
ms.author: dmaguire
author: msdmaguire
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "633"
- "3500007"
ms.assetid: 0c37ab75-c81c-44e7-bda8-ea43263f9fdf
ms.openlocfilehash: a2a902e8fdfd8628772364c173979c633d25a169
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47714267"
---
# <a name="changing-public-folder-permissions"></a><span data-ttu-id="d3e6c-102">Ortak klasör izinlerini değiştirme</span><span class="sxs-lookup"><span data-stu-id="d3e6c-102">Changing public folder permissions</span></span>

<span data-ttu-id="d3e6c-103">Ortak klasör izinleri Outlook 'taki kullanıcılar ve yöneticiler tarafından değiştirilebilir.</span><span class="sxs-lookup"><span data-stu-id="d3e6c-103">Public folder permissions can be changed by users and administrators in Outlook.</span></span> <span data-ttu-id="d3e6c-104">Yöneticiler, aşağıdakileri yaparak Exchange Yönetim Merkezi 'nden (EAC) izinleri denetleyebilir:</span><span class="sxs-lookup"><span data-stu-id="d3e6c-104">Administrators can also control permissions from the Exchange Admin Center (EAC), by doing the following:</span></span>
  
1. <span data-ttu-id="d3e6c-105">Microsoft 365 Yönetim merkezinde, **Yönetim Merkezleri** \> **Exchange**'e gidin.</span><span class="sxs-lookup"><span data-stu-id="d3e6c-105">In the Microsoft 365 admin center, go to **Admin centers** \> **Exchange**.</span></span>

2. <span data-ttu-id="d3e6c-106">**Ortak klasörler**'i seçin.</span><span class="sxs-lookup"><span data-stu-id="d3e6c-106">Select **Public folders**.</span></span>

3. <span data-ttu-id="d3e6c-107">Burada, izinler için güvenlik grupları atayarak, genel klasörlerin izinlerini değiştirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d3e6c-107">From there, you can change permissions for individual public folders by assigning security groups to permissions.</span></span> <span data-ttu-id="d3e6c-108">Son kullanıcının ortak klasör izinlerini değiştirmesi için, kullanıcının klasörde sahip haklarına sahip olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="d3e6c-108">For an end user to change public folder permissions, the user needs to have Owner rights on the folder.</span></span>

<span data-ttu-id="d3e6c-109">Lütfen ortak klasör izni sorunlarını gidermek için [ortak klasör izni sorunlarını tanılama ve düzeltme konusunda](https://docs.microsoft.com/exchange/troubleshoot/public-folders/public-folder-permission-issues) açıklanan yordamı izleyin.</span><span class="sxs-lookup"><span data-stu-id="d3e6c-109">Please follow the procedure described in [How to diagnose and fix public folder permission issues](https://docs.microsoft.com/exchange/troubleshoot/public-folders/public-folder-permission-issues) to troubleshoot public folder permission issues.</span></span>

<span data-ttu-id="d3e6c-110">**Not**: ortak klasörlerdeki izinleri değiştirmeye çalıştığınızda karşılaşabileceğiniz birçok sorun vardır.</span><span class="sxs-lookup"><span data-stu-id="d3e6c-110">**Note**: There are several known issues you might encounter when you try to change permissions on public folders.</span></span> <span data-ttu-id="d3e6c-111">Daha fazla bilgi için aşağıdaki makalelere bakın.</span><span class="sxs-lookup"><span data-stu-id="d3e6c-111">See the following articles for more information.</span></span>

- [<span data-ttu-id="d3e6c-112">EAC 'deki ortak klasör alt klasörlerine izinler uygulayamazsınız</span><span class="sxs-lookup"><span data-stu-id="d3e6c-112">Can't apply permissions to public folder subfolders in EAC</span></span>](https://docs.microsoft.com/exchange/troubleshoot/public-folders/can%E2%80%99t-apply-permissions-public-folder-subfolders)

- [<span data-ttu-id="d3e6c-113">Ortak klasörlere eriştiğinizde "posta kutusu yerel ormanda bulunamadı" hatası</span><span class="sxs-lookup"><span data-stu-id="d3e6c-113">"The mailbox is not found in the local forest" error when you access public folders</span></span>](https://docs.microsoft.com/exchange/troubleshoot/public-folders/mailbox-not-found-local-forest-public-folder)
