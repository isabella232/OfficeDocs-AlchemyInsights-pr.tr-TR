---
title: Kök site olarak modern site
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid:
- "9000153"
- "1692"
ms.openlocfilehash: 6f55f1c63551027cc5522d296cb3f3f342356d95
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36576706"
---
# <a name="modernize-your-classic-sharepoint-site"></a><span data-ttu-id="570fd-102">Klasik SharePoint sitenizi modernize edin</span><span class="sxs-lookup"><span data-stu-id="570fd-102">Modernize your classic SharePoint site</span></span>

<span data-ttu-id="570fd-103">Modern bir kullanıcı arabirimine geçiş yapmak için aşağıdakilere odaklanmanız gerekir:</span><span class="sxs-lookup"><span data-stu-id="570fd-103">To make the switch to a modern user interface, you need to focus on the following:</span></span>

- <span data-ttu-id="570fd-104">**Listelerinizi ve kitaplıklarınızı** modern kullanıcı arabirimini (modern liste ve kitaplık deneyimi olarak da adlandırılır) kullanmak üzere geçiş yapmak.</span><span class="sxs-lookup"><span data-stu-id="570fd-104">Transitioning your **lists and libraries** to use the modern user interface (also referred to as the modern list and library experience).</span></span>
- <span data-ttu-id="570fd-105">**Site sayfalarınızı** klasik wiki ve web bölümü sayfalarından modern istemci tarafındaki sayfalara dönüştürme.</span><span class="sxs-lookup"><span data-stu-id="570fd-105">Transforming your **site pages** from classic wiki and web part pages into modern client-side pages.</span></span>
- <span data-ttu-id="570fd-106">**Modern siteler** oluşturma (Ekip sitesi veya İletişim Sitesi).</span><span class="sxs-lookup"><span data-stu-id="570fd-106">Creating **modern sites** (Team site or Communication Site).</span></span>

<span data-ttu-id="570fd-107">Deneyiminizi şu şekilde modernize edin:</span><span class="sxs-lookup"><span data-stu-id="570fd-107">Modernize your experience by:</span></span>
- <span data-ttu-id="570fd-108">Özelleştirmeleri değiştirerek, kullanılan görünümlerden uyumsuz sütunları kaldırarak veya (son çare olarak) verileri modern bir kullanıcı arabirimi uyumlu liste türüne taşıyarak [listelerin ve kitaplıkların modern kullanıcı arabiriminde gösterilmesini etkinleştirmek.](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries)</span><span class="sxs-lookup"><span data-stu-id="570fd-108">[Enabling lists and libraries to show in the modern user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries) by replacing customizations, removing incompatible columns from the used views, or (as a last resort) moving data into a modern user interface-compatible list type.</span></span>
- <span data-ttu-id="570fd-109">Sitenizi, sitenize modern bir giriş sayfası sağlayan ve sitenizin örneğin bir posta kutusu veya Microsoft Planlayıcısı kullanmasını sağlayan [bir Office 365 grubuna bağlamak.](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group)</span><span class="sxs-lookup"><span data-stu-id="570fd-109">[Connecting your site to an Office 365 group](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group), which gives your site a modern home page and enables your site to use, for example, a mailbox or Microsoft Planner.</span></span> <span data-ttu-id="570fd-110">Bu, takvim ve görev listesinin modern bir sürümünü kullanmanıza olanak tanır.</span><span class="sxs-lookup"><span data-stu-id="570fd-110">This enables you to use a modern version of a calendar and task list.</span></span>
- <span data-ttu-id="570fd-111">[Modern sayfalar oluşturma,](https://support.office.com/article/create-and-use-modern-pages-on-a-sharepoint-site-b3d46deb-27a6-4b1e-87b8-df851e503dec)görüntüleri, Excel, Word ve PowerPoint belgeleri, video ve daha fazlasını kullanarak fikir paylaşmak için harika bir yoldur.</span><span class="sxs-lookup"><span data-stu-id="570fd-111">[Creating modern pages](https://support.office.com/article/create-and-use-modern-pages-on-a-sharepoint-site-b3d46deb-27a6-4b1e-87b8-df851e503dec), is a great way to share ideas using images, Excel, Word and PowerPoint documents, video, and more.</span></span>
- <span data-ttu-id="570fd-112">[Modern istemci tarafı sayfaları oluşturma](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-site-pages) ve bunları anahtar klasik wiki ve web parçası sayfalarınıza "benzer" olarak yapılandırın.</span><span class="sxs-lookup"><span data-stu-id="570fd-112">[Creating modern client-side pages](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-site-pages) and configuring these to be "similar" to your key classic wiki and web part pages.</span></span> <span data-ttu-id="570fd-113">Tüm sayfaları dönüştürmek kaynak yoğun olduğundan ve genellikle gerekli olmadığı için, sitelerinizin önemli sayfaları için programlı sayfa dönüşümü yapılmalıdır.</span><span class="sxs-lookup"><span data-stu-id="570fd-113">Programmatic page transformation should be done for the key pages of your sites, as transforming all pages is resource-intensive and often not needed.</span></span> <span data-ttu-id="570fd-114">Bu önceliklendirmeye yardımcı olmak için, SharePoint Modernizasyon tarayıcısı size geçerli wiki ve web bölümü sayfaları hakkında kullanım bilgileri verebilir.</span><span class="sxs-lookup"><span data-stu-id="570fd-114">To assist in this triage, the SharePoint Modernization scanner can give you usage information about the current wiki and web part pages.</span></span>
- <span data-ttu-id="570fd-115">[Modern siteler oluşturma.](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d)</span><span class="sxs-lookup"><span data-stu-id="570fd-115">[Creating modern sites](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span> <span data-ttu-id="570fd-116">Bir ekip sitesi mi yoksa iletişim sitesi mi oluşturmalıyım?</span><span class="sxs-lookup"><span data-stu-id="570fd-116">Should I create a team site or a communication site?</span></span>

<span data-ttu-id="570fd-117">Ek Bilgi:</span><span class="sxs-lookup"><span data-stu-id="570fd-117">Additional Info:</span></span> 
- <span data-ttu-id="570fd-118">Klasik SharePoint Sitelerinizi modern deneyime modernleştirmeye adım adım genel bir bakış için [bkz.](https://docs.microsoft.com/sharepoint/dev/transform/modernize-classic-sites)</span><span class="sxs-lookup"><span data-stu-id="570fd-118">For a step-by-step overview of modernizing your classic SharePoint Sites to the modern experience, see [Modernize your classic SharePoint Sites](https://docs.microsoft.com/sharepoint/dev/transform/modernize-classic-sites).</span></span>
- <span data-ttu-id="570fd-119">[Modern Deneyim](https://docs.microsoft.com/sharepoint/guide-to-sharepoint-modern-experience)rehberine bakın.</span><span class="sxs-lookup"><span data-stu-id="570fd-119">See a guide to [Modern Experience](https://docs.microsoft.com/sharepoint/guide-to-sharepoint-modern-experience).</span></span>
- <span data-ttu-id="570fd-120">[Bkz. SharePoint Klasik ve Modern deneyimler.](https://support.office.com/article/sharepoint-classic-and-modern-experiences-5725c103-505d-4a6e-9350-300d3ec7d73f)</span><span class="sxs-lookup"><span data-stu-id="570fd-120">See [SharePoint Classic and Modern experiences](https://support.office.com/article/sharepoint-classic-and-modern-experiences-5725c103-505d-4a6e-9350-300d3ec7d73f).</span></span> 




