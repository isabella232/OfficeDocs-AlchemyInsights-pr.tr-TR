---
title: OneDrive eşitleme istemcisi için kuruluş adını değiştirme
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003077"
- "5850"
ms.openlocfilehash: ca545ba51e39209f3302acdee1c24048515e2c1b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818344"
---
# <a name="change-the-organization-name-for-the-onedrive-sync-client"></a><span data-ttu-id="28502-102">OneDrive eşitleme istemcisi için kuruluş adını değiştirme</span><span class="sxs-lookup"><span data-stu-id="28502-102">Change the organization name for the OneDrive sync client</span></span>

<span data-ttu-id="28502-103">OneDrive, kiracı yöneticisi tarafından ayarlanmış kuruluş adını kullanır.</span><span class="sxs-lookup"><span data-stu-id="28502-103">OneDrive uses the organization name set by a tenant administrator.</span></span>  <span data-ttu-id="28502-104">Kuruluşun [adresini, teknik iletişim bilgilerini ve daha fazlasını değiştirebilirsiniz.](https://docs.microsoft.com/microsoft-365/admin/manage/change-address-contact-and-more)</span><span class="sxs-lookup"><span data-stu-id="28502-104">You can [change your organization's address, technical contact, and more](https://docs.microsoft.com/microsoft-365/admin/manage/change-address-contact-and-more).</span></span> <span data-ttu-id="28502-105">Kiracı için bu değişiklik uygulandıktan sonra, kullanıcılar OneDrive hesaplarının bağlantısını kaldırana ve yeniden bağladığı zaman OneDrive eşitleme istemcisi yeni adı yansıtmaz.</span><span class="sxs-lookup"><span data-stu-id="28502-105">Once that change is performed for the tenant, the OneDrive sync client will not reflect the new name until users unlink and relink their OneDrive account.</span></span>

<span data-ttu-id="28502-106">Hesabın bağlantısını kesebilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="28502-106">To unlink the account:</span></span>

1. <span data-ttu-id="28502-107">Görev çubuğunun sağ en sağ köşesindeki mavi OneDrive bulut simgesini seçin ve ardından Diğer Seçenekler'i **> OneDrive > seçin.**</span><span class="sxs-lookup"><span data-stu-id="28502-107">Select the blue OneDrive cloud icon at the far right of the taskbar, then select  **More > Settings > Account**.</span></span>
2. <span data-ttu-id="28502-108">Bağlantısını silmek istediğiniz hesabı bulun ve Bu PC'nin bağlantısını **kaldır'ı ve** sonra Hesabın bağlantısını **kaldır'ı seçin.**</span><span class="sxs-lookup"><span data-stu-id="28502-108">Find the account you want to unlink and select  **Unlink this PC**, and then  **Unlink account**.</span></span>

<span data-ttu-id="28502-109">Hesabı yeniden bağ yapmak için **Ayarlar'daki Hesap sekmesinde** Hesap ekle'yi seçin ve yeniden OneDrive'da oturum açın. </span><span class="sxs-lookup"><span data-stu-id="28502-109">To relink the account, select  **Add an account** from the  **Account** tab in Settings, and sign back into OneDrive.</span></span>