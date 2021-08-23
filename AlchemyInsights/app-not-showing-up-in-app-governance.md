---
title: Uygulamam, Uygulama Yönetimi'ne görünmüyor
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12734"
ms.openlocfilehash: a8d176fdee073e41b61de6f53c728601da955aaa
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/16/2021
ms.locfileid: "58454987"
---
# <a name="my-app-isnt-showing-up-in-app-governance"></a>Uygulamam, Uygulama Yönetimi'ne görünmüyor

Uygulama Yönetimi'nin içinde uygulamanız göster görünmüyorsa, şunları kontrol edin:

1. Azure [AD'ye](https://aad.portal.azure.com/) gidin ve Genel Bakış sayfasının üst çubuğunda uygulama adını arayarak uygulama kimliğini bulun.

1. Access Graph Explorer'da bu sorguyu kullanarak ve ilgili uygulama kimliğiyle değiştirerek hizmet sorumlunuz içinde uygulama kimliğini <appId> arayabilirsiniz: < https://graph.microsoft.com/v1.0/servicePrincipals? $search= "appId: <appId> ">

1. Sonuç döndürülzse, bu sorguyu kullanarak uygulama içinde uygulama kimliğini arayın ve ilgili uygulama kimliğini: <appId> < https://graph.microsoft.com/v1.0/applications? $search= "appId: <appId> ">

Sorguyla ilgili sorunlar görüyorsanız, bkz. [Destek al](https://docs.microsoft.com/microsoft-365/business-video/get-help-support). 

Uygulama Yönetimi'niz hakkında daha fazla bilgi veya içgörü için [bkz. Görünürlük ve öngörüler hakkında bilgi edinin.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-overview)

Uygulamalarınızı görüntüleme hakkında daha fazla bilgi için [bkz. Uygulamalarınızı görüntüleme](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-view-apps).
