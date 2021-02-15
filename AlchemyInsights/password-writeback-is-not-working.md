---
title: Parola Geri Yazma çalışmıyor
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243732"
---
# <a name="password-writeback-is-not-working"></a><span data-ttu-id="06e08-102">Parola Geri Yazma çalışmıyor</span><span class="sxs-lookup"><span data-stu-id="06e08-102">Password Writeback is not working</span></span>

<span data-ttu-id="06e08-103">**Parola geri yazma yapılandırmada sorunm var**</span><span class="sxs-lookup"><span data-stu-id="06e08-103">**I'm having problems configuring password writeback**</span></span>

- <span data-ttu-id="06e08-104">Parola geri yazma, premium bir özelliktir.</span><span class="sxs-lookup"><span data-stu-id="06e08-104">Password writeback is a premium feature.</span></span>
- <span data-ttu-id="06e08-105">Lisans gereksinimlerini anlamadan emin olun:</span><span class="sxs-lookup"><span data-stu-id="06e08-105">Make sure that you understand the licensing requirements:</span></span>
  - <span data-ttu-id="06e08-106">Kuruluşta en az bir lisans atanmış olması gerekir</span><span class="sxs-lookup"><span data-stu-id="06e08-106">You must have at least one license assigned in your organization</span></span>
  - <span data-ttu-id="06e08-107">**Yalnızca bulut kullanıcıları** - Ücretli tüm Office 365 (O365) SKU'ları veya Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="06e08-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
  - <span data-ttu-id="06e08-108">**Bulut ve/veya şirket içi** kullanıcılar - Azure AD Premium P1 veya P2, Enterprise Mobility + Security (EMS) veya Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="06e08-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="06e08-109">Lisans gereksinimleri hakkında daha fazla bilgi edinmek için, Azure AD self servis parola sıfırlama [lisans gereksinimlerine bakın](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span><span class="sxs-lookup"><span data-stu-id="06e08-109">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span></span>
- <span data-ttu-id="06e08-110">En az bir yönetici hesabınız ve uygun lisanslardan birini olan bir test kullanıcı hesabınız var.</span><span class="sxs-lookup"><span data-stu-id="06e08-110">You have at least one administrator account and one test user account with one of the appropriate license.</span></span>
- <span data-ttu-id="06e08-111">Parola geri yazmanın çalışması için Azure AD Connect'i Birincil Etki Alanı Denetleyicisi Öykünücüsü'ne bağlamanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="06e08-111">You must connect Azure AD Connect to the Primary Domain Controller Emulator for password writeback to work.</span></span> <span data-ttu-id="06e08-112">Active Directory eşitleme bağlayıcısı özelliklerine sağ tıklayarak ve  ardından dizin bölümlerini yapılandır seçeneğini seçerek, Azure AD Connect'i Birincil Etki Alanı Denetleyicisi'nden kullanmak **üzere yapılandırabilirsiniz.**</span><span class="sxs-lookup"><span data-stu-id="06e08-112">You can configure Azure AD Connect to use a Primary Domain Controller by right clicking on the **properties** of the Active Directory synchronization connector, then selecting **configure directory partitions**.</span></span> <span data-ttu-id="06e08-113">Buradan, etki alanı denetleyicisi **bağlantı ayarları bölümünü** bakın ve yalnızca tercih edilen etki alanı denetleyicilerinin kullanımı başlıklı kutuyu **işaretleyin.**</span><span class="sxs-lookup"><span data-stu-id="06e08-113">From there, look for the **domain controller connection settings** section and check the box titled **only use preferred domain controllers**.</span></span>
  > [!NOTE]
  > <span data-ttu-id="06e08-114">Tercih edilen DC bir PDC öykünücüsü değilse, Azure AD Connect parola geri yazma için PDC'ye ulaşmaya devam eder.</span><span class="sxs-lookup"><span data-stu-id="06e08-114">If the preferred DC is not a PDC emulator, Azure AD Connect will still reach out to the PDC for password writeback.</span></span>
