---
title: Öznitelik vecoping filtresiyle ilgili sorun
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482925"
---
# <a name="problem-with-attribute-and-scoping-filter"></a>Öznitelik vecoping filtresiyle ilgili sorun

**UPN değerlerinin çakışması sorunu**

The Workday to AD User Provisioning Workday to AD User Provisioning, **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique** hata iletisini gösterir. Ekleme/değiştirme için sağlanan UPN değeri orman genelinde benzersiz bir değer olduğundan işlem başarısız oldu. Hata Ayrıntıları: **CONSTRAINT_ATT_TYPE - userPrincipalName**.

Workday bağlayıcısı AD kullanıcı hesabını oluştururken ayarlamaya çalıştığı **userPrincipalName** değeri, hedef AD etki alanında zaten var. Bu, (1) kullanıcının zaten var olduğunu ve kullanıcı için eşleşen kimlik denetiminin başarısız olduğunu veya (2) UPN oluşturma kuralının çakışan bir değer üreterek bunu ima eder.

Önerilen çözüm adımları:

Kullanıcı zaten varsa ve eşleşen kimlik denetimi İşGünü hesabını Active Directory hesabına bağlayamamışsa, hem İşGünü'deki hem de AD'deki eşleşen kimlik özniteliğinin (normalde çalışanKimsi) tam eşleşmesi olup olduğunu kontrol edin.  Eşleşmesi yoksa, bu sorunun düzeltilecek bir veri sorunudur. Örneğin, İşGünü'nin ÇalışanKimlikKimlikKimsi 001052 ve AD'de 1052 ise, sağlama altyapısı iki hesabı bağamaz ve zaten var olan bir kullanıcıyı oluşturmayı dener. Bu durumda çözüm, AD'de **ÇalışanKimlik** değerini baştaki sıfırları içerecek şekilde değiştirmek ve bunu 001052 yapmaktır.
UPN oluşturan ifade benzersiz bir değer oluşturamazsa, her zaman benzersiz bir değer oluşturmak için **SelectUniqueValue** de-duplication işlevini kullanmayı göz önünde bulundurabilirsiniz.

**İşGünü'nde AD Kullanıcı Sağlama, AD kullanıcı hesabı için yönetici öznitelik değeri ayarlanmıyor**

İşGünü'nde AD Kullanıcı Hazırlama işi, AD kullanıcı **hesapları** için yönetici öznitelik değerini ayar çalışmıyor. Bu davranış görülürken iki olası senaryo vardır:

1. İşGünü'nde yönetici ilgili AD Kullanıcı hesabına çözüm bulunamaz, çünkü yönetici kapsamda değildir.
2. Birden **çok AD etki alanı** senaryosunda, İşGünü'nde yönetici kullanıcıyla aynı etki alanında değildir.

Sorunu çözmek için şu adımları deneyin:

1. Kapsam filtreleme filtrelerini tanımladıysanız, önce yöneticinin kapsam içinde olup olduğunu ve kapsam kapsamının kapsamının tamamlandığı yan tümcesini kontrol edin. Yönetici kapsam filtrelemesini karşılayana kadar filtreyi değiştirerek, yöneticinin sağlama işlemi kapsamında da yer alamayacak şekilde filtreyi değiştirmesini sağlar.
2. Birden çok AD etki alanınız varsa, bağlayıcının etki alanı yöneticisi başvurularını çözememeyle ilgili bilinen bir sınırlaması vardır.

Otomatik sağlama için iş günü yapılandırma hakkında daha fazla ayrıntı için öğreticiye bakın: Otomatik kullanıcı [sağlama için İşGünü'ne yapılandırma.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)













