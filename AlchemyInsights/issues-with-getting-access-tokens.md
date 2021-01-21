---
title: Access belirteçlerini alma sorunları
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7776"
- "9004351"
ms.openlocfilehash: e2d15603835d3fb43df1b6b5dadec64af00290ff
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/20/2021
ms.locfileid: "49917209"
---
# <a name="issues-with-getting-access-tokens"></a><span data-ttu-id="2d978-102">Access belirteçlerini alma sorunları</span><span class="sxs-lookup"><span data-stu-id="2d978-102">Issues with getting access tokens</span></span>

<span data-ttu-id="2d978-103">Bu konu başlığı altında, kaynağa erişmek için erişim belirteçlerini alma hataları ele verilmektedir.</span><span class="sxs-lookup"><span data-stu-id="2d978-103">This topic deals with failures to acquire access tokens to access a resource.</span></span>

<span data-ttu-id="2d978-104">**Başlarken sorun yaşıyorum**</span><span class="sxs-lookup"><span data-stu-id="2d978-104">**I'm having trouble getting started**</span></span>

<span data-ttu-id="2d978-105">Başlarken karşılaştığınız sorunları gidermek için aşağıdaki makalelere bakın:</span><span class="sxs-lookup"><span data-stu-id="2d978-105">To troubleshoot issues you encounter when trying to get started, see the following articles:</span></span>

- [<span data-ttu-id="2d978-106">Başlamak için kod örneği bulamıyorum</span><span class="sxs-lookup"><span data-stu-id="2d978-106">I can't find a code sample to get started</span></span>](https://docs.microsoft.com/azure/active-directory/develop/sample-v2-code) 
- [<span data-ttu-id="2d978-107">.NET 'ta belirteç almada yardım gerekiyor</span><span class="sxs-lookup"><span data-stu-id="2d978-107">I need help getting a token in .NET</span></span>](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios)

<span data-ttu-id="2d978-108">**Belirteçlerin nasıl isteneceğini bilmiyorum**</span><span class="sxs-lookup"><span data-stu-id="2d978-108">**I don't know how to request and use tokens**</span></span>

<span data-ttu-id="2d978-109">Belirteçleri isteme ve kullanma konusunda rehberlik için aşağıdaki makalelere bakın:</span><span class="sxs-lookup"><span data-stu-id="2d978-109">For guidance on how to request and use tokens, see the following articles:</span></span>

- [<span data-ttu-id="2d978-110">Yetkilendirme kodu istemeyi bilmiyorum</span><span class="sxs-lookup"><span data-stu-id="2d978-110">I don’t know how to request an authorization code</span></span>](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#request-an-authorization-code) 
- [<span data-ttu-id="2d978-111">Erişim belirteci istemeyi bilmiyorum</span><span class="sxs-lookup"><span data-stu-id="2d978-111">I don’t know how to request an access token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#use-the-authorization-code-to-request-an-access-token) 
- [<span data-ttu-id="2d978-112">Bir kaynağa erişmek için erişim belirtecinin nasıl kullanılacağını bilmiyorum</span><span class="sxs-lookup"><span data-stu-id="2d978-112">I don’t know how to use an access token to access a resource</span></span>](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#use-the-access-token-to-access-the-resource) 
- [<span data-ttu-id="2d978-113">Erişim belirtecini nasıl yenileyeceğdum</span><span class="sxs-lookup"><span data-stu-id="2d978-113">I don’t know how to refresh an access token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#refreshing-the-access-tokens)

<span data-ttu-id="2d978-114">**Belirteç isterken bir hata aldım**</span><span class="sxs-lookup"><span data-stu-id="2d978-114">**I got an error while requesting a token**</span></span>

<span data-ttu-id="2d978-115">Belirteç isterken karşılaştığınız hataların sorunlarını gidermek için aşağıdaki makalelere bakın:</span><span class="sxs-lookup"><span data-stu-id="2d978-115">To troubleshoot errors you have encountered while requesting for a token, see the following articles:</span></span>

- [<span data-ttu-id="2d978-116">Belirteç isterken bir hizmet hatası aldım</span><span class="sxs-lookup"><span data-stu-id="2d978-116">I received a service error when requesting a token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) 
- [<span data-ttu-id="2d978-117">Daha önce çalışan bir uygulamaya yeni bir hata alıyorum</span><span class="sxs-lookup"><span data-stu-id="2d978-117">I'm getting a new error to a previously working app</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reference-breaking-changes)

<span data-ttu-id="2d978-118">**ADSTS hata kodları hakkında nasıl daha fazla bilgi edinebilirim?**</span><span class="sxs-lookup"><span data-stu-id="2d978-118">**How do I get more information about AADSTS error codes?**</span></span>

<span data-ttu-id="2d978-119">Daha fazla bilgi için [kimlik doğrulama ve yetkilendirme hata kodları](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes)bölümüne bakın.</span><span class="sxs-lookup"><span data-stu-id="2d978-119">For more information, see [Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes).</span></span>





