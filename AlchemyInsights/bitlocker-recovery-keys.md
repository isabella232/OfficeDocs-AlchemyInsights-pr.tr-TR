---
title: Bitlocker kurtarma anahtarları
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: ec90e412302c74748e253f2e5430fa4205466f0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820306"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="c61c4-102">Bitlocker kurtarma anahtarlara erişme</span><span class="sxs-lookup"><span data-stu-id="c61c4-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="c61c4-103">Bitlocker ayarları Intune Uç Nokta Koruma İlkesi yapılandırılamazken, Bitlocker kurtarma bilgisinin Azure Active Directory'de depo gerekip depo gerek olmadığını tanımlamak mümkündür.</span><span class="sxs-lookup"><span data-stu-id="c61c4-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="c61c4-104">Bu ayar yapılandırılmışsa, Intune Cihaz Blade'sinde cihaz kaydı verileri iki şekilde bir intune yöneticisi tarafından görülebilir:</span><span class="sxs-lookup"><span data-stu-id="c61c4-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="c61c4-105">Cihazlar - Azure AD cihazlar ->" VEYA Cihazlar -> Tüm Cihazlar ->" -> Kurtarma anahtarları</span><span class="sxs-lookup"><span data-stu-id="c61c4-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="c61c4-106">Alternatif olarak, cihazın kendisine yönetim erişimi varsa, yükseltilmiş komut isteminden aşağıdaki komut çalıştırarak kurtarma anahtarı (Parola) görülebilir:</span><span class="sxs-lookup"><span data-stu-id="c61c4-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="c61c4-107">Cihaz Intune'da işlenmeden önce şifrelenmişse, kurtarma anahtarı OOBE işlemi sırasında cihazda oturum aparken kullanılan "Microsoft Hesabı" (MSA) ile ilişkilendirilmiş olabilir.</span><span class="sxs-lookup"><span data-stu-id="c61c4-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="c61c4-108">Böyle bir durumda, MSA'ya erişme ve bu MSA ile oturum açma, kurtarma  https://onedrive.live.com/recoverykey anahtarlarının depolandığı cihazları gösterir.</span><span class="sxs-lookup"><span data-stu-id="c61c4-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="c61c4-109">Etki alanı tabanlı grup ilkesi aracılığıyla yapılandırma sonucunda cihaz şifrelenirse, kurtarma bilgileri şirket içi Active Directory'de depolanıyor olabilir.</span><span class="sxs-lookup"><span data-stu-id="c61c4-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>

<span data-ttu-id="c61c4-110">Kurtarma anahtarını Azure Active Directory'de depolamak üzere yapılandırılmış Uç Nokta koruma ilkesi yapılandırdınız ancak belirli bir cihazın anahtarı karşıya yüklenmedi ise, bu cihaz için kurtarma anahtarını MEM konsolundan döndürerek karşıya yüklemenin tetiklenir.</span><span class="sxs-lookup"><span data-stu-id="c61c4-110">If you have configured Endpoint protection policy to store the recovery key in Azure Active Directory but the key for a specific device has not been uploaded, you can trigger the upload by rotating the recovery key for that device from the MEM console.</span></span> <span data-ttu-id="c61c4-111">Ayrıntılar için bkz. [BitLocker kurtarma anahtarlarını döndürme.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys)</span><span class="sxs-lookup"><span data-stu-id="c61c4-111">For details, see [Rotate BitLocker recovery keys](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).</span></span>

