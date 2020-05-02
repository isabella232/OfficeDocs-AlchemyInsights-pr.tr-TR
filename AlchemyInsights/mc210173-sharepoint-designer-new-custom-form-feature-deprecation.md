---
title: MC210173 - SharePoint Designer yeni özel Form özelliğini kullanımdan kaldırma
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002886"
- "5508"
- "9000127"
- "5507"
ms.openlocfilehash: 185e8fc94345b240667490b1ffc63af8459d8daf
ms.sourcegitcommit: a9e6b2fcce8bd12fd079ed967f426b67d5c6d239
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/28/2020
ms.locfileid: "43928547"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a><span data-ttu-id="0daa5-102">MC210173 - SharePoint Designer yeni özel Form özelliğini kullanımdan kaldırma</span><span class="sxs-lookup"><span data-stu-id="0daa5-102">MC210173 - SharePoint Designer new custom Form feature deprecation</span></span>

<span data-ttu-id="0daa5-103">SharePoint Online içinde [özel Formlar oluşturmaya](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) yönelik SharePoint Designer işlevselliğini etkileyen sorunu tanımladık.</span><span class="sxs-lookup"><span data-stu-id="0daa5-103">We’ve identified an issue affecting SharePoint Designer functionality for [creating custom Forms](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) within SharePoint Online.</span></span> <span data-ttu-id="0daa5-104">Dikkatli inceleme sonrasında bu sorun için bilinen bir düzeltme olmadığına karar verdik ve özel Form oluşturma özelliğini 25 Nisan 2020 Cumartesi, saat 03:00 UTC itibariyle devre dışı bırakmayı seçtik.</span><span class="sxs-lookup"><span data-stu-id="0daa5-104">After careful examination, we’ve determined that there is no known fix for this issue and have elected to disable the custom Form creation feature effective as of 3:00 AM UTC on Saturday, April 25, 2020.</span></span> <span data-ttu-id="0daa5-105">Bu değişiklik, daha önce oluşturulmuş Formları veya SharePoint Online Designer’da var olan özellikleri düzenleme yeteneğini etkilemez.</span><span class="sxs-lookup"><span data-stu-id="0daa5-105">This change does not impact the ability to edit previously created Forms or other existing features in SharePoint Online Designer.</span></span>

<span data-ttu-id="0daa5-106">Bu değişiklik yapıldıktan sonra kullanıcılar şu hatayı almış olabilir: Yeni Formlar oluşturulurken “Liste değişiklikleri sunucuya kaydedilemedi”.</span><span class="sxs-lookup"><span data-stu-id="0daa5-106">After this change was made, users may have received the error: "Could not save the list changes to the server," when creating new Forms.</span></span>

<span data-ttu-id="0daa5-107">Daha önce özel Formlar oluşturmak için SharePoint Designer’dan yararlanmış olan kullanıcılar, bu amaç için alternatif olarak [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form)’i kullanabilir.</span><span class="sxs-lookup"><span data-stu-id="0daa5-107">Users who have previously leveraged SharePoint Designer to create custom Forms are instead able to utilize [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) for this purpose.</span></span>

<span data-ttu-id="0daa5-108">PowerApps, SharePoint Online Modern deneyiminde çalışan kullanıcıların SharePoint listeleri ve belge kitaplıkları için özel Formları doğrudan tarayıcı penceresinden oluşturmalarına ve düzenlemelerine izin veren kolay ve güçlü bir araçtır.</span><span class="sxs-lookup"><span data-stu-id="0daa5-108">PowerApps is an easy and powerful tool that allows users operating in the SharePoint Online Modern experience to create and edit custom Forms for SharePoint lists and document libraries right from a browser window.</span></span> <span data-ttu-id="0daa5-109">PowerApps geleneksel kodlama bilgisi veya InfoPath gibi ek uygulama indirmeleri gerektirmez.</span><span class="sxs-lookup"><span data-stu-id="0daa5-109">PowerApps does not require traditional coding knowledge or any additional app downloads such as InfoPath.</span></span>

<span data-ttu-id="0daa5-110">**Not**: SharePoint Online Klasik kullanıcılarının PowerApps’e erişmek ve onu kullanmak için geçici olarak Modern deneyimine geçiş yapmaları gerekecektir; yine de PowerApps’te oluşturulan tüm özel Formlar SharePoint Online Klasik deneyimi kullanıcıları tarafından erişilebilir.</span><span class="sxs-lookup"><span data-stu-id="0daa5-110">**Note**: SharePoint Online Classic users will need to temporarily switch to the Modern experience to access and utilize PowerApps; though, all custom Forms created in PowerApps are accessible by SharePoint Online Classic experience users.</span></span>
