---
title: Intune’dan verileri kaldırma ve cihazları silme
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: cada3c6f1e7d1dcd576baa1245fb5a62ed938613
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416333"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="e9e24-102">Intune’dan verileri kaldırma ve cihazları silme</span><span class="sxs-lookup"><span data-stu-id="e9e24-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="e9e24-103">Cihaz Devre Dışı Bırakma ve Cihaz Silme uzak eylemleri Inture tarafından yönetilen şirket verilerini kaldırmak veya bir fabrika sıfırlaması yapıp cihazı varsayılan ayarlarına döndürmek için kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="e9e24-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="e9e24-104">Microsoft 365 Cihaz Yönetimi’nde oturum açın ve **Cihazlar** > **Tüm Cihazlar**’a gidin.</span><span class="sxs-lookup"><span data-stu-id="e9e24-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="e9e24-105">Silmek istediğiniz cihazı seçin.</span><span class="sxs-lookup"><span data-stu-id="e9e24-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="e9e24-106">Yapmak istediğiniz uzaktan silme türünü seçin.</span><span class="sxs-lookup"><span data-stu-id="e9e24-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="e9e24-107">Devre dışı bırakma işlemi yalnızca kurumsal bilgileri silerken, tam silme işlemi cihazı fabrika ayarlarına geri yükler.</span><span class="sxs-lookup"><span data-stu-id="e9e24-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="e9e24-108">Onaylamak için **Evet**'i seçin.</span><span class="sxs-lookup"><span data-stu-id="e9e24-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="e9e24-109">Silme işlemi bitene kadar Cihazın eylem durumu *Devre Dışı Bırakma Bekliyor* olarak gösterilir.</span><span class="sxs-lookup"><span data-stu-id="e9e24-109">Until the wipe finishes, the Device action status shows as *Retire Pending*.</span></span>
    <span data-ttu-id="e9e24-110">Eylem tamamlandıktan sonra artık yönetilen cihaz listesinde mobil cihazı görmezsiniz.</span><span class="sxs-lookup"><span data-stu-id="e9e24-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

> [!NOTE]
> <span data-ttu-id="e9e24-111">Şirket verileri Azure AD’ye KATILMIŞ cihazlardan kaldırılamaz.</span><span class="sxs-lookup"><span data-stu-id="e9e24-111">Company data can't be removed from devices JOINED to Azure AD.</span></span> 

<span data-ttu-id="e9e24-112">Devre Dışı Bırakma ve Silme eylemlerinin etkisiyle ilgili olarak, nelerin tutulduğu ve nelerin silindiği de dahil olmak üzere tüm ayrıntılar için aşağıdaki belgelere bakın:</span><span class="sxs-lookup"><span data-stu-id="e9e24-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see following documentation:</span></span>

- <span data-ttu-id="e9e24-113">[Silme veya devre dışı bırakma işlemlerini kullanarak ya da cihazın kaydını el ile kaldırarak cihazları kaldırma](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="e9e24-113">[Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span></span>
- [<span data-ttu-id="e9e24-114">Intune tarafından yönetilen uygulamalardan yalnızca kurumsal verileri silme</span><span class="sxs-lookup"><span data-stu-id="e9e24-114">How to wipe only corporate data from Intune-managed apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- <span data-ttu-id="e9e24-115">[macOS cihazından tüm verileri silme](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span><span class="sxs-lookup"><span data-stu-id="e9e24-115">[Erase all data from a macOS device](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span></span>