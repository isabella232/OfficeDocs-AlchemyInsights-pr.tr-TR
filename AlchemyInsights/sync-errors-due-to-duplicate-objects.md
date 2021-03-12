---
title: 902 (Yinelenen nesneler nedeniyle oluşan eşitleme hataları)
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
ms.openlocfilehash: 75b684c5c6b4a594af069d8ed668df95726e1b31
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708082"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="e52a3-102">Yinelenen nesneler nedeniyle eşitleme hataları</span><span class="sxs-lookup"><span data-stu-id="e52a3-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="e52a3-103">Microsoft 365'te dizin eşitlemesi sona geldiğinde aşağıdaki hata iletilerinden birini alabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="e52a3-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="e52a3-104">Bu nesneyle ilişkilendirilmiş aşağıdaki öznitelikler yerel dizininizin başka bir nesnesiyle zaten ilişkilendirilmiş olabilir değerleri olduğundan, bu nesne Microsoft Online Services'ta güncelleştirilemiyor.</span><span class="sxs-lookup"><span data-stu-id="e52a3-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="e52a3-105">Microsoft Online Services dizininizin içinde aynı proxy adresine sahip eşitlenmiş bir nesne zaten var.</span><span class="sxs-lookup"><span data-stu-id="e52a3-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="e52a3-106">Bu nesneyle ilişkilendirilmiş aşağıdaki öznitelikler, yerel dizin hizmetlerinizin başka bir nesnesiyle zaten ilişkilendirilmiş olabilir değerleri olduğundan bu nesne güncelleştirilemiyor: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="e52a3-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="e52a3-107">Sorunu tanımlamak ve düzeltmek için IdFix DirSync Hata Düzeltme [Aracı'nı indirin ve çalıştırın.](https://github.com/Microsoft/idfix)</span><span class="sxs-lookup"><span data-stu-id="e52a3-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://github.com/Microsoft/idfix).</span></span>

<span data-ttu-id="e52a3-108">Daha fazla bilgi için [bkz. KB2647098.](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)</span><span class="sxs-lookup"><span data-stu-id="e52a3-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
