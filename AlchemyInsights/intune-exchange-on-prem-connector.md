---
title: Intune Exchange şirket içi Bağlayıcısı
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6732"
- "9003775"
ms.openlocfilehash: 8b470655efa2dfb460c29b6b840fa793ed2aa448
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/28/2020
ms.locfileid: "48808138"
---
# <a name="intune-exchange-on-premise-connector"></a><span data-ttu-id="6d21a-102">Intune Exchange şirket içi Bağlayıcısı</span><span class="sxs-lookup"><span data-stu-id="6d21a-102">Intune Exchange on-premise Connector</span></span>

<span data-ttu-id="6d21a-103">Şirket içinde barındırılan Intune ile Exchange arasındaki bağlayıcıyı ayarlama ayrıntıları için aşağıdaki belgelere bakın:</span><span class="sxs-lookup"><span data-stu-id="6d21a-103">For details of setting up the connector between Intune and Exchange which is hosted on-premises please see the following documentation:</span></span>

[<span data-ttu-id="6d21a-104">Microsoft Intune Azure 'da Intune şirket içi Exchange Connector 'ı ayarlama</span><span class="sxs-lookup"><span data-stu-id="6d21a-104">Set up the Intune on-premises Exchange connector in Microsoft Intune Azure</span></span>](https://docs.microsoft.com/intune/exchange-connector-install)

<span data-ttu-id="6d21a-105">**SSS:**</span><span class="sxs-lookup"><span data-stu-id="6d21a-105">**FAQ:**</span></span>

<span data-ttu-id="6d21a-106">S: Exchange Connector 'ı ayarlamaya çalışırken "Exchange Connector sürümü desteklenmiyor" gibi bir hata görüyorum.</span><span class="sxs-lookup"><span data-stu-id="6d21a-106">Q: I see an error such as "The Exchange Connector version is not supported" when attempting to set up the Exchange connector.</span></span> <span data-ttu-id="6d21a-107">Neden olabilir?</span><span class="sxs-lookup"><span data-stu-id="6d21a-107">What could be the cause?</span></span>

<span data-ttu-id="6d21a-108">A: kullandığınız hesap lisanslıdır; etkin bir Intune lisansı olmalıdır</span><span class="sxs-lookup"><span data-stu-id="6d21a-108">A: The account you are using is licensed appropriately - it must have an active Intune license</span></span>

<span data-ttu-id="6d21a-109">S: birden çok Exchange Bağlayıcısı olabilir mi?</span><span class="sxs-lookup"><span data-stu-id="6d21a-109">Q: Is it possible to have multiple Exchange connectors?</span></span>

<span data-ttu-id="6d21a-110">A: her bir Exchange kuruluşu için yalnızca bir Exchange Connector 'ı Intune kiracı başına ayarlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6d21a-110">A: You can only set up one Exchange connector per Intune tenant per Exchange organization.</span></span> <span data-ttu-id="6d21a-111">Bağlayıcı, çok sunuculu bir Exchange kuruluşunda yalnızca bir sunucuya yüklenebilir.</span><span class="sxs-lookup"><span data-stu-id="6d21a-111">The connector can only be installed on one server in a multi server exchange organization.</span></span>

<span data-ttu-id="6d21a-112">Ayrıca aynı kiracıda yapılandırılmış şirket içi hem de Exchange Online için yapılandırılmış bağlayıcılar olamaz.</span><span class="sxs-lookup"><span data-stu-id="6d21a-112">Also you cannot have connectors configured for both Exchange on-premise and Exchange Online configured in the same tenant.</span></span>

<span data-ttu-id="6d21a-113">S: bağlayıcının Exchange 'e bağlı olarak CAS dizisi kullanması mı istiyorsunuz?</span><span class="sxs-lookup"><span data-stu-id="6d21a-113">Q: Can the connector use a CAS array as its connection to Exchange?</span></span>

<span data-ttu-id="6d21a-114">A: CAS oluştururken desteklenen bir yapılandırma değildir.</span><span class="sxs-lookup"><span data-stu-id="6d21a-114">A: Specifying a CAS array is not a supported configuration in the connector setup.</span></span> <span data-ttu-id="6d21a-115">Yalnızca tek bir sunucu belirtilmeli ve bağlayıcı yapılandırma dosyasında bulunan ve</span><span class="sxs-lookup"><span data-stu-id="6d21a-115">Only a single server should be specified and should be hardcoded in the connector configuration file which can be found in</span></span>

<span data-ttu-id="6d21a-116">Program data\microsoft\şirket içi Exchange Connector \ OnpremiseExchangeConnectorServiceConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="6d21a-116">program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml</span></span>

<span data-ttu-id="6d21a-117">Aşağıdaki girdiyi bulun ```<ExchangeWebServiceURL />``` ve URL 'yi Exchange sunucusuyla değiştirin.</span><span class="sxs-lookup"><span data-stu-id="6d21a-117">Locate the following entry ```<ExchangeWebServiceURL />``` and replace the URL with the exchange server.</span></span>

<span data-ttu-id="6d21a-118">**Örnekteki**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span><span class="sxs-lookup"><span data-stu-id="6d21a-118">**Example:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span></span>

<span data-ttu-id="6d21a-119">Ek sorun giderme için aşağıdaki belgelere bakın: [Intune şirket Içi Exchange bağlayıcısından sorun giderme](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span><span class="sxs-lookup"><span data-stu-id="6d21a-119">Please see the following documentation for additional troubleshooting: [Troubleshoot the Intune on-premises Exchange connector](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span></span>

<span data-ttu-id="6d21a-120">**Exchange Connector için ayrıntılı günlüğü etkinleştirme**</span><span class="sxs-lookup"><span data-stu-id="6d21a-120">**Enabling Verbose logging for the Exchange connector**</span></span>

1. <span data-ttu-id="6d21a-121">Exchange Connector izleme yapılandırma dosyasını düzenleme için açın.</span><span class="sxs-lookup"><span data-stu-id="6d21a-121">Open the Exchange Connector tracing configuration file for editing.</span></span>  
<span data-ttu-id="6d21a-122">Dosya:% ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="6d21a-122">The file is located at : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span></span>  

<span data-ttu-id="6d21a-123">**Örnekteki**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span><span class="sxs-lookup"><span data-stu-id="6d21a-123">**Example:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span></span>
  
2. <span data-ttu-id="6d21a-124">Aşağıdaki anahtarla TraceSourceLine bulun: OnPremisesExchangeConnectorService</span><span class="sxs-lookup"><span data-stu-id="6d21a-124">Locate the TraceSourceLine with the following key: OnPremisesExchangeConnectorService</span></span>  
  
3. <span data-ttu-id="6d21a-125">Bilgi etkinlik Izleme (varsayılan) ile ayrıntılı ActivityTracing</span><span class="sxs-lookup"><span data-stu-id="6d21a-125">Change the SourceLevel node value from Information ActivityTracing (the default) to Verbose ActivityTracing</span></span>  

<span data-ttu-id="6d21a-126">**Örnekteki**</span><span class="sxs-lookup"><span data-stu-id="6d21a-126">**Example:**</span></span>
```
<TraceSourceLine>  
<Key xsi:type="xsd:string">OnPremisesExchangeConnectorService</Key>  
<Value xsi:type="TraceSource">  
<SourceLevel>All</SourceLevel>  
<Listeners>  
<Listener>  
<ListenerType>CircularTraceListener</ListenerType>
<SourceLevel>Verbose ActivityTracing</SourceLevel>
```
4. <span data-ttu-id="6d21a-127">Microsoft Intune Exchange hizmetini yeniden başlatma</span><span class="sxs-lookup"><span data-stu-id="6d21a-127">Restart the Microsoft Intune Exchange Service</span></span>  
5. <span data-ttu-id="6d21a-128">Sona erene kadar Intune portalında tam eşitleme ve XML 'i "bilgi ActivityTracing" olarak değiştirin ve Microsoft Intune Exchange hizmetini yeniden başlatın.</span><span class="sxs-lookup"><span data-stu-id="6d21a-128">Full sync in Intune Portal until it finishes and then change the XML back to "Information ActivityTracing" and restart the Microsoft Intune Exchange Service.</span></span>  
6. <span data-ttu-id="6d21a-129">Günlüklerin Konumu: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span><span class="sxs-lookup"><span data-stu-id="6d21a-129">Location of the logs is : `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span></span>