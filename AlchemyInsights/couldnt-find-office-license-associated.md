---
title: Microsoft 365 uygulamalarını düzeltme
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
- "3421"
- "9001426"
ms.openlocfilehash: bd127d6287b4438f6105a6158abdbd5b964b7e70
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747715"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="2a3df-102">Microsoft 365 uygulamalarını düzeltme "Office lisansları ilişkili bulunamadı" iletisi</span><span class="sxs-lookup"><span data-stu-id="2a3df-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="2a3df-103">Bu iletiyi alırsanız, aşağıdakileri deneyin:</span><span class="sxs-lookup"><span data-stu-id="2a3df-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="2a3df-104">Güvenlik duvarınızın, virüsten koruma yazılımınızın ve proxy ayarlarınızın Internet erişimini Microsoft 365 uygulamalarına engellemediğinden emin olmak için denetleyin.</span><span class="sxs-lookup"><span data-stu-id="2a3df-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="2a3df-105">[Microsoft 365 URL 'lerini ve IP adresi aralıklarını](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)görüntüleyin.</span><span class="sxs-lookup"><span data-stu-id="2a3df-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="2a3df-106">Etkilenen Kullanıcı için [Office lisansını kaldırın ve yeniden atayın](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) .</span><span class="sxs-lookup"><span data-stu-id="2a3df-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="2a3df-107">Bir Office uygulamasını açın ve var olan kullanıcı hesaplarından [oturum açın](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) .</span><span class="sxs-lookup"><span data-stu-id="2a3df-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="2a3df-108">Windows ayarları > **hesapları**  >  **e-posta & hesaplarına**gidin ve etkilenen hesap dışındaki tüm iş hesaplarını kaldırın.</span><span class="sxs-lookup"><span data-stu-id="2a3df-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="2a3df-109">Windows ayarları > **hesaplar**  >  **iş veya okul**hesabına gidin ve etkilenen hesap dışında tüm iş hesaplarının bağlantılarını kesin.</span><span class="sxs-lookup"><span data-stu-id="2a3df-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="2a3df-110">Office etkinleştirme durumunu sıfırlama.</span><span class="sxs-lookup"><span data-stu-id="2a3df-110">Reset the Office activation state.</span></span> <span data-ttu-id="2a3df-111">[Nasıl yapıldığını öğrenin](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="2a3df-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="2a3df-112">Etkilenen Kullanıcı hesabını kullanarak [oturum açın](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) .</span><span class="sxs-lookup"><span data-stu-id="2a3df-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="2a3df-113">Ek sorun giderme çözümleri için, [Office 'Teki Lisanssız ürün ve etkinleştirme hatalarına](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)bakın.</span><span class="sxs-lookup"><span data-stu-id="2a3df-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>