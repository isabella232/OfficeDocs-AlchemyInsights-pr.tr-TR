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
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a>Apple MDM Push Sertifikası ayarlanmadı

Apple MDM Push Sertifikası (Apple Push Bildirim Hizmeti (APNS) sertifikası olarak da bilinir) aboneliğiniz için yapılandırılmamıştır. Apple MDM Push Sertifikası yapılandırılmadan iOS ve Mac OS aygıtlarını kaydedemez ve yönetemezsiniz. Sertifikayı Intune'a ekledikten sonra, kullanıcılar iOS aygıtlarını kaydetmek için Şirket Portalı uygulamasını yükleyebilir.

1. **"Katılıyorum" seçeneğini belirleyin.** Microsoft'a Apple'a veri gönderme izni vermek.

2. Apple MDM itme sertifikası oluşturmak için gereken **CSR** Sertifikası imzalama isteğini indir'i seçin. Dosya, Apple Push Certificates Portal'dan güven ilişkisi sertifikası istemek için kullanılır.

3. Apple Push Sertifikalar Portalı'na gitmek için **MDM push Sertifikanızı Oluştur'u** seçin. Şirketinizapple Kimliği ile oturum açın ve ardından **Sertifika Oluştur'u**seçin. **Dosya'yı seçin,** sertifika imzalama isteği dosyasına göz atın ve ardından **Yükle'yi**seçin. Onay sayfasında, sertifika (.pem) dosyasını indirmek ve dosyayı yerel olarak kaydetmek için **İndir'i** seçin.
 
**Not**: Sertifika, oluşturmak için kullanılan Apple Kimliği ile ilişkilidir. En iyi uygulama olarak, yönetim görevleri için bir şirket Apple Kimliği kullanın ve posta kutusunun birden fazla kişi tarafından veya bir dağıtım listesi kullanılarak izlendiğinden emin olun. Asla kişisel Apple Kimliği kullanmayın. Apple Push Sertifikasını her 12 ayda bir yenilemek için aynı Apple Kimliğini kullanın.
 
4. Apple MDM itme sertifikanızı oluşturmak için kullanılan Apple Kimliğini girin. Sertifikayı yenilemeniz gereken zaman için bu kimliği hatırlatıcı olarak kaydedin.

5. Sertifika (.pem) dosyasına gidin, **Aç'ı**seçin ve sonra **Yükle'yi**seçin. Itme sertifikası ile Intune Apple aygıtlarını kaydedebilir ve yönetebilir.