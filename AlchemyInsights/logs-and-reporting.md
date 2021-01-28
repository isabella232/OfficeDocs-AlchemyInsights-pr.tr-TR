---
title: Günlükler ve Raporlama
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004331"
- "7727"
ms.openlocfilehash: 7349efb02f8d6ac5d73f6d6cd06eef6308ffe9be
ms.sourcegitcommit: 117c64e1fbcb5eec04f94eadad71423b974e7b14
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50036100"
---
# <a name="logs-and-reporting"></a><span data-ttu-id="332e4-102">Günlükler ve Raporlama</span><span class="sxs-lookup"><span data-stu-id="332e4-102">Logs and Reporting</span></span>

<span data-ttu-id="332e4-103">[Azure Active Directory raporlama SSS,](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) Azure Active Directory (Azure AD) raporlaması hakkında sık sorulan soruların yanıtlarıdır.</span><span class="sxs-lookup"><span data-stu-id="332e4-103">[Azure Active Directory reporting FAQ](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) answers frequently asked questions about Azure Active Directory (Azure AD) reporting.</span></span> <span data-ttu-id="332e4-104">Daha fazla bilgi için [Azure Active Directory raporlarına bakın.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports)</span><span class="sxs-lookup"><span data-stu-id="332e4-104">For more information, see [Azure Active Directory reporting](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports).</span></span>

<span data-ttu-id="332e4-105">**Denetim ile ilgili sorunları giderme**</span><span class="sxs-lookup"><span data-stu-id="332e4-105">**Troubleshooting issues with Audit**</span></span>

1. <span data-ttu-id="332e4-106">Bazı denetim etkinliklerini görmeyle ilgili sorunlar görüyorsanız ve eksik Etkinlik bu listede yer alıyorsa [lütfen](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities)bir destek bileti dosyalayın.</span><span class="sxs-lookup"><span data-stu-id="332e4-106">If you are having issues seeing some audit activities and the missing Activity is in this [list](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities), please file a support ticket.</span></span>
2. <span data-ttu-id="332e4-107">Kiracınız içinde denetim günlüklerini görmeyle ilgili sorunlar varsa lütfen bir destek bileti dosyalayın.</span><span class="sxs-lookup"><span data-stu-id="332e4-107">If you are having issues seeing any Audit logs in your tenant, please file a support ticket.</span></span>
3. <span data-ttu-id="332e4-108">Denetim etkinlikleriniz Azure Portal'da hemen görünmüyorsa, gecikme [](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) bilgilerimize göz atarak gecikme süresi belgelenmiş gecikme süresini aşarsa destek bileti dosyası ekleyin.</span><span class="sxs-lookup"><span data-stu-id="332e4-108">If your audit activities are not showing up immediately in the Azure Portal, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. [<span data-ttu-id="332e4-109">Azure AD Etkinlik Günlüklerini Bekletme</span><span class="sxs-lookup"><span data-stu-id="332e4-109">Azure AD Activity Logs Retention</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention)
5. <span data-ttu-id="332e4-110">Seçtiğiniz tarih aralığı için tüm denetimi görmüyorsanız, Azure portaldan en çok 250.000 satır (en son oturum açma bilgilerine göre sıralanmış) indirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="332e4-110">If you don't see all the audit for the date range you selected, you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="332e4-111">Daha fazla bilgi için Denetim [etkinlikleri indirmeye bakın.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report)</span><span class="sxs-lookup"><span data-stu-id="332e4-111">For more information, see [Audit activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report).</span></span>

<span data-ttu-id="332e4-112">**Oturum açma ile ilgili sorunları giderme**</span><span class="sxs-lookup"><span data-stu-id="332e4-112">**Troubleshooting issues with Sign-ins**</span></span>

1. <span data-ttu-id="332e4-113">Yalnızca kiracınız için Azure AD Premium (P1 veya P2) lisansınız varsa, son 30 günlük verileri görüntüebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="332e4-113">You can only see the last 30 days of data if you have an Azure AD Premium (P1 or P2) license for your tenant.</span></span>
2. <span data-ttu-id="332e4-114">Oturum açma yalnızca Azure AD Premium kiracılarında kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="332e4-114">Sign-ins are available only for Azure AD Premium tenants.</span></span> <span data-ttu-id="332e4-115">Ücretsiz veya Temel lisanslı kiracılar için kullanılamaz.</span><span class="sxs-lookup"><span data-stu-id="332e4-115">It's not available for Free or Basic licensed tenants.</span></span>
3. <span data-ttu-id="332e4-116">Kiracınız Premium P1 lisansına sahipse ve oturum açmaları görmüyorsanız, [](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) gecikme bilgilerimize göz atarak gecikme süresi belgelenmiş gecikme süresini aşıyorsa destek bileti dosyası ekleyin.</span><span class="sxs-lookup"><span data-stu-id="332e4-116">If your tenant has a Premium P1 license and you can't see the sign-ins, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. <span data-ttu-id="332e4-117">Seçtiğiniz tarih aralığı için tüm oturum açmaları görmüyorsanız, Azure portaldan en çok 250.000 satır (en son oturum açma bilgilerine göre sıralanmış) indirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="332e4-117">If you don't see all the sign-ins for the date range you selected, note that you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="332e4-118">Daha fazla bilgi için [bkz. Oturum açma etkinlikleri indirme.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities)</span><span class="sxs-lookup"><span data-stu-id="332e4-118">For more information, see [Sign-ins activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities).</span></span>

<span data-ttu-id="332e4-119">**Güvenlik Raporları sorunlarını giderme (Risk altında Bayrakla İşaretlenen Kullanıcılar, Riskli Oturum Açma)**</span><span class="sxs-lookup"><span data-stu-id="332e4-119">**Troubleshoot Security Reports (Users Flagged at Risk, Risky Sign-In)**</span></span>

1. [<span data-ttu-id="332e4-120">Risk güvenliği raporu için bayrakla işaretlenmiş kullanıcılar</span><span class="sxs-lookup"><span data-stu-id="332e4-120">Users flagged for risk security report</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-user-at-risk)
2. [<span data-ttu-id="332e4-121">Azure Active Directory portalında riskli oturum açma raporu</span><span class="sxs-lookup"><span data-stu-id="332e4-121">Risky sign-ins report in the Azure Active Directory portal</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risky-sign-ins)
3. [<span data-ttu-id="332e4-122">Azure Active Directory risk olayları</span><span class="sxs-lookup"><span data-stu-id="332e4-122">Azure Active Directory risk events</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risk-events)
