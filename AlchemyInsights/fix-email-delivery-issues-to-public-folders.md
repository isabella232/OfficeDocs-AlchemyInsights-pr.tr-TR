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
ms.openlocfilehash: 74a26306766ed7952a3bbbcb06f1f0113a113024
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366484"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="c2dd5-102">Posta etkin ortak klasörler için e-posta teslim sorunlarını düzeltme</span><span class="sxs-lookup"><span data-stu-id="c2dd5-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="c2dd5-103">Dış Gönderenler posta özellikli ortak klasörlerinize ileti gönderemediğinde ve Gönderenler hatayı alıyorsa: **bulunamadı (550 5.4.1)**, ortak klasörün e-posta etki alanının yetkili etki alanı yerine iç geçiş etki alanı olarak yapılandırıldığını doğrulayın:</span><span class="sxs-lookup"><span data-stu-id="c2dd5-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="c2dd5-104">[Exchange Yönetim merkezini (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center)açın.</span><span class="sxs-lookup"><span data-stu-id="c2dd5-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="c2dd5-105">**Posta akışı** \> **kabul edilen etki alanlarına**gidin, kabul edilen etki alanını seçin ve **Düzenle**'ye tıklayın.</span><span class="sxs-lookup"><span data-stu-id="c2dd5-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="c2dd5-106">Açılan Özellikler sayfasında, etki alanı türü **yetkili**olarak ayarlanmışsa, değeri **iç geçiş** olarak değiştirin ve **Kaydet**'e tıklayın.</span><span class="sxs-lookup"><span data-stu-id="c2dd5-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="c2dd5-107">Dış Gönderenler **izniniz olmayan (550 5.7.13)** bir hatayı alıyorsa, ortak klasördeki anonim kullanıcıların izinlerini görmek Için [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) 'de aşağıdaki komutu çalıştırırsınız:</span><span class="sxs-lookup"><span data-stu-id="c2dd5-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="c2dd5-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Örneğin, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .</span><span class="sxs-lookup"><span data-stu-id="c2dd5-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="c2dd5-109">Dış kullanıcıların bu ortak klasöre e-posta göndermesine izin vermek için anonim öğeleri Access 'e anonim olarak ekleyin.</span><span class="sxs-lookup"><span data-stu-id="c2dd5-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="c2dd5-110">Örneğin, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .</span><span class="sxs-lookup"><span data-stu-id="c2dd5-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
