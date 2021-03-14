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
# <a name="unable-to-activate-office"></a>Office etkinleştirilemiyor

- Abonelik durumunuzun sona erip ermediğini kontrol edin.
- Office 365 İş veya İş Ekstra gibi istemci lisanslarına izin verilen bir aboneliğe sahip olduğunuzdan ve [kullanıcıya bir lisans atanmış olduğundan](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide) emin olun.
- Kullanıcının lisansın atandığı hesapla Office’te oturum açtığından emin olun. 
- Hizmetle ilgili bilinen sorunlar olup olmadığını görmek için [Office 365 Hizmet Durumu sayfasını](https://docs.microsoft.com/office365/enterprise/view-service-health) gözden geçirin.
- Güvenlik duvarı, virüsten koruma yazılımı ve proxy ayarlarını kontrol ederek Microsoft 365 uygulamalarının internete erişimini engellemediklerini onaylayın. Lütfen [Office 365 URL’leri ve IP adresi aralıkları](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365 URL’leri ve IP adresi aralıkları") makalesine bakın.

**İpucu** Windows makinelerde sizin için birçok genel Office oturum açma sorunlarını tanılayabilir ve otomatik olarak düzeltebiliriz. Otomatik aracımızı kullanmak için  **[Office 365 Destek ve Kurtarma Yardımcısını](https://aka.ms/SaRA-OfficeSignInScenario)** indirip çalıştırın.

Aşağıdaki sorun giderme eylemlerini uygulayın:

- Bir Office uygulamasını açın ve mevcut tüm kullanıcı hesaplarında [oturumu kapatın](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071). Office lisansını [kaldırın](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) ve [yeniden atayın](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users), ardından etkilenen kullanıcı hesabını kullanarak [Office’te oturum açın](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9).
- [Etkinleştirme Sorun Gidericisi](https://aka.ms/SARA-OfficeActivation-Alchemy)’ni çalıştırma
- [Office etkinleştirme durumunu sıfırlama](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Office etkinleştirme durumunu sıfırlama")
- [Office’te Çevrimiçi Onarım yapma](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

Ek sorun giderme çözümleri için bkz:  

- [Office’te Lisanssız Ürün ve etkinleştirme hataları](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [Office’i etkinleştirdiğinizde görünen “Üzgünüz, hesabınıza bağlanılamıyor. Lütfen daha sonra yeniden deneyin” hatası](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)