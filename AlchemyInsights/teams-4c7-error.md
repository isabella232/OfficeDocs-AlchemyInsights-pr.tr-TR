---
title: Teams 4c7 hatası
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
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786689"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="1a215-102">Microsoft Teams'de 4c7 hatası</span><span class="sxs-lookup"><span data-stu-id="1a215-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="1a215-103">Bu hata, Microsoft Teams'de Forms Authentication'ın gerekli olduğu için oluşur.</span><span class="sxs-lookup"><span data-stu-id="1a215-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="1a215-104">Active Directory Federasyon Hizmetleri'nin (AD FS) dağıtımında, Forms Kimlik Doğrulaması intranet için varsayılan olarak etkinleştirilmez.</span><span class="sxs-lookup"><span data-stu-id="1a215-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="1a215-105">Windows Tümleşik Kimlik Doğrulaması başarısız olursa, Forms Authentication'ı kullanarak oturum açmanız istenir.</span><span class="sxs-lookup"><span data-stu-id="1a215-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="1a215-106">Bu sorunu çözmek için, Active Directory'nin yerel kopyasına sahip bilgisayarda AD FS Microsoft Yönetim Konsolu (MMC) ek bileşenini kullanarak Forms Kimlik Doğrulamasını etkinleştirin.</span><span class="sxs-lookup"><span data-stu-id="1a215-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="1a215-107">Bunu yapmak için şu adımları uygulayın:</span><span class="sxs-lookup"><span data-stu-id="1a215-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="1a215-108">Gezinti bölmesinde Kimlik Doğrulama İlkeleri'ne **gidin.**</span><span class="sxs-lookup"><span data-stu-id="1a215-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="1a215-109">Ayrıntılar **bölmesindeki** Eylemler'in altında Genel Birincil Kimlik **Doğrulamayı Düzenle'yi seçin.**</span><span class="sxs-lookup"><span data-stu-id="1a215-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="1a215-110">Intranet sekmesinde **Forms** Authentication öğesini **seçin.**</span><span class="sxs-lookup"><span data-stu-id="1a215-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="1a215-111">**Tamam'ı** (veya **Uygula'yi) seçin.**</span><span class="sxs-lookup"><span data-stu-id="1a215-111">Select **OK** (or **Apply**).</span></span>