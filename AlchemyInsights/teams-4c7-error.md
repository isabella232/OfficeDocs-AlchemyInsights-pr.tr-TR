---
title: Takımlar 4c7 hatası
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796440"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="a0977-102">Microsoft Teams'de 4c7 hatası</span><span class="sxs-lookup"><span data-stu-id="a0977-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="a0977-103">Microsoft Teams Formkimlik Doğrulaması gerektirdiğinden bu hata oluşur.</span><span class="sxs-lookup"><span data-stu-id="a0977-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="a0977-104">Active Directory Federation Services (AD FS) dağıttığınızda, Form kimlik doğrulaması varsayılan olarak intranet için etkinleştirilmez.</span><span class="sxs-lookup"><span data-stu-id="a0977-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="a0977-105">Windows Tümleşik Kimlik Doğrulama başarısız olursa, Form kimlik doğrulaması kullanarak oturum açmanız istenir.</span><span class="sxs-lookup"><span data-stu-id="a0977-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="a0977-106">Bu sorunu gidermek için, Active Directory'nin yerel kopyasına sahip bilgisayarda AD FS Microsoft Yönetim Konsolu (MMC) snap-in'i kullanarak Form Kimlik Doğrulaması'nı etkinleştirin.</span><span class="sxs-lookup"><span data-stu-id="a0977-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="a0977-107">Bunu yapmak için aşağıdaki adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="a0977-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="a0977-108">Gezinti bölmesinde Kimlik Doğrulama **İlkeleri'ne**göz atın.</span><span class="sxs-lookup"><span data-stu-id="a0977-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="a0977-109">Ayrıntılar bölmesindeki **Eylemler** altında, **Genel Birincil Kimlik Doğrulamasını Edit'i**seçin.</span><span class="sxs-lookup"><span data-stu-id="a0977-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="a0977-110">**Intranet** sekmesinde **Form kimlik doğrulaması'nı**seçin.</span><span class="sxs-lookup"><span data-stu-id="a0977-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="a0977-111">**Tamam** 'ı (veya **Uygula'yı**) seçin.</span><span class="sxs-lookup"><span data-stu-id="a0977-111">Select **OK** (or **Apply**).</span></span>