---
title: Etkin posta ortak klasörlere e-posta teslim sorunları düzeltme
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1956
ms.assetid: ''
ms.openlocfilehash: 45665f900014c52e6a920325b0a3b0f6f79fb72d
ms.sourcegitcommit: d1c1d5bcb52ba9083e8dd7603feb72436c5154c8
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/17/2019
ms.locfileid: "31910637"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="6efdc-102">Etkin posta ortak klasörlere e-posta teslim sorunları düzeltme</span><span class="sxs-lookup"><span data-stu-id="6efdc-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="6efdc-103">Dış Gönderenler, etkin posta ortak klasörlere ileti gönderemiyor ve Gönderenler hata iletisini alıyorsunuz: **(550 5.4.1) bulunamadığını belirten**, ortak klasör yerine bir iç aktarma etki alanı olarak yapılandırıldığı için e-posta etki alanını doğrulayın bir yetkili etki alanı:</span><span class="sxs-lookup"><span data-stu-id="6efdc-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="6efdc-104">[Exchange Yönetim Merkezi (TZT)](https://docs.microsoft.com/Exchange/exchange-admin-center)açın.</span><span class="sxs-lookup"><span data-stu-id="6efdc-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="6efdc-105">**Posta akışı** Git \> **kabul edilen etki alanları**, kabul edilen etki alanını seçin ve sonra **Düzenle**' yi tıklatın.</span><span class="sxs-lookup"><span data-stu-id="6efdc-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="6efdc-106">Özellikler için **yetkili**etki alanı türü ayarlanmışsa, bu açılır sayfa, **iç geçiş** için değerini değiştirin ve **Kaydet**' i tıklatın.</span><span class="sxs-lookup"><span data-stu-id="6efdc-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="6efdc-107">Dış Gönderenler hata **(550 5.7.13) izniniz yoksa**alırsanız, [Çevrimiçi PowerShell Exchange](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) ortak klasör içinde anonim kullanıcılar için izinleri görmek için aşağıdaki komutu çalıştırın:</span><span class="sxs-lookup"><span data-stu-id="6efdc-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="6efdc-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Örneğin, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span><span class="sxs-lookup"><span data-stu-id="6efdc-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="6efdc-109">Bu ortak klasöre e-posta göndermek dış kullanıcılara izin vermek için CreateItems erişim hakkı kullanıcı anonim ekleyin.</span><span class="sxs-lookup"><span data-stu-id="6efdc-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="6efdc-110">Örneğin, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span><span class="sxs-lookup"><span data-stu-id="6efdc-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
