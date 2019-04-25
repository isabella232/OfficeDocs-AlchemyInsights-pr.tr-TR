---
title: Akış kimlik doğrulama hatalarında sorun giderme
ms.author: kaarins
author: kaarins
ms.date: 6/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c15fed9f-65c6-422e-9d32-87e889a44b51
ms.openlocfilehash: e578149e37c86178b98cf6073f6ed6325f42c455
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32393633"
---
# <a name="troubleshoot-flow-authentication-errors"></a><span data-ttu-id="bd965-102">Akış kimlik doğrulama hatalarında sorun giderme</span><span class="sxs-lookup"><span data-stu-id="bd965-102">Troubleshoot Flow authentication errors</span></span>

<span data-ttu-id="bd965-103">Çoğu durumda, akışı bir kimlik doğrulama hatası nedeniyle başarısız.</span><span class="sxs-lookup"><span data-stu-id="bd965-103">In many cases, flows fail because of an authentication error.</span></span> <span data-ttu-id="bd965-104">Bu tür bir hata varsa, hata iletisi "Yetkisiz" içeriyor veya 401 veya 403 hata kodu görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="bd965-104">If you have this type of error, the error message contains "Unauthorized," or an error code of 401 or 403 appears.</span></span> <span data-ttu-id="bd965-105">Genellikle, bağlantı güncelleştirerek kimlik doğrulama hatası düzeltebilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="bd965-105">You can usually fix an authentication error by updating the connection:</span></span>
  
1. <span data-ttu-id="bd965-106">Web portalı üstündeki dişli simgesini ayarları menüsünü açın ve ardından **bağlantıları**dokunun dokunun veya tıklatın.</span><span class="sxs-lookup"><span data-stu-id="bd965-106">At the top of the web portal, click or tap the gear icon to open the Settings menu, and then click or tap **Connections**.</span></span>
    
2. <span data-ttu-id="bd965-107">Yetkisiz hata iletisinde gördüğünüz bağlantıya gidin.</span><span class="sxs-lookup"><span data-stu-id="bd965-107">Scroll to the connection for which you saw the Unauthorized error message.</span></span>
    
3. <span data-ttu-id="bd965-108">Bağlantının ileti kimlik doğrulaması bağlantısı hakkında **Parolayı doğrula** bağlantısını dokunun veya tıklatın.</span><span class="sxs-lookup"><span data-stu-id="bd965-108">Next to the connection, click or tap the **Verify password** link in the message about the connection not being authenticated.</span></span> 
    
4. <span data-ttu-id="bd965-109">Görünür, akış çalıştırma hatası için geri dönmek ve ardından **yeniden**dokunun yönergeleri izleyerek kimlik bilgilerinizi doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="bd965-109">Verify your credentials by following the instructions that appear, return to your flow-run failure, and then click or tap **Resubmit**.</span></span>
    
<span data-ttu-id="bd965-110">Daha fazla yardım için bkz: [Akış sorunlarını giderme](https://go.microsoft.com/fwlink/?linkid=872110).</span><span class="sxs-lookup"><span data-stu-id="bd965-110">For more help, see [Troubleshooting a flow](https://go.microsoft.com/fwlink/?linkid=872110).</span></span>
  

