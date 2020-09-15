---
title: OneDrive Iş sitelerine erişim reddedildi iletilerine sorun giderme
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9001cf0b7d9f1f05a2ecedca2c3137dd1b8a1c38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670636"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="42590-102">OneDrive Iş sitelerine erişim reddedildi iletilerine sorun giderme</span><span class="sxs-lookup"><span data-stu-id="42590-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="42590-103">Bu sorun en sık, Kullanıcı aynı Kullanıcı adı (UPN) ile silinip yeniden oluşturulduğunda oluşur.</span><span class="sxs-lookup"><span data-stu-id="42590-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="42590-104">Yeni hesap farklı bir PUıD (Passport benzersiz KIMLIĞI) değeri kullanılarak oluşturulur.</span><span class="sxs-lookup"><span data-stu-id="42590-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="42590-105">Kullanıcı bir site koleksiyonuna veya OneDrive 'a erişmeyi denediğinde, kullanıcının yanlış PUıD 'si vardır.</span><span class="sxs-lookup"><span data-stu-id="42590-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="42590-106">İkinci senaryo, Active Directory kuruluş birimi (OU) ile dizin eşitlemesi içerir.</span><span class="sxs-lookup"><span data-stu-id="42590-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="42590-107">Kullanıcılar zaten SharePoint 'te oturumlarsa, başka bir kuruluş birimine taşınmış ve SharePoint ile yeniden eşitleniyor</span><span class="sxs-lookup"><span data-stu-id="42590-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="42590-108">Bu sorunu çözmek için, [Microsoft 365 'da bir kullanıcıyı geri yüklemek](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)IÇIN özgün UPN 'yi makaledeki adımlarla geri yüklemelisiniz.</span><span class="sxs-lookup"><span data-stu-id="42590-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>
2. <span data-ttu-id="42590-109">Özgün kullanıcıyı geri yükleyemezsiniz, bu adımları kullanarak eski kullanıcıyı OneDrive sitesinden kaldırmanız gerekir, Kullanıcı [bilgileri listesinden bir kullanıcıyı kaldırabilirsiniz]().</span><span class="sxs-lookup"><span data-stu-id="42590-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="42590-110">Bu yapıldıktan sonra, kullanıcının [OneDrive sitesine yönetici ekleme](https://docs.microsoft.com/sharepoint/manage-user-profiles) adımlarını Izleyerek kullanıcının OneDrive sitesinde yönetici haklarına sahip olduğunu doğrulayabilirsiniz</span><span class="sxs-lookup"><span data-stu-id="42590-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span></span>

<span data-ttu-id="42590-111">İzin düzeyleri hakkında daha fazla bilgi için [SharePoint 'teki izin düzeylerini anlama](https://docs.microsoft.com/sharepoint/understanding-permission-levels)makalesine bakın.</span><span class="sxs-lookup"><span data-stu-id="42590-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
