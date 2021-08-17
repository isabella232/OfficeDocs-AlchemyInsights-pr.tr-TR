---
title: MC210173 - SharePoint Designer yeni özel Form özelliğini kullanımdan kaldırma
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
- "9002886"
- "5508"
- "9000127"
- "5507"
ms.openlocfilehash: f72d6ce6931b39d5d4a4835cee0ed2952407b13187213cca5bd483acb1e192bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54077700"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a>MC210173 - SharePoint Designer yeni özel Form özelliğini kullanımdan kaldırma

SharePoint Online içinde [özel Formlar oluşturmaya](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) yönelik SharePoint Designer işlevselliğini etkileyen sorunu tanımladık. Dikkatli inceleme sonrasında bu sorun için bilinen bir düzeltme olmadığına karar verdik ve özel Form oluşturma özelliğini 25 Nisan 2020 Cumartesi, saat 03:00 UTC itibariyle devre dışı bırakmayı seçtik. Bu değişiklik, daha önce oluşturulmuş Formları veya SharePoint Online Designer’da var olan özellikleri düzenleme yeteneğini etkilemez.

Bu değişiklik yapıldıktan sonra kullanıcılar şu hatayı almış olabilir: Yeni Formlar oluşturulurken “Liste değişiklikleri sunucuya kaydedilemedi”.

Daha önce özel Formlar oluşturmak için SharePoint Designer’dan yararlanmış olan kullanıcılar, bu amaç için alternatif olarak [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form)’i kullanabilir.

PowerApps, SharePoint Online Modern deneyiminde çalışan kullanıcıların SharePoint listeleri ve belge kitaplıkları için özel Formları doğrudan tarayıcı penceresinden oluşturmalarına ve düzenlemelerine izin veren kolay ve güçlü bir araçtır. PowerApps geleneksel kodlama bilgisi veya InfoPath gibi ek uygulama indirmeleri gerektirmez.

**Not**: SharePoint Online Klasik kullanıcılarının PowerApps’e erişmek ve onu kullanmak için geçici olarak Modern deneyimine geçiş yapmaları gerekecektir; yine de PowerApps’te oluşturulan tüm özel Formlar SharePoint Online Klasik deneyimi kullanıcıları tarafından erişilebilir.
