---
title: Permisos de API y proceso de consentimiento
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "9200"
ms.openlocfilehash: 23fed786e7b33adf0b6c76fc71a7e69f2cfcceb7
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/26/2021
ms.locfileid: "51379895"
---
# <a name="api-permissions-and-consent-process"></a><span data-ttu-id="47b92-102">Permisos de API y proceso de consentimiento</span><span class="sxs-lookup"><span data-stu-id="47b92-102">API Permissions and Consent Process</span></span>

<span data-ttu-id="47b92-103">Para que su aplicación pueda obtener acceso a los datos de Microsoft Graph, el usuario o el administrador deben concederle los permisos correctos a través de un proceso de consentimiento.</span><span class="sxs-lookup"><span data-stu-id="47b92-103">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="47b92-104">[La referencia de permisos de Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) enumera los permisos asociados con cada conjunto principal de API de Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="47b92-104">[Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="47b92-105">También se proporciona información sobre cómo usar los permisos.</span><span class="sxs-lookup"><span data-stu-id="47b92-105">It also provides guidance about how to use the permissions.</span></span>

<span data-ttu-id="47b92-106">**Configurar o actualizar la entidad de servicio**</span><span class="sxs-lookup"><span data-stu-id="47b92-106">**Set up or update service principal**</span></span>

- <span data-ttu-id="47b92-107">[Crear serviceprincipal:](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) en este artículo se muestra cómo crear un nuevo objeto servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="47b92-107">[Create serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) - This article shows you how to create a new servicePrincipal object.</span></span>
- <span data-ttu-id="47b92-108">Crear una entidad de servicio de & de azure AD en el [portal:](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) en este artículo se muestra cómo crear una nueva aplicación de Azure Active Directory (Azure AD) y una entidad de servicio que se pueda usar con el control de acceso basado en roles.</span><span class="sxs-lookup"><span data-stu-id="47b92-108">[Create an Azure AD app & service principal in the portal](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) - This article shows you how to create a new Azure Active Directory (Azure AD) application and service principal that can be used with the role-based access control.</span></span>
- <span data-ttu-id="47b92-109">Aplicaciones & de servicio en [Azure AD:](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) en este artículo se describen el registro de aplicaciones, los objetos de aplicación y las entidades de servicio en Azure Active Directory: qué son, cómo se usan y cómo se relacionan entre sí.</span><span class="sxs-lookup"><span data-stu-id="47b92-109">[Apps & service principals in Azure AD](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) - This article describes application registration, application objects, and service principals in Azure Active Directory: what they are, how they are used, and how they are related to each other.</span></span>

<span data-ttu-id="47b92-110">**Agregar o actualizar el registro de la aplicación y proporcionar el consentimiento del administrador**</span><span class="sxs-lookup"><span data-stu-id="47b92-110">**Add or update app registration and provide admin consent**</span></span>

- <span data-ttu-id="47b92-111">[Crear un registro de aplicación:](https://docs.microsoft.com/graph/api/application-post-applications) en este artículo se muestra cómo crear un nuevo objeto de aplicación.</span><span class="sxs-lookup"><span data-stu-id="47b92-111">[Create an app registration](https://docs.microsoft.com/graph/api/application-post-applications) - This article shows you how to create a new application object.</span></span>
- <span data-ttu-id="47b92-112">[Actualizar un registro de aplicación: permisos de API:](https://docs.microsoft.com/graph/api/application-update) en este artículo se muestra cómo actualizar las propiedades de un objeto de aplicación.</span><span class="sxs-lookup"><span data-stu-id="47b92-112">[Update an app registration - API permissions](https://docs.microsoft.com/graph/api/application-update) - This article shows you how to update the properties of an application object.</span></span>
- <span data-ttu-id="47b92-113">[Proporcionar consentimiento de administrador:](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) para el consentimiento de administrador y el consentimiento en general, se requiere que un administrador conceda explícitamente el consentimiento.</span><span class="sxs-lookup"><span data-stu-id="47b92-113">[Provide admin consent](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) - For admin consent and consent in general, we require that an admin explicitly grants consent.</span></span>
- <span data-ttu-id="47b92-114">[RBAC (beta):](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) contenedor de administración de roles para definiciones de roles unificadas y asignaciones de roles para proveedores RBAC de Microsoft 365 que admiten varias entidades de seguridad y varios ámbitos en una sola asignación de roles.</span><span class="sxs-lookup"><span data-stu-id="47b92-114">[RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) - Role management container for unified role definitions and role assignments for Microsoft 365 RBAC providers that support multiple principals and multiple scopes in a single role assignment.</span></span> <span data-ttu-id="47b92-115">Esto es diferente del tipo *de recurso rbacApplication.*</span><span class="sxs-lookup"><span data-stu-id="47b92-115">This is different from *rbacApplication* resource type.</span></span> <span data-ttu-id="47b92-116">Microsoft Intune es un ejemplo de un proveedor RBAC de este tipo.</span><span class="sxs-lookup"><span data-stu-id="47b92-116">Microsoft Intune is an example of such a RBAC provider.</span></span> <span data-ttu-id="47b92-117">Una asignación de roles en Intune puede tener una matriz de entidades de seguridad y una matriz de grupos de ámbito.</span><span class="sxs-lookup"><span data-stu-id="47b92-117">A role assignment in Intune can have an array of principals and an array of scope groups.</span></span> <span data-ttu-id="47b92-118">**Esto está en beta, lo que significa que aún está en desarrollo y no se recomienda su uso en producción.**</span><span class="sxs-lookup"><span data-stu-id="47b92-118">**This is in beta, meaning that it is still in development and not recommended for use in production.**</span></span>