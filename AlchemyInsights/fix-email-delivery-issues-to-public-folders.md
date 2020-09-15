---
title: Posta etkin ortak klasörler için e-posta teslim sorunlarını düzeltme
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: da35ae4bd911fb75f23cc1c99aacbaa2392425dd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677948"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="02e25-102">Posta etkin ortak klasörler için e-posta teslim sorunlarını düzeltme</span><span class="sxs-lookup"><span data-stu-id="02e25-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="02e25-103">Dış Gönderenler posta özellikli ortak klasörlerinize ileti gönderemediğinde ve Gönderenler hatayı alıyorsa: **bulunamadı (550 5.4.1)**, ortak klasörün e-posta etki alanının yetkili etki alanı yerine iç geçiş etki alanı olarak yapılandırıldığını doğrulayın:</span><span class="sxs-lookup"><span data-stu-id="02e25-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="02e25-104">[Exchange Yönetim merkezini (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center)açın.</span><span class="sxs-lookup"><span data-stu-id="02e25-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="02e25-105">**Posta akışı** \> **kabul edilen etki alanlarına**gidin, kabul edilen etki alanını seçin ve **Düzenle**'ye tıklayın.</span><span class="sxs-lookup"><span data-stu-id="02e25-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="02e25-106">Açılan Özellikler sayfasında, etki alanı türü **yetkili**olarak ayarlanmışsa, değeri **iç geçiş** olarak değiştirin ve **Kaydet**'e tıklayın.</span><span class="sxs-lookup"><span data-stu-id="02e25-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="02e25-107">Dış Gönderenler **izniniz olmayan (550 5.7.13)** bir hatayı alıyorsa, ortak klasördeki anonim kullanıcıların izinlerini görmek Için [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) 'de aşağıdaki komutu çalıştırırsınız:</span><span class="sxs-lookup"><span data-stu-id="02e25-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="02e25-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Örneğin, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .</span><span class="sxs-lookup"><span data-stu-id="02e25-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="02e25-109">Dış kullanıcıların bu ortak klasöre e-posta göndermesine izin vermek için anonim öğeleri Access 'e anonim olarak ekleyin.</span><span class="sxs-lookup"><span data-stu-id="02e25-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="02e25-110">Örneğin, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .</span><span class="sxs-lookup"><span data-stu-id="02e25-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
