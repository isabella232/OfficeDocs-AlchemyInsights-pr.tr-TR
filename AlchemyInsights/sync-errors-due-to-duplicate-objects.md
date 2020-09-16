---
title: 902 (yinelenen nesneler nedeniyle eşitleme hataları)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 33b8ad0a33eb02eb9ec5bd26f94b00e5645b3fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737361"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="14423-102">Yinelenen nesneler nedeniyle eşitleme hataları</span><span class="sxs-lookup"><span data-stu-id="14423-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="14423-103">Microsoft 365 'da dizin eşitlemesi tamamlandığında aşağıdaki hata iletilerinden birini alabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="14423-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="14423-104">Bu nesneyle ilişkilendirilmiş olan aşağıdaki özniteliklerin yerel dizininizde başka bir nesneyle ilişkilendirilmiş değerleri olduğundan, bu nesne Microsoft Online Services 'ta güncelleştirilemiyor.</span><span class="sxs-lookup"><span data-stu-id="14423-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="14423-105">Microsoft Online Services dizininizde aynı proxy adresine sahip eşitlenmiş bir nesne zaten var.</span><span class="sxs-lookup"><span data-stu-id="14423-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="14423-106">Bu nesneyle ilişkili aşağıdaki özniteliklerin yerel dizin hizmetinizdeki başka bir nesneyle ilişkilendirilmiş değerleri olduğundan, bu nesne güncelleştirilemiyor: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="14423-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="14423-107">Sorunu tanımlayıp çözmek için [IdFix DirSync hata düzeltme aracını](https://www.microsoft.com/download/details.aspx?id=36832)indirin ve yükleyin.</span><span class="sxs-lookup"><span data-stu-id="14423-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="14423-108">Daha fazla bilgi için bkz: [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="14423-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
