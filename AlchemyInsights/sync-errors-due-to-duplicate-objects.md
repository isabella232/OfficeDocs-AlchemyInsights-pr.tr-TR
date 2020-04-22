---
title: 902 (Yinelenen nesnelernedeniyle eşitleme hataları)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 6ea833e0c4aebe72bc5c02e3dc10c1edc4136dcc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767161"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="347b3-102">Yinelenen nesneler nedeniyle eşitleme hataları</span><span class="sxs-lookup"><span data-stu-id="347b3-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="347b3-103">Microsoft 365'te dizin eşitlemesi bittiğinde aşağıdaki hata iletilerinden birini alabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="347b3-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="347b3-104">Bu nesneyle ilişkili aşağıdaki öznitelikler, yerel dizininizdeki başka bir nesneyle zaten ilişkilendirilebilecek değerlere sahip olduğundan, Microsoft Çevrimiçi Hizmetler'de bu nesneyi güncelleştiremiyor.</span><span class="sxs-lookup"><span data-stu-id="347b3-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="347b3-105">Microsoft Çevrimiçi Hizmetler dizininizde aynı proxy adresine sahip eşitlenmiş bir nesne zaten bulunmaktadır.</span><span class="sxs-lookup"><span data-stu-id="347b3-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="347b3-106">Bu nesneyle ilişkili aşağıdaki öznitelikler, yerel dizin hizmetlerinizde başka bir nesneyle zaten ilişkilendirilebilecek değerlere sahip olduğundan, bu nesneyi güncelleştiremiyor: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="347b3-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="347b3-107">Sorunu tanımlamak ve gidermek için [IdFix DirSync Hata Düzeltme Aracı'nı](https://www.microsoft.com/download/details.aspx?id=36832)indirin ve çalıştırın.</span><span class="sxs-lookup"><span data-stu-id="347b3-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="347b3-108">Daha fazla bilgi için [Bkz. KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="347b3-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
