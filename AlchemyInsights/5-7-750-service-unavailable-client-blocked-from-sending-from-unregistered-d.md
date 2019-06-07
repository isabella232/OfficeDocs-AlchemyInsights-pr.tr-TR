---
title: 1048 5.7.750 hizmeti kullanılamıyor. İstemci kaydı etki alanlarından göndermesini engelledi
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom: 1048
ms.openlocfilehash: 9417fef2584e9b81a2ca71cbcc5e23ce093d94e8
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34751723"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="76e9e-103">5.7.750 kayıtlı olmayan etki alanındaki tüm gönderenlerden gelen istemci engellendi.</span><span class="sxs-lookup"><span data-stu-id="76e9e-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="76e9e-104">Büyük bir hata oluşur Office (kabul edilen etki alanı olarak eklenen ve onaylanmış) 365 hazırlandı olmayan etki alanlarından gelen iletiler hacmini gönderilir.</span><span class="sxs-lookup"><span data-stu-id="76e9e-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in Office 365 (added as accepted domains and validated).</span></span>

<span data-ttu-id="76e9e-105">Bu hatanın oluşmaması için burada sertifika etki alanı sağlanan bir etki alanı veya tüm gönderen etki alanları hazırlayabilirsiniz sertifika tabanlı posta akışı bağlayıcı kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="76e9e-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
