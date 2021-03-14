---
title: Office etkinleştirilemiyor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: 3a42c221047e7be6a173694cd45136baa6bff39a
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704950"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="2adf1-102">Office etkinleştirilemiyor</span><span class="sxs-lookup"><span data-stu-id="2adf1-102">Unable to activate Office</span></span>

- <span data-ttu-id="2adf1-103">Abonelik durumunuzun sona erip ermediğini kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="2adf1-103">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="2adf1-104">Office 365 İş veya İş Ekstra gibi istemci lisanslarına izin verilen bir aboneliğe sahip olduğunuzdan ve [kullanıcıya bir lisans atanmış olduğundan](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide) emin olun.</span><span class="sxs-lookup"><span data-stu-id="2adf1-104">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide).</span></span>
- <span data-ttu-id="2adf1-105">Kullanıcının lisansın atandığı hesapla Office’te oturum açtığından emin olun. </span><span class="sxs-lookup"><span data-stu-id="2adf1-105">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="2adf1-106">Hizmetle ilgili bilinen sorunlar olup olmadığını görmek için [Office 365 Hizmet Durumu sayfasını](https://docs.microsoft.com/office365/enterprise/view-service-health) gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="2adf1-106">Check the [Office 365 Service Health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="2adf1-107">Güvenlik duvarı, virüsten koruma yazılımı ve proxy ayarlarını kontrol ederek Microsoft 365 uygulamalarının internete erişimini engellemediklerini onaylayın.</span><span class="sxs-lookup"><span data-stu-id="2adf1-107">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="2adf1-108">Lütfen [Office 365 URL’leri ve IP adresi aralıkları](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365 URL’leri ve IP adresi aralıkları") makalesine bakın.</span><span class="sxs-lookup"><span data-stu-id="2adf1-108">Please see [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="2adf1-109">**İpucu** Windows makinelerde sizin için birçok genel Office oturum açma sorunlarını tanılayabilir ve otomatik olarak düzeltebiliriz.</span><span class="sxs-lookup"><span data-stu-id="2adf1-109">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="2adf1-110">Otomatik aracımızı kullanmak için  **[Office 365 Destek ve Kurtarma Yardımcısını](https://aka.ms/SaRA-OfficeSignInScenario)** indirip çalıştırın.</span><span class="sxs-lookup"><span data-stu-id="2adf1-110">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="2adf1-111">Aşağıdaki sorun giderme eylemlerini uygulayın:</span><span class="sxs-lookup"><span data-stu-id="2adf1-111">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="2adf1-112">Bir Office uygulamasını açın ve mevcut tüm kullanıcı hesaplarında [oturumu kapatın](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071).</span><span class="sxs-lookup"><span data-stu-id="2adf1-112">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="2adf1-113">Office lisansını [kaldırın](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) ve [yeniden atayın](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users), ardından etkilenen kullanıcı hesabını kullanarak [Office’te oturum açın](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="2adf1-113">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="2adf1-114">[Etkinleştirme Sorun Gidericisi](https://aka.ms/SARA-OfficeActivation-Alchemy)’ni çalıştırma</span><span class="sxs-lookup"><span data-stu-id="2adf1-114">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="2adf1-115">Office etkinleştirme durumunu sıfırlama</span><span class="sxs-lookup"><span data-stu-id="2adf1-115">Reset Office activation state</span></span>](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Office etkinleştirme durumunu sıfırlama")
- [<span data-ttu-id="2adf1-116">Office’te Çevrimiçi Onarım yapma</span><span class="sxs-lookup"><span data-stu-id="2adf1-116">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="2adf1-117">Ek sorun giderme çözümleri için bkz:</span><span class="sxs-lookup"><span data-stu-id="2adf1-117">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="2adf1-118">Office’te Lisanssız Ürün ve etkinleştirme hataları</span><span class="sxs-lookup"><span data-stu-id="2adf1-118">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="2adf1-119">Office’i etkinleştirdiğinizde görünen “Üzgünüz, hesabınıza bağlanılamıyor. Lütfen daha sonra yeniden deneyin” hatası</span><span class="sxs-lookup"><span data-stu-id="2adf1-119">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)