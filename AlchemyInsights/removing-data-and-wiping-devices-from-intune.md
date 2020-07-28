---
title: Verileri kaldırma ve cihazları Intune'dan silme
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440463"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="58d5e-102">Verileri kaldırma ve cihazları Intune'dan silme</span><span class="sxs-lookup"><span data-stu-id="58d5e-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="58d5e-103">Aygıt Emekli Ve Aygıt Silme uzak eylemleri, Intune tarafından yönetilen şirket verilerini kaldırmak veya fabrika sıfırlama gerçekleştirmek ve aygıtı varsayılan ayarlarına döndürmek için kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="58d5e-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="58d5e-104">Microsoft 365 Aygıt Yönetimi'nde oturum açın ve **Tüm Aygıtlar**  >  **Aygıtları'na**gidin.</span><span class="sxs-lookup"><span data-stu-id="58d5e-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="58d5e-105">Silmek istediğiniz aygıtı seçin.</span><span class="sxs-lookup"><span data-stu-id="58d5e-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="58d5e-106">Yapmak istediğiniz uzaktan silme türünü seçin.</span><span class="sxs-lookup"><span data-stu-id="58d5e-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="58d5e-107">Retire yalnızca kuruluş bilgilerini silerken, tam silmeler aygıtı fabrika ayarlarına geri yüklenir.</span><span class="sxs-lookup"><span data-stu-id="58d5e-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="58d5e-108">Onaylamak için **Evet'i** seçin.</span><span class="sxs-lookup"><span data-stu-id="58d5e-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="58d5e-109">Silme bitene kadar, Aygıt eylem durumu Bekleyen Emekli olarak gösterir.</span><span class="sxs-lookup"><span data-stu-id="58d5e-109">Until the wipe finishes, the Device action status shows as Retire Pending.</span></span></br>
    <span data-ttu-id="58d5e-110">Eylem tamamlandıktan sonra, mobil aygıtı artık yönetilen aygıt listesinde görmezsiniz.</span><span class="sxs-lookup"><span data-stu-id="58d5e-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

<span data-ttu-id="58d5e-111">**Not** Şirket verileri, Azure AD'ye katılan aygıtlardan kaldırılamaz.</span><span class="sxs-lookup"><span data-stu-id="58d5e-111">**Note** Company data can't be removed from devices JOINED to Azure AD.</span></span>

<span data-ttu-id="58d5e-112">Nelerin tutulduğu ve silindiği de dahil olmak üzere Emekli Ve Sil eylemlerinin [etkisinin](https://docs.microsoft.com/intune/devices-wipe)tüm ayrıntıları için bkz.</span><span class="sxs-lookup"><span data-stu-id="58d5e-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see [Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/intune/devices-wipe).</span></span>

<span data-ttu-id="58d5e-113">MacOS aygıtından tüm verileri silmek için [bkz.](https://docs.microsoft.com/intune/device-erase)</span><span class="sxs-lookup"><span data-stu-id="58d5e-113">To erase all data from a macOS device, see [Erase all data from a macOS device](https://docs.microsoft.com/intune/device-erase).</span></span>