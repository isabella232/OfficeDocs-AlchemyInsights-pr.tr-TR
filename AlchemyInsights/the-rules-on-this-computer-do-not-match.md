---
title: 'Hata: Bu bilgisayardaki kurallar eşleşmiyor'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c0982da82826d1644f437b19e0d343a59d7ac473
ms.sourcegitcommit: e09af4285c6b81ca0a5320fdb811713ac25748c3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/09/2020
ms.locfileid: "44664266"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="ef0b8-102">Hata: Bu bilgisayardaki kurallar eşleşmiyor</span><span class="sxs-lookup"><span data-stu-id="ef0b8-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="ef0b8-103">Bu bilinen sorunun güncelleştirilmiş durumunu görmek için [bkz.](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="ef0b8-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="ef0b8-104">Outlook Ekibi, Build 12928.10000'de bir düzeltme uygulamıştır.</span><span class="sxs-lookup"><span data-stu-id="ef0b8-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="ef0b8-105">Düzeltme Insider Fast zaten ve Geç Haziran 2020'de Monthly Channel gidecek.</span><span class="sxs-lookup"><span data-stu-id="ef0b8-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="ef0b8-106">Sabit yapıya sahip olduktan sonra son bir kez "Hangi kuralları tutmak istiyorsunuz" istemini alabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="ef0b8-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="ef0b8-107">İstendiğinde Sunucu'yı seçin ve ardından Outlook'a geri gidin ve devre dışı bırakılan kuralları yeniden etkinleştirin.</span><span class="sxs-lookup"><span data-stu-id="ef0b8-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="ef0b8-108">Düzeltme kullanılabilir olana kadar lütfen aşağıdaki geçici çözümden yararlanın:</span><span class="sxs-lookup"><span data-stu-id="ef0b8-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="ef0b8-109">**Geçici Çözüm**: Son raporlarda, yalnızca Outlook masaüstünde istemci kuralları oluşturmuş olanlar için sorun oluştu.</span><span class="sxs-lookup"><span data-stu-id="ef0b8-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="ef0b8-110">Sorunla çalışmaya devam ederseniz, kuralları silmeyi düşünün ve sorun çözülene kadar yalnızca OWA'da (Outlook Web App) kurallar oluşturun ve düzenleyin.</span><span class="sxs-lookup"><span data-stu-id="ef0b8-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="ef0b8-111">Kuralları el ile silemiyorsanız, Outlook.exe /cleanrules çalıştırarak Outlook'u başlattığınızda bir Outlook komutu çalıştırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="ef0b8-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="ef0b8-112">Bu, hem istemci hem de sunucu kurallarını siler.</span><span class="sxs-lookup"><span data-stu-id="ef0b8-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="ef0b8-113">Outlook Profili'ndeki tüm hesapların tüm kurallarını siler.</span><span class="sxs-lookup"><span data-stu-id="ef0b8-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="ef0b8-114">Bu komut, Komut satırı anahtarları makalesinde daha da belgelenmiştir.</span><span class="sxs-lookup"><span data-stu-id="ef0b8-114">This command is further documented in the Command-line switches article.</span></span>

