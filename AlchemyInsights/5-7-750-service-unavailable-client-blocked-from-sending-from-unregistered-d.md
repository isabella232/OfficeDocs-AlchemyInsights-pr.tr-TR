---
title: 1048 5.7.750 hizmeti kullanılamıyor. İstemcinin kayıtlı olmayan etki alanlarından gönderilmesini engellediği
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: 731aa2e155ba3fdaaca7fed9dd51b3e4a3f20f29
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664262"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="edfb8-103">5.7.750 istemcisinin kayıtlı olmayan etki alanından gönderilmesini engellediği</span><span class="sxs-lookup"><span data-stu-id="edfb8-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="edfb8-104">Hata, kiracınızda sağlanmayan (kabul edilen etki alanları ve doğrulanmış) etki alanlarından büyük bir ileti gönderildiğinde oluşur.</span><span class="sxs-lookup"><span data-stu-id="edfb8-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in your tenant (added as accepted domains and validated).</span></span>

<span data-ttu-id="edfb8-105">Bu hatadan kaçınmak için, sertifika etki alanının sağlanan etki alanı olduğu veya tüm gönderen etki alanlarını temin edebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="edfb8-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
