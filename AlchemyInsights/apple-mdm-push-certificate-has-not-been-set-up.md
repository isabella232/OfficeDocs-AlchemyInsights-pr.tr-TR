---
title: Apple MDM Push Sertifikası ayarlanmadı
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440007"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a><span data-ttu-id="79567-102">Apple MDM Push Sertifikası ayarlanmadı</span><span class="sxs-lookup"><span data-stu-id="79567-102">Apple MDM Push Certificate has not been set up</span></span>

<span data-ttu-id="79567-103">Apple MDM Push Sertifikası (Apple Push Bildirim Hizmeti (APNS) sertifikası olarak da bilinir) aboneliğiniz için yapılandırılmamıştır.</span><span class="sxs-lookup"><span data-stu-id="79567-103">An Apple MDM Push Certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured for your subscription.</span></span> <span data-ttu-id="79567-104">Apple MDM Push Sertifikası yapılandırılmadan iOS ve Mac OS aygıtlarını kaydedemez ve yönetemezsiniz.</span><span class="sxs-lookup"><span data-stu-id="79567-104">Without an Apple MDM Push Certificate configured, you are unable to enroll and manage iOS and Mac OS devices.</span></span> <span data-ttu-id="79567-105">Sertifikayı Intune'a ekledikten sonra, kullanıcılar iOS aygıtlarını kaydetmek için Şirket Portalı uygulamasını yükleyebilir.</span><span class="sxs-lookup"><span data-stu-id="79567-105">After you add the certificate to Intune, users can install the Company Portal app to enroll their iOS devices.</span></span>

1. <span data-ttu-id="79567-106">**"Katılıyorum" seçeneğini belirleyin.**</span><span class="sxs-lookup"><span data-stu-id="79567-106">Select **"I agree."**</span></span> <span data-ttu-id="79567-107">Microsoft'a Apple'a veri gönderme izni vermek.</span><span class="sxs-lookup"><span data-stu-id="79567-107">to give Microsoft permission to send data to Apple.</span></span>

2. <span data-ttu-id="79567-108">Apple MDM itme sertifikası oluşturmak için gereken **CSR** Sertifikası imzalama isteğini indir'i seçin.</span><span class="sxs-lookup"><span data-stu-id="79567-108">Select **Download your CSR** the Intune certificate signing request required to create an Apple MDM push certificate.</span></span> <span data-ttu-id="79567-109">Dosya, Apple Push Certificates Portal'dan güven ilişkisi sertifikası istemek için kullanılır.</span><span class="sxs-lookup"><span data-stu-id="79567-109">The file is used to request a trust relationship certificate from the Apple Push Certificates Portal.</span></span>

3. <span data-ttu-id="79567-110">Apple Push Sertifikalar Portalı'na gitmek için **MDM push Sertifikanızı Oluştur'u** seçin.</span><span class="sxs-lookup"><span data-stu-id="79567-110">Select **Create your MDM push Certificate** to go to the Apple Push Certificates Portal.</span></span> <span data-ttu-id="79567-111">Şirketinizapple Kimliği ile oturum açın ve ardından **Sertifika Oluştur'u**seçin.</span><span class="sxs-lookup"><span data-stu-id="79567-111">Sign in with your company Apple ID, and then select **Create a Certificate**.</span></span> <span data-ttu-id="79567-112">**Dosya'yı seçin,** sertifika imzalama isteği dosyasına göz atın ve ardından **Yükle'yi**seçin.</span><span class="sxs-lookup"><span data-stu-id="79567-112">Select **Choose File**, browse to the certificate signing request file, and then choose **Upload**.</span></span> <span data-ttu-id="79567-113">Onay sayfasında, sertifika (.pem) dosyasını indirmek ve dosyayı yerel olarak kaydetmek için **İndir'i** seçin.</span><span class="sxs-lookup"><span data-stu-id="79567-113">On the Confirmation page, choose **Download** to download the certificate (.pem) file, and save the file locally.</span></span>
 
<span data-ttu-id="79567-114">**Not**: Sertifika, oluşturmak için kullanılan Apple Kimliği ile ilişkilidir.</span><span class="sxs-lookup"><span data-stu-id="79567-114">**Note**: The certificate is associated with the Apple ID used to create it.</span></span> <span data-ttu-id="79567-115">En iyi uygulama olarak, yönetim görevleri için bir şirket Apple Kimliği kullanın ve posta kutusunun birden fazla kişi tarafından veya bir dağıtım listesi kullanılarak izlendiğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="79567-115">As a best practice, use a company Apple ID for management tasks, and make sure the mailbox is monitored by more than one person or by using a distribution list.</span></span> <span data-ttu-id="79567-116">Asla kişisel Apple Kimliği kullanmayın.</span><span class="sxs-lookup"><span data-stu-id="79567-116">Never use a personal Apple ID.</span></span> <span data-ttu-id="79567-117">Apple Push Sertifikasını her 12 ayda bir yenilemek için aynı Apple Kimliğini kullanın.</span><span class="sxs-lookup"><span data-stu-id="79567-117">Use the same Apple ID to renew the Apple Push Certificate every 12 months.</span></span>
 
4. <span data-ttu-id="79567-118">Apple MDM itme sertifikanızı oluşturmak için kullanılan Apple Kimliğini girin.</span><span class="sxs-lookup"><span data-stu-id="79567-118">Enter the Apple ID used to create your Apple MDM push certificate.</span></span> <span data-ttu-id="79567-119">Sertifikayı yenilemeniz gereken zaman için bu kimliği hatırlatıcı olarak kaydedin.</span><span class="sxs-lookup"><span data-stu-id="79567-119">Record this ID as a reminder for when you need to renew the certificate.</span></span>

5. <span data-ttu-id="79567-120">Sertifika (.pem) dosyasına gidin, **Aç'ı**seçin ve sonra **Yükle'yi**seçin.</span><span class="sxs-lookup"><span data-stu-id="79567-120">Go to the certificate (.pem) file, choose **Open**, and then choose **Upload**.</span></span> <span data-ttu-id="79567-121">Itme sertifikası ile Intune Apple aygıtlarını kaydedebilir ve yönetebilir.</span><span class="sxs-lookup"><span data-stu-id="79567-121">With the push certificate, Intune can enroll and manage Apple devices.</span></span>