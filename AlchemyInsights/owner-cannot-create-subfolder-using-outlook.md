---
title: Sahip, Outlook kullanarak alt klasör oluşturamaz
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 9590f780cffeaf644733752c763e04d748b1b39e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665738"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="4acaf-102">Sahip, Outlook kullanarak alt klasör oluşturamaz</span><span class="sxs-lookup"><span data-stu-id="4acaf-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="4acaf-103">**Outlook kullanan ortak klasör sahiplerinin alt klasörlerini oluşturmakla ilgili bir sorun var. Sorun yakında düzeltilecektir.**</span><span class="sxs-lookup"><span data-stu-id="4acaf-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="4acaf-104">Bu arada, aşağıdaki geçici çözümlerden birini kullanın:</span><span class="sxs-lookup"><span data-stu-id="4acaf-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="4acaf-105">MAC için Outlook 'U kullanarak sorun yalnızca masaüstü Windows için Outlook 'U (tüm sürümler) etkilediğdeyken alt klasörü oluşturmak için</span><span class="sxs-lookup"><span data-stu-id="4acaf-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="4acaf-106">EXO kabuğu veya EAC kullanarak alt klasörü oluşturma</span><span class="sxs-lookup"><span data-stu-id="4acaf-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="4acaf-107">Kullanıcıya, soruna neden olan klasördeki DefaultPublicFolderMailbox/Efekt\tüm</span><span class="sxs-lookup"><span data-stu-id="4acaf-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="4acaf-108">*Set-Mailbox Kullanıcı1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="4acaf-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="4acaf-109">Saat bekle, Outlook istemcisini yeniden başlatın</span><span class="sxs-lookup"><span data-stu-id="4acaf-109">Wait for an hour, restart outlook client</span></span>