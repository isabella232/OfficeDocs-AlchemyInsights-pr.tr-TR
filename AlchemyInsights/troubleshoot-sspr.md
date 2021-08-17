---
title: SSPR sorunlarını giderme
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 9d8184efdc60befd359059c62ea3eb1a14ad7d2a20dade921d4a71e424f52033
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038978"
---
# <a name="troubleshoot-sspr"></a>SSPR sorunlarını giderme

**Parola sıfırlamayı yapılandırmada sorunlanıyorum**

- Yöneticiyseniz ve kendi kendine parola sıfırlamayı etkinleştirmeyi öğrenmek arıyorsanız, Öğretici, [SSPR'yi](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr)etkinleştirme, kurum için parola sıfırlamayı yapılandırma öğreticisi'ne bakın. Lisans gereksinimlerini gözden geçirmek [de istemeniz gerekir.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support) Kuruluşta en az bir lisans atanmış olması gerekir.
    - **Yalnızca bulut kullanıcıları** - Tüm Office 365 (O365) ücretli SKU veya Azure AD Basic
    - **Bulut ve/veya şirket içi kullanıcılar** - Azure AD Premium P1 veya P2, Enterprise Mobility + Security (EMS) veya Secure Productive Enterprise (SPE)
- Self servis parola sıfırlama hakkında daha fazla soru için SSS bölümünü [inceleyin.](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)

**Bir hata iletisi alıyorum**

Sık karşılaşılan hataları ve çözümlerini bulmak için bu makaleyi gözden geçirme: [Self servis parola sıfırlama sorunlarını giderme](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Parola sıfırlama ilkemde sorun var**

- Parola sıfırlama ilkeniz beklendiği gibilenmiyorsa veya parola sıfırlama ilkeleri hakkında sorularınız varsa, şu makaleyi gözden geçirebilirsiniz: parola ilkeleri ve [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).
- Parola sıfırlama ilkeleri yöneticiler için geçerli değildir. Microsoft, herhangi bir Azure yönetici rolü için güçlü bir varsayılan iki sınırlı parola sıfırlama ilkesi zorlar. Yönetici olmadığınız bir kullanıcıyla test olduğundan emin olun. Yönetici sıfırlama ilkesi hakkında daha fazla bilgi için şu makaleye bakın: [Yönetici sıfırlama ilkesi farklılıkları.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences)

**Kullanıcılarımın parola sıfırlama için ek güvenlik bilgilerini kaydetmelerini istemiyorum**

API, PowerShell veya Azure AD kimlik bilgileri kullanarak kullanıcılarınız için verileri (e-posta ve telefon öznitelikleri) önceden Bağlan. Okumayı öğrenmek için:

- [Kullanıcıların kaydolması gerekmeden parola sıfırlamayı dağıtma](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Parola sıfırlama ile kullanılan veriler](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Kullanıcılarımın parola sıfırlama için ek güvenlik bilgilerini kaydetmelerini istiyorum**

1. Kullanıcılarınızı güvenlik bilgilerini self servis parola sıfırlama için kaydetmelerini ve bu bilgileri kullanıcılarınızı [aka.ms/ssprsetup.](https://mysignins.microsoft.com/security-info)
1. Veriler kullanıcı (kullanıcı veya yönetici tarafından) doldurulduğunda, kullanıcılarınızı [](https://passwordreset.microsoftonline.com/) parolalarını sıfırlamaya aka.ms/sspr için kullanıcınızı bu verilere yönlendirin.
1. Kullanıcılar hala sorun yaşıyorsa, bunlar büyük olasılıkla federasyon veya parola **karması** **eşitlenmiş kullanıcılardır.** Bu, parola geri yazma hizmette büyük olasılıkla bir sorun olduğu anlamına gelir.