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
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: b94fcc697bb7ac065cef57f3e3eb0b515c3094a0
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35352873"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="89ea5-103">5.7.750 kayıtlı olmayan etki alanındaki tüm gönderenlerden gelen istemci engellendi.</span><span class="sxs-lookup"><span data-stu-id="89ea5-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="89ea5-104">Büyük bir hata oluşur Office (kabul edilen etki alanı olarak eklenen ve onaylanmış) 365 hazırlandı olmayan etki alanlarından gelen iletiler hacmini gönderilir.</span><span class="sxs-lookup"><span data-stu-id="89ea5-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in Office 365 (added as accepted domains and validated).</span></span>

<span data-ttu-id="89ea5-105">Bu hatanın oluşmaması için burada sertifika etki alanı sağlanan bir etki alanı veya tüm gönderen etki alanları hazırlayabilirsiniz sertifika tabanlı posta akışı bağlayıcı kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="89ea5-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
