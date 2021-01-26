---
title: Errores de aplicación
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "7841"
ms.openlocfilehash: 2ef90b54ce222a06740e05891fabe87b6565cb14
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/25/2021
ms.locfileid: "49976937"
---
# <a name="application-errors"></a><span data-ttu-id="70915-102">Errores de aplicación</span><span class="sxs-lookup"><span data-stu-id="70915-102">Application errors</span></span>

<span data-ttu-id="70915-103">¿Está buscando información sobre los códigos de error de **AADSTS** que se devuelven desde el servicio de token de seguridad (STS) de Azure Active Directory (Azure AD)?</span><span class="sxs-lookup"><span data-stu-id="70915-103">Looking for info about the **AADSTS error codes** that are returned from the Azure Active Directory (Azure AD) security token service (STS)?</span></span> <span data-ttu-id="70915-104">Lea [los códigos de error de autenticación](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) y autorización de Azure AD para encontrar descripciones de errores de AADSTS, correcciones y algunas soluciones alternativas sugeridas.</span><span class="sxs-lookup"><span data-stu-id="70915-104">Read [Azure AD Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) to find AADSTS error descriptions, fixes, and some suggested workarounds.</span></span>

<span data-ttu-id="70915-105">Los errores de autorización pueden ser el resultado de varios problemas diferentes, la mayoría de los cuales generan un error 401 o 403.</span><span class="sxs-lookup"><span data-stu-id="70915-105">Authorization errors can be a result of several different issues, most of which generate a 401 or 403 error.</span></span> <span data-ttu-id="70915-106">Por ejemplo, lo siguiente puede dar lugar a errores de autenticación:</span><span class="sxs-lookup"><span data-stu-id="70915-106">For example, the following can all lead to authorization errors:</span></span>

- <span data-ttu-id="70915-107">[Flujos de adquisición de token de acceso](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) incorrectos</span><span class="sxs-lookup"><span data-stu-id="70915-107">Incorrect [access token acquisition flows](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes)</span></span> 
- <span data-ttu-id="70915-108">[Ámbitos de permiso](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) mal configurado</span><span class="sxs-lookup"><span data-stu-id="70915-108">Poorly configured [permission scopes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)</span></span> 
- <span data-ttu-id="70915-109">Ausencia de [consentimiento](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)</span><span class="sxs-lookup"><span data-stu-id="70915-109">Lack of [consent](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)</span></span>

<span data-ttu-id="70915-110">Para resolver errores comunes de autorización, pruebe los pasos que se indican a continuación que coincidan más estrechamente con el error que está recibiendo.</span><span class="sxs-lookup"><span data-stu-id="70915-110">To resolve common authorization errors, try the steps provided below that most closely matches the error you are receiving.</span></span> <span data-ttu-id="70915-111">Se pueden aplicar más de uno.</span><span class="sxs-lookup"><span data-stu-id="70915-111">More than one may apply.</span></span>

<span data-ttu-id="70915-112">**Error 401 No autorizado: ¿es válido el token?**</span><span class="sxs-lookup"><span data-stu-id="70915-112">**401 Unauthorized error: Is your token valid?**</span></span>

<span data-ttu-id="70915-113">Asegúrese de que la aplicación presenta un token de acceso válido a Microsoft Graph como parte de la solicitud.</span><span class="sxs-lookup"><span data-stu-id="70915-113">Ensure that your application is presenting a valid access token to Microsoft Graph as part of the request.</span></span> <span data-ttu-id="70915-114">Este error suele indicar que es posible que falte el token de acceso en el encabezado de solicitud de autenticación HTTP o que el token no sea válido o haya expirado.</span><span class="sxs-lookup"><span data-stu-id="70915-114">This error often means that the access token may be missing in the HTTP authenticate request header or that the token is invalid or has expired.</span></span> <span data-ttu-id="70915-115">Le recomendamos encarecidamente que use la [biblioteca de autenticación de Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) para la adquisición de tokens de acceso.</span><span class="sxs-lookup"><span data-stu-id="70915-115">We strongly recommend that you use the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) for access token acquisition.</span></span> <span data-ttu-id="70915-116">Además, este error puede producirse si intenta usar un token de acceso delegado concedido a una cuenta personal de Microsoft para tener acceso a una API que solo admite cuentas de trabajo o educativas (cuentas organizativas).</span><span class="sxs-lookup"><span data-stu-id="70915-116">Additionally this error may occur if you try to use a delegated access token granted to a personal Microsoft account to access an API that only supports work or school accounts (organizational accounts).</span></span>

<span data-ttu-id="70915-117">**Error 403 Prohibido: ¿ha elegido el conjunto adecuado de permisos?**</span><span class="sxs-lookup"><span data-stu-id="70915-117">**403 Forbidden error: Have you chosen the right set of permissions?**</span></span>

