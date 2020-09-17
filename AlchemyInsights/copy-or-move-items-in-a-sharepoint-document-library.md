---
title: SharePoint belge kitaplığındaki öğeleri kopyalama veya taşıma
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "454"
- "5300013"
ms.assetid: 592f502a-493f-4bf4-adc3-5bc8aea87bb5
ms.openlocfilehash: d7aa865a6b3db0871a57313dd7d6f5b0213ca0e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807139"
---
# <a name="copy-or-move-items-in-a-sharepoint-document-library"></a><span data-ttu-id="d9114-102">SharePoint belge kitaplığındaki öğeleri kopyalama veya taşıma</span><span class="sxs-lookup"><span data-stu-id="d9114-102">Copy or move items in a SharePoint document library</span></span>

<span data-ttu-id="d9114-103">Dosya, klasör ve bağlantıları belge kitaplığında farklı konumlara kopyalayabilir ve taşıyabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d9114-103">You can copy and move files, folders, and links to different locations within a document library.</span></span> <span data-ttu-id="d9114-104">Ayrıca öğeler arasında öğeleri kopyalayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d9114-104">You can also copy items across sites.</span></span> 
  
1. <span data-ttu-id="d9114-105">Tarayıcıda, taşımak istediğiniz dosyaları, klasörleri veya bağlantıları bulun ve **Kopyala** 'Ya veya **Taşı 'ya**tıklayın.</span><span class="sxs-lookup"><span data-stu-id="d9114-105">In a browser, browse to the files, folders, or links you want to move, and then click **Copy to** or **Move to**.</span></span>

    > [!NOTE]
    > <span data-ttu-id="d9114-106">SharePoint Online 'ın klasik deneyimini kullanıyorsanız, **Kopyala** ve **Taşı 'ya** de kullanılamaz.</span><span class="sxs-lookup"><span data-stu-id="d9114-106">**Copy to** and **Move to** aren't available if you're using the classic experience of SharePoint Online.</span></span>
  
2. <span data-ttu-id="d9114-107">**Hedef Seç**'in altında, öğeleri kopyalamak veya taşımak istediğiniz konumu seçin veya sitelerin tam listesini görmek Için **sitelere Gözat** 'a tıklayın.</span><span class="sxs-lookup"><span data-stu-id="d9114-107">Under **Choose a destination**, select the location to which you want to copy or move the items or click **Browse sites** to see the full list of sites.</span></span>

    > [!NOTE]
    > <span data-ttu-id="d9114-108">Öğeleri kopyaladığınızda listelenen diğer siteleri görmüyorsanız, siteler arasında kopyalama yapılandırılmamış.</span><span class="sxs-lookup"><span data-stu-id="d9114-108">If you don't see other sites listed when you copy items, copying across sites hasn't been configured.</span></span> <span data-ttu-id="d9114-109">Etkinleştirmek için, SharePoint yönetim merkezinin ayarlar sayfasına gidin ve **Tamam**'ı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="d9114-109">To enable it, go to the settings page of the SharePoint admin center and click **OK**.</span></span>
  
    <span data-ttu-id="d9114-110">Yeni bir klasör oluşturmak için, klasör hiyerarşisinde bir konum seçin, **Yeni klasör**'ü tıklatın, klasör için bir ad girin ve sonra da adı kaydetmek için denetim işaretini tıklatın.</span><span class="sxs-lookup"><span data-stu-id="d9114-110">To create a new folder, select a location in the folder hierarchy, click **New folder**, enter a name for the folder, and click the check mark to save the name.</span></span>

3. <span data-ttu-id="d9114-111">**Buraya Kopyala** 'yı veya **buraya taşı**'yı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="d9114-111">Click **Copy here** or **Move here**.</span></span>

    > [!NOTE]
    > <span data-ttu-id="d9114-112">Bir kerede 500 MB 'ye kadar dosya ve klasör kopyalayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d9114-112">You can copy up to 500 MB of files and folders at one time.</span></span> <span data-ttu-id="d9114-113">Sürüm geçmişi olan belgeleri kopyaladığınızda >, yalnızca en son sürüm kopyalanır.</span><span class="sxs-lookup"><span data-stu-id="d9114-113">>  When you copy documents that have version history, only the latest version is copied.</span></span> <span data-ttu-id="d9114-114">Belgeleri taşıdığınızda, geçmişi de taşınır.</span><span class="sxs-lookup"><span data-stu-id="d9114-114">When you move documents, their history is also moved.</span></span>
  
 <span data-ttu-id="d9114-115">Bir dosya taşındığında, kaynak dizinde tamamen olana kadar görünmeye devam eder ve sonra silinir.</span><span class="sxs-lookup"><span data-stu-id="d9114-115">When a file is moving, it will still appear in the source directory until its fully moved to the destination, and then it will be deleted.</span></span> <span data-ttu-id="d9114-116">Dosya, taşıma tamamlandıktan sonra kaynak siteler geri dönüşüm kutusu 'nda kalacak ve Kullanıcı geri dönüşüm kutusu 'ndan kurtarmadıkça normal geri dönüşüm zamanlamasına tabidir.</span><span class="sxs-lookup"><span data-stu-id="d9114-116">The file will remain in the source sites recycle bin after the move is complete and be subject to the normal recycle schedule unless a user recovers it from the recycle bin.</span></span>

<span data-ttu-id="d9114-117">Daha fazla bilgi için bkz.:</span><span class="sxs-lookup"><span data-stu-id="d9114-117">For more information, see:</span></span>

 - <span data-ttu-id="d9114-118">[SharePoint 'te dosyaları taşıma veya kopyalama](https://support.office.com/article/move-or-copy-files-in-sharepoint-00e2f483-4df3-46be-a861-1f5f0c1a87bc) (Office Destek makalesi)</span><span class="sxs-lookup"><span data-stu-id="d9114-118">[Move or copy files in SharePoint](https://support.office.com/article/move-or-copy-files-in-sharepoint-00e2f483-4df3-46be-a861-1f5f0c1a87bc) (Office support article)</span></span>
 - <span data-ttu-id="d9114-119">[Dosyaları herhangi bir klasörden taşıma](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Now-move-files-anywhere-in-Office-365-SharePoint-and-OneDrive/ba-p/146973) (Microsoft Tech Community Web günlüğü makalesi)</span><span class="sxs-lookup"><span data-stu-id="d9114-119">[Move files from any folder](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Now-move-files-anywhere-in-Office-365-SharePoint-and-OneDrive/ba-p/146973) (Microsoft Tech Community blog article)</span></span>  