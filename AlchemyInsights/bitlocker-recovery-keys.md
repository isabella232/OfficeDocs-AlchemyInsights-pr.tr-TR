---
title: Bitlocker kurtarma anahtarları
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
- "1922"
- "9000220"
ms.openlocfilehash: 8708ed76f6abe81582823c8af89db8fffef9a3c5
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505088"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="8b730-102">Bitlocker kurtarma tuşlarına erişme</span><span class="sxs-lookup"><span data-stu-id="8b730-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="8b730-103">Bitlocker ayarlarını Intune Uç Nokta Koruma İlkesi yapılandırarak Bitlocker kurtarma bilgisinin Azure Active Directory'de depolanmış olup olmadığını tanımlamak mümkündür.</span><span class="sxs-lookup"><span data-stu-id="8b730-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="8b730-104">Bu ayar yapılandırılmışsa, Intune Devices blade'te cihaz kaydı verileri iki şekilde bir intune yöneticisi tarafından görülebilir:</span><span class="sxs-lookup"><span data-stu-id="8b730-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="8b730-105">Cihazlar - Azure AD cihazları -> "Cihaz" VEYA Cihazlar -> Tüm Cihazlar -> "Cihaz" -> Kurtarma anahtarları</span><span class="sxs-lookup"><span data-stu-id="8b730-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="8b730-106">Alternatif olarak, cihazın kendisine yönetim erişimi varsa, yükseltilmiş komut isteminden aşağıdaki komutu çalıştırarak kurtarma anahtarı (Parola) görülebilir:</span><span class="sxs-lookup"><span data-stu-id="8b730-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="8b730-107">Cihaz Intune'da şifrelenmeden önce şifrelenmişse, kurtarma anahtarı OOBE işlemi sırasında cihazda oturum a açmada kullanılan "Microsoft Hesabı" (MSA) ile ilişkilendirilmiş olabilir.</span><span class="sxs-lookup"><span data-stu-id="8b730-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="8b730-108">Böyle bir durumda, MSA'ya erişme ve bu MSA ile oturum açma, kurtarma  https://onedrive.live.com/recoverykey anahtarlarının depolandığı cihazları gösterir.</span><span class="sxs-lookup"><span data-stu-id="8b730-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="8b730-109">Cihaz, etki alanı tabanlı grup ilkesi aracılığıyla yapılandırma sonucunda şifrelenirse, kurtarma bilgileri şirket içi Active Directory'de depolanıyor olabilir.</span><span class="sxs-lookup"><span data-stu-id="8b730-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>

<span data-ttu-id="8b730-110">Kurtarma anahtarını Azure Active Directory'de depolamak için Uç Nokta koruma ilkesi yapılandırdınız ancak belirli bir cihaza yönelik anahtar karşıya yüklenmedi ise, mem konsolundan bu cihazın kurtarma anahtarını döndürerek karşıya yüklemenin tetiklenir.</span><span class="sxs-lookup"><span data-stu-id="8b730-110">If you have configured Endpoint protection policy to store the recovery key in Azure Active Directory but the key for a specific device has not been uploaded, you can trigger the upload by rotating the recovery key for that device from the MEM console.</span></span> <span data-ttu-id="8b730-111">Ayrıntılar için bkz. [BitLocker kurtarma anahtarlarını döndürme.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys)</span><span class="sxs-lookup"><span data-stu-id="8b730-111">For details, see [Rotate BitLocker recovery keys](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).</span></span>