<span data-ttu-id="70915-118">Compruebe que ha solicitado el conjunto correcto de permisos en función de las API de Microsoft Graph a las que llama la aplicación.</span><span class="sxs-lookup"><span data-stu-id="70915-118">Check that you have requested the correct set of permissions based on the Microsoft Graph APIs your app calls.</span></span> <span data-ttu-id="70915-119">Los permisos con privilegios mínimos recomendados se proporcionan en todos los temas del método de referencia de la API de Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="70915-119">Recommended least privileged permissions are provided in all the Microsoft Graph API reference method topics.</span></span> <span data-ttu-id="70915-120">Además, un usuario o un administrador deben conceder estos permisos a la aplicación.</span><span class="sxs-lookup"><span data-stu-id="70915-120">Additionally, those permissions must be granted to the application by a user or an administrator.</span></span> <span data-ttu-id="70915-121">La concesión de permisos suele hacerse con una página de consentimiento o concediendo permisos mediante la hoja de registro de aplicaciones del portal de Azure.</span><span class="sxs-lookup"><span data-stu-id="70915-121">Granting permissions normally happens through a consent page or by granting permissions using the Azure Portal application registration blade.</span></span> <span data-ttu-id="70915-122">En la hoja **Configuración** de la aplicación, haga clic en **Permisos necesarios** y haga clic en **Conceder permisos**.</span><span class="sxs-lookup"><span data-stu-id="70915-122">From the **Settings** blade for the application, click **Required Permissions**, and then click **Grant Permissions**.</span></span>

