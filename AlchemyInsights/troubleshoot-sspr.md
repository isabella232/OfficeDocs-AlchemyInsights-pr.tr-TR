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
ms.openlocfilehash: 85bfc812dcffce008a6fa5394a6069bd64c514d6
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430361"
---
# <a name="troubleshoot-sspr"></a>SSPR sorunlarını giderme

**Parola sıfırlamayı yapılandırmada sorun istemiyorum**

- Yöneticiyseniz ve kendi kendine parola sıfırlamayı nasıl etkinleştirebilirsiniz diye arıyorsanız, [öğreticide SSPR'yi](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr)etkinleştirme, parola sıfırlamayı yapılandırmaya bakın. Lisans gereksinimlerini gözden geçirmek [de istiyor olabilirsiniz.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support) Kuruluşta en az bir lisans atanmış olması gerekir.
    - **Yalnızca bulut kullanıcıları** - Ücretli tüm Office 365 (O365) SKU'ları veya Azure AD Basic
    - **Bulut ve/veya şirket içi** kullanıcılar - Azure AD Premium P1 veya P2, Enterprise Mobility + Security (EMS) veya Secure Productive Enterprise (SPE)
- Self servis parola sıfırlama hakkında daha fazla soru için SSS [bölümlerimizi inceleyin.](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)

**Hata iletisi alıyorum**

Sık karşılaşılan hataları ve bunların çözümlerini bulmak için bu makaleyi gözden geçirme: Self [servis parola sıfırlama sorunlarını giderme](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Parola sıfırlama ilkemde sorun var**

- Parola sıfırlama ilkeniz beklendiği gibilenmiyorsa veya parola sıfırlama ilkeleri hakkında sorularınız varsa şu makaleyi gözden geçirebilirsiniz: Azure Active Directory'de parola ilkeleri ve [kısıtlamaları.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support)
- Parola sıfırlama ilkeleri yöneticiler için geçerli değildir. Microsoft, herhangi bir Azure yönetici rolü için güçlü bir varsayılan iki kapılı parola sıfırlama ilkesi zorunlu tutulmaktadır. Yönetici olmadığınız bir kullanıcıyla test etmekte olduğundan emin olun. Yönetici sıfırlama ilkesi hakkında daha fazla bilgi için bu makaleye bakın: Yönetici sıfırlama [ilkesi farklılıkları.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences)

**Kullanıcılarımı parola sıfırlama için ek güvenlik bilgileri kaydetmelerini istemiyorum**

API, PowerShell veya Azure AD Connect kullanarak kullanıcılarınız için verileri (e-posta ve telefon öznitelikleri) önceden doldurmak için kullanabilirsiniz. Okumayı öğrenmek için:

- [Kullanıcıların kaydolması gerekmeden parola sıfırlamayı dağıtma](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Parola sıfırlama ile kullanılan veriler](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Kullanıcılarımı parola sıfırlama için ek güvenlik bilgilerini kaydetmelerini istiyorum**

1. Kullanıcılarınızı, güvenlik bilgilerini kendi kendine parola sıfırlama için kaydetmelerini ve bu bilgileri kullanıcılarınızı [aka.ms/ssprsetup.](https://mysignins.microsoft.com/security-info)
1. Veriler kullanıcı (kullanıcı veya yönetici tarafından) doldurulduğunda, kullanıcılarınızı kendi parolalarını [sıfırlama](https://passwordreset.microsoftonline.com/) gücü aka.ms/sspr için kullanıcınızı e-postaya yönlendirin.
1. Kullanıcılar hala sorun yaşıyorsa, bunlar büyük olasılıkla **federasyon** veya parola karması **eşitlenmiş kullanıcılardır.** Bu, Büyük olasılıkla Parola Geri Yazma hizmetiyle ilgili bir sorun olduğu anlamına gelir.