---
title: Bitlocker kurtarma tuşları
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 4e06e0e43b63836b9e9cf923e554dd474b82c671
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908834"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="a4899-102">Bitlocker kurtarma tuşlarına erişim</span><span class="sxs-lookup"><span data-stu-id="a4899-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="a4899-103">Bitlocker ayarlarını Intune Endpoint Protection İlke'yi yapılandırırken, Bitlocker kurtarma bilgilerinin Azure Etkin Dizini'nde depolanıp depolanmayacağını tanımlamak mümkündür.</span><span class="sxs-lookup"><span data-stu-id="a4899-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="a4899-104">Bu ayar yapılandırılırsa, depolanan kurtarma verileri, Intune Devices bıtırcı bıçaktaki aygıt kaydı verilerinin bir parçası olarak bir Intune yöneticisi tarafından iki şekilde görülebilir:</span><span class="sxs-lookup"><span data-stu-id="a4899-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="a4899-105">Cihazlar - Azure AD aygıtları -> "Aygıt" VEYA Aygıtlar -tüm cihazlar > -> "Aygıt" -> Kurtarma tuşları</span><span class="sxs-lookup"><span data-stu-id="a4899-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="a4899-106">Alternatif olarak, aygıtın kendisine yönetimsel erişim varsa, kurtarma anahtarı (Parola) yükseltilmiş bir komut isteminden aşağıdaki komutu çalıştırarak görülebilir:</span><span class="sxs-lookup"><span data-stu-id="a4899-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
<span data-ttu-id="a4899-107">Aygıt Intune'a kaydolmadan önce şifrelenmişse, kurtarma anahtarı OOBE işlemi sırasında aygıtta oturum açmada kullanılan "Microsoft Hesabı" (MSA) ile ilişkilendirilmiş olabilir.</span><span class="sxs-lookup"><span data-stu-id="a4899-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="a4899-108">Bu durumda, msa https://onedrive.live.com/recoverykey ile erişim ve oturum açma, kurtarma anahtarlarının depolandığı aygıtları göstermelidir.</span><span class="sxs-lookup"><span data-stu-id="a4899-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="a4899-109">Aygıt etki alanı tabanlı grup ilkesi aracılığıyla yapılandırma sonucunda şifrelenmişse, kurtarma bilgileri şirket içi Etkin Dizinde depolanabilir.</span><span class="sxs-lookup"><span data-stu-id="a4899-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>
 