- <span data-ttu-id="06e08-115">Parola sıfırlama kiracınız içinde yapılandırıldı ve etkinleştirildi.</span><span class="sxs-lookup"><span data-stu-id="06e08-115">Password reset has been configured and enabled in your tenant.</span></span> <span data-ttu-id="06e08-116">Daha fazla bilgi için [bkz. Kullanıcıların Azure AD parolalarını sıfırlamalarını etkinleştirme.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)</span><span class="sxs-lookup"><span data-stu-id="06e08-116">For more information, see [Enable users to reset their Azure AD passwords](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span></span>
- <span data-ttu-id="06e08-117">Parola Geri Yazma'nın etkinleştirmek için kullanılan yönetici hesabının bir bulut yöneticisi hesabı olduğundan emin olun (şirket içi AD'de değil Azure AD'de oluşturulur)</span><span class="sxs-lookup"><span data-stu-id="06e08-117">Make sure that the administrator account being used to enable Password Writeback is a cloud administrator account (created in Azure AD not on-premises AD)</span></span>
- <span data-ttu-id="06e08-118">En son hizmet paketlerinin yüklü olduğu Windows Server 2008 R2, Windows Server 2012 veya Windows Server 2012 R2 çalıştıran tek veya çok ormanlı bir AD şirket içi dağıtımınız var</span><span class="sxs-lookup"><span data-stu-id="06e08-118">You have a single or multi-forest AD on-premises deployment running Windows Server 2008 R2, Windows Server 2012, or Windows Server 2012 R2 with the latest service packs installed</span></span>
- <span data-ttu-id="06e08-119">Azure AD Connect aracı yüklü ve AD ortamınızı bulutla eşitleme için hazırladınız.</span><span class="sxs-lookup"><span data-stu-id="06e08-119">You have the Azure AD Connect tool installed and you have prepared your AD environment for synchronization to the cloud.</span></span> <span data-ttu-id="06e08-120">Parola geri yazma işlemini sınamadan önce, Azure AD Connect'te hem AD'den hem de Azure AD'den tam içeri aktarma ve tam eşitlemeyi tamamlayamadan önce emin olun.</span><span class="sxs-lookup"><span data-stu-id="06e08-120">Before testing password writeback, make sure that you first complete a full import and full sync from both AD and Azure AD in Azure AD Connect.</span></span>
- <span data-ttu-id="06e08-121">Daha fazla bilgi edinmek için [Azure AD Connect'te tam eşitleme ve tam içeri aktarma yapmayı öğrenin](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span><span class="sxs-lookup"><span data-stu-id="06e08-121">To learn more, see how to do a [full sync and full import in Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span></span>

<span data-ttu-id="06e08-122">**Parola geri yazma bağlantısıyla ilgili bir sorun var**</span><span class="sxs-lookup"><span data-stu-id="06e08-122">**I'm having a problem with password writeback connectivity**</span></span>

1. <span data-ttu-id="06e08-123">[Azure AD Connect'in](https://www.microsoft.com/download/details.aspx?id=47594) en son sürümünü indirme ve etkinleştirme</span><span class="sxs-lookup"><span data-stu-id="06e08-123">Download and enable the latest version of [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span></span>
2. <span data-ttu-id="06e08-124">Güvenlik duvarı yapılandırması: Azure AD Connect aracının (1.1.443 ve üzeri) aşağıdakilere giden **HTTPS** erişimi olması gerekir:</span><span class="sxs-lookup"><span data-stu-id="06e08-124">Firewall configuration: The Azure AD Connect tool (1.1.443 and above) will need **outbound HTTPS** access to:</span></span>
    - <span data-ttu-id="06e08-125">passwordreset.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="06e08-125">passwordreset.microsoftonline.com</span></span>
    - <span data-ttu-id="06e08-126">servicebus.windows.networks</span><span class="sxs-lookup"><span data-stu-id="06e08-126">servicebus.windows.networks</span></span>
3. <span data-ttu-id="06e08-127">Boşta bağlantının en az 2-3 dakika kalıcı olmasına izin ver</span><span class="sxs-lookup"><span data-stu-id="06e08-127">Allow idle connections to persist for at least 2-3 minutes</span></span>

<span data-ttu-id="06e08-128">**Parola geri yazma sorunlarım devam ediyor**</span><span class="sxs-lookup"><span data-stu-id="06e08-128">**I'm still having problems with password writeback**</span></span>

- <span data-ttu-id="06e08-129">Hala sorun yaşıyorsanız, Azure AD Connect aracında parola geri yazma hizmetini devre dışı bırakmayı ve yeniden etkinleştirmeyi deneyin</span><span class="sxs-lookup"><span data-stu-id="06e08-129">If you are still having difficulty, try disabling and re-enabling the password writeback service in the Azure AD Connect tool</span></span>
- <span data-ttu-id="06e08-130">Daha fazla bilgi edinmek için parola geri [yazma özelliğini devre dışı bırakmayı ve yeniden etkinleştirmeyi öğrenin](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span><span class="sxs-lookup"><span data-stu-id="06e08-130">To learn more, see how to [disable and re-enable password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span></span>
