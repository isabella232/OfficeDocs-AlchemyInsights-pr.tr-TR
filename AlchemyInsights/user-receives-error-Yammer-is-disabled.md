---
title: Kullanıcı hata alır AADSTS7000112 Yammer devre dışı bırakılır
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198368"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a><span data-ttu-id="c9cca-102">Kullanıcı hata alır AADSTS7000112 Yammer devre dışı bırakılır</span><span class="sxs-lookup"><span data-stu-id="c9cca-102">User receives error AADSTS7000112 Yammer is disabled</span></span>

<span data-ttu-id="c9cca-103">"AADSTS7000112: Application '0000000-0ff1-ce00-000000000000'(Yammer) devre dışı bırakılır" hatasını alırsanız, Azure AD içindeki hizmet müdüründe bir sorun vardır.</span><span class="sxs-lookup"><span data-stu-id="c9cca-103">If you receive the error "AADSTS7000112: Application '00000005-0000-0ff1-ce00-000000000000'(Yammer) is disabled", a problem exists with the service principal within Azure AD.</span></span> <span data-ttu-id="c9cca-104">Bir yönetici, Yammer'a erişimi engellemek için hizmet yöneticisini devre dışı bıraktı.</span><span class="sxs-lookup"><span data-stu-id="c9cca-104">An administrator might have disabled the service principal to block access to Yammer.</span></span>

<span data-ttu-id="c9cca-105">Hizmet ilkesini devre dışı bırakmak önerilmez ve ek sorunlara neden olabilir.</span><span class="sxs-lookup"><span data-stu-id="c9cca-105">Disabling the service principal is not recommended and can cause additional issues.</span></span> <span data-ttu-id="c9cca-106">Yammer kullanıcı erişimini engellemek için desteklenen yaklaşım hakkında daha fazla bilgi için [bkz.](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access)</span><span class="sxs-lookup"><span data-stu-id="c9cca-106">For more info about the supported approach to block user access to Yammer, see [Turn off Yammer access for Microsoft 365 users](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span></span>  

<span data-ttu-id="c9cca-107">Azure Portalı'ndaki bu sorunu düzeltmek ve Kullanıcı erişimini Yammer'a geri yüklemek için:</span><span class="sxs-lookup"><span data-stu-id="c9cca-107">To correct this issue in the Azure Portal and restore user access to Yammer:</span></span>

1.  <span data-ttu-id="c9cca-108">Azure Etkin Dizin sayfasını açın ve sol gezinti bölmesinde **Yönet** altındaki **Kurumsal uygulamaları** seçin.</span><span class="sxs-lookup"><span data-stu-id="c9cca-108">Open the Azure Active Directory page, and select **Enterprise applications** under **Manage** in the left navigation pane.</span></span>
3.  <span data-ttu-id="c9cca-109">Arama kutusuna **Office 365 Yammer** yazın ve ayarları açmak için uygulama adını seçin.</span><span class="sxs-lookup"><span data-stu-id="c9cca-109">Type **Office 365 Yammer** in the search box, and select the application name to open settings.</span></span>
4.  <span data-ttu-id="c9cca-110">Sol gezinti bölmesinde **Yönet** altındaki **Özellikleri** seçin.</span><span class="sxs-lookup"><span data-stu-id="c9cca-110">Select **Properties** under **Manage** in the left navigation pane.</span></span>
5.  <span data-ttu-id="c9cca-111">Kullanıcıların oturum **açmaları için Etkin'in** değerini evet **olarak**ayarlayın ve ardından **Kaydet'i**seçin.</span><span class="sxs-lookup"><span data-stu-id="c9cca-111">Set the value of **Enabled for users to sign-in?** to **Yes**, and then select **Save**.</span></span>
6.  <span data-ttu-id="c9cca-112">Yammer'la tekrar anlaş.</span><span class="sxs-lookup"><span data-stu-id="c9cca-112">Sign in to Yammer again.</span></span> <span data-ttu-id="c9cca-113">Çerezleri temizlemeniz gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="c9cca-113">You might need to clear cookies.</span></span>

<span data-ttu-id="c9cca-114">Alternatif olarak, değeri ayarlamak için PowerShell komutlarını çalıştırın.</span><span class="sxs-lookup"><span data-stu-id="c9cca-114">Alternatively, run PowerShell commands to set the value.</span></span> <span data-ttu-id="c9cca-115">Daha fazla bilgi için, [Office 365'teki Yammer döşemesini tıklattığınızda "Üzgünüz, ancak oturum açmada sorun yaşıyoruz" hatasına](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365)bakın.</span><span class="sxs-lookup"><span data-stu-id="c9cca-115">For more info, see ["Sorry, but we're having trouble signing you in" error when you click the Yammer tile in Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span></span> 