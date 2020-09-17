---
title: Nasıl yapılır-içeri aktar-NK2-Files
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: 6a823f6e0c4c46de64dd7b70fb40c76255d78ec1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47780079"
---
# <a name="how-to-import-nk2-files"></a><span data-ttu-id="6d44a-102">Nk2 dosyalarını içeri aktarma</span><span class="sxs-lookup"><span data-stu-id="6d44a-102">How to import .nk2 files</span></span> 

<span data-ttu-id="6d44a-103">Microsoft Outlook 2013, Outlook 2016, Outlook 2019 veya Microsoft 365 için Outlook 'u ilk kez başlattığınızda, ( *ProfilAdı*. nk2 dosyasında depolanan) takma ad önbelleğiniz, varsayılan ileti deponuzun gizli bir iletiye aktarılır.</span><span class="sxs-lookup"><span data-stu-id="6d44a-103">When you start Microsoft Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Microsoft 365 for the first time, your nickname cache (stored in the *profilename*.nk2 file) is imported into a hidden message in your default message store.</span></span>

<span data-ttu-id="6d44a-104">Nk2 dosyalarını Outlook 2013, Outlook 2016, Outlook 2019 veya Microsoft 365 için Outlook 'a aktarmak için,. nk2 dosyasının aşağıdaki klasörde olduğundan emin olun:%appdata%\Microsoft\Outlook</span><span class="sxs-lookup"><span data-stu-id="6d44a-104">To import .nk2 files into Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Microsoft 365, make sure that the .nk2 file is in the following folder: %appdata%\Microsoft\Outlook</span></span>

<span data-ttu-id="6d44a-105">**Not**:. nk2 dosyası, geçerli Outlook 2013 veya Outlook 2016 profilinizle aynı ada sahip olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="6d44a-105">**Note**: The .nk2 file must have the same name as your current Outlook 2013 or Outlook 2016 profile.</span></span> <span data-ttu-id="6d44a-106">Varsayılan olarak, profil adı "Outlook" olur.</span><span class="sxs-lookup"><span data-stu-id="6d44a-106">By default, the profile name is "Outlook."</span></span> <span data-ttu-id="6d44a-107">Profil adını denetlemek için aşağıdaki adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="6d44a-107">To check the profile name, follow these steps:</span></span> 
1. <span data-ttu-id="6d44a-108">**Başlat**'a ve ardından **Denetim Masası**'na tıklayın.</span><span class="sxs-lookup"><span data-stu-id="6d44a-108">Click **Start**, and then click **Control Panel**.</span></span>
2. <span data-ttu-id="6d44a-109">**Posta**'yı çift tıklatın.</span><span class="sxs-lookup"><span data-stu-id="6d44a-109">Double-click **Mail**.</span></span>
3. <span data-ttu-id="6d44a-110">Posta Kurulumu iletişim kutusunda **profilleri göster**'i seçin.</span><span class="sxs-lookup"><span data-stu-id="6d44a-110">In the Mail Setup dialog box, select **Show Profiles**.</span></span>
4. <span data-ttu-id="6d44a-111">Çalıştırmayı **Başlat**'ı seçin  >  **Run**.</span><span class="sxs-lookup"><span data-stu-id="6d44a-111">Select **Start** > **Run**.</span></span>
5. <span data-ttu-id="6d44a-112">**Aç** kutusuna *outlook.exe/Importnk2*yazın ve **Tamam 'ı**seçin.</span><span class="sxs-lookup"><span data-stu-id="6d44a-112">In the **Open** box, type *outlook.exe /importnk2*, and then select **OK**.</span></span> 

<span data-ttu-id="6d44a-113">. Nk2 dosyasını içeri aktardıktan sonra, dosyanın içeriği posta kutunuzda depolanan varolan takma ad önbelleğine birleştirilir.</span><span class="sxs-lookup"><span data-stu-id="6d44a-113">After you import the .nk2 file, the contents of the file are merged into the existing nickname cache stored in your mailbox.</span></span>

<span data-ttu-id="6d44a-114">**Not**: Outlook 2013, Outlook 2016, Outlook 2019 veya Microsoft 365 için Outlook 'u çalıştırdığınızda. nk2 dosyası. old dosya adı uzantısıyla yeniden adlandırılır.</span><span class="sxs-lookup"><span data-stu-id="6d44a-114">**Note**: The .nk2 file is renamed with a .old file name extension the next time you start Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Microsoft 365.</span></span> <span data-ttu-id="6d44a-115">. Nk2 dosyasını yeniden içeri aktarmak istiyorsanız, önce. old dosya adı uzantısını kaldırın.</span><span class="sxs-lookup"><span data-stu-id="6d44a-115">If want to re-import the .nk2 file, remove the .old file name extension first.</span></span>

<span data-ttu-id="6d44a-116">Daha fazla bilgi için bkz: [Otomatik Tamamlama listesini başka bir bilgisayara aktarma veya kopyalama](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%).</span><span class="sxs-lookup"><span data-stu-id="6d44a-116">For more information, see [Import or copy the Auto-Complete List to another computer](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%).</span></span>