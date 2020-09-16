---
title: Dosya salt okunur açılıyor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: 2fdb4f048c2bee022a49c2cca2ce9770f42a87a2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745627"
---
# <a name="file-open-read-only"></a><span data-ttu-id="f330e-102">Dosya salt okunur açılıyor</span><span class="sxs-lookup"><span data-stu-id="f330e-102">File open read-only</span></span>

<span data-ttu-id="f330e-103">Dosyaları açarken salt okunur olarak açıldığını görebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="f330e-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="f330e-104">Bazı durumlarda bu, internet 'ten dosya açarken ve başka zamanlarda da değiştirilebilen bir ayardan kaynaklanıyor gibi ek güvenlik için.</span><span class="sxs-lookup"><span data-stu-id="f330e-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="f330e-105">Burada, bir dosyanın salt okunur olarak açıldığı bazı senaryolar ve bunu değiştirmek için uygulayabileceğiniz bazı adımlar vardır.</span><span class="sxs-lookup"><span data-stu-id="f330e-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="f330e-106">**Virüsten koruma, kişilerin salt okunur açmasına neden oluyor**</span><span class="sxs-lookup"><span data-stu-id="f330e-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="f330e-107">Bazı virüsten koruma programları, güvenli olmayabilecek dosyaların salt okunur olarak açılmasını koruyabilir.</span><span class="sxs-lookup"><span data-stu-id="f330e-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="f330e-108">Bu ayarları ayarlamayı öğrenmek için virüsten koruma sağlayıcınızla iletişim kurmanız gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="f330e-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="f330e-109">Örneğin, BitDefender 'ın içinde uygulama dışlamaları ekleme hakkında içeriği vardır: [BitDefender denetim merkezinde uygulama veya süreç dışlamaları nasıl eklenir?](https://aka.ms/AA6098i)</span><span class="sxs-lookup"><span data-stu-id="f330e-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="f330e-110">**Dosya özellikleri salt okunur olarak ayarlandı mı?**</span><span class="sxs-lookup"><span data-stu-id="f330e-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="f330e-111">Dosya özelliklerini, dosyayı sağ tıklatıp Özellikler 'i seçerek denetleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="f330e-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="f330e-112">Salt okunur özniteliği işaretliyse, işareti kaldırıp Tamam 'ı tıklatabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="f330e-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="f330e-113">**İçerik korumalı görünümde**</span><span class="sxs-lookup"><span data-stu-id="f330e-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="f330e-114">Internet 'ten ve güvenli olmayabilecek diğer konumlardan gelen dosyalar bilgisayarınıza zarar verebilecek virüs, solucan veya başka türde kötü amaçlı yazılımlar içerebilir.</span><span class="sxs-lookup"><span data-stu-id="f330e-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="f330e-115">Bu, e-posta ekleri</span><span class="sxs-lookup"><span data-stu-id="f330e-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="f330e-116">Bilgisayarınızı korumaya yardımcı olmak için, güvenli olmayabilecek konumlardan gelen dosyalar korumalı görünüm 'de açılır.</span><span class="sxs-lookup"><span data-stu-id="f330e-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="f330e-117">Korumalı Görünüm 'ü kullanarak, bir dosyayı okuyabilir ve risklerini azaltırken içeriğini görebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="f330e-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="f330e-118">Korumalı Görünüm ve ayarları değiştirme hakkında daha fazla bilgi için şu makaleye bakın: [Korumalı Görünüm nedir?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="f330e-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="f330e-119">**OneDrive mı?**</span><span class="sxs-lookup"><span data-stu-id="f330e-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="f330e-120">Dosya OneDrive 'da depolanıyorsa ve OneDrive depolama alanınız doluysa, size ayrılan alanınız gelene kadar belgeyi kaydedemezsiniz.</span><span class="sxs-lookup"><span data-stu-id="f330e-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="f330e-121">Bildirim merkezinde OneDrive simgesine tıklayıp depolama alanını yönet 'i seçerek OneDrive 'daki boş alanınızı denetleyebilir ve Depolamayı Yönet 'i seçerek [https://onedrive.live.com](https://onedrive.live.com) , oturum açabilir, oturum açabilir ve ekranın sol alt kısmındaki kullanılan alanın miktarına bakabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="f330e-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="f330e-122">**Office etkinleştirildi mi?**</span><span class="sxs-lookup"><span data-stu-id="f330e-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="f330e-123">Office etkinleştirilmemişse veya aboneliğinizin süresi dolduysa salt okunur Işlevi azaltılmış olabilir.</span><span class="sxs-lookup"><span data-stu-id="f330e-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="f330e-124">Office 'i etkinleştirme hakkında bilgi için bkz: [Office 'Teki Lisanssız ürün ve etkinleştirme hataları](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="f330e-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="f330e-125">**Tümü başarısız olursa...**</span><span class="sxs-lookup"><span data-stu-id="f330e-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="f330e-126">Bilgisayarı yeniden başlatmayı deneyin</span><span class="sxs-lookup"><span data-stu-id="f330e-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="f330e-127">Office güncelleştirmelerini yükleme</span><span class="sxs-lookup"><span data-stu-id="f330e-127">Install Office updates</span></span>
    
- <span data-ttu-id="f330e-128">Office 'in çevrimiçi onarımını gerçekleştirme</span><span class="sxs-lookup"><span data-stu-id="f330e-128">Perform an Online repair of Office</span></span>
    

