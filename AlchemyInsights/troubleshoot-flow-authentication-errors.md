---
title: Sorun Giderme Akışı kimlik doğrulama hataları
ms.author: pebaum
author: pebaum
ms.date: 6/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c15fed9f-65c6-422e-9d32-87e889a44b51
ms.openlocfilehash: 3d49d15d243dd98afc6f78b9e75f0cfa74c2cd7c
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050653"
---
# <a name="troubleshoot-flow-authentication-errors"></a><span data-ttu-id="240ab-102">Sorun Giderme Akışı kimlik doğrulama hataları</span><span class="sxs-lookup"><span data-stu-id="240ab-102">Troubleshoot Flow authentication errors</span></span>

<span data-ttu-id="240ab-103">Çoğu durumda, bir kimlik doğrulama hatası nedeniyle akışlar başarısız olur.</span><span class="sxs-lookup"><span data-stu-id="240ab-103">In many cases, flows fail because of an authentication error.</span></span> <span data-ttu-id="240ab-104">Bu tür bir hata varsa, hata iletisi "Yetkisiz" içerir veya 401 veya 403 hata kodu görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="240ab-104">If you have this type of error, the error message contains "Unauthorized," or an error code of 401 or 403 appears.</span></span> <span data-ttu-id="240ab-105">Genellikle bağlantıyı güncelleştirerek bir kimlik doğrulama hatasını düzeltebilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="240ab-105">You can usually fix an authentication error by updating the connection:</span></span>
  
1. <span data-ttu-id="240ab-106">Web portalının üst kısmında Ayarlar menüsünü açmak için vites simgesine tıklayın veya dokunun ve ardından **Bağlantılar'ı**tıklatın veya dokunun.</span><span class="sxs-lookup"><span data-stu-id="240ab-106">At the top of the web portal, click or tap the gear icon to open the Settings menu, and then click or tap **Connections**.</span></span>
    
2. <span data-ttu-id="240ab-107">Yetkisiz hata iletisini gördüğünüz bağlantıya gidin.</span><span class="sxs-lookup"><span data-stu-id="240ab-107">Scroll to the connection for which you saw the Unauthorized error message.</span></span>
    
3. <span data-ttu-id="240ab-108">Bağlantının yanında, bağlantının kimliği doğrulanmaması yla ilgili iletideki **parolayı doğrula** bağlantısını tıklatın veya dokunun.</span><span class="sxs-lookup"><span data-stu-id="240ab-108">Next to the connection, click or tap the **Verify password** link in the message about the connection not being authenticated.</span></span> 
    
4. <span data-ttu-id="240ab-109">Görünen yönergeleri izleyerek kimlik bilgilerinizi doğrulayın, akış çalıştırma hatanıza dönün ve ardından **Yeniden Gönder'e**tıklayın veya dokunun.</span><span class="sxs-lookup"><span data-stu-id="240ab-109">Verify your credentials by following the instructions that appear, return to your flow-run failure, and then click or tap **Resubmit**.</span></span>
    
<span data-ttu-id="240ab-110">Daha fazla yardım için, [sorun giderme akışını](https://go.microsoft.com/fwlink/?linkid=872110)görün.</span><span class="sxs-lookup"><span data-stu-id="240ab-110">For more help, see [Troubleshooting a flow](https://go.microsoft.com/fwlink/?linkid=872110).</span></span>
  

