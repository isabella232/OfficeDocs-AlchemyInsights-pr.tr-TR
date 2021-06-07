---
title: Office etkinleştirilemiyor
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: 81941d84127a096c3bd588dafc61b492ab6d6458
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798700"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="f3629-102">Office etkinleştirilemiyor</span><span class="sxs-lookup"><span data-stu-id="f3629-102">Unable to activate Office</span></span>

<span data-ttu-id="f3629-103">**Not:** Windows'in eski bir sürümünü kullanıyorsanız (örneğin, Windows 7), TLS 1.2'nin varsayılan olarak etkinleştirildiğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="f3629-103">**Note**: If you are using an older version of Windows (For example, Windows 7), ensure that TLS 1.2 is enabled as the default.</span></span> <span data-ttu-id="f3629-104">Daha fazla bilgi için bkz. Windows'da WinHTTP'da varsayılan güvenli protokol olarak [TLS 1.1 ve TLS 1.2'yi](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)etkinleştirmek için Windows.</span><span class="sxs-lookup"><span data-stu-id="f3629-104">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

- <span data-ttu-id="f3629-105">Abonelik durumunuzun sona erip ermediğini kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="f3629-105">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="f3629-106">Office 365 İş veya İş Ekstra gibi istemci lisanslarına izin verilen bir aboneliğe sahip olduğunuzdan ve [kullanıcıya bir lisans atanmış olduğundan](/microsoft-365/admin/manage/assign-licenses-to-users) emin olun.</span><span class="sxs-lookup"><span data-stu-id="f3629-106">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](/microsoft-365/admin/manage/assign-licenses-to-users).</span></span>
- <span data-ttu-id="f3629-107">Kullanıcının lisansın atandığı hesapla Office’te oturum açtığından emin olun. </span><span class="sxs-lookup"><span data-stu-id="f3629-107">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="f3629-108">Hizmetle ilgili bilinen sorunlar olup olmadığını görmek için [Office 365 Hizmet Durumu sayfasını](/office365/enterprise/view-service-health) gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="f3629-108">Check the [Office 365 Service Health page](/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="f3629-109">Güvenlik duvarı, virüsten koruma yazılımı ve proxy ayarlarını kontrol ederek Microsoft 365 uygulamalarının internete erişimini engellemediklerini onaylayın.</span><span class="sxs-lookup"><span data-stu-id="f3629-109">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="f3629-110">Lütfen [Office 365 URL’leri ve IP adresi aralıkları](/office365/enterprise/urls-and-ip-address-ranges "Office 365 URL’leri ve IP adresi aralıkları") makalesine bakın.</span><span class="sxs-lookup"><span data-stu-id="f3629-110">Please see [Office 365 URLs and IP address ranges](/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="f3629-111">**İpucu** Windows makinelerde sizin için birçok genel Office oturum açma sorunlarını tanılayabilir ve otomatik olarak düzeltebiliriz.</span><span class="sxs-lookup"><span data-stu-id="f3629-111">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="f3629-112">Otomatik aracımızı kullanmak için  **[Office 365 Destek ve Kurtarma Yardımcısını](https://aka.ms/SaRA-OfficeSignInScenario)** indirip çalıştırın.</span><span class="sxs-lookup"><span data-stu-id="f3629-112">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="f3629-113">Aşağıdaki sorun giderme eylemlerini uygulayın:</span><span class="sxs-lookup"><span data-stu-id="f3629-113">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="f3629-114">Bir Office uygulamasını açın ve mevcut tüm kullanıcı hesaplarında [oturumu kapatın](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071).</span><span class="sxs-lookup"><span data-stu-id="f3629-114">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="f3629-115">Office lisansını [kaldırın](/microsoft-365/admin/manage/remove-licenses-from-users) ve [yeniden atayın](/microsoft-365/admin/manage/assign-licenses-to-users), ardından etkilenen kullanıcı hesabını kullanarak [Office’te oturum açın](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="f3629-115">[Remove](/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="f3629-116">[Etkinleştirme Sorun Gidericisi](https://aka.ms/SARA-OfficeActivation-Alchemy)’ni çalıştırma</span><span class="sxs-lookup"><span data-stu-id="f3629-116">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="f3629-117">Office etkinleştirme durumunu sıfırlama</span><span class="sxs-lookup"><span data-stu-id="f3629-117">Reset Office activation state</span></span>](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Office etkinleştirme durumunu sıfırlama")
- [<span data-ttu-id="f3629-118">Office’te Çevrimiçi Onarım yapma</span><span class="sxs-lookup"><span data-stu-id="f3629-118">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="f3629-119">Ek sorun giderme çözümleri için bkz:</span><span class="sxs-lookup"><span data-stu-id="f3629-119">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="f3629-120">Office’te Lisanssız Ürün ve etkinleştirme hataları</span><span class="sxs-lookup"><span data-stu-id="f3629-120">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="f3629-121">Office’i etkinleştirdiğinizde görünen “Üzgünüz, hesabınıza bağlanılamıyor. Lütfen daha sonra yeniden deneyin” hatası</span><span class="sxs-lookup"><span data-stu-id="f3629-121">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)