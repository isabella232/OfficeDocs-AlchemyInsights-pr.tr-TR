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
ms.openlocfilehash: 9a33b7880aff6016ef6df88960d6f59ac9dd50382c7e99d72ca36bc3c9f344ea
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53928389"
---
# <a name="unable-to-activate-office"></a>Office etkinleştirilemiyor

**Not:** Windows'in eski bir sürümünü kullanıyorsanız (örneğin, Windows 7), TLS 1.2'nin varsayılan olarak etkinleştirildiğinden emin olun. Daha fazla bilgi için bkz. Windows'da WinHTTP'da varsayılan güvenli protokol olarak [TLS 1.1 ve TLS 1.2'yi](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)etkinleştirmek için Windows.

- Abonelik durumunuzun sona erip ermediğini kontrol edin.
- Office 365 İş veya İş Ekstra gibi istemci lisanslarına izin verilen bir aboneliğe sahip olduğunuzdan ve [kullanıcıya bir lisans atanmış olduğundan](/microsoft-365/admin/manage/assign-licenses-to-users) emin olun.
- Kullanıcının lisansın atandığı hesapla Office’te oturum açtığından emin olun. 
- Hizmetle ilgili bilinen sorunlar olup olmadığını görmek için [Office 365 Hizmet Durumu sayfasını](/office365/enterprise/view-service-health) gözden geçirin.
- Güvenlik duvarı, virüsten koruma yazılımı ve proxy ayarlarını kontrol ederek Microsoft 365 uygulamalarının internete erişimini engellemediklerini onaylayın. Lütfen [Office 365 URL’leri ve IP adresi aralıkları](/office365/enterprise/urls-and-ip-address-ranges "Office 365 URL’leri ve IP adresi aralıkları") makalesine bakın.

**İpucu** Windows makinelerde sizin için birçok genel Office oturum açma sorunlarını tanılayabilir ve otomatik olarak düzeltebiliriz. Otomatik aracımızı kullanmak için  **[Office 365 Destek ve Kurtarma Yardımcısını](https://aka.ms/SaRA-OfficeSignInScenario)** indirip çalıştırın.

Aşağıdaki sorun giderme eylemlerini uygulayın:

- Bir Office uygulamasını açın ve mevcut tüm kullanıcı hesaplarında [oturumu kapatın](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071). Office lisansını [kaldırın](/microsoft-365/admin/manage/remove-licenses-from-users) ve [yeniden atayın](/microsoft-365/admin/manage/assign-licenses-to-users), ardından etkilenen kullanıcı hesabını kullanarak [Office’te oturum açın](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9).
- [Etkinleştirme Sorun Gidericisi](https://aka.ms/SARA-OfficeActivation-Alchemy)’ni çalıştırma
- [Office etkinleştirme durumunu sıfırlama](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Office etkinleştirme durumunu sıfırlama")
- [Office’te Çevrimiçi Onarım yapma](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

Ek sorun giderme çözümleri için bkz:  

- [Office’te Lisanssız Ürün ve etkinleştirme hataları](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [Office’i etkinleştirdiğinizde görünen “Üzgünüz, hesabınıza bağlanılamıyor. Lütfen daha sonra yeniden deneyin” hatası](/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)