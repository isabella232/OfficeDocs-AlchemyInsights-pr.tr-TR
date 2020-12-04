---
title: Windows 10 cihazlarını yapılandırmak için Microsoft Intune güvenlik temellerini kullanma
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573785"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="5dda3-102">Windows 10 cihazlarını yapılandırmak için Microsoft Intune güvenlik temellerini kullanma</span><span class="sxs-lookup"><span data-stu-id="5dda3-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="5dda3-103">Intune güvenlik temelleri, kullanıcıları ve cihazları korur.</span><span class="sxs-lookup"><span data-stu-id="5dda3-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="5dda3-104">Güvenlik temelleri, bilinen bir ayar grubunu uygulamak için kullanılan önceden yapılandırılmış gruplar ve ilgili güvenlik ekipleri tarafından önerilen varsayılan değerleri, Windows ayarları 'nı uygulamak için kullanılır.</span><span class="sxs-lookup"><span data-stu-id="5dda3-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="5dda3-105">Intune 'da bir güvenlik temel profili oluşturarak, birden çok cihaz yapılandırma profilinden oluşan bir şablon oluşturacaksınız.</span><span class="sxs-lookup"><span data-stu-id="5dda3-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="5dda3-106">Güvenlik temellerini Kullanıcı veya cihaz gruplarına dağıtırken, ayarlar Windows 10 veya üstünde çalışan cihazlara uygulanır.</span><span class="sxs-lookup"><span data-stu-id="5dda3-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="5dda3-107">Örneğin, MDM güvenlik temeli otomatik olarak (1) çıkarılabilir sürücüler için BitLocker 'ı, (2) cihazın kilidini açmak için parola gerektirir ve (3) temel kimlik doğrulamasını devre dışı bırakır.</span><span class="sxs-lookup"><span data-stu-id="5dda3-107">For example, MDM Security Baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="5dda3-108">Varsayılan bir değer ortamınızda çalışmazsa, ihtiyacınız olan ayarları uygulamak için taban çizgisini özelleştirin.</span><span class="sxs-lookup"><span data-stu-id="5dda3-108">When a default value doesn't work for your environment, customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="5dda3-109">Güvenlik temelleri, Microsoft 365 'da uçtan uca güvenli bir iş akışı oluşturmaya da yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="5dda3-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="5dda3-110">Aşağıda, bunun avantajları verilmiştir:</span><span class="sxs-lookup"><span data-stu-id="5dda3-110">The following are some benefits of this:</span></span>

- <span data-ttu-id="5dda3-111">Güvenlik temeli, güvenliği etkileyen ayarlar için en iyi yöntemleri ve önerileri içerir.</span><span class="sxs-lookup"><span data-stu-id="5dda3-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="5dda3-112">Intune, Grup ilkeleri için taban çizgileri oluşturan Windows Güvenlik ekibinden gelen iş ortakları nedeniyle, bu öneriler düz kılavuza ve kapsamlı deneyimlere dayanır.</span><span class="sxs-lookup"><span data-stu-id="5dda3-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="5dda3-113">Intune 'a yeni bağlıysanız ve nereden başlayacağınızı bilmiyorsanız, güvenlik temelleri hızlı bir şekilde güvenli bir profil oluşturup dağıtmanızı sağlayacaktır.</span><span class="sxs-lookup"><span data-stu-id="5dda3-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="5dda3-114">Şu anda bir grup ilkesi kullanıyorsanız, yönetim amaçları için Intune 'a geçirmek, güvenlik temelleriyle çok daha kolaydır çünkü bu, Intune 'da yerleşik olmaları ve yönetim için uçtan uca özellikler içermektedir.</span><span class="sxs-lookup"><span data-stu-id="5dda3-114">If you currently use a group policy, then migrating to Intune for management purposes is much easier with security baselines, because they are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="5dda3-115">Daha fazla bilgi edinmek için [Windows güvenlik temelleri](https://go.microsoft.com/fwlink/?linkid=2141503) ve [mobil cihaz yönetimi](https://go.microsoft.com/fwlink/?linkid=2141701)'ne bakın.</span><span class="sxs-lookup"><span data-stu-id="5dda3-115">To learn more, see [Windows security baselines](https://go.microsoft.com/fwlink/?linkid=2141503) and [Mobile device management](https://go.microsoft.com/fwlink/?linkid=2141701).</span></span>