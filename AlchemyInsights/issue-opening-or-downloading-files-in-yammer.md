---
title: Yammer'da dosya açma veya indirme sorunu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148438"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a><span data-ttu-id="f1637-102">Yammer'da dosya açma veya indirme sorunu</span><span class="sxs-lookup"><span data-stu-id="f1637-102">Issue opening or downloading files in Yammer</span></span>

<span data-ttu-id="f1637-103">Klasik Yammer, iletilere ve gruplara dosya yüklemeleri için birden çok seçeneği destekler.</span><span class="sxs-lookup"><span data-stu-id="f1637-103">Classic Yammer supports multiple option for file uploads to messages and groups.</span></span> <span data-ttu-id="f1637-104">Ağ yapılandırmasına bağlı olarak, dosyalar SharePoint'te depolama için varsayılan dır.</span><span class="sxs-lookup"><span data-stu-id="f1637-104">Depending on network configuration, files default to storage in SharePoint.</span></span>

<span data-ttu-id="f1637-105">Yeni Yammer dosya seçici henüz klasik Yammer mevcut tüm seçenekleri desteklemez.</span><span class="sxs-lookup"><span data-stu-id="f1637-105">The file picker in new Yammer does not yet support all the options available in classic Yammer.</span></span> <span data-ttu-id="f1637-106">Gelecekteki bir güncelleştirme ek özellikler ekler.</span><span class="sxs-lookup"><span data-stu-id="f1637-106">A future update will add additional features.</span></span> <span data-ttu-id="f1637-107">Daha fazla bilgi için bkz: [Bir Yammer konuşma gönderisine dosya veya resim ekle.](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8)</span><span class="sxs-lookup"><span data-stu-id="f1637-107">For more info, see [Attach a file or image to a Yammer conversation post](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span></span>

<span data-ttu-id="f1637-108">**Dosya açılmıyor veya indiremiyor**</span><span class="sxs-lookup"><span data-stu-id="f1637-108">**Unable to open or download a file**</span></span>  

<span data-ttu-id="f1637-109">Bir dosya Yammer'a yüklenebilir, ancak SharePoint Online'daki bir dosyaya da bağlantı verebilir.</span><span class="sxs-lookup"><span data-stu-id="f1637-109">A file might upload to Yammer but also be linking to a file in SharePoint Online.</span></span> <span data-ttu-id="f1637-110">Sorun gidermek için önce dosyanın konumunu belirlemeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="f1637-110">To troubleshoot, first you must determine the location of the file.</span></span> <span data-ttu-id="f1637-111">Dosya Yammer'a yüklenmişse, \*.yammer.com URL'si olacaktır.</span><span class="sxs-lookup"><span data-stu-id="f1637-111">If the file has been uploaded to Yammer, it will have a \*.yammer.com URL.</span></span> <span data-ttu-id="f1637-112">Gerekli URL'lerin ve IP adreslerinin engelinin kaldırDığından emin olun.</span><span class="sxs-lookup"><span data-stu-id="f1637-112">Ensure that required URLs and IP addresses are unblocked.</span></span> <span data-ttu-id="f1637-113">Daha fazla bilgi için, [Yammer için sabit kodlu IP adreslerini kullanarak](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592)blog yazısına bakın tavsiye edilmez.</span><span class="sxs-lookup"><span data-stu-id="f1637-113">For more info, see the blog post [Using hard coded IP addresses for Yammer is not recommended](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span></span>

<span data-ttu-id="f1637-114">Aynı zamanda genel yönetici olan bir kullanıcının dosyayı karşıdan yükleyip indiremeyeceğini kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="f1637-114">Check whether a user who is also a global admin can download the file.</span></span> <span data-ttu-id="f1637-115">Dosya özelse, Özel İçerik Modu'nu kullanmanız gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="f1637-115">If the file is private, you might have to use Private Content Mode.</span></span> <span data-ttu-id="f1637-116">Daha fazla bilgi için, daha sonra [Yammer özel içeriği izleyin](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content)bakın.</span><span class="sxs-lookup"><span data-stu-id="f1637-116">For more info, see then [Monitor private content in Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span></span>  

<span data-ttu-id="f1637-117">**Yammer ağ düzeyinde konuklar ve SharePoint Online dosyaları**</span><span class="sxs-lookup"><span data-stu-id="f1637-117">**Yammer network-level guests and files in SharePoint Online**</span></span>  

<span data-ttu-id="f1637-118">[Yammer'daki ağ düzeyindeki konuklar](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) Azure AD B2B kullanmaz ve Yammer hizmetine dahil olduğundan SharePoint'te depolanan Yammer dosyalarına erişemezler.</span><span class="sxs-lookup"><span data-stu-id="f1637-118">[Network-level guests in Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) do not use Azure AD B2B and are internal to the Yammer service, so they can't access Yammer files stored in SharePoint.</span></span> <span data-ttu-id="f1637-119">Bu kimliği kullanarak SharePoint Online'daki belge kitaplıklara erişebilen harici bir AAD B2B kullanıcısı oluşturun.</span><span class="sxs-lookup"><span data-stu-id="f1637-119">Create an external AAD B2B user who can access document libraries in SharePoint Online by using that identity.</span></span> <span data-ttu-id="f1637-120">Yammer'da gelecekteki Azure AD B2B konuk desteği hakkında daha fazla bilgi için, [Yammer Preview - Müşteri Koşulları ve SSS'de İşletmeden İşletmeye (B2B) Konuk desteğine](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer)bakın.</span><span class="sxs-lookup"><span data-stu-id="f1637-120">For information about future Azure AD B2B guest support in Yammer, see [Business-to-business (B2B) Guest support in Yammer Preview - Customer Terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span></span>