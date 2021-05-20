---
title: Mac veya Linux üzerine Microsoft Defender yükleme sorunları
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 39f180852fd0438597fa1ce665b2703fbc7b1aa4
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539700"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a><span data-ttu-id="a404b-102">Mac veya Linux üzerine Microsoft Defender yükleme sorunları</span><span class="sxs-lookup"><span data-stu-id="a404b-102">Issues installing Microsoft Defender on Mac or Linux</span></span>

<span data-ttu-id="a404b-103">**Mac**</span><span class="sxs-lookup"><span data-stu-id="a404b-103">**Mac**</span></span>

- <span data-ttu-id="a404b-104">Mac için Office'i yüklemeden önce sistem Microsoft Defender ATP karşı olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="a404b-104">Ensure that system requirements are met before installing Microsoft Defender ATP for Mac.</span></span> <span data-ttu-id="a404b-105">Daha fazla bilgi için [bkz. Mac için Microsoft Defender ATP yükleme](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).</span><span class="sxs-lookup"><span data-stu-id="a404b-105">For more info, see [How to install Microsoft Defender ATP for Mac](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).</span></span>  
- <span data-ttu-id="a404b-106">Dosyada bilgileri gözden geçirme: "/Library/Logs/Microsoft/mdatp/install.log".</span><span class="sxs-lookup"><span data-stu-id="a404b-106">Review the information in the file: "/Library/Logs/Microsoft/mdatp/install.log".</span></span>

<span data-ttu-id="a404b-107">**Linux**</span><span class="sxs-lookup"><span data-stu-id="a404b-107">**Linux**</span></span>

- <span data-ttu-id="a404b-108">Linux için Microsoft Defender ATP yüklemeden önce sistem Microsoft Defender ATP karşı olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="a404b-108">Ensure that system requirements are met before installing Microsoft Defender ATP for Linux.</span></span> <span data-ttu-id="a404b-109">Daha fazla bilgi için [bkz. Linux için MDATP yükleme.](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)</span><span class="sxs-lookup"><span data-stu-id="a404b-109">For more info, see [How to install MDATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span> 
- <span data-ttu-id="a404b-110">Hizmet hizmetinin MDATP doğrulamak için bkz. [Yükleme başarısız.](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)</span><span class="sxs-lookup"><span data-stu-id="a404b-110">To verify that MDATP service is running, see [Installation failed](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).</span></span>  
    <span data-ttu-id="a404b-111">Hizmet çalışmıyorsa sorunları gidermek ve gidermek için bkz. [Mdatp hizmeti](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)çalışmıyorsa giderme adımları .</span><span class="sxs-lookup"><span data-stu-id="a404b-111">To troubleshoot and resolve issues if the service is not running, see [Steps to troubleshoot if mdatp service isn't running](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).</span></span>
- <span data-ttu-id="a404b-112">Ürünün durumunu doğrular ve EICAR metin dosyasında bir algılama testi çalıştırmak için istemci yapılandırmasını denetleme adımları için bkz. [İstemci yapılandırması](/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).</span><span class="sxs-lookup"><span data-stu-id="a404b-112">For steps to check the client configuration, which verifies the health of the product, and to run a detection test on the EICAR text file, see [Client configuration](/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).</span></span>  

    <span data-ttu-id="a404b-113">**Not** Erişime açık etkinlikler için desteklenen dosya sistemlerinin listesi için Linux için [Microsoft Defender ATP'e bakın.](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)</span><span class="sxs-lookup"><span data-stu-id="a404b-113">**Note** For a list of supported file systems for on-access activity, see [Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span>