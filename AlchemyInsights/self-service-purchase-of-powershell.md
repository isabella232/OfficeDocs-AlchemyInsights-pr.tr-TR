---
title: PowerShell 'in self servis satın alımı
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3516"
ms.openlocfilehash: e6cc504ebef19cbe78f576d9b207fe2d951d0ef5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47739990"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="ac20d-102">PowerShell 'in self servis satın alımı</span><span class="sxs-lookup"><span data-stu-id="ac20d-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="ac20d-103">MSCommerce PowerShell modülünü kullanmak için TLS 1,2 (yerel yönetici izinleri gerekir) ile bir Windows 10 aygıtına yüklemeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="ac20d-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="ac20d-104">MSCommerce modülünü içeri ve bağlantı kurun.</span><span class="sxs-lookup"><span data-stu-id="ac20d-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="ac20d-105">Oturum açmanız istendiğinde, genel veya Fatura Yöneticisi rol kimlik bilgilerini kullanmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="ac20d-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="ac20d-106">TLS 1,2 yoksa, ilkeyi almaya veya güncelleştirmeye çalıştığınızda aşağıdaki hatayı alabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="ac20d-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="ac20d-107">*ErrorMessage-temeldeki bağlantı kapatıldı: gönderme sırasında beklenmeyen bir hata oluştu*.</span><span class="sxs-lookup"><span data-stu-id="ac20d-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



