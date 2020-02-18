---
title: PowerShell self servis satın alma
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3516"
ms.openlocfilehash: 5e47e08e3309b3d58908e10ee06021da00f230bb
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091781"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="c6b77-102">PowerShell self servis satın alma</span><span class="sxs-lookup"><span data-stu-id="c6b77-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="c6b77-103">MSCommerce PowerShell modüllerini kullanmak için TLS 1.2 (yerel yönetici izinleri gereklidir) içeren bir Windows 10 cihazına yüklemeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="c6b77-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="c6b77-104">MSCommerce modülüne bağlanın ve içe aktarın.</span><span class="sxs-lookup"><span data-stu-id="c6b77-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="c6b77-105">Oturum açmanız istendiğinde, Genel Veya Fatura Yöneticisi rol kimlik bilgilerini kullanmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="c6b77-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="c6b77-106">TLS 1.2'niz yoksa, poliçeyi almaya veya güncellemeye çalışırken aşağıdaki hatayı alabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="c6b77-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="c6b77-107">*ErrorMessage -Temel bağlantı kapatıldı: Gönder'de beklenmeyen bir hata oluştu.*</span><span class="sxs-lookup"><span data-stu-id="c6b77-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



