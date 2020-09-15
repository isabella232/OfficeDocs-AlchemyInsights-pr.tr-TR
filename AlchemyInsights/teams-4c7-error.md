---
title: Ekipler 4c7 hatası
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
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700223"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="c388b-102">Microsoft ekiplerde 4c7 hatası</span><span class="sxs-lookup"><span data-stu-id="c388b-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="c388b-103">Bu hata, Microsoft ekipleri Forms kimlik doğrulaması gerektirdiğinden oluşur.</span><span class="sxs-lookup"><span data-stu-id="c388b-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="c388b-104">Active Directory Federasyon Hizmetleri 'ni (AD FS) dağıtırken, Forms kimlik doğrulaması varsayılan olarak intranet için etkinleştirilmez.</span><span class="sxs-lookup"><span data-stu-id="c388b-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="c388b-105">Windows tümleşik kimlik doğrulaması başarısız olursa, Forms kimlik doğrulaması kullanarak oturum açmanız istenir.</span><span class="sxs-lookup"><span data-stu-id="c388b-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="c388b-106">Bu sorunu çözmek için, Active Directory yerel kopyasının bulunduğu bilgisayarda AD FS Microsoft Yönetim Konsolu (MMC) ek bileşenini kullanarak Forms kimlik doğrulamasını etkinleştirin.</span><span class="sxs-lookup"><span data-stu-id="c388b-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="c388b-107">Bunu yapmak için şu adımları uygulayın:</span><span class="sxs-lookup"><span data-stu-id="c388b-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="c388b-108">Gezinti bölmesinde, **kimlik doğrulama ilkelerine**göz atın.</span><span class="sxs-lookup"><span data-stu-id="c388b-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="c388b-109">Ayrıntılar bölmesindeki **Eylemler** 'In altında **genel birincil kimlik doğrulamasını Düzenle**'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="c388b-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="c388b-110">**Intranet** sekmesinde **Forms Authentication**öğesini seçin.</span><span class="sxs-lookup"><span data-stu-id="c388b-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="c388b-111">**Tamam 'ı** (veya **Uygula**) seçin.</span><span class="sxs-lookup"><span data-stu-id="c388b-111">Select **OK** (or **Apply**).</span></span>