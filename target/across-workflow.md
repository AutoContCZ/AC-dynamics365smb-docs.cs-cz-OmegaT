---
    title: Workflows in Dynamic 365 Business Central
    description: Use workflows to connect business-process tasks performed by different users. System tasks, such as automatic posting, can be included as workflow steps.
    author: SorenGP

    ms.service: dynamics365-business-central
    ms.topic: conceptual
    ms.devlang: na
    ms.tgt_pltfrm: na
    ms.workload: na
    ms.search.keywords:
    ms.date: 06/11/2021
    ms.author: edupont

---
# Workflows in Dynamics 365 Business Central

Můžete nastavovat a používat workflow, které spojují úlohy podnikových procesů prováděné různými uživateli. Systémové úlohy, jako je například automatické účtování, lze zahrnout jako kroky do workflow, které předchází nebo následují úkoly uživatele. Vyžádání a udělení souhlasu k vytvoření nových záznamů jsou typické kroky workflow.

On the **Workflow** page, you create a workflow by listing the involved steps on the lines. Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options. You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.

The generic version of [!INCLUDE[prod_short](includes/prod_short.md)] includes a number of preconfigured workflows represented by workflow templates that you can copy to create workflows. The code for workflow templates that are added by Microsoft are prefixed with “MS-“. For more information, see the list of workflow templates in the Workflow Templates page.

If a business scenario requires a workflow event or response that is not supported, you can either use Power Automate or work with a Microsoft partner to customize the application code. For more information, see [Using [!INCLUDE[prod_short](includes/prod_short.md)] in an Automated Workflow](across-how-use-financials-data-source-flow.md).

Any workflow template that you create with Power Automate is added to the list of workflow templates within [!INCLUDE[prod_short](includes/prod_short.md)]. For more information, see [Using Business Central in an Automated Workflow](across-how-use-financials-data-source-flow.md).

Následující tabulka popisuje sekvenci úloh s odkazy na témata, které je popisují.

| **Viz** | **také** |
|------------|-------------|  
| Set up workflow users, specify how users get notified, and create new workflows. For new workflows for unsupported scenarios, implement the required workflow elements by customizing the application code. | [Setting Up Workflows](across-set-up-workflows.md) |
| Enable workflows, act on workflow notifications, including request approvals and approve requests to perform a workflow step. Archive and delete workflows. | [Using Workflows](across-use-workflows.md) |

## Viz také

[Sales](sales-manage-sales.md)  
[Purchasing](purchasing-manage-purchasing.md)  
[Managing Projects](projects-manage-projects.md)  
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]