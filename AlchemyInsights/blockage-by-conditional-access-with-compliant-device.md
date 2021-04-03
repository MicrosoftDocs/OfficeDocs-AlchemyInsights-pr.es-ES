---
title: El Acceso condicional con dispositivos compatibles me bloquea
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9835"
- "9003257"
ms.openlocfilehash: 240bd25f4d62505202c8cd7ceabe4c1cd3d5c0b5
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897984"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a><span data-ttu-id="369f2-102">El Acceso condicional con dispositivos compatibles me bloquea</span><span class="sxs-lookup"><span data-stu-id="369f2-102">I’m getting blocked by Conditional Access with compliant device</span></span>

<span data-ttu-id="369f2-103">**Herramientas altamente recomendadas**</span><span class="sxs-lookup"><span data-stu-id="369f2-103">**Highly Recommended Tools**</span></span>

- <span data-ttu-id="369f2-104">[Herramienta solucionador de problemas de registro de dispositivo](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) : una herramienta completa que ayuda a solucionar los problemas de registro de dispositivos más comunes.</span><span class="sxs-lookup"><span data-stu-id="369f2-104">[Device Registration Troubleshooter Tool](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - A comprehensive tool that helps troubleshoot the most common device registration issues.</span></span>
- <span data-ttu-id="369f2-105">[Script de conectividad de registro de dispositivos de prueba](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) : una herramienta que se usa para asegurarse de que un dispositivo puede tener acceso a los puntos de conexión de Registro de dispositivos en la cuenta del sistema.</span><span class="sxs-lookup"><span data-stu-id="369f2-105">[Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - A tool used to ensure that a device can access Device Registration endpoints under the system account.</span></span>
- <span data-ttu-id="369f2-106">[Script de limpieza de dispositivos de Azure AD](https://github.com/mzmaili/AzureADDeviceCleanup) : una herramienta usada para buscar y administrar dispositivos obsoletos en su entorno.</span><span class="sxs-lookup"><span data-stu-id="369f2-106">[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) - A tool used to seek and manage stale devices in your environment.</span></span>

<span data-ttu-id="369f2-107">Estas son algunas de las razones comunes por las que puede producirse un error de Acceso condicional en un dispositivo compatible o por qué los usuarios pueden recibir un mensaje de **No puede llegar al destino desde aquí** durante una solicitud de inicio de sesión a un recurso de la organización.</span><span class="sxs-lookup"><span data-stu-id="369f2-107">Here are some common reasons why Conditional Access may be failing for a compliant device or why your users may be receiving **You can't get there from here** message during a sign-in request to an organizational resource.</span></span>

1. <span data-ttu-id="369f2-108">**El dispositivo no está en un estado de dispositivo requerido con un MDM**:</span><span class="sxs-lookup"><span data-stu-id="369f2-108">**Device is not in a required device state with an MDM**:</span></span>

<span data-ttu-id="369f2-109">Valide que el dispositivo esté inscrito con un proveedor de MDM aprobado como Intune y esté *marcado como compatible*.</span><span class="sxs-lookup"><span data-stu-id="369f2-109">Validate that the device is enrolled with an approved MDM provider like Intune and *marked as compliant*.</span></span> <span data-ttu-id="369f2-110">Para obtener más información sobre Intune, consulte este [documento](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment).</span><span class="sxs-lookup"><span data-stu-id="369f2-110">For more information on Intune see this [document](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment).</span></span> <span data-ttu-id="369f2-111">Para obtener una descripción más clara del cumplimiento de dispositivos e Intune, consulte [usar la directiva de cumplimiento para establecer reglas para los dispositivos que administra con Intune](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started).</span><span class="sxs-lookup"><span data-stu-id="369f2-111">For better understanding of device compliance and Intune, see [use compliance policy to set rules for devices you manage with Intune](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started).</span></span> <span data-ttu-id="369f2-112">Si tiene problemas al inscribir un dispositivo con Intune, encuentre los detalles para la solución de problemas en [Solucionar problemas de inscripción de dispositivos en Microsoft](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="369f2-112">If you are having issues enrolling a device with Intune, find troubleshooting details at [Troubleshoot device enrollment in Microsoft](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span> <span data-ttu-id="369f2-113">Para obtener más soporte de Intune, cree una solicitud de soporte técnico.</span><span class="sxs-lookup"><span data-stu-id="369f2-113">For further Intune support, create a support request.</span></span> <span data-ttu-id="369f2-114">Para hacerlo, visite la [página de Ayuda y soporte técnico de Intune](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport).</span><span class="sxs-lookup"><span data-stu-id="369f2-114">To do so, visit the [Intune Help and Support page](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport).</span></span>

2. <span data-ttu-id="369f2-115">**El dispositivo no está unido a la red de la organización**:</span><span class="sxs-lookup"><span data-stu-id="369f2-115">**Device is not joined to the organizations network**:</span></span>

<span data-ttu-id="369f2-116">Para obtener acceso a los recursos de la organización, el dispositivo tiene que estar conectado a la red de la organización, ya sea a través de una conexión directa o una red privada virtual (VPN), y también debe estar unido a una red local o Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="369f2-116">For access to organizational resources, the device has to be connected to the organization's network, either through direct connection or a virtual private network (VPN), and also joined to on-premise or Azure Active Directory.</span></span> <span data-ttu-id="369f2-117">Para unir un dispositivo de trabajo a la red de la organización, vea [Unir el dispositivo de trabajo a la red de su organización](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network).</span><span class="sxs-lookup"><span data-stu-id="369f2-117">To join a work device to the organization network, see [Join your work device to your organization's network](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network).</span></span> <span data-ttu-id="369f2-118">Para registrar un dispositivo personal/BYOD, vea [Registrar su dispositivo personal en la red de su organización](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network).</span><span class="sxs-lookup"><span data-stu-id="369f2-118">To register a personal/BYOD device, see [Register your personal device on your organization's network](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network).</span></span>

- <span data-ttu-id="369f2-119">Para validar si el dispositivo se ha unido a la red, puede seguir los pasos para dispositivos registrados [aquí](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) o para dispositivos de trabajo [aquí](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined).</span><span class="sxs-lookup"><span data-stu-id="369f2-119">To validate whether the device has joined the network, you can follow the steps for registered devices [here](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) or work devices [here](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined).</span></span> <span data-ttu-id="369f2-120">Para localizar el problema de conectividad de red de la organización, siga las siguientes instrucciones:</span><span class="sxs-lookup"><span data-stu-id="369f2-120">To scope the issue to Org network connectivity, follow guidelines below:</span></span>

    1. <span data-ttu-id="369f2-121">Inicie sesión en Windows con su cuenta del trabajo o de la escuela,  por ejemplo, alain@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="369f2-121">Sign in to Windows using your work or school account,  for example, alain@contoso.com.</span></span>
    2. <span data-ttu-id="369f2-122">Conéctese a la red de su organización a través de una VPN o DirectAccess.</span><span class="sxs-lookup"><span data-stu-id="369f2-122">Connect to your organization's network through a VPN or DirectAccess.</span></span>
    3. <span data-ttu-id="369f2-123">Después de conectarse, pulse la **Tecla del logotipo de Windows+L** para bloquear el dispositivo.</span><span class="sxs-lookup"><span data-stu-id="369f2-123">After you're connected, press the **Windows logo key+L** to lock your device.</span></span>
    4. <span data-ttu-id="369f2-124">Desbloquee el dispositivo con su cuenta profesional o educativa y, a continuación, intente obtener acceso a la aplicación o el servicio problemático nuevamente.</span><span class="sxs-lookup"><span data-stu-id="369f2-124">Unlock your device using your work or school account, and then try to access the problematic app or service again.</span></span>

<span data-ttu-id="369f2-125">Si ve el mensaje de error **No puede llegar al destino desde aquí** de nuevo, es probable que el problema esté en otro lugar.</span><span class="sxs-lookup"><span data-stu-id="369f2-125">If you see the **You can't get there from here** error message again, issue is likely elsewhere.</span></span>

3. <span data-ttu-id="369f2-126">**El sistema operativo no es compatible**:</span><span class="sxs-lookup"><span data-stu-id="369f2-126">**Operating system is not supported**:</span></span>

<span data-ttu-id="369f2-127">Asegúrese de que ejecuta una versión compatible del sistema operativo, que incluye:</span><span class="sxs-lookup"><span data-stu-id="369f2-127">Ensure that you're running a supported version of the operating system, including:</span></span>

- <span data-ttu-id="369f2-128">**Cliente de Windows**: Windows 7 o versiones posteriores</span><span class="sxs-lookup"><span data-stu-id="369f2-128">**Windows Client**: Windows 7 or later</span></span>

- <span data-ttu-id="369f2-129">**Windows Server**: Windows Server 2008 R2 o posteriores</span><span class="sxs-lookup"><span data-stu-id="369f2-129">**Windows Server**: Windows Server 2008 R2 or later</span></span>

- <span data-ttu-id="369f2-130">**macOS**: macOS X o posteriores</span><span class="sxs-lookup"><span data-stu-id="369f2-130">**macOS**: macOS X or later</span></span>

- <span data-ttu-id="369f2-131">**Android e iOS**: Última versión de los sistemas operativos móviles de Android e iOS</span><span class="sxs-lookup"><span data-stu-id="369f2-131">**Android and iOS**: Latest version of Android and iOS mobile operating systems</span></span>

4. <span data-ttu-id="369f2-132">**El explorador web no es compatible**:</span><span class="sxs-lookup"><span data-stu-id="369f2-132">**Web browser is not supported**:</span></span>

<span data-ttu-id="369f2-133">Encontrará los exploradores admitidos a continuación.</span><span class="sxs-lookup"><span data-stu-id="369f2-133">Please find supported browsers below.</span></span> <span data-ttu-id="369f2-134">Para la compatibilidad de Chrome con Windows 1703 o versiones posteriores, se necesita una extensión de cuentas de Windows 10.</span><span class="sxs-lookup"><span data-stu-id="369f2-134">For Chrome support with Windows 1703 or later versions, a Windows 10 Accounts extension is required.</span></span> <span data-ttu-id="369f2-135">Para Edge 85+, es necesario que el usuario haya iniciado sesión para transmitir correctamente la información de cumplimiento del dispositivo.</span><span class="sxs-lookup"><span data-stu-id="369f2-135">For Edge 85+, the user needs to be signed in to properly pass device compliance information.</span></span> <span data-ttu-id="369f2-136">Para obtener más información, consulte [aquí](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span><span class="sxs-lookup"><span data-stu-id="369f2-136">For more details, see [here](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span></span>

- <span data-ttu-id="369f2-137">**Windows 10**: Microsoft Edge, Internet Explorer, Chrome</span><span class="sxs-lookup"><span data-stu-id="369f2-137">**Windows 10**: Microsoft Edge, Internet Explorer, Chrome</span></span>
- <span data-ttu-id="369f2-138">**Windows 8 / 8.1**: Internet Explorer, Chrome</span><span class="sxs-lookup"><span data-stu-id="369f2-138">**Windows 8 / 8.1**: Internet Explorer, Chrome</span></span>
- <span data-ttu-id="369f2-139">**Windows 7**: Internet Explorer, Chrome</span><span class="sxs-lookup"><span data-stu-id="369f2-139">**Windows 7**: Internet Explorer, Chrome</span></span>
- <span data-ttu-id="369f2-140">**iOS**: Microsoft Edge, Intune Managed Browser, Safari</span><span class="sxs-lookup"><span data-stu-id="369f2-140">**iOS**: Microsoft Edge, Intune Managed Browser, Safari</span></span>
- <span data-ttu-id="369f2-141">**Android**: **Microsoft Edge**: Intune Managed Browser, Chrome</span><span class="sxs-lookup"><span data-stu-id="369f2-141">**Android**: **Microsoft Edge**: Intune Managed Browser, Chrome</span></span>
- <span data-ttu-id="369f2-142">**Windows Phone**: Microsoft Edge, Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="369f2-142">**Windows Phone**: Microsoft Edge, Internet Explorer</span></span>
- <span data-ttu-id="369f2-143">**Windows Server 2019**: Microsoft Edge, Internet Explorer, Chrome</span><span class="sxs-lookup"><span data-stu-id="369f2-143">**Windows Server 2019**: Microsoft Edge, Internet Explorer, Chrome</span></span>
- <span data-ttu-id="369f2-144">**Windows Server 2016**: Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="369f2-144">**Windows Server 2016**: Internet Explorer</span></span>
- <span data-ttu-id="369f2-145">**Windows Server 2012 R2**: Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="369f2-145">**Windows Server 2012 R2**: Internet Explorer</span></span>
- <span data-ttu-id="369f2-146">**Windows Server 2008 R2**: Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="369f2-146">**Windows Server 2008 R2**: Internet Explorer</span></span>
- <span data-ttu-id="369f2-147">**macOS**: Chrome, Safari</span><span class="sxs-lookup"><span data-stu-id="369f2-147">**macOS**: Chrome, Safari</span></span>

<span data-ttu-id="369f2-148">Obtenga más información sobre el mensaje **No puede llegar al destino desde aquí** y los pasos de solución de problemas [aquí](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation).</span><span class="sxs-lookup"><span data-stu-id="369f2-148">Find more information on the **You can't get there** message and troubleshooting steps [here](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation).</span></span>