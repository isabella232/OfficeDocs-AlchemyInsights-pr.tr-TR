---
title: Cihazları Microsoft Intune için güvenlik taban çizgilerini Windows 10 kullanma
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 88525fccd6dcde0cb3949e348d1f2a7df3ee7ce7
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794127"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="4af57-102">Cihazları Microsoft Intune için güvenlik taban çizgilerini Windows 10 kullanma</span><span class="sxs-lookup"><span data-stu-id="4af57-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="4af57-103">Intune güvenlik taban çizgisi, kullanıcıları ve cihazları korumaya yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="4af57-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="4af57-104">Güvenlik taban Windows, bilinen bir grup ayarı ve ilgili güvenlik ekipleri tarafından önerilen varsayılan değerleri uygulamak için kullanılan önceden yapılandırılmış ayarlardır.</span><span class="sxs-lookup"><span data-stu-id="4af57-104">Security baselines are Windows settings pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="4af57-105">Intune'da güvenlik taban çizgisi profili oluşturarak, birden çok cihaz yapılandırma profili içeren bir şablon oluşturabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4af57-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="4af57-106">Kullanıcı veya cihaz gruplarına güvenlik taban çizgilerini dağıtıyorken, ayarlar daha sonra veya birden çok Windows 10 uygulanır.</span><span class="sxs-lookup"><span data-stu-id="4af57-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="4af57-107">Örneğin, Microsoft mobil cihaz yönetimi (MDM) güvenlik temeli çıkarılabilir sürücülerde BitLocker'i otomatik olarak etkinleştirebilir, cihazın kilidini açmak için parolayı gerektirir ve temel kimlik doğrulamasını devre dışı bırakacaktır.</span><span class="sxs-lookup"><span data-stu-id="4af57-107">For example, the Microsoft mobile device management (MDM) security baseline automatically enables BitLocker for removable drives, requires the password for unlocking a device, and disables basic authentication.</span></span> <span data-ttu-id="4af57-108">Ortamınız için varsayılan değer işe yaramadı mı, ihtiyacınız olan ayarları uygulamak için temeli özelleştirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4af57-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="4af57-109">Güvenlik taban çizgisi, aynı zamanda iş akışlarında uç- uç güvenli iş akışı Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="4af57-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="4af57-110">Güvenlik temeli, güvenliği etkileyen en iyi yöntemleri ve ayarların önerilerini içerir.</span><span class="sxs-lookup"><span data-stu-id="4af57-110">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="4af57-111">Intune, grup ilkeleri Windows temeller oluşturan güvenlik ekibiyle ortak çalışmalarına sahip olur; bu nedenle bu öneriler sağlam kılavuzdan ve kapsamlı deneyimden temel almaktadır.</span><span class="sxs-lookup"><span data-stu-id="4af57-111">Intune partners with the Windows security team that creates baselines for group policies, so these recommendations are based on solid guidance and extensive experience.</span></span>

<span data-ttu-id="4af57-112">Intune'da yeniyseniz ve nereden başlayacağınıza emin değilseniz, güvenlik taban çizgisi hızla güvenli bir profil oluşturmanıza ve dağıtmanıza yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="4af57-112">If you're new to Intune and unsure of where to start, security baselines help you quickly create and deploy a secure profile.</span></span> <span data-ttu-id="4af57-113">Şu anda bir grup ilkesi kullanıyorsanız, intune'da yerleşik olarak bulunan ve en yeni yönetim özelliklerini içeren bu ilkeler, güvenlik taban çizgileriyle yönetim amacıyla Intune'a olmak çok daha kolaydır.</span><span class="sxs-lookup"><span data-stu-id="4af57-113">If you currently use a group policy, migrating to Intune for management purposes is much easier with security baselines because they are built into Intune and include cutting-edge management capabilities.</span></span>

<span data-ttu-id="4af57-114">Daha fazla bilgi edinmek için [bkz. Windows temelleri ve](/windows/security/threat-protection/windows-security-baselines) [Mobil cihaz yönetimi.](/windows/client-management/mdm/)</span><span class="sxs-lookup"><span data-stu-id="4af57-114">To learn more, see [Windows security baselines](/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](/windows/client-management/mdm/).</span></span>

