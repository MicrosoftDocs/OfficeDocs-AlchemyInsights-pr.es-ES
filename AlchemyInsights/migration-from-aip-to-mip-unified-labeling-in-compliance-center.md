---
title: Migración de AIP a MIP o etiquetado unificado en el centro de seguridad y cumplimiento
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
- "9002278"
- "5114"
ms.openlocfilehash: 12f5f5c46edd7918618c55a8a1905f3b28643092
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825388"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="3ec8f-102">Migración de AIP a MIP o etiquetado unificado en el centro de seguridad y cumplimiento</span><span class="sxs-lookup"><span data-stu-id="3ec8f-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="3ec8f-103">Para migrar de etiquetas de AIP a etiquetado unificado en el centro de seguridad y cumplimiento, haga lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="3ec8f-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="3ec8f-104">**Activar la protección desde Azure Portal**</span><span class="sxs-lookup"><span data-stu-id="3ec8f-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="3ec8f-105">Si aún no lo ha hecho, abra una nueva ventana del explorador e [inicie sesión en Azure Portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="3ec8f-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="3ec8f-106">Desplácese hasta la hoja de **Azure Information Protection**.</span><span class="sxs-lookup"><span data-stu-id="3ec8f-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="3ec8f-107">Por ejemplo, en el menú de central, haga clic en **Todos los servicios** y comience a escribir **Información** en el cuadro Filtro.</span><span class="sxs-lookup"><span data-stu-id="3ec8f-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="3ec8f-108">Seleccione **Azure Information Protection**.</span><span class="sxs-lookup"><span data-stu-id="3ec8f-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="3ec8f-109">Si no ha accedido a la hoja de Azure Information Protection antes, consulte los [pasos adicionales](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) únicos para agregar esta hoja al portal.</span><span class="sxs-lookup"><span data-stu-id="3ec8f-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="3ec8f-110">Para abrir la hoja de Azure Information Protection, debe tener un [plan de Azure Information Protection Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) o un plan de Office 365 que incluya derechos de administración.</span><span class="sxs-lookup"><span data-stu-id="3ec8f-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="3ec8f-111">Si tiene una de estas suscripciones pero ve un mensaje que indica que no se puede encontrar una suscripción válida, [póngase en contacto con el soporte técnico de Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) o use los canales de soporte técnico estándar.</span><span class="sxs-lookup"><span data-stu-id="3ec8f-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="3ec8f-112">Localice las opciones del menú **Administrar** y seleccione **Activación de protección**.</span><span class="sxs-lookup"><span data-stu-id="3ec8f-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="3ec8f-113">Haga clic en **Activar** y confirme la acción.</span><span class="sxs-lookup"><span data-stu-id="3ec8f-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="3ec8f-114">Cuando haya finalizado la activación, la barra de información mostrará **La activación se completó correctamente**.</span><span class="sxs-lookup"><span data-stu-id="3ec8f-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="3ec8f-115">**Migrar las etiquetas de Azure Information Protection al Centro de seguridad y cumplimiento de Office 365**</span><span class="sxs-lookup"><span data-stu-id="3ec8f-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="3ec8f-116">Asegúrese de que ha iniciado sesión como un usuario con permisos de administrador global.</span><span class="sxs-lookup"><span data-stu-id="3ec8f-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="3ec8f-117">Desplácese hasta la hoja de **Azure Information Protection**.</span><span class="sxs-lookup"><span data-stu-id="3ec8f-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="3ec8f-118">En la opción del menú **Administrar**, seleccione **Etiquetado unificado**.</span><span class="sxs-lookup"><span data-stu-id="3ec8f-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="3ec8f-119">En la hoja **Azure Information Protection: etiquetado unificado**, haga clic en **Activar** y siga las instrucciones que se muestran en línea.</span><span class="sxs-lookup"><span data-stu-id="3ec8f-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="3ec8f-120">**Nota**: compruebe que tiene los permisos adecuados antes de activar la Migración del Centro de seguridad y cumplimiento.</span><span class="sxs-lookup"><span data-stu-id="3ec8f-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="3ec8f-121">Vea estos artículos para obtener más información:</span><span class="sxs-lookup"><span data-stu-id="3ec8f-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="3ec8f-122">¿Necesita ser un administrador global para configurar Azure Information Protection o se puede delegar en otros administradores?</span><span class="sxs-lookup"><span data-stu-id="3ec8f-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="3ec8f-123">Información importante sobre los roles administrativos después de migrar al Centro de seguridad y cumplimiento.</span><span class="sxs-lookup"><span data-stu-id="3ec8f-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="3ec8f-124">Para obtener más información sobre la migración de AIP al etiquetado unificado en el centro de seguridad y cumplimiento, vea [Migrar etiquetas](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span><span class="sxs-lookup"><span data-stu-id="3ec8f-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
