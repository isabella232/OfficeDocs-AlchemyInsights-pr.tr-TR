---
title: 126 OWA'da Posta Kutusu alma hatası bulunamıyor mu?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426682"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="81f66-102">Web üzerinde Outlook'ta posta kutusu bulunamadı hatası mı alasınız?</span><span class="sxs-lookup"><span data-stu-id="81f66-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="81f66-103">Web üzerinde Outlook kullanıyorsanız ve hata için bir Posta Kutusu bulunamadı varsa, Web üzerinde **Outlook'a** bağlanmak için kullanılan hesabın Exchange Online lisansı yoktur ve dolayısıyla hesapla ilişkilendirilmiş posta kutusu yoktur.</span><span class="sxs-lookup"><span data-stu-id="81f66-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="81f66-104">Yöneticiniz aşağıdaki adımları kullanarak hesabınıza lisans atayabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="81f66-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="81f66-105">Microsoft [365 yönetim](https://portal.office.com/adminportal/home#/homepage) merkezini açın  ve Kullanıcılar  bölümünün altında Etkin kullanıcılar'a gidin ve hatayı gören kullanıcıyı seçin.</span><span class="sxs-lookup"><span data-stu-id="81f66-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="81f66-106">Açılan kullanıcı sayfasında Lisanslar ve  Uygulamalar bölümüne gidin, uygun  Konum değerini seçin ve Exchange Online içeren bir lisans attayın (ayrıntılarını görmek için lisansı genişletin).</span><span class="sxs-lookup"><span data-stu-id="81f66-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="81f66-107">Bitirdikten sonra, Değişiklikleri **kaydet'e tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="81f66-107">When you're finished, click **Save changes**.</span></span>

<span data-ttu-id="81f66-108">Bazı durumlarda, lisans bir kullanıcı hesabına zaten atanmışsa, lisansın kaldırılması ve yeniden atanmış olması sorunu çözmenize ve sistemde düzgün bir şekilde sağlanmasına yardımcı olur:</span><span class="sxs-lookup"><span data-stu-id="81f66-108">In some cases, if the license is already assigned to a user account, removing and reassigning the license helps to resolve the issue and get it properly provisioned in the system:</span></span> 

- <span data-ttu-id="81f66-109">M365 Exchange Online (ve varsa diğer) aboneliklerinizi güncel olup olmadığını ve henüz süresinin dolmadı olup olmadığını kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="81f66-109">Check to see if your M365 Exchange Online (and other, if you have any) subscriptions are current and have not recently expired.</span></span>

<span data-ttu-id="81f66-110">Aboneliğinizin süresinin dolmamış olduğundan ve kullanıcı hesabına geçerli bir lisans atanmalarından emin olduktan sonra, lisansın sağlanması 24 saate kadar sürebilir, bu nedenle sorununuzu çözmeyi beklemeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="81f66-110">Once you have made sure that your subscription has not expired and a valid license has been assigned to the user account, it can take up to 24 hours for license to get provisioned, so you might have to wait for your issue to resolve.</span></span> <span data-ttu-id="81f66-111">Daha fazla bilgi için bkz. [Lisans atama ve yönetme.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)</span><span class="sxs-lookup"><span data-stu-id="81f66-111">For more info, see [Assign and manage licenses](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).</span></span>