- [<span data-ttu-id="70915-123">Permisos de Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="70915-123">Microsoft Graph permissions</span></span>](https://docs.microsoft.com/graph/permissions-reference) 
- [<span data-ttu-id="70915-124">Descripción de permisos y consentimiento de Azure AD</span><span class="sxs-lookup"><span data-stu-id="70915-124">Understanding Azure AD permissions and consent</span></span>](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

<span data-ttu-id="70915-125">**Error 403 Prohibido: ¿ha adquirido su aplicación un token para coincidir con los permisos seleccionados?**</span><span class="sxs-lookup"><span data-stu-id="70915-125">**403 Forbidden error: Did your app acquire a token to match chosen permissions?**</span></span>

<span data-ttu-id="70915-126">Asegúrese de que el tipo de permisos solicitado o concedido coincida con el tipo de token de acceso que la aplicación adquiere.</span><span class="sxs-lookup"><span data-stu-id="70915-126">Make sure that the type of permissions requested or granted matches the type of access token that your app acquires.</span></span> <span data-ttu-id="70915-127">Es posible que solicite y conceda permisos de aplicación, pero que use tokens de flujo de código interactivo delegados en lugar de tokens de flujo de credenciales de cliente, o bien que solicite y conceda permisos delegados, pero que utilice tokens de flujo de credenciales de cliente en lugar de los tokens de flujo de código delegado.</span><span class="sxs-lookup"><span data-stu-id="70915-127">You might be requesting and granting application permissions but using delegated interactive code flow tokens instead of client credential flow tokens, or requesting and granting delegated permissions but using client credential flow tokens instead of delegated code flow tokens.</span></span>

- [<span data-ttu-id="70915-128">Obtener acceso en nombre de usuarios y permisos delegados</span><span class="sxs-lookup"><span data-stu-id="70915-128">Get access on behalf of users and delegated permissions</span></span>](https://docs.microsoft.com/graph/auth_v2_user) 
- [<span data-ttu-id="70915-129">Azure AD v 2.0: Flujo de código de autenticación de OAuth 2.0</span><span class="sxs-lookup"><span data-stu-id="70915-129">Azure AD v2.0 - OAuth 2.0 authorization code flow</span></span>](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [<span data-ttu-id="70915-130">Obtener acceso sin usuario (servicio de demonio) y permisos de aplicación</span><span class="sxs-lookup"><span data-stu-id="70915-130">Get access without a user (daemon service) and application permissions</span></span>](https://docs.microsoft.com/graph/auth_v2_service) 
- [<span data-ttu-id="70915-131">Azure AD v 2.0: Flujo de credenciales de cliente de OAuth 2.0</span><span class="sxs-lookup"><span data-stu-id="70915-131">Azure AD v2.0 - OAuth 2.0 client credentials flow</span></span>](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

<span data-ttu-id="70915-132">**Error 403 Prohibido:: restableciendo contraseña**</span><span class="sxs-lookup"><span data-stu-id="70915-132">**403 Forbidden error: Resetting password**</span></span>

<span data-ttu-id="70915-133">Actualmente, no hay permisos de servicio a servicio de demonio de permiso de aplicación que permitan restablecer las contraseñas de usuario.</span><span class="sxs-lookup"><span data-stu-id="70915-133">Currently, there are no application permission daemon service-to-service permissions that allow resetting user passwords.</span></span> <span data-ttu-id="70915-134">Las API solo se admiten con el código delegado interactivo en los flujos con una sesión de administrador iniciada.</span><span class="sxs-lookup"><span data-stu-id="70915-134">These APIs are only supported using the interactive delegated code flows with a signed-in administrator.</span></span>

- [<span data-ttu-id="70915-135">Permisos de Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="70915-135">Microsoft Graph permissions</span></span>](https://docs.microsoft.com/graph/permissions-reference)

<span data-ttu-id="70915-136">**Error 403 Prohibido: ¿tiene acceso el usuario y está autorizado?**</span><span class="sxs-lookup"><span data-stu-id="70915-136">**403 Forbidden: Does the user have access and are they licensed?**</span></span>

<span data-ttu-id="70915-137">Para flujos de código delegados, Microsoft Graph evalúa si la solicitud se permite en función de los permisos concedidos a la aplicación y los permisos que tiene el usuario que ha iniciado sesión.</span><span class="sxs-lookup"><span data-stu-id="70915-137">For delegated code flows, Microsoft Graph evaluates if the request is allowed based on the permissions granted to the app and the permissions that the signed-in user has.</span></span> <span data-ttu-id="70915-138">Por lo general, este error indica que el usuario no tiene privilegios suficientes para realizar la solicitud o el usuario no tiene licencia para tener acceso a los datos.</span><span class="sxs-lookup"><span data-stu-id="70915-138">Generally, this error indicates that the user is not privileged enough to perform the request or the user is not licensed for the data being accessed.</span></span> <span data-ttu-id="70915-139">Solo los usuarios con los permisos o licencias necesarios pueden realizar la solicitud correctamente.</span><span class="sxs-lookup"><span data-stu-id="70915-139">Only users with the required permissions or licenses can make the request successfully.</span></span>

<span data-ttu-id="70915-140">**Error 403 Prohibido: ¿seleccionó la API de recurso adecuada?**</span><span class="sxs-lookup"><span data-stu-id="70915-140">**403 Forbidden: Did you select the correct resource API?**</span></span>

<span data-ttu-id="70915-141">Los servicios de API como Microsoft Graph comprueban que la notificación de aud (audiencia) en el token de acceso recibido coincide con el valor que espera para sí mismo y, si no es así, produce un error 403 Prohibido.</span><span class="sxs-lookup"><span data-stu-id="70915-141">API services like Microsoft Graph check that the aud claim (audience) in the received access token matches the value it expects for itself, and if not, it results in a 403 Forbidden error.</span></span> <span data-ttu-id="70915-142">Un error común que resulta en este error es intentar usar un token adquirido para las API de Azure AD Graph, las API de Outlook o las API de SharePoint/OneDrive para llamar a Microsoft Graph (o viceversa).</span><span class="sxs-lookup"><span data-stu-id="70915-142">A common mistake resulting in this error is trying to use a token acquired for Azure AD Graph APIs, Outlook APIs, or SharePoint/OneDrive APIs to call Microsoft Graph (or vice versa).</span></span> <span data-ttu-id="70915-143">Asegúrese de que el recurso (o ámbito) para el que la aplicación está adquiriendo un token coincida con la API a la que llama la aplicación.</span><span class="sxs-lookup"><span data-stu-id="70915-143">Ensure that the resource (or scope) your app is acquiring a token for matches the API that the app is calling.</span></span>

<span data-ttu-id="70915-144">**400 Solicitud incorrecta o 403 Prohibido: ¿cumple el usuario las directivas de acceso condicional (CA) de su organización?**</span><span class="sxs-lookup"><span data-stu-id="70915-144">**400 Bad Request or 403 Forbidden: Does the user comply with their organization's conditional access (CA) policies?**</span></span>

<span data-ttu-id="70915-145">En función de las directivas de ca de una organización, un usuario que obtiene acceso a los recursos de Microsoft Graph a través de la aplicación puede ser objeto de un desafío por información adicional que no está presente en el token de acceso que adquirió originalmente la aplicación.</span><span class="sxs-lookup"><span data-stu-id="70915-145">Based on an organization's CA policies, a user accessing Microsoft Graph resources via your app may be challenged for additional information that is not present in the access token your app originally acquired.</span></span> <span data-ttu-id="70915-146">En este caso, la aplicación recibe un error 400 con *interaction_required* durante la adquisición del token de acceso o un error 403 con *insufficient_claims* cuando se llama a Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="70915-146">In this case, your app receives a 400 with an *interaction_required* error during access token acquisition or a 403 with *insufficient_claims* error when calling Microsoft Graph.</span></span> <span data-ttu-id="70915-147">En ambos casos, la respuesta del error contiene información adicional que puede mostrarse al punto de conexión de autorización para pedir al usuario información adicional (por ejemplo, autenticación multifactor o inscripción de dispositivo).</span><span class="sxs-lookup"><span data-stu-id="70915-147">In both cases, the error response contains additional information that can be presented to the authorize endpoint to challenge the user for additional information (like multi-factor authentication or device enrollment).</span></span>

- [<span data-ttu-id="70915-148">Controlar los desafíos de acceso condicional mediante MSAL </span><span class="sxs-lookup"><span data-stu-id="70915-148">Handling conditional access challenges using MSAL </span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [<span data-ttu-id="70915-149">Guía para desarrolladores para acceso condicional de Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="70915-149">Developer guidance for Azure Active Directory conditional access</span></span>](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)