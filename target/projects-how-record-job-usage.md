---
title: Record Consumption or Usage of Job Resources and Items
description: Describes how to record the consumption or usage of items or resources on jobs to facilitate project management.
author: SorenGP

ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: project management, consumption
ms.search.form: 89, 92, 201, 1007, 1014
ms.date: 04/01/2021
ms.author: edupont

---
# Record Consumption or Usage for Jobs

On the **Job Planning Lines** page, you can review and record usage on various parts of your job, which is automatically updated as you modify and transfer information between jobs and job journals or job invoices. This requires that you have set up a job so that the **Apply Usage Link** is turned on. For more information, see [Set Up Jobs](projects-how-setup-jobs.md).

For example, for planning lines of type **Budget**, you can enter the quantity of a resource, and indicate what quantity to transfer to the job journal. If the type of the planning line is **Billable**, you can enter the quantity of the resource, and indicate what quantity to transfer to an invoice. For more information about invoicing the customer, see [Invoice Jobs](projects-how-invoice-jobs.md). By comparing the original quantity, remaining quantity, or posted quantity you can quickly review usage information. For information about estimating budgeted values during planning, see [Manage Job Budgets](projects-how-manage-budgets.md).

The following procedures describe how to record actual (budgeted) quantities and costs with job journal. Alternatively you can use purchase documents to record purchase for a job. For more information, see [Manage Job Supplies](projects-how-manage-project-supplies.md).

## To record usage for a job planning line of type Budget

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Jobs**, and then choose the related link.
2. Select the relevant job, and then choose the **Job Planning Lines** action.
3. Select a job planning line of type **Budget** or **Both Budget and Billable** for which you want to record usage.

   > [!NOTE]
   > You can also record usage for a job planning line of type **Billable**. Typically, you use this lines to create invoices, but you can also transfer it to a journal. For more information, see [Invoice Jobs](projects-how-invoice-jobs.md) <!--However, when you do that, a job planning line of type **Budget** is created to match the billable line. For more information, see [Manage Job Budgets](projects-how-manage-budgets.md).-->

4. V poli **Mno??. To Transfer to Journal** field, enter the number that you want to transfer. The default quantity is the value that you enter in the **Quantity** field.

   The **Remaining Quantity** field shows the quantity that remains to complete the job and be transferred to the journal.
5. Choose the **Create Job Journal Lines** action.

   > [!TIP]
   > If you are going to add more job planning lines for this job, wait with this step until you have added all job planning lines.
6. On the **Job Transfer Job Planning Line** page, fill in the fields as necessary, and then choose the **OK** button. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
7. Choose the **Open Job Journal** action.
8. On the **Job Journal** page, select the relevant line and then choose the **Post** action.
9. On the **Job Planning Lines** page, review the recorded usage by observing the **Quantity**, **Remaining Quantity**, and **Qty. To Transfer to Journal** fields.
10. Repeat steps 3 through 8 to record additional usage.

## To create job journal lines manually

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Job Journals**, and then choose the related link.
2. In the **Batch Name** field, choose a relevant job journal batch.
3. On a new line, enter document number, job number, job task number, type, and the quantity of the type being consumed.
4. When the job journal lines are complete, choose the **Post** action.

## N??hled odhad?? vyu??it?? projekt?? a pr??b????n?? ????tov??n??

V jednom kroku m????ete zobrazit vyu??it?? prjekt?? a?? do dokon??en?? projektu. To do so, you use the **Job Calc. Remaining Usage** batch job for all the tasks up to and including the end of a job.

To v??m umo??n?? sledovat a porovn??vat p??vodn?? odhady se skute??n??mi v??sledky a podle pot??eby prov??d??t ??pravy nebo p??id??vat nov?? polo??ky. M????ete nap????klad odhadnout, ??e ??loha vy??aduje 10 hodin a k dne??n??mu dni to trvalo 15 hodin. M????ete p??idat dal????ch p??t hodin do existuj??c??ho ????dku den??ku nebo vytvo??it nov?? ????dek den??ku pro vykazov??n?? t??chto p??ti hodin jako p??es??as, jako jin?? typ pr??ce. Jsou vypo??teny p????slu??n?? n??klady a cena, kdy n??sledn?? m????ete ????tovat v den??ku.

> [!NOTE]  
> Item entries create item ledger entries and reduce the inventory quantity. The **Post Inventory Cost to G/L** batch job transfers the cost from inventory to the general ledger. Zdroje vytv????ej?? polo??ky zdroj??.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Job Journals**, and then choose the related link.
2. Select a relevant job journal, and then choose the **Calc. zb??vaj??c??ho pou??it??**.
3. Na str??nce **V??po??et zb??vaj??c??ho  Remaining Usage** page, enter the document number and posting date that is to be inserted in the journal, and then choose the **OK** button.
4. Aktualizujte den??k s p????padn??mi pot??ebn??mi ??pravami.
5. Choose the **Post**.



## To review planning lines for a job ledger entry

After you have posted job journal lines, you can see the planning lines that are associated with the job journal entries that have been posted.

> [!NOTE]  
> This requires that the **Apply Usage Link** check box has been selected for the job. For more information, see [Set Up Jobs](projects-how-setup-jobs.md).

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Job Journals**, and then choose the related link.
2. Select a relevant job journal, and then choose the **Ledger Entries** action.
3. On the **Job Ledger Entries** page, choose **Show Linked Job Planning Lines** action.

## Viz tak??
[Project Management](projects-manage-projects.md)  
[Finance](finance.md)  
[Purchasing](purchasing-manage-purchasing.md)         
[Sales](sales-manage-sales.md)      
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]
