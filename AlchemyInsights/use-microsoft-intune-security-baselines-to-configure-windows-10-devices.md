---
title: Windows 10 cihazlarını yapılandırmak için Microsoft Intune güvenlik taban çizgilerini kullanma
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50696385"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a><span data-ttu-id="be458-102">Windows 10 cihazlarını yapılandırmak için Microsoft Intune güvenlik taban çizgilerini kullanma</span><span class="sxs-lookup"><span data-stu-id="be458-102">Use the Microsoft Intune security baselines for configuring Windows 10 devices</span></span>

<span data-ttu-id="be458-103">Intune güvenlik taban çizgisi, kullanıcıların ve cihazların korunmasına yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="be458-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="be458-104">Güvenlik taban çizgisi, Windows ayarlarının bilinen bir ayar grubunu ve ilgili güvenlik ekipleri tarafından önerilen varsayılan değerleri uygulamak için kullanılan önceden yapılandırılmış gruplarıdır.</span><span class="sxs-lookup"><span data-stu-id="be458-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="be458-105">Intune'da bir güvenlik temeli profili oluşturarak, birden çok cihaz yapılandırma profili içeren bir şablon oluşturabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="be458-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="be458-106">Güvenlik taban çizgilerini kullanıcı veya cihaz gruplarına dağıtsanız, ayarlar Windows 10 veya daha sonraki sürümlerde çalıştıran cihazlara uygulanır.</span><span class="sxs-lookup"><span data-stu-id="be458-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later versions.</span></span> <span data-ttu-id="be458-107">Örneğin, Microsoft mobil cihaz yönetimi (MDM) güvenlik temeli (1) çıkarılabilir sürücüler için BitLocker'ı otomatik olarak etkinleştirir, (2) cihazın kilidini açmak için parolayı gerektirir ve (3) temel kimlik doğrulamasını devre dışı bırakır.</span><span class="sxs-lookup"><span data-stu-id="be458-107">For example, the Microsoft mobile device management (MDM) security baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="be458-108">Ortamınız için varsayılan bir değer işe yaramadı mı, ihtiyacınız olan ayarları uygulamak için taban çizgisini özelleştirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="be458-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="be458-109">Güvenlik taban çizgisi, Microsoft 365'te uç- uç güvenli iş akışı kurulmasına da yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="be458-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="be458-110">Bu işlevin bazı avantajları aşağıda ve aşağıda ve ve aşağıda ve ve listelerde ve listelerde yer alan bilgiler ve bilgileri bulunmaktadır:</span><span class="sxs-lookup"><span data-stu-id="be458-110">The following are some benefits of this functionality:</span></span>
- <span data-ttu-id="be458-111">Güvenlik temeli, güvenliği etkileyen ayarlarla ilgili en iyi yöntemleri ve önerileri içerir.</span><span class="sxs-lookup"><span data-stu-id="be458-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="be458-112">Intune, grup ilkeleri için taban çizgisi oluşturan Windows güvenlik ekibiyle ortak çalışmalarından dolayı, bu öneriler sağlam bir kılavuza ve kapsamlı deneyime dayalıdır.</span><span class="sxs-lookup"><span data-stu-id="be458-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="be458-113">Intune'da yeniyseniz ve nereden başlayacağınıza emin değilseniz, güvenlik taban çizgisi hızla güvenli bir profil oluşturmanıza ve dağıtmanıza yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="be458-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="be458-114">Şu anda grup ilkesi kullanıyorsanız, intune'a yönetim amacıyla bu güvenlik taban çizgileriyle daha kolay bir şekilde devam etmektir, çünkü bu güvenlik taban değerleri Intune'da yerleşiktir ve yönetim için en son özellikleri içerir.</span><span class="sxs-lookup"><span data-stu-id="be458-114">If you are currently using a group policy, then migrating to Intune for management purposes is much easier with security baselines, because these security baselines are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="be458-115">Daha fazla bilgi için Windows güvenlik [taban çizgilerine ve](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) Mobil cihaz [yönetimine bakın.](https://docs.microsoft.com/windows/client-management/mdm/)</span><span class="sxs-lookup"><span data-stu-id="be458-115">For more information, see [Windows security baselines](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](https://docs.microsoft.com/windows/client-management/mdm/).</span></span>