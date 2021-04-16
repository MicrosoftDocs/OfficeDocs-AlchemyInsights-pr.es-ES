---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 4a34de7fa2aaaae365cf4562d31590d4b5fb7544
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51771008"
---
# <a name="verify-your-domain"></a><span data-ttu-id="0952e-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="0952e-102">Verify your domain</span></span>

 <span data-ttu-id="0952e-103">**Es probable que el registro no se haya actualizado en Internet.**</span><span class="sxs-lookup"><span data-stu-id="0952e-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="0952e-104">Normalmente, solo nos lleva unos minutos poder ver el nuevo registro, pero de vez en cuando puede tardar unas horas.</span><span class="sxs-lookup"><span data-stu-id="0952e-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="0952e-105">Si ya ha esperado tanto tiempo, compruebe que ha copiado y pegado el valor exacto en el registro de comprobación TXT en el host DNS.</span><span class="sxs-lookup"><span data-stu-id="0952e-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="0952e-106">Uno de los problemas habituales es no incluir la parte de "MS=" del registro.</span><span class="sxs-lookup"><span data-stu-id="0952e-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="0952e-107">¡También la necesitamos!</span><span class="sxs-lookup"><span data-stu-id="0952e-107">We need that too!</span></span>

- <span data-ttu-id="0952e-108">En algunos hosts DNS, tiene que llevar a cabo un paso adicional para guardar el archivo de zona (donde se almacena el registro DNS), de modo que se actualice a través de Internet.</span><span class="sxs-lookup"><span data-stu-id="0952e-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="0952e-109">Asegúrese de que guardó los cambios para que Microsoft pueda ver y comprobar el registro.</span><span class="sxs-lookup"><span data-stu-id="0952e-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
