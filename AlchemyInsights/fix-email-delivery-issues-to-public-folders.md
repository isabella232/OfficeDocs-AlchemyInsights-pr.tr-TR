---
title: E-posta yla etkin ortak klasörlere e-posta teslim sorunlarını düzeltme
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e261fe60843555fa45927b0a6b36e1ccf79fb028
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716372"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="df31d-102">E-posta yla etkin ortak klasörlere e-posta teslim sorunlarını düzeltme</span><span class="sxs-lookup"><span data-stu-id="df31d-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="df31d-103">Dış gönderenler posta yla etkinleştirilmiş ortak klasörlerinize ileti gönderemiyorsa ve gönderenler hatayı alıyorsa: **bulunamadı (550 5.4.1)** ortak klasörün e-posta etki alanının yetkili bir etki alanı yerine dahili röle etki alanı olarak yapılandırıldığı doğrula:</span><span class="sxs-lookup"><span data-stu-id="df31d-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="df31d-104">Exchange [yönetici merkezini (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center)açın.</span><span class="sxs-lookup"><span data-stu-id="df31d-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="df31d-105">Posta **akışına** \> git **Kabul edilen etki alanları,** kabul edilen etki alanını seçin ve sonra **Edit'i**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="df31d-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="df31d-106">Açılan özellikler sayfasında, etki alanı türü **Yetkili**olarak ayarlanmışsa, değeri **İç röle** olarak değiştirin ve ardından **Kaydet'i**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="df31d-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="df31d-107">Harici **gönderenler izniniz yoksa hata alırsanız (550 5.7.13)** ortak klasörde anonim kullanıcıların izinlerini görmek için [Exchange Online PowerShell'de](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) aşağıdaki komutu çalıştırın:</span><span class="sxs-lookup"><span data-stu-id="df31d-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="df31d-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Örneğin, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span><span class="sxs-lookup"><span data-stu-id="df31d-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="df31d-109">Harici kullanıcıların bu ortak klasöre e-posta göndermesine izin vermek için CreateItems erişim hakkını Anonim kullanıcıya ekleyin.</span><span class="sxs-lookup"><span data-stu-id="df31d-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="df31d-110">Örneğin, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span><span class="sxs-lookup"><span data-stu-id="df31d-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
