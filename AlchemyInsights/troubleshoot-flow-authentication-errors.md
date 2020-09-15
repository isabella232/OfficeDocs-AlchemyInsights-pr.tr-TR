---
title: Kimlik doğrulama hatalarını giderme
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c15fed9f-65c6-422e-9d32-87e889a44b51
ms.openlocfilehash: 3c4ad806ed446803d8c1e0ba17b3a06d591985d9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690587"
---
# <a name="troubleshoot-flow-authentication-errors"></a><span data-ttu-id="83cf4-102">Kimlik doğrulama hatalarını giderme</span><span class="sxs-lookup"><span data-stu-id="83cf4-102">Troubleshoot Flow authentication errors</span></span>

<span data-ttu-id="83cf4-103">Birçok durumda, kimlik doğrulama hatası nedeniyle akış başarısız olur.</span><span class="sxs-lookup"><span data-stu-id="83cf4-103">In many cases, flows fail because of an authentication error.</span></span> <span data-ttu-id="83cf4-104">Bu tür bir hatadır, hata iletisi "yetkisiz" içeriyor veya 401 veya 403 hata kodu görüntüleniyor.</span><span class="sxs-lookup"><span data-stu-id="83cf4-104">If you have this type of error, the error message contains "Unauthorized," or an error code of 401 or 403 appears.</span></span> <span data-ttu-id="83cf4-105">Bağlantıyı güncelleştirerek bir kimlik doğrulama hatasını genellikle düzeltebilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="83cf4-105">You can usually fix an authentication error by updating the connection:</span></span>
  
1. <span data-ttu-id="83cf4-106">Web portalının en üstünde, Ayarlar menüsünü açmak için dişli simgesine tıklayın veya dokunun ve ardından **Bağlantılar**'ı tıklatın veya dokunun.</span><span class="sxs-lookup"><span data-stu-id="83cf4-106">At the top of the web portal, click or tap the gear icon to open the Settings menu, and then click or tap **Connections**.</span></span>
    
2. <span data-ttu-id="83cf4-107">Yetkisiz hata iletisini gördüğünüz bağlantıya gidin.</span><span class="sxs-lookup"><span data-stu-id="83cf4-107">Scroll to the connection for which you saw the Unauthorized error message.</span></span>
    
3. <span data-ttu-id="83cf4-108">Bağlantının yanında, bağlantının doğrulanmadığına ilişkin iletideki **Parolayı Doğrula** bağlantısına tıklayın veya dokunun.</span><span class="sxs-lookup"><span data-stu-id="83cf4-108">Next to the connection, click or tap the **Verify password** link in the message about the connection not being authenticated.</span></span> 
    
4. <span data-ttu-id="83cf4-109">Görüntülenen yönergeleri izleyerek kimlik bilgilerinizi doğrulayın, akış çalışması hatasına dönün ve ardından yeniden **Gönder**'e tıklayın veya dokunun.</span><span class="sxs-lookup"><span data-stu-id="83cf4-109">Verify your credentials by following the instructions that appear, return to your flow-run failure, and then click or tap **Resubmit**.</span></span>
    
<span data-ttu-id="83cf4-110">Daha fazla yardım için bkz [.](https://go.microsoft.com/fwlink/?linkid=872110)</span><span class="sxs-lookup"><span data-stu-id="83cf4-110">For more help, see [Troubleshooting a flow](https://go.microsoft.com/fwlink/?linkid=872110).</span></span>
  

