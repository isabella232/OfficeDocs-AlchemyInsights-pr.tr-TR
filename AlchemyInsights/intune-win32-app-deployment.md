---
title: Intune Win32 uygulama dağıtımı
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461996"
---
# <a name="intune-win32-app-deployment"></a><span data-ttu-id="8e7e3-102">Intune Win32 uygulama dağıtımı</span><span class="sxs-lookup"><span data-stu-id="8e7e3-102">Intune Win32 app deployment</span></span>

<span data-ttu-id="8e7e3-103">Microsoft Intune, MSI ve bunlarla sınırlı olmamak kaydıyla, Win32 uygulamalarına olanak tanır. Windows 10 cihazlarına dağıtılacak olan EXE.</span><span class="sxs-lookup"><span data-stu-id="8e7e3-103">Microsoft Intune allows Win32 applications, including but not limited to MSI and .EXE’s to be deployed to Windows 10 devices.</span></span> <span data-ttu-id="8e7e3-104">Kullanılan dağıtım mekanizması, hedef cihazda Intune yönetim uzantısının (IME) olmasını gerektirir.</span><span class="sxs-lookup"><span data-stu-id="8e7e3-104">The deployment mechanism used requires the Intune Management Extension (IME) to be present on the target device.</span></span> <span data-ttu-id="8e7e3-105">Bir Kullanıcı/cihaza PowerShell betiği veya Win32 uygulama dağıtımının hedeflenmesi sonucunda, IME otomatik olarak yüklenir.</span><span class="sxs-lookup"><span data-stu-id="8e7e3-105">The IME will be installed automatically as a result of targeting a powershell script or win32 application deployment to a user / device.</span></span>

<span data-ttu-id="8e7e3-106">Ayrıca, aşağıdakileri içeren Win32 uygulamalarını dağıtmak için karşılanması gereken bir dizi ön koşullar vardır:</span><span class="sxs-lookup"><span data-stu-id="8e7e3-106">There are also a set of pre-requisites which must be met in order to deploy Win32 apps which include:</span></span>

- <span data-ttu-id="8e7e3-107">Desteklenen platformlar: Windows 10 sürüm 1607 veya üstü (kurumsal, Pro ve eğitim sürümleri).</span><span class="sxs-lookup"><span data-stu-id="8e7e3-107">Supported platforms: Windows 10 version 1607 or later (Enterprise, Pro, and Education versions).</span></span>
- <span data-ttu-id="8e7e3-108">Desteklenen mimari: x86 ve x64.</span><span class="sxs-lookup"><span data-stu-id="8e7e3-108">Supported architecture: x86 and x64.</span></span>
- <span data-ttu-id="8e7e3-109">Cihaz yönetimi: AAD katılmış ve otomatik kayıtlı (karma etki alanına katılmış ve Grup ilkesi otomatik olarak kayıtlı).</span><span class="sxs-lookup"><span data-stu-id="8e7e3-109">Device Management: AAD joined and auto-enrolled (including hybrid domain joined and group policy auto-enrolled).</span></span>
- <span data-ttu-id="8e7e3-110">Uygulama paketi biçimi:. [Microsoft Win32 Içerik Prep aracı](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare)tarafından hazırlanan **intunewın** dosyası.</span><span class="sxs-lookup"><span data-stu-id="8e7e3-110">Application Package format: .**intunewin**  file prepared by the [Microsoft Win32 content Prep tool](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span></span>
- <span data-ttu-id="8e7e3-111">Malar</span><span class="sxs-lookup"><span data-stu-id="8e7e3-111">Limitations:</span></span>
    - <span data-ttu-id="8e7e3-112">Maksimum boyut: 8MM.</span><span class="sxs-lookup"><span data-stu-id="8e7e3-112">Maximum size: 8GB.</span></span>
    - <span data-ttu-id="8e7e3-113">Desteklenmeyen mimari: kolları.</span><span class="sxs-lookup"><span data-stu-id="8e7e3-113">Unsupported architecture: ARMs.</span></span>

<span data-ttu-id="8e7e3-114">Bu adımlarla ilgili bilgiler için belgeyi "[Microsoft Intune 'Da Win32 uygulaması ekleme, atama ve izleme](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" bölümünü gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="8e7e3-114">Review the doc "[Add, assign, and monitor a Win32 app in Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" for information related to those steps.</span></span>

<span data-ttu-id="8e7e3-115">Win32 uygulamaları da dahil olmak üzere Windows 'da uygulama dağıtımının sorunlarını giderme ile ilgili ayrıntılar aşağıdaki belgelerde incelenebilir</span><span class="sxs-lookup"><span data-stu-id="8e7e3-115">Details on troubleshooting application deployment on Windows including Win32 apps can be reviewed in the following documents</span></span>

- [<span data-ttu-id="8e7e3-116">Uygulama yükleme sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="8e7e3-116">Troubleshoot App Installation issues</span></span>](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [<span data-ttu-id="8e7e3-117">Win32 uygulamalarında sorun giderme</span><span class="sxs-lookup"><span data-stu-id="8e7e3-117">Troubleshoot Win32 Apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)