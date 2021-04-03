---
title: Problemas con una entidad de servicio o recurso
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
- "9004336"
- "7741"
ms.openlocfilehash: 9c37ad8e4dfecdb59a37d767f8eb4a5d99be7fa1
ms.sourcegitcommit: d13f23fb7994871d4e0e6e3e43672a101bd779e8
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/28/2021
ms.locfileid: "50716134"
---
# <a name="issues-with-a-resource-or-service-principal"></a><span data-ttu-id="7fc4d-102">Problemas con una entidad de servicio o recurso</span><span class="sxs-lookup"><span data-stu-id="7fc4d-102">Issues with a Resource or Service Principal</span></span>

1. <span data-ttu-id="7fc4d-103">Si acaba de empezar, los objetos de entidad de seguridad de aplicaciones y servicios de [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) describen el registro de aplicaciones, los objetos de aplicación y las entidades de servicio en Azure Active Directory: qué son, cómo se usan y cómo se relacionan entre sí.</span><span class="sxs-lookup"><span data-stu-id="7fc4d-103">If you are just getting started, [Application and service principal objects in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) describes application registration, application objects, and service principals in Azure Active Directory: what they are, how they are used, and how they are related to each other.</span></span> <span data-ttu-id="7fc4d-104">También se presenta un escenario de ejemplo multiinquilino para ilustrar la relación entre el objeto de aplicación de una aplicación y los objetos de entidad de servicio correspondientes.</span><span class="sxs-lookup"><span data-stu-id="7fc4d-104">A multi-tenant example scenario is also presented to illustrate the relationship between an application's application object and corresponding service principal objects.</span></span>
2. <span data-ttu-id="7fc4d-105">Para obtener más información sobre la relación entre las aplicaciones y las entidades de servicio, lea aplicaciones y objetos de entidad de seguridad de [servicio en Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).</span><span class="sxs-lookup"><span data-stu-id="7fc4d-105">You can learn more about the relationship between applications and service principals by reading [applications and service principal objects in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).</span></span>
3. <span data-ttu-id="7fc4d-106">[How to:](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) Use the portal to create an Azure AD application and service principal that can access resources shows you how to create a new Azure Active Directory (Azure AD) application and service principal that can be used with the role-based access control.</span><span class="sxs-lookup"><span data-stu-id="7fc4d-106">[How to: Use the portal to create an Azure AD application and service principal that can access resources](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) shows you how to create a new Azure Active Directory (Azure AD) application and service principal that can be used with the role-based access control.</span></span>
4. <span data-ttu-id="7fc4d-107">Con la [API de la entidad de](https://docs.microsoft.com/graph/api/resources/serviceprincipal)servicio, puede administrar mediante programación instancias de aplicaciones y controlar lo que una aplicación puede hacer dentro del espacio empresarial.</span><span class="sxs-lookup"><span data-stu-id="7fc4d-107">With the [service principal API](https://docs.microsoft.com/graph/api/resources/serviceprincipal), you can programmatically manage instances of applications and control what an application can do within your tenant.</span></span>
5. <span data-ttu-id="7fc4d-108">[Tipo de recurso servicePrincipal](https://docs.microsoft.com/graph/api/resources/serviceprincipal) enumera todas las propiedades y métodos para el tipo de recurso servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="7fc4d-108">[servicePrincipal resource type](https://docs.microsoft.com/graph/api/resources/serviceprincipal) lists all properties and methods for the servicePrincipal resource type.</span></span>
6. <span data-ttu-id="7fc4d-109">[Las diferencias de tipo de recurso entre Azure AD Graph y Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) resaltan las diferencias entre los recursos de Azure AD Graph y Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7fc4d-109">[Resource type differences between Azure AD Graph and Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) highlights differences between Azure AD Graph and Microsoft Graph resources.</span></span> <span data-ttu-id="7fc4d-110">Muestra recursos que tienen nombres diferentes o que no están disponibles; también destaca los recursos disponibles en la versión beta de Microsoft Graph, pero no en la versión v1.0.</span><span class="sxs-lookup"><span data-stu-id="7fc4d-110">It shows resources that have different names or are not available; it also highlights resources available in the beta version of Microsoft Graph but not in the v1.0 version.</span></span>

<span data-ttu-id="7fc4d-111">**Problemas con los usuarios invitados**</span><span class="sxs-lookup"><span data-stu-id="7fc4d-111">**Issues with Guest Users**</span></span>

- <span data-ttu-id="7fc4d-112">[Inicio rápido:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) agregar usuarios invitados al directorio en Azure Portal muestra cómo agregar un nuevo usuario invitado al directorio de Azure AD a través de Azure Portal, enviar una invitación y ver cómo es el proceso de canje de invitaciones del usuario invitado.</span><span class="sxs-lookup"><span data-stu-id="7fc4d-112">[Quickstart: Add guest users to your directory in the Azure portal](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) shows you how to add a new guest user to your Azure AD directory via the Azure portal, send an invitation, and see what the guest user's invitation redemption process looks like.</span></span>
- <span data-ttu-id="7fc4d-113">[Tutorial: Crear flujos de usuario en Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) muestra cómo crear algunos flujos de usuario recomendados mediante Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="7fc4d-113">[Tutorial: Create user flows in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) shows you how to create some recommended user flows by using the Azure portal.</span></span> <span data-ttu-id="7fc4d-114">Si está buscando información sobre cómo configurar un flujo de credenciales de contraseña de propietario de recursos (ROPC) en la aplicación, consulte Configure the resource owner password credentials flow in Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="7fc4d-114">If you are looking for information about how to set up a resource owner password credentials (ROPC) flow in your application, see Configure the resource owner password credentials flow in Azure AD B2C.</span></span>