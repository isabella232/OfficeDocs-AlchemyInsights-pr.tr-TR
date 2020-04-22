---
title: Sorun Giderme Akışı kimlik doğrulama hataları
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c15fed9f-65c6-422e-9d32-87e889a44b51
ms.openlocfilehash: 70451f074a65a4454faeadd188a31783be8e6c7e
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759748"
---
# <a name="troubleshoot-flow-authentication-errors"></a><span data-ttu-id="0bcd3-102">Sorun Giderme Akışı kimlik doğrulama hataları</span><span class="sxs-lookup"><span data-stu-id="0bcd3-102">Troubleshoot Flow authentication errors</span></span>

<span data-ttu-id="0bcd3-103">Çoğu durumda, bir kimlik doğrulama hatası nedeniyle akışlar başarısız olur.</span><span class="sxs-lookup"><span data-stu-id="0bcd3-103">In many cases, flows fail because of an authentication error.</span></span> <span data-ttu-id="0bcd3-104">Bu tür bir hata varsa, hata iletisi "Yetkisiz" içerir veya 401 veya 403 hata kodu görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="0bcd3-104">If you have this type of error, the error message contains "Unauthorized," or an error code of 401 or 403 appears.</span></span> <span data-ttu-id="0bcd3-105">Genellikle bağlantıyı güncelleştirerek bir kimlik doğrulama hatasını düzeltebilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="0bcd3-105">You can usually fix an authentication error by updating the connection:</span></span>
  
1. <span data-ttu-id="0bcd3-106">Web portalının üst kısmında Ayarlar menüsünü açmak için vites simgesine tıklayın veya dokunun ve ardından **Bağlantılar'ı**tıklatın veya dokunun.</span><span class="sxs-lookup"><span data-stu-id="0bcd3-106">At the top of the web portal, click or tap the gear icon to open the Settings menu, and then click or tap **Connections**.</span></span>
    
2. <span data-ttu-id="0bcd3-107">Yetkisiz hata iletisini gördüğünüz bağlantıya gidin.</span><span class="sxs-lookup"><span data-stu-id="0bcd3-107">Scroll to the connection for which you saw the Unauthorized error message.</span></span>
    
3. <span data-ttu-id="0bcd3-108">Bağlantının yanında, bağlantının kimliği doğrulanmaması yla ilgili iletideki **parolayı doğrula** bağlantısını tıklatın veya dokunun.</span><span class="sxs-lookup"><span data-stu-id="0bcd3-108">Next to the connection, click or tap the **Verify password** link in the message about the connection not being authenticated.</span></span> 
    
4. <span data-ttu-id="0bcd3-109">Görünen yönergeleri izleyerek kimlik bilgilerinizi doğrulayın, akış çalıştırma hatanıza dönün ve ardından **Yeniden Gönder'e**tıklayın veya dokunun.</span><span class="sxs-lookup"><span data-stu-id="0bcd3-109">Verify your credentials by following the instructions that appear, return to your flow-run failure, and then click or tap **Resubmit**.</span></span>
    
<span data-ttu-id="0bcd3-110">Daha fazla yardım için, [sorun giderme akışını](https://go.microsoft.com/fwlink/?linkid=872110)görün.</span><span class="sxs-lookup"><span data-stu-id="0bcd3-110">For more help, see [Troubleshooting a flow](https://go.microsoft.com/fwlink/?linkid=872110).</span></span>
  

