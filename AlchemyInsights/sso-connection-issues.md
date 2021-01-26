---
title: Problemas de conexión sso
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
- "9004357"
- "7810"
ms.openlocfilehash: 33074d70377866332feeccfb8b6400eff2de5a73
ms.sourcegitcommit: e188ec7a583837a3e07880d05b3607b8bdac729c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/21/2021
ms.locfileid: "49918148"
---
# <a name="sso-connection-issues"></a><span data-ttu-id="fcc73-102">Problemas de conexión sso</span><span class="sxs-lookup"><span data-stu-id="fcc73-102">SSO Connection Issues</span></span>

1. <span data-ttu-id="fcc73-103">Siga la guía [Inicio rápido: configurar las propiedades de una aplicación](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) para configurar la aplicación.</span><span class="sxs-lookup"><span data-stu-id="fcc73-103">Follow the [Quickstart: Configure properties for an application](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) guide to configure your application.</span></span>
2. <span data-ttu-id="fcc73-104">Según la aplicación y la [opción de inicio de sesión único](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) que elija, siga las instrucciones adecuadas a continuación:</span><span class="sxs-lookup"><span data-stu-id="fcc73-104">Depending on the application and [Single sign-on option](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) you chose, follow the appropriate guidance below:</span></span>
    - <span data-ttu-id="fcc73-105">Para configurar una **aplicación local** para el inicio de sesión único basado en **SAML,** vea inicio de sesión único saml para aplicaciones locales [con proxy de aplicación.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)</span><span class="sxs-lookup"><span data-stu-id="fcc73-105">To configure an **on-premises application** for **SAML-based single sign-on**, see [SAML single-sign-on for on-premises applications with Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps).</span></span>
    - <span data-ttu-id="fcc73-106">Para configurar una **aplicación en la nube** para **el** inicio de sesión único basado en contraseña, vea Configurar el inicio de sesión único [de contraseña.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)</span><span class="sxs-lookup"><span data-stu-id="fcc73-106">To configure a **cloud application** for **password-based single sign-on**, see  [Configure password single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications).</span></span>
    - <span data-ttu-id="fcc73-107">Para configurar una **aplicación local** para el inicio de sesión único a través del **Proxy** de aplicación, consulte Almacén de contraseñas para el inicio de sesión único con proxy [de aplicación.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)</span><span class="sxs-lookup"><span data-stu-id="fcc73-107">To configure an **on-premises application** for **single sign-on through Application Proxy**, see [Password vaulting for single sign-on with Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).</span></span>
3. <span data-ttu-id="fcc73-108">**Solución de problemas de Proxy** de aplicación: se recomienda empezar con la revisión del flujo de solución de problemas, depurar problemas del conector de [proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)de aplicación para determinar si los conectores de proxy de aplicación están configurados correctamente.</span><span class="sxs-lookup"><span data-stu-id="fcc73-108">**Troubleshooting Application Proxy issues**: we recommend you start with reviewing the troubleshooting flow, [Debug Application Proxy Connector issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), to determine if Application Proxy connectors are configured correctly.</span></span> <span data-ttu-id="fcc73-109">Si todavía tiene problemas para conectarse a la aplicación, siga el flujo de solución de problemas en depurar problemas de [la aplicación proxy de aplicación.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps)</span><span class="sxs-lookup"><span data-stu-id="fcc73-109">If you are still having trouble connecting to the application, follow the troubleshooting flow in [Debug Application Proxy application issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps).</span></span> <span data-ttu-id="fcc73-110">Puede identificar [problemas de CORS con](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) las herramientas de depuración del explorador:</span><span class="sxs-lookup"><span data-stu-id="fcc73-110">You can [identify CORS issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) by using browser debug tools:</span></span>
    - <span data-ttu-id="fcc73-111">Inicie el explorador y busque la aplicación web.</span><span class="sxs-lookup"><span data-stu-id="fcc73-111">Launch the browser and browse to the web app.</span></span>
    - <span data-ttu-id="fcc73-112">Presione **F12** para abrir la consola de depuración.</span><span class="sxs-lookup"><span data-stu-id="fcc73-112">Press **F12** to bring up the debug console.</span></span>
    - <span data-ttu-id="fcc73-113">Intente reproducir la transacción y revise el mensaje de la consola.</span><span class="sxs-lookup"><span data-stu-id="fcc73-113">Try to reproduce the transaction, and review the console message.</span></span> <span data-ttu-id="fcc73-114">Una infracción de CORS produce un error de consola sobre el origen.</span><span class="sxs-lookup"><span data-stu-id="fcc73-114">A CORS violation produces a console error about origin.</span></span>
    - <span data-ttu-id="fcc73-115">Algunos problemas de CORS no se pueden resolver, como cuando la aplicación redirige a login.microsoft.com para autenticarse y el token de acceso expira.</span><span class="sxs-lookup"><span data-stu-id="fcc73-115">Some CORS issues can't be resolved, such as when your app redirects to login.microsoft.com to authenticate, and the access token expires.</span></span> <span data-ttu-id="fcc73-116">A continuación, se produce un error en la llamada cors.</span><span class="sxs-lookup"><span data-stu-id="fcc73-116">The CORS call then fails.</span></span> <span data-ttu-id="fcc73-117">Una solución para este escenario es extender la duración del token de acceso para evitar que expire durante la sesión de un usuario.</span><span class="sxs-lookup"><span data-stu-id="fcc73-117">A workaround for this scenario is to extend the lifetime of the access token, to prevent it from expiring during a user’s session.</span></span> <span data-ttu-id="fcc73-118">Para más información sobre cómo hacer esto, vea [Vigencia de tokens configurable en la Plataforma de identidad de Microsoft](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="fcc73-118">For more information about how to do this, see [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>
4. <span data-ttu-id="fcc73-119">Solución de problemas del inicio de sesión único basado en **SAML:** le recomendamos que consulte Problemas al iniciar sesión en aplicaciones configuradas de inicio de sesión único basado en [SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)para encontrar las soluciones a los problemas que es más probable que encuentre.</span><span class="sxs-lookup"><span data-stu-id="fcc73-119">**Troubleshooting SAML-based single sign-on**: we recommend checking [Problems signing in to SAML-based single sign-on configured apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery), to find the solutions to the issues you are most likely to encounter.</span></span>
5. <span data-ttu-id="fcc73-120">**Solución de problemas del** inicio de sesión único basado en contraseña: recomendamos comprobar el inicio de sesión único basado en contraseña en [Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)para encontrar las soluciones a los problemas que son más probables que se encuentren.</span><span class="sxs-lookup"><span data-stu-id="fcc73-120">**Troubleshooting password-based single sign-on**: we recommend checking [Troubleshoot password-based single sign-on in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso), to find the solutions to the issues you are most likely to encounter.</span></span>
6. <span data-ttu-id="fcc73-121">Para ver los problemas de conexión al usar una VPN, consulte Cómo usar el inicio de sesión único [(SSO)](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections)a través de VPN y Wi-Fi vpn.</span><span class="sxs-lookup"><span data-stu-id="fcc73-121">For connection issues while using a VPN, see [How to use single sign on (SSO) over VPN and Wi-Fi connections](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections).</span></span>