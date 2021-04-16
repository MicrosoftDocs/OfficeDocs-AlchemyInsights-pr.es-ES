---
title: Desuso de Exchange PowerShell y autenticación básica
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 01938a59b53ccf8b7867ed9c256e141205d31dff
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813489"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="48330-102">Desuso de Exchange PowerShell y autenticación básica</span><span class="sxs-lookup"><span data-stu-id="48330-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="48330-103">Para obtener la información más reciente sobre cómo conectarse a Exchange Online PowerShell sin usar autenticación básica, [vaya aquí](https://aka.ms/exops-docs).</span><span class="sxs-lookup"><span data-stu-id="48330-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/exops-docs).</span></span> <span data-ttu-id="48330-104">El módulo PowerShell V2 no usa la autenticación básica.</span><span class="sxs-lookup"><span data-stu-id="48330-104">The PowerShell V2 module does not use basic authentication.</span></span>

<span data-ttu-id="48330-105">Tenga en cuenta que la Autenticación básica debe estar habilitada en el equipo cliente.</span><span class="sxs-lookup"><span data-stu-id="48330-105">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="48330-106">El nuevo módulo PowerShell V2 usa la Autenticación moderna para establecer la conexión con el fin de habilitar todos los cmdlets V2 basados en REST.</span><span class="sxs-lookup"><span data-stu-id="48330-106">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="48330-107">Además de los cmdlets V2, también le permite tener acceso a cmdlets antiguos remotos de PowerShell (RPS), lo que requiere que se establezca una sesión de PowerShell remota.</span><span class="sxs-lookup"><span data-stu-id="48330-107">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="48330-108">Establecer una sesión de RPS en un equipo con Windows requiere que se habilite la Autenticación básica WinRM en el equipo cliente aunque el módulo use un mecanismo de autenticación moderno para autenticarse en el servicio.</span><span class="sxs-lookup"><span data-stu-id="48330-108">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="48330-109">La canalización de autenticación básica de WinRM se usa para transportar los tokens de autenticación modernos.</span><span class="sxs-lookup"><span data-stu-id="48330-109">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="48330-110">Si la Autenticación básica WinRM está deshabilitada en el equipo cliente, los nuevos cmdlets V2 seguirán funcionando (pero los cmdlets de RPS antiguos no se mostrarán).</span><span class="sxs-lookup"><span data-stu-id="48330-110">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
