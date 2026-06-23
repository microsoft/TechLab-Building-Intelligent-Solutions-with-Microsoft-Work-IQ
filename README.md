@lab.Title

**Please enter your own Microsoft alias (without the @microsoft.com) in the field below before starting the lab**. This information is required to correctly associate your activity with your learner record and ensure your completion is accurately captured and reported. For data integrity and compliance reasons, learners may only enter their own alias. After completing the lab, please allow up to five business days for all reporting systems to fully reflect your completion.

@lab.ActivityGroup(aliascapture)

===
## Survey

@lab.ActivityGroup(initialsurvey)

===
# Building Intelligent Solutions with Microsoft Work IQ - Hands-on Lab 
 
**The estimated time to complete this lab is 1 hour.**

**DISCLAIMER**
 
This presentation, demonstration, and demonstration model are for informational purposes only and (1) are not subject to SOC 1 and SOC 2 compliance audits, and (2) are not designed, intended, or made available as a medical device or as a substitute for professional medical advice, diagnosis, treatment or judgment. Microsoft makes no warranties, express or implied, in this presentation, demonstration, and demonstration model. Nothing in this presentation, demonstration, or demonstration model modifies any of the terms and conditions of Microsoft's written and signed agreements. This is not an offer, and applicable terms and the information provided are subject to revision and may be changed at any time by Microsoft.
 
This presentation, demonstration, and demonstration model do not grant you or your organization any license to patents, trademarks, copyrights, or other intellectual property covering the subject matter herein.
 
The information contained in this presentation, demonstration, and demonstration model represents the current view of Microsoft on the issues discussed as of the date of presentation and/or demonstration, for the duration of your access to the demonstration model. Because Microsoft must respond to changing market conditions, it should not be interpreted as a commitment on the part of Microsoft, and Microsoft cannot guarantee the accuracy of any information presented after the date of presentation and/or demonstration or for the duration of your access to the demonstration model.
 
No Microsoft technology, nor any of its component technologies, including the demonstration model, is intended or made available as a substitute for the professional advice, opinion, or judgment of (1) a certified financial services professional, or (2) a certified medical professional. Partners or customers are responsible for ensuring the regulatory compliance of any solution they build using Microsoft technologies.
 
**Copyright**
 
©2026 Microsoft Corporation. All rights reserved. 
 
By using this demo/lab, you agree to the following terms:
 
The technology and functionality described in this demo/lab are provided by Microsoft Corporation for the purposes of obtaining your feedback and providing you with a learning experience. You may only use the demo/lab to evaluate such technology features and functionality and to provide feedback to Microsoft. You may not use it for any other purpose. You may not modify, copy, distribute, transmit, display, perform, reproduce, publish, license, create derivative works from, transfer, or sell this demo/lab or any portion thereof.
 
COPYING OR REPRODUCTION OF THE DEMO/LAB (OR ANY PORTION OF IT) TO ANY OTHER SERVER OR LOCATION FOR FURTHER REPRODUCTION OR REDISTRIBUTION IS EXPRESSLY PROHIBITED.
 
THIS DEMO/LAB PROVIDES CERTAIN SOFTWARE TECHNOLOGY AND PRODUCT FEATURES AND FUNCTIONALITY, INCLUDING POTENTIAL NEW FEATURES AND CONCEPTS, IN A SIMULATED ENVIRONMENT WITHOUT COMPLEX SETUP OR INSTALLATION FOR THE PURPOSE DESCRIBED ABOVE. THE TECHNOLOGY AND CONCEPTS REPRESENTED IN THIS DEMO/LAB MAY NOT REPRESENT FULL FEATURE FUNCTIONALITY AND MAY NOT WORK THE WAY A FINAL VERSION WOULD WORK. WE ALSO MAY NOT RELEASE A FINAL VERSION OF SUCH FEATURES OR CONCEPTS. YOUR EXPERIENCE USING SUCH FEATURES AND FUNCTIONALITY IN A PHYSICAL ENVIRONMENT MAY ALSO BE DIFFERENT.

## Lab: Building Work IQ

### Overview  

This lab demonstrates how **Work IQ** transforms operational disruptions into intelligent, coordinated workplace actions within **Microsoft 365**.  

Using the **Zava Retail** scenario, participants experience how a modern organization evolves from disconnected workflows and manual coordination into a Frontier Organization - one that is human-led and AI-operated.  

Zava operates hundreds of physical stores alongside a rapidly growing **e-commerce** platform. Despite significant investments in operational systems and workplace collaboration tools, store operations teams continue to face critical challenges:  

- Delayed operational response during workforce disruptions  
- Manual coordination across **emails**, **calendars**, and **operational** systems  
- Limited visibility into operational **ownership** and **business impact ** 
- Slow approvals and inconsistent execution across teams  
- No connected workflow between operational insights, decision-making, and execution  

To address these challenges, **Zava's** leadership adopts **Work IQ** to unify workplace context, intelligent coordination, approvals, and operational execution across Microsoft 365.  

Throughout the lab, **Ashley**, a Store Manager, relies on **Work IQ** to coordinate operational workflows when **Robin**, a Store Associate, is unexpectedly out on sick leave. Instead of manually assessing impact and coordinating responses, **Work IQ** analyzes the disruption, recommends actions, routes approvals, and executes workflows across specialized agents and **Microsoft 365** services.  

## Why Work IQ?

After establishing a **unified data foundation** with **Fabric IQ** and building **intelligent agents** with **Foundry IQ**, the final challenge is bringing AI-driven decisions into the **flow of work**.

This is where **Work IQ** becomes essential.

**Work IQ** is the execution layer that brings data insights and AI reasoning directly into **Microsoft 365 workflows**.

While **Fabric IQ** creates business intelligence and **Foundry IQ** enables intelligent agents, **Work IQ** ensures that agents can:

- See the workplace context (emails, Teams, meetings, organizational roles).
- Make decisions grounded in that context.
- Execute actions directly within Microsoft 365 (assign tasks, send messages, update documents).

Building on the trusted insights from **Fabric IQ** and reasoning capabilities from **Foundry IQ**, **Work IQ** transforms AI from a dashboard tool into an active workplace assistant.

Work IQ bridges the final gap in the intelligence lifecycle:

| Layer | Purpose | Example |
|------|--------|--------|
| Data | Unified enterprise data foundation | OneLake, Lakehouse, Eventhouse |
| Intelligence | Business understanding of the data | Fabric IQ Ontology |
| Reasoning | AI agents that analyze and recommend | Foundry IQ Agents |
| Execution | In-flow actions within Microsoft 365 | Work IQ Automation |

Most AI platforms stop at **recommendations and insights**.  
Work IQ moves organizations beyond intelligence into **automated execution and policy learning**.

---

## Business context

**What are the benefits of Work IQ and what do we want to achieve?**

**Work IQ** enables organizations to:

* **Reduce response time** - From hours to minutes by automating decision workflows
* **Improve customer satisfaction** - Proactive notifications and faster issue resolution  
* **Eliminate manual handoffs** - Actions execute automatically across Microsoft 365  
* **Enable predictive operations** - Learn from patterns to prevent future issues  
* **Maintain human oversight** - Critical decisions still require approval  
* **Ensure transparency** - Complete audit trail of all automated actions

---

## Architecture overview: Understanding the Microsoft IQ integration


!IMAGE[xeny6oa6.png](../../media/xeny6oa6.png)

The ideal scenario demonstrates how **Copilot → Work IQ → Foundry IQ → Fabric IQ** work together:

!IMAGE[Scenerio-Demonstration-matched-style.png](../../media/Scenerio-Demonstration-matched-style.png)

**Microsoft IQ responsibilities:**

| IQ Layer | Responsibility | Output |
|----------|---------------|--------|
| **Fabric IQ** | Provides trusted business data and real-time signals | Inventory levels, sales velocity, risk metrics |
| **Foundry IQ** | Reasons over data and recommends intelligent actions | Action recommendations with business context |
| **Work IQ** | Executes approved actions in Microsoft 365 | Tasks assigned, emails sent, documents updated |

---

## The Challenge
Store managers like **Ashley** frequently face unexpected workforce disruptions that can impact daily operations and customer commitments. 

When a team member becomes unavailable, managers often need to: 

- Determine the **operational** **impact** of the absence  

- Identify who can take over **critical** responsibilities  

- Coordinate **schedules** and **workload** adjustments  

- Notify affected **employees** and **stakeholders**  

- Document **decisions** and **approvals**  

These activities are often spread across emails, calendars, operational systems, and documentation tools, creating delays and increasing manual effort. 

**Work IQ** solves this by connecting:

| Layer | What It Does |
|-------|------------|
| **Fabric IQ** | Provides real-time inventory data and risk analysis |
| **Foundry IQ** | Reasons about the risks and recommends actions |
| **Work IQ** | Identifies Ashley in Teams, approves actions, executes in Microsoft 365 |

---

## The Scenario: Managing Workforce Disruptions at Zava

**Ashley** (Store Manager) is managing a busy store during a high-demand operational period. 

She uses **Microsoft 365 Copilot** with Work IQ to:

1. **Ask**: "What are my priorities for today?"

1. **Understand**: Copilot identifies workforce disruptions, operational impact, and scheduling conflicts.

1. **Review**: Copilot recommends actions such as reassignment, notifications, and schedule adjustments.

1. **Approve**: Ashley clicks "Approve" and Work IQ coordinates the workflow.

1. **Execute**: Calendars are updated, notifications are sent, responsibilities are reassigned, and operational policies are documented for future use.

---

## What we're building using Work IQ

In this lab, we extend the **Fabric IQ and Foundry IQ** foundation by introducing **Work IQ execution capabilities**.

The solution demonstrates how AI agents can:

- **Detect risks** using Fabric IQ data.
- **Recommend actions** using Foundry IQ intelligence.
- **Execute workflows** using Work IQ automation.
- **Learn policies** for future prevention.

---

## Personas in this lab

| Persona | Role | Task |
|---------|------|------|
| **Ashley** | Store Manager | Reviews recommendations, approves actions |
| **Ryan** | Store Associate | Receives assigned tasks for stock transfers |
| **Robin** | Store Associate | Receives assigned tasks for stock transfers |
| **Copilot** | AI Assistant | Analyzes risks, recommends actions, executes tasks |

---

## Key concepts

### **Context-aware Copilot**
Copilot understands:
- Who Ashley is (role, responsibilities, reporting structure)  
- Which employees are affected by the disruption  
- What emails, Teams messages, and calendar events are relevant  
- Who needs to be notified regarding reassignment and coverage  

### **Fabric IQ integration**
Copilot queries the Fabric IQ ontology to get:
- Assigned orders and operational ownership  
- Workforce impact metrics  
- Employee workload distribution  
- Operational and fulfilment risks 

### **Work IQ execution**
Approved actions are executed directly in Microsoft 365:
- Update calendars and schedules  
- Send Outlook emails  
- Send Teams notifications  
- Create and update operational documents  
- Record approvals and workflow decisions 

### **Policy learning**
After execution, Copilot learns:
- Which workforce disruptions occur most frequently? 
- What operational impact requires manager approval?  
- Who should be notified automatically during staffing disruptions?  
- Which reassignment patterns are most effective?  

These insights become **automated operational policies** for future workforce disruptions. 

---

## What this section demonstrates

By building the Work IQ layer in this lab, participants learn how organizations move beyond analytics and intelligence into **AI-powered automated execution**.

You'll see how:

- **Fabric IQ** provides trusted business intelligence.
- **Foundry IQ** enables AI agents to reason and recommend.
- **Work IQ** executes actions within Microsoft 365.
- **Policy learning prevents future issues automatically**.

Together, **Microsoft Fabric IQ, Foundry IQ, and Work IQ** create a single platform that connects **data, intelligence, reasoning, and automated execution** across the enterprise.


===
# Exercise 1: Building the Work IQ foundation
A dedicated **Microsoft Fabric** workspace is established to serve as the centralized foundation for all **Fabric IQ** capabilities, enabling seamless integration of data, analytics, and AI-driven insights. A **Lakehouse** will be created in Fabric workspace. 



## Outcome
- Fabric-enabled workspace created  
- Capacity-backed environment configured  
- Workspace ready

In this section of the workshop, you'll sign into the Microsoft Fabric Portal and create a new Fabric workspace.

### Task 1.1: Sign in to Microsoft Fabric

1. Sign in to the lab desktop using **LabUser** and +++@lab.VirtualMachine(Win11-Pro-Base).Password+++.


1. In Microsoft Edge, connect to `https://app.fabric.microsoft.com/home?experience=fabric-developer`  


1. At the Fabric sign in screen, enter the following information:



    | Object | Value |
    | -------- | -------- |
    | Email | `@lab.CloudPortalCredential(Ashley).Username` |
    | TAP | `@lab.CloudPortalCredential(Ashley).AccessToken` |

1. If prompted with "Stay signed in?" select **Yes** and proceed.



    >[!Note] If you receive a message that **You've selected Microsoft Fabric free**, select **Continue**.
	!IMAGE[2m04cjde.png](instructions345319/2m04cjde.png)
At the Fabric free window, create your account pages, enter any information, and select **Get Started**.

>[!Note] You can safely ignore any notifications about Microsoft Fabric (Free) license being assigned.

### Task 1.2: Set up a Fabric workspace

1. You should be able to find a New Workspace tile near the upper-left area of the screen. Select it to open the **Create a workspace** pane on the right side.


   
   !IMAGE[8g82u4mq.png](instructions344992/8g82u4mq.png)

1. In the **Create a workspace** pane, in the **Name** field, enter `workspace@lab.LabInstance.Id`.


   
   !IMAGE[bysvn2ik.png](instructions344992/bysvn2ik.png)
	>[!Note] You can safely ignore any messages about **PREMIUM CAPACITY SETTINGS**.

1. Select **Advanced** and move down to see the License mode. Ensure that **Fabric** is selected.



	!IMAGE[k1mwhjcz.png](instructions344992/k1mwhjcz.png)

1. Next, select the green **Apply** button at the lower left of the **Create a workspace** pane.


   
   !IMAGE[gse1xrsm.png](instructions344992/gse1xrsm.png)

1. On the following page, you may get a pop-up window titled "Introducing task flows (preview)". Select the green **Got it** button.


   
   !IMAGE[hth7guac.png](instructions344992/hth7guac.png)

### Task 1.3: Building a Lakehouse
In this task of the workshop, you'll be creating a Lakehouse.

1. Select the **Workspaces** option and choose the **workspace@lab.LabInstance.Id** workspace.



    !IMAGE[Workspace11.png](instructions345319/Workspace11.png)

1. Select **+ New item** and select `Lakehouse` from the available options.



	!IMAGE[Lakehouse11.png](instructions345319/Lakehouse11.png)      

1. In the **New Lakehouse** dialog, enter `Retail_Lakehouse_@lab.LabInstance.Id` for the **Name**, and ensure the **Lakehouse schemas** option is enabled.


1. Select **Create**.



    ![Lakehouse](instructions344992/LakehouseName.png)

    >[!Note] Wait for the Lakehouse to be successfully provisioned. Once created, the Lakehouse will open automatically.

1. Verify the following components are available:


   - **Tables** section
   - **Files** section

    ![BlankLakehouse](instructions344992/BlankLakehouse.png)

    >[!Note] Both **Tables** and **Files** sections are empty.

1. To upload files, select **...** in the **Files** section. Hover over the **Upload** option and select the **Upload files** option.



    ![FileSelection](instructions344992/FileSelection.png)

1. **Select** the folder icon at the right side to choose a file path.



    !IMAGE[Fileimg.png](../../media/Fileimg.png)

1. To browse the files from your virtual machine, open File Explorer. Select the address bar and enter the path `C:\FabricIQLab\Ontology`.



    !IMAGE[qkfipn1a.png](instructions345319/qkfipn1a.png)

1. Select **all files** from this folder and select **Open** to proceed.


 
 	!IMAGE[file1.png](instructions345319/file1.png)

1. Select **Upload**.


    - **retail_ontology_package.iq** 
    - **fabriciq_ontology_accelerator-0.1.0-py3-none-any.whl**
    - **Zava Black Friday Return Policy**

    ![SelectAllFiles](instructions344992/SelectAllFiles.png)

1. Close the upload window once these files have been uploaded.



    ![CurrentUploads](instructions344992/CurrentUploads.png)

1. Now, the **Files** section of the Lakehouse has all three files. 



    ![LakehouseWithFiles](instructions344992/LakehouseWithFiles.png)

### Task 1.4: Loading data into the Lakehouse
#### Step 1: Import notebook 

1. Navigate to your **Fabric workspace**.


    
    !IMAGE[Workspace11.png](instructions345319/Workspace11.png)

1. On the workspace homepage, select the **Import** option.


1. From the available options, select **Notebook**. 


1. Choose **From this computer** as the source.



    ![Notebookimport](instructions344992/Notebookimport.png)

1. Select **Upload** to import the notebook.



    ![UploadNotebook](instructions344992/UploadNotebook.png)

1. To browse the notebooks from your virtual machine, open File Explorer. Select the address bar, enter the path `C:\FabricIQLab\Notebooks`, then select the **Generate Lakehouse Data** notebook file and select the **Open** button.



     !IMAGE[NBImportNew.png](instructions345319/NBImportNew.png) 

1. After upload, the notebook will be listed in the workspace area.



    !IMAGE[NBImportNew1.png](instructions345319/NBImportNew1.png)

#### Step 2: Execute notebook

1. Click on **Generate Lakehouse Data** notebook from the list.


  
     !IMAGE[Notebook1.png](../../media/Notebook1.png)

1. The notebook will open in a different tab without binding with any datastore (Lakehouse).



    ![NotebookwithoutLakehouse](../../media/NBwoutlakehouse.png)

1. Select **Add data items** and select **From OneLake catalog** to open OneLake areas.



    ![Choosedata](../../media/choosedata.png)

1. Click on the **Filter** option in the **OneLake Catalog**, In the filter pane, select **Lakehouse**, Choose the   **Retail_Lakehouse_@lab.LabInstance.Id** Lakehouse that was created previously and Click on **Add**.




    !IMAGE[SelectLakehouse.png](../../media/SelectLakehouse.png) 

1. Now, the selected **Lakehouse** will be bound with the notebook.



    ![lakehousebind](../../media/lakehousebind.png)

1. Move down to the bottom of the four cells.



	!IMAGE[qh937xi7.png](../../media/qh937xi7.png)

1. In the bottom cell, replace the existing names with the following:



    | Object | Value |
    | -------- | -------- |
    | Ashley | `Ashley-@lab.LabInstance.Id` |
    | Robin | `Robin-@lab.LabInstance.Id` |
    | Ryan | `Ryan-@lab.LabInstance.Id` |

	!IMAGE[r56npfau.png](../../media/r56npfau.png)

1. On the menu bar at the top of the section, select **Run all** to execute all four cells.



    !IMAGE[3zlx1i5h.png](../../media/3zlx1i5h.png)

1. Wait for the execution to complete successfully.



    >[!Note] All cells have **completed** execution once the final cell displays a green check mark. This process may take a **couple of minutes**.
    !IMAGE[jkda78zp.png](../../media/jkda78zp.png)

1. Navigate to the **Lakehouse** that was created earlier and verify that the data is successfully loaded (it should be open in another tab).



    ![LakehouseData](../../media/LHnavigation.png)

1. Go to the **Tables** section and select the three dots (⋯), then select **Refresh** to load all tables under **dbo** schema.



    ![LakehouseData](../../media/tablerefresh.png)

1. Verify that tables are created automatically.


    
    ![LakehouseData](../../media/LakehouseData.png)

1. Click on the **orders** table and observe that the **username** column has been populated with the **usernames** that you added to the notebook before execution.


    !IMAGE[Table order.png](../../media/Table order.png)

### Task 1.5: Create a data agent with a Lakehouse as the data source
In this task, a **Data Agent** will be created in Fabric workspace and linked with the **Lakehouse** data source.

1. Navigate to your **Fabric workspace**.


1. In your Fabric workspace, select the **New item** button in the top command bar.


1. In the **New item** creation pane, in the search bar, enter `Data Agent`.


1. Select the **Data Agent** card in the search results and select it to initiate creation.



    ![DAnavigation](instructions344992/DAnavigation.png)

1. In the **Input a data agent name** field, enter `Retail_DataAgent_@lab.LabInstance.Id`, and select **Create**.



    ![FoundryDataAgent](instructions344992/FoundryDataAgent.png)

    > [!Note] If any message appears, please select **Skip for now**.

    !IMAGE[popup2.png](instructions345319/popup2.png)

1. Once the data agent opens, navigate to the **Data** tab in the Explorer pane, select **Add Data**, and select **Data source**.



    ![datasource](instructions344992/datasource.png)

1. Select the **Retail_Lakehouse_@lab.LabInstance.Id** Lakehouse, then select **Add** and verify that the Lakehouse is successfully attached.



    ![FoundryDataAgentLakehouse](instructions344992/FoundryDataAgentLakehouse.png)

1. Expand **Retail_Lakehouse → schemas → dbo → Tables** and select all tables (carriers, customers, demand_signals, forecasts, inventories, order_lines, orders, product_categories, products, promotions, regions, returns, shipments, stores, warehouses).



    ![FoundryDataAgentLakehouse](instructions344992/LHselection.png)

 > If you are unable to see **tables** after adding the **Lakehouse**, **remove** the Lakehouse from the **data source ** and add it again. 

>[!Note] Ensure all the above tables are selected to enable complete analytical coverage for the Retail data agent.

## Task 1.6: Validate the data agent using natural language queries

1. Click on **Agent instructions** from the **top menu**.



     !IMAGE[Agent inst.png](../../media/Agent inst.png)

1. In the **Agent instructions** section, remove any existing default content present in the instruction box, and enter instructions to provide guidance to control how the agent responds. 



     
    ### Sample agent instructions (copy & paste)

    Copy the following instructions and replace any existing text with them in the **Agent instructions** section:

     
     ```
    **Purpose**
    This data agent is designed to answer analytical and operational retail business questions using governed retail Lakehouse data from Microsoft Fabric.
    The agent uses curated retail tables to provide insights across:
    - sales
    - orders
    - customers
    - products
    - inventory
    - campaigns
    - store performance
    - operational ownership

    The agent should provide business-friendly insights, KPI summaries, revenue analysis, operational trends, and sales representative performance without requiring additional semantic modeling.

    **Planning Rules**
    - Understand the business intent and classify requests into:
    - Sales & Revenue
    - Orders & Fulfillment
    - Customer Insights
    - Product Performance
    - Inventory & Supply Chain
    - Campaign Analysis
    - Regional Performance
    - Sales Representative Performance

    - Identify whether the request requires:
    - Historical analytics
    - Operational insights
    - Revenue impact analysis
    - User ownership analysis
    - Trend analysis
    - KPI summarization

    - Break complex questions into:
    - Data identification
    - Business filtering
    - Metric aggregation
    - Trend evaluation
    - Comparative analysis

    - Always validate:
    - Date filters
    - Region or store filters
    - Product or category filters
    - Sales representative filters
    - Order status filters
    - Revenue and operational KPIs

    **Data Source Usage**
    - Orders
    - orders
    - order analytics
    - order status tracking
    - revenue analysis
    - payment analysis
    - operational ownership
    - order fulfillment insights
    - Customers
    - customers
    - customer behavior
    - customer segmentation
    - purchase patterns
    - customer value analysis
    - Products
    - products
    - product performance
    - category analysis
    - brand trends
    - product contribution analysis
    - Inventory
    - inventory
    - stock availability
    - inventory monitoring
    - fulfillment readiness
    - inventory risk analysis
    - Sales Summary
    - gold_sales_summary
        - sales KPIs
        - revenue trends
        - business performance metrics
    - Customer Summary
    - gold_customer_summary
        - customer insights
        - customer growth trends
        - customer spending analysis
    - Store Performance
    - gold_store_performance
        - store analytics
        - regional performance
        - operational performance metrics
    - Campaigns
    - campaigns
        - promotion analytics
        - campaign effectiveness
        - campaign-driven sales impact

    **Business Terminology Standardization**
    - Revenue = Sum(ord_total_amt)
    - Total Orders = Count(ord_id)
    - Sales Volume = Number of completed or shipped orders
    - Average Order Value = Revenue / Total Orders
    - Inventory Level = Available stock quantity
    - Processing Orders = Orders with processing status
    - Cancelled Orders = Orders with cancelled status
    - Customer Spend = Total purchase amount per customer
    - Sales Representative = username assigned to orders
    - Revenue Impact = Total impacted order amount
    - Fulfillment Impact = Delayed or processing orders affecting operations
    - Representative Leave Impact = All orders assigned to that representative (username), where:
    - Impacted Orders = Count(ord_id) for that username
    - Impacted Revenue = Sum(ord_total_amt) for that username
    - Always equals the representative's Total Orders and Revenue (no status, date, or partial filter applied)

    **Relationship Guidance**
    - orders.cust_id → customers.cust_id
    - orders.product_id → products.product_id
    - inventory.product_id → products.product_id
    - inventory.store_id → stores.store_id

    Use these relationships when generating aggregated insights and operational summaries.

    **Sales Representative Analysis Rules**
    The username column represents the operational owner or sales representative assigned to retail orders.
    The agent should support questions such as:
    - How many orders are assigned to Ashley?
    - What is the total revenue handled by Robin?
    - Show cancelled orders managed by Ryan
    - Which sales representative has the highest sales amount?
    - Compare order performance between Ashley and Robin
    - Which representative has the highest impacted revenue?
    - Show processing orders assigned to Ryan
    - Which representative manages the most completed orders?
    - Show operational impact by sales representative
    - What is the impact of Robin on leave?

    For "impact of <representative> on leave" questions:
    - Always use Representative Leave Impact definition
    - Return Impacted Orders = Count(ord_id) for that username
    - Return Impacted Revenue = Sum(ord_total_amt) for that username
    - Do not apply order status, date, or partial filters
    - Result must match the representative's Total Orders and Total Order Amount

    When analyzing sales representatives:
    -Always include:
    - Total Orders
    - Revenue Impact
    - Order Status Distribution
    - Operational Trends
    - Fulfillment Impact

    - Prefer summarized insights over raw transactional outputs

    **Query Behavior Rules**
    - Prefer aggregated business insights over raw data unless explicitly requested
    - Always:
    - Apply relevant filters
    - Include KPIs
    - Provide summarized insights
    - Include business impact metrics
    - Use business-friendly calculations
    - For ambiguous questions:
    - Ask clarifying questions when required
    - Otherwise provide the best business assumption with explanation
    - When operational impact is requested:
    - Include impacted order count
    - Include impacted revenue
    - Include operational ownership
    - Include order status trends
    - When time-based analysis is requested:
    - Include trends
    - Include comparisons
    - Highlight growth or decline patterns

    **Response Style**
    - Provide:
    - concise executive summaries
    - KPI-driven insights
    - business-friendly explanations
    - operational impact summaries
    - revenue analysis
    - trend highlights
    - Use:
    - bullet points
    - summarized explanations
    - business terminology
    - comparative insights
    - Avoid:
    - raw SQL explanations
    - technical database terminology
    - schema-heavy outputs
    - unnecessary low-level details
    - Highlight:
    - revenue impact
    - operational bottlenecks
    - inventory shortages
    - customer trends
    - campaign effectiveness
    - representative ownership patterns
    - sales and fulfilment risks
 

     ```

1. After entering the instructions, select **Publish**, and then select **Publish** again to save the configuration.



    ![agentpublish](../../media/agentpublish.png)

1. In the pop-up window, click **Publish**.


   !IMAGE[Publish Dagent.png](../../media/Publish Dagent.png)

1. After adding the instructions, select the **close (✕)** icon on the **Agent instructions** tab to exit the window.



    ![agentclosing](../../media/agentclosing.png)

1. Once closed, the main Data Agent interface will be displayed, where you can start querying the agent using natural language.


1. In the query input area, ask questions using natural language, for example:


    
`
       How many orders are assigned to Ashley-@lab.LabInstance.Id and what is the total order amount?
    
`

1. Submit the query and review the response generated by the Data Agent.



    ![agentresponse](../../media/agentrespns.png)

1. Observe how the agent:


   - Interprets the question.  
   - Queries the underlying data using the ontology.  
   - Provides insights in a readable format.  

1. Try multiple queries and refine your questions to explore additional insights.



    `
    How many orders are assigned to Ryan-@lab.LabInstance.Id and what is the total order amount?
    `

    `
    How many orders are assigned to Robin-@lab.LabInstance.Id and what is the total order amount?
	`
>[!Note] **
> - Clear and specific questions provide more accurate results.  
> - Responses may vary depending on how the question is framed.  
> - The Data Agent uses the ontology to translate natural language into meaningful queries.

===
# Exercise 2: Building intelligent agents

## Summary

In this exercise, you'll get a hands-on experience of how Work IQ can transform the experience of store employees at Zava, a fictitious retail company. You'll define Work IQ action logic, integrate it with agents to generate recommendations, and enable human-in-the-loop approval workflows. Work IQ is an important part of Microsoft IQ, along with Foundry IQ and Fabric IQ. Work IQ uses predefined instructions and contextual information (as well as the other IQs such as Foundry and Fabric) to evaluate situations, recommend actions, and determine whether actions should be completed automatically or require manager approval. It's key to note that all three IQs work seamlessly with each other as one offering of Microsoft IQ to help customers achieve their business goals.


## Outcome
- Agent personas are created with clearly defined responsibilities.
- System instructions are configured for role-specific behavior.
- Agent responsibilities are aligned to workflow requirements.
- Foundation is established for coordinated multi-agent execution.

### Task 2.1: Create agent persona and system instructions
Ashley, the store manager begins her day. She simply asks with a prompt "What are my priorities for the day?". AI lets her know that Robin, a Store Associate in her team, is unexpectedly out on sick leave. The absence creates a workflow disruption that affects orders assigned to Robin, schedules, and team responsibilities. To help Ashley respond effectively, Work IQ relies on multiple specialized agents working together to understand the impact of this situation and support decision-making.
In this task, you'll create agent personas and define system instructions that establish the role, responsibilities, and behavior of each agent within the workflow.
- **Inventory-Agent** - Evaluates operational and business impact
- **Communication Agent** - Manages notifications, messaging, and scheduling activities
- **Hierarchy Agent** - Retrieves organizational structure and reporting relationships
- **Summarizer-Agent** - Consolidates findings into actionable insights
- **SOP Agent** - Creates and manages process documentation

**User:** "What are my priorities for today?"

This request initiates the workflow, where agents collaborate to gather context, detect disruptions, and generate an actionable response.

1. Open a new browser tab and connect to your foundry project at `https://ai.azure.com/foundryProject/overview?wsid=/subscriptions/@lab.CloudSubscription.Id/resourceGroups/RG1/providers/Microsoft.CognitiveServices/accounts/foundry-iq-lab-@lab.LabInstance.Id/projects/proj-foundry-iq-lab-@lab.LabInstance.Id&amp;tid=4cfe372a-37a4-44f8-91b2-5faf34253c62`


1. If prompted for credentials, enter the following information:



    | Object | Value |
    | -------- | -------- |
    | User | `@lab.CloudPortalCredential(Ashley).Username` |
    | TAP | `@lab.CloudPortalCredential(Ashley).AccessToken` |

1. If it's not selected by default, select the **proj-foundry-iq-lab-@lab.LabInstance.Id**


1. Ensure that the **New Foundry** toggle switch is **on** at the top of the menu bar, and select **Build** to create agents, deploy models, and build workflows.



	![Step 7 Image](instructions344992/image7.png)

1. On the Microsoft Foundry page, on the left side, select **Agents**.



    ![Select step 1](../../media/image32.png)

1. Select **New agent > Build an agent**. 



    !IMAGE[1byvi19r.png](../../media/1byvi19r.png)

1. Enter `Supervisor-Agent` as Agent name, then select **Create and open playground**.



    !IMAGE[8rs6c6pg.png](../../media/8rs6c6pg.png)

1. Once the agent is created, you'll be redirected to the agent playground page. From the **Model** dropdown list, select **gpt-4.1**  and paste the following instructions in the **Instructions** section.



    ```
    # Supervisor Agent

    ## Role
    You are the **Supervisor Agent**. Read the user's query, infer intent, and route it to exactly **one** specialized agent from the list below.

    ## Agents

    ### Inventory-Agent
    Product availability, stock levels/status, warehouse or store location, stockout risk, proactive/preventive actions to avoid stockouts, recommended actions, and inter-store transfer/rebalancing **recommendations** (operational data only). Also route here when the user asks about the **operational impact of a person's unavailability/leave/absence** on inventory, stock, store/warehouse coverage, or pending transfers (e.g. "what's the impact if Ryan is on leave today", "who covers his stock tasks", "impact of his absence on inventory ops").

    ### Work-IQ-Orchestrator-Agent
    Any task that touches a Work IQ tool - **Calendar, Teams, Mail, SharePoint, OneDrive, Word** Examples: "block Ryan's calendar today", "send a mail to the team", "schedule a meeting", "post on Teams", "update the SOP / standard operating procedure document", "share the policy doc", "summarize the Word file".

    Also route here for:
    - **Personal daily / workday summary queries** that span mail, chat, and calendar - e.g. "what are my priorities for today", "morning briefing", "what's on my plate", "who's out today", "team status".
    - **Executing** a stock/inventory transfer (initiate, confirm, complete, "transfer the stock", "proceed with the transfer", status of an ongoing transfer).
    - **Policy / approval-authority** lookups about inventory or transfers (who can approve, sign-off, SOP, governance, policy document) - these are SharePoint/Word document lookups.

    ## Routing Rules
    - Inventory **data or recommendations** → `Inventory-Agent`.
    - **Impact of a person's unavailability/leave/absence on inventory or operations** → `Inventory-Agent`.
    - Inventory **action execution** (do the transfer) → `Work-IQ-Orchestrator-Agent`.
    - Inventory **policy / who-can-approve** questions (trigger words: `authorized`, `approve`, `approval`, `sign-off`, `permitted`, `policy`, `SOP`, `procedure`, `governance`, `who can`, `who needs to`) → `Work-IQ-Orchestrator-Agent`.
    - Any Work IQ tool task (Calendar, Teams, Mail, SharePoint, OneDrive, Word - including creating, editing, or updating SOP/policy documents) → `Work-IQ-Orchestrator-Agent`.
    - Personal daily summary / priorities / "who's out today" / morning briefing queries → `Work-IQ-Orchestrator-Agent`.
    - Combined data + Work IQ action (e.g. "actions taken after the meeting and current status") → `Work-IQ-Orchestrator-Agent`.

    ## Output
    Return only the agent name as a plain string - no quotes, no extra whitespace, no newline. Example:
    `Inventory-Agent`
    ```
   !IMAGE[SA 1.png](../../media/SA 1.png)

1. By default, **Web Search** is added. **Click** on the three dots and remove it before proceeding.



  
  !IMAGE[Webs.png](../../media/Webs.png)

1. Select **Save**, then select the back arrow (**⬅**) to create additional agents.



    ![Step 5.png](../../media/image36.png)

1. Select **New agent > Build an agent**. 



    !IMAGE[1byvi19r.png](../../media/1byvi19r.png)

1. Enter `Inventory-Agent` as agent name and then select **Create and open playground**.



    !IMAGE[0eyw9xed.png](../../media/0eyw9xed.png)

1. Select **gpt-4.1** from the dropdown list and paste the following instructions in the **Instructions** section.



    ```
     # Inventory Agent

    ## Role
    You answer questions about products, orders, inventory, shipments, stores, warehouses, customers, and the workforce that handles them, including the **operational impact** of events (e.g. a person on leave).

    ## Tool
    You have the **Fabric Data Agent** as a tool. Forward the user's question to it and return its response. Do not invent numbers.

    ## Response shape
    Short, factual, label : value lines. Currency includes the symbol; counts are integers. No prose padding, no tool names, no reasoning steps.
    ```

   !IMAGE[IA 1.png](../../media/IA 1.png)

1. By default, **Web Search** is added. Click on the **three dots** and **remove** it before proceeding.



     !IMAGE[Webs.png](../../media/Webs.png)

1. Under the Tools dropdown,Click on **Add**, then click on **Browse all tools**.



    !IMAGE[image58New.png](../../media/image58New.png)

1. Search for +++**Fabric IQ (OneLake Catalog)**+++ in the search bar, select it, then click on **Add tool**.



    !IMAGE[image59New.png](../../media/image59New.png)

1. Select the **data agent**, then click on **Add tool**.



   !IMAGE[image60New.png](../../media/image60New.png)

1. Review the connected **Fabric IQ (OneLake Catalog)** tool, click on **Save** and click on **⬅**.



    !IMAGE[image61New.png](../../media/image61New.png)

1. Select **New agent > Build an agent**. 



    !IMAGE[1byvi19r.png](../../media/1byvi19r.png)

1. Enter `Hierarchy-Agent` as agent name, then select **Create and open playground**.



    !IMAGE[HACreate1.png](../../media/HACreate1.png)

1. Once the agent is created, you'll be redirected to the agent playground page. From the **Model** dropdown list, select **gpt-4.1**  and paste the following instructions in the **Instructions** section.



    ```
    You are the Hierarchy-Agent.

    Your only job: fetch the signed-in user's organizational hierarchy information from Microsoft Teams (Microsoft Graph) - manager, manager chain, direct reports, and peers - and return it as JSON.

    Output strictly in this JSON format (no extra prose, no markdown fences):

    {
      "hierarchy": {
        "name": "",
        "email": "",
        "role": "",
        "subordinates": [
          {
            "name": "",
            "email": "",
            "role": ""
          }
        ]
      }
    }

    Field mapping (from Microsoft Graph):
    - `hierarchy.name` / `hierarchy.email` / `hierarchy.role` = signed-in user's `displayName` / `mail` (or `userPrincipalName`) / `jobTitle`
    - `hierarchy.subordinates[]` = the user's direct reports, each with `displayName`, `mail`, `jobTitle`

    Rules:
    - Return only the JSON object. No explanations, no commentary, no answering the user's broader question.
    - Use null for any field that is not available, and an empty array for missing lists.
    - Do not fabricate data.
    ```
    
    !IMAGE[HA 1.png](../../media/HA 1.png)

1. By default, **Web Search** is added. Click on the **three dots** and **remove** it before proceeding.


	!IMAGE[Webs.png](../../media/Webs.png)

1. Select **Save**, then select the back arrow (**⬅**) to return.



    ![Step 5.png](../../media/image80.png)

1. Select **New agent > Build an agent**. 



    !IMAGE[1byvi19r.png](../../media/1byvi19r.png)

1. Enter `SOP-Agent` as agent name, then select **Create and open playground**.



    !IMAGE[tsl2aqm2.png](../../media/tsl2aqm2.png)

1. Once the agent is created, you'll be redirected to the agent playground page. From the **Model** dropdown list, select **gpt-4.1** and paste the following instructions in the **Instructions** section.



    ```
        # SOP-Agent

    ## Role

    You are the **SOP-Agent** - a Microsoft Foundry agent operating in ACTION-ONLY mode.

    You execute OneDrive and Word file operations using:
    - Work IQ OneDrive
    - Work IQ Word

    You do not use any other tools.

    Core behavior:
    - Execute only what the user explicitly asks.
    - No conversational replies. No recommendations. No unnecessary explanations.
    - Return concise action confirmations only.

    ---

    ## 1. Operating Rules

    - Capabilities are independent. Never auto-chain unrelated actions.
    - For write/update/delete/share actions: execute only if explicitly authorized by the user.
    - Never ask the user to repeat values already present in context.
    - Never expose raw tool payloads or internal IDs.

    ---

    ## 2. Capability - Create SOP

    **Triggers:** "update the SOP", "add this to the SOP", "make this a SOP", "save as standard operating procedure".

    ### Steps

    1. **Create** a new Word file directly in OneDrive named `Standard Operating Procedure(<SOP ID>).docx` where `<SOP ID>` is the current date in `DD-MM-YYYY` format. Do not locate or read any existing file.
    2. **Compose** content from the current chat context. Never fabricate. If no relevant context exists -> `No recent information available to record as SOP.` Use this structure:


    Standard Operating Procedure (SOP):
    SOP ID: <DD-MM-YYYY>
    Applicability: <Department> Team

    1. Objective -
    2. Standard Workflow - [Step 1] -> [Step 2] -> [Step 3] -> [Step 4]
    3. Step-by-Step
    Step 1:
    Step 2:
    Step 3:
    Step 4:
    4. Notification Template
    Subject:
    To:
    Content:


    3. **Confirm:** success -> `SOP updated: new entry appended to "Standard Operating Procedure(<SOP ID>).docx" in OneDrive. Link: <file URL>` ; failure -> `Failed to update SOP in OneDrive.`

    ### Guardrails
    - Never invent data - reuse only what is already shown in the current chat.
    - SOP creation is an explicit write action; run only when the user asks for it.

    ---

    ## 3. General File Operations

    ### OneDrive
    Use for: personal files, drafts, exported documents, user-owned content, locating the SOP document.

    Capabilities: find files, read files, create documents, upload files, move/copy files, rename files, share files, find SOP file for Work IQ Word updates.

    ### Word (Work IQ Word)
    Use for: reading .docx files located via OneDrive, appending new content to existing Word documents (e.g., SOP entries).

    Rules: Only used in combination with OneDrive Work IQ (to locate the file first). Never overwrite existing document content - append only, unless the user explicitly requests a rewrite.

    ---

    ## 4. Output Rules

    Return concise action confirmations only. Examples:
    - `Document successfully created in OneDrive.`
    - `Couldn't fetch the information at the moment.`

    Do not: explain internal logic, expose raw JSON, expose file IDs, narrate reasoning.

    ---

    ## 5. Guardrails

    - Never fabricate file content.
    - Always read the actual file content before answering questions about a file.
    - Never search unrelated OneDrive folders unless the user explicitly asks.
    - Never overwrite/delete files unless explicitly requested.
    - Prefer concise deterministic execution over reasoning-heavy responses.
    ```

  !IMAGE[SOPA1.png](../../media/SOPA1.png)
>[!Note] ** Read the instructions carefully before pasting them into the agent configuration.

1. By default, **Web Search** is added. Click on the **three dots** and **remove** it before proceeding.


	!IMAGE[Webs.png](../../media/Webs.png)

1. Select **Save**, then select the back arrow (**⬅**) to return.



    ![Step 17.png](../../media/image76.png)

1. Select **New agent > Build an agent**. 



    !IMAGE[1byvi19r.png](../../media/1byvi19r.png)

1. Enter `Communication-Agent` as agent name, then select **Create and open playground**.



    !IMAGE[ykwlonuw.png](../../media/ykwlonuw.png)

1. Once the agent is created, you'll be redirected to the agent playground page. From the **Model** dropdown list, select **gpt-4.1** and paste the following instructions in the **Instructions** section.



    ```
    ## Role

    You are the **Communication-Agent** in a Foundry multi-agent workflow. You handle mail, chat, and calendar actions for the user, and - when asked - assess subordinate availability using the hierarchy provided by the upstream agent.

    ## Tools

    - **Work IQ Mail** - read, search, draft, reply, forward, send mail.
    - **Work IQ Teams** - read presence, search/post/reply in chats and channels.
    - **Work IQ Calendar** - read, search, create, update, cancel, block events; check availability.

    ## Input from upstream agent
    You may receive a hierarchy JSON:
    json
    {
    "hierarchy": {
    "name": "", "email": "", "role": "",
    "subordinates": [ { "name": "", "email": "", "role": "" } ]
    }
    }

    Trust names and emails exactly as provided. Do not re-resolve people.

    ## Intent routing

    Execute only what the user asked for. Do not run unrelated steps.

    - **Direct action** (e.g. "block Ryan's calendar today", "send a mail to X", "message the team"): perform the requested action on the relevant tool only. Do not check presence or scan for leave.

    - **Availability / priorities review** (e.g. "what are my priorities for today", "who's out today", "team status"): run the subordinate availability workflow below.

    - **Read / search** (mail, chat, events): execute the lookup and return results.

    ## Subordinate availability workflow

    Run only when the intent requires it. For each subordinate in `hierarchy.subordinates`, in parallel:

    1. **Teams presence** via their email.

    2. **Teams messages** (last ~7 days) - search their recent messages and chat with the user for leave keywords: `sick`, `unwell`, `OOO`, `out of office`, `on leave`, `PTO`, `vacation`, `WFH`.

    3. **Mail** (last ~7 days) - search mail from them to the user for the same keywords and any auto-reply.

    Mark a person **on leave** if presence is `Out of Office`, an auto-reply is active, or a message explicitly states sick/leave/OOO covering today. Extract the date range when stated; otherwise assume today. Distinguish sick leave, PTO, and WFH from the wording. Prefer the most recent explicit message over stale presence. If nothing is found, treat them as available.

    ## Response shape

    Conversational prose. No headings, tables, tool names, or JSON.

    - Direct actions: confirm in one line (e.g. "Blocked Ryan's calendar for today.").

    - Availability review: one short line per affected person, then "the rest are available." If none are out: "Everyone on your team is available today."

    - Read / search: summarize in 1-3 sentences.

    ## Guardrails

    - **Directive requests** ("block Ryan's calendar today", "send him an email", "cancel the meeting"): execute immediately without asking for confirmation. Do not say "I will block" or "do you want me to" - just perform the action and confirm in one line.

    - Only ask for confirmation if the request is ambiguous or missing required info.

    - Read-only actions execute immediately.

    - Every fact must come from a tool result - never fabricate addresses, dates, attendees, or contents.

    - Never expose tool names, raw payloads, or internal ids.

    - On a tool failure inside the availability workflow, silently skip that signal and continue.

    - If a required input is missing (e.g. no hierarchy for an availability review), ask once and stop.
    ```

    !IMAGE[CA1.png](../../media/CA1.png)

1. By default, **Web Search** is added. Click on the **three dots** and **remove** it before proceeding.


	!IMAGE[Webs.png](../../media/Webs.png)

1. Select **Save**, then select the back arrow (**⬅**) to return.



    ![Step 17.png](../../media/image74.png)

1. Select **New agent > Build an agent**. 



    !IMAGE[1byvi19r.png](../../media/1byvi19r.png)

1. Enter `Summarizer-Agent` as agent name, then select **Create and open playground**.



    !IMAGE[8l4e6ctr.png](../../media/8l4e6ctr.png)  

1. Once the agent is created, you'll be redirected to the agent playground page. From the **Model** dropdown list, select **gpt-4.1** and paste the following instructions in the **Instructions** section.



    ```
        # Summarizer-Agent

    ## Role

    You are the **Summarizer-Agent**. You take output from upstream agents (Communication-Agent, Files-Agent, others) or Workflow and return a clean, structured summary plus context-aware follow-up questions.

    You use **no tools**. You do not fetch, send, or modify anything.

    ---

    # 1. Rules

    * Use only the data provided by upstream agents.
    * Never invent names, emails, numbers, dates, or files.
    * Preserve exact values (names, emails, amounts, times, deadlines).
    * Omit any section with no data.
    * No conversational filler, no reasoning narration, no raw payloads/IDs.

    ---

    # 2. Output Style

    Write the summary as a short, friendly, human-sounding briefing - like a helpful teammate giving a quick update. Use natural sentences and light paragraphs, not headings, tables, or bullet lists.

    Guidelines:

    * Lead with the most important point (who's out, what's at risk, what needs attention today).
    * Weave related facts into the same sentence where it reads naturally .
    * Mention people by name, keep numbers and times exact, and reference files or meetings inline.
    * Keep it to a few sentences - aim for a brief, skimmable paragraph or two.
    * Tone: warm, professional, conversational. No corporate jargon, no bullet dumps, no "Summary:" headers.
    * If multiple unrelated topics are present, separate them with a blank line between short paragraphs.


    ---

    # 3. Suggested Follow-Up

    After the summary, append **exactly one** follow-up question - the single most relevant one given the content. Do not list multiple options.

    Pick the question using this priority order (use the first trigger that applies):

    1. **Employee Unavailability (ALWAYS takes priority)** → If the upstream content mentions in ANY form that a person is unavailable - including but not limited to: leave, on leave, sick leave, out of office, OOO, PTO, vacation, time off, absent, away, not available, unavailable, off today, called in sick, medical leave, personal leave, parental leave, bereavement, or any similar phrasing - you MUST ask exactly:
    **"Would you like to know what is the impact of \<Name> on leave?"**
    - Substitute `\<Name>` with the exact employee name from the upstream content.
    - This rule overrides every other trigger below. If unavailability is mentioned anywhere in the input, stop here and ask this question - do not evaluate triggers 2-4.
    2. **Monetary impact or deadlines at risk** → "Want me to notify the team about the **$\<Total>** at-risk orders?"


    Rules:

    * Substitute real values from the summary - never leave placeholders.
    * Ask only one question. Stop at the first matching trigger in the list above.
    * If no trigger applies, do not append any follow-up.
    * Phrase it naturally as a single sentence on a new line after the summary - no heading, no bullet, no list.

    ---

    # 4. Failure Handling

    * Empty input: `No content received from previous agents to summarize.`
    * Unreadable input: `Couldn't summarize the information at the moment.`
    * Upstream error: surface it verbatim under an `Errors` section.

    ```

    !IMAGE[SA1.png](../../media/SA1.png)

1. By default, **Web Search** is added. Click on the **three dots** and **remove** it before proceeding.


	!IMAGE[Webs.png](../../media/Webs.png)

1. Select **Save**, then select the back arrow (**⬅**) to return.



    ![Step 17.png](../../media/image75.png)

1. Select **New agent > Build an agent**. 



    !IMAGE[1byvi19r.png](../../media/1byvi19r.png)

1. Enter `Work-IQ-Orchestrator-Agent` as agent name, then select **Create and open playground**.



    !IMAGE[3uo6k8pd.png](../../media/3uo6k8pd.png)

1. Once the agent is created, you'll be redirected to the agent playground page. From the **Model** dropdown list, select **gpt-4.1** and paste the following instructions in the **Instructions** section.



    ```
       You are the Work-IQ-Orchestrator-Agent - a lightweight routing agent. Your sole responsibility is to analyze the user's request and forward it to the correct sub-agent. You do not execute any actions yourself.

    Routing Rules

    -> Hierarchy-Agent
    Route here when the user's request involves any of the following tools or intents:
    - Mail (Outlook): Sending, replying to, or drafting mails; notifying stakeholders; distributing MOM via email
    - Calendar: Scheduling, updating, or cancelling meetings/events; checking availability; sending meeting invites
    - Teams: Sending messages or notifications to Teams chats or channels; posting MOM on Teams; tagging team members; checking Teams presence/availability of a person

    -> SOP-Agent
    Route here when the user's request involves any of the following tools or intents:
    - OneDrive: Creating, saving, uploading, or sharing files/documents in OneDrive
    - Word: Generating or editing Word documents; exporting conversation/action summaries as a .docx

    Decision Rules
    - Analyze the user's message and identify which tool(s) are needed.
    - Route to only one sub-agent per turn.
    - "Check availability of <Name/Email>" or "Is <Name> available?" -> route to Hierarchy-Agent only.
    - Any request to send, draft, compose, or forward a mail/email -> ALWAYS route to Hierarchy-Agent.
    - Do not automatically chain agents.
    - Do not respond conversationally. Do not execute any tool calls directly.

    Output Format
    Return ONLY one of the following two values as a plain string with no extra text:
    Hierarchy-Agent
    or
    SOP-Agent

    Never return "Work IQ orchestrator" or any other agent name. Your only valid outputs are "Hierarchy-Agent" or "SOP-Agent".
    ```
    
    !IMAGE[WorkIQ Orch Agent.png](../../media/WorkIQ Orch Agent.png)  

1. By default, **Web Search** is added. Click on the **three dots** and **remove** it before proceeding.


	!IMAGE[Webs.png](../../media/Webs.png)

1. Select **Save**, then select the back arrow (**⬅**) to return.


    ![Step 5.png](../../media/image79.png)

<!-- Multi-agent orchestrator (workflow) and end-to-end validation steps moved to the next exercise. -->

### Task 2.2: Implement agent Tool Calling capabilities
<!-- #### Task 2.2.1: Implement Fabric Data Agent tool Calling capabilities for the Inventory-Agent -->

<!-- 1. Return to the **Fabric browser tab**.

1. Navigate to your **Fabric Workspace**.


1. Select **Retail_DataAgent_@lab.LabInstance.Id**.


1. Look at the **URL** at the top of the **browser** and **copy** the following information into text **boxes** below:



	!IMAGE[dataagent.png](instructions345319/dataagent.png)

	**Workspace ID**  @lab.TextBox(WorkspaceID)

  The Workspace ID is the string that appears between **groups**/ and /**aiskills**. It should look similar to c66e7718-3218-47b4-a6e4-6807a572a3c9

	**Artifact ID**  @lab.TextBox(ArtifactID)

	The Artifact ID is the string that appears between **aiskills**/ **and** ? (do not include the ?). It should look similar to aa8ba4b0-a1fa-42f9-920d-dbdd1043f07a -->
<!-- 

1. Return to the **Microsoft Foundry browser tab**.


1. Select **Inventory-Agent**.



    ![Step 1.png](../../media/image57.png)

1. By default, under Tools on the Playground tab, Web Search is added. Select three dots and then select **remove**.



	!IMAGE[t1n755ob.png](../../media/t1n755ob.png)

1. Under the Tools dropdown,Select **Add**, then select **Browse all tools**.



    ![Step 2.png](../../media/image58.png)

1. Select **Fabric Data Agent**, and then select **Add tool**.



  !IMAGE[qc93aq49.png](instructions345319/qc93aq49.png)

1. On the **Connect to Fabric Data Agent** page, enter the following:



  | Option | Value |
  | -------- | -------- |
  | Connection | **Add a new connection** |
  | Name | `fabriciq_dataagent` |
  | Workspace ID | `@lab.Variable(WorkspaceID)` |
  | Artifact ID | `@lab.Variable(ArtifactID)` |

1. Select **Connect**.



  !IMAGE[5izgg71g.png](instructions345319/5izgg71g.png)

1. Review the connected **Fabric Data Agent** tool, select **Save** and select **⬅**.



    ![Step 8.png](../../media/image61.png)

 -->


#### Task 2.2.1: Implement Work IQ Tool Calling capabilities for the Hierarchy-Agent

Add the following Work IQ tools to the Hierarchy-Agent: 
- Work IQ User.

1. From the Agents list, select **Hierarchy-Agent**.


    ![Step 1.png](../../media/image86.png)

1. Under the Tools dropdown, select **Add**, then select **Browse all tools**.



    ![Step 2.png](../../media/image58.png)

#### Add Work IQ User

1. Select **Catalog**, search for `Work IQ User` in the search bar, then select **Work IQ User**.



    ![Step 3.png](../../media/image87.png)

1. Select **Create**.



    ![Step 4.png](../../media/image85.png)

1. Review the details and select **Connect**.



    ![Step 5.png](../../media/image88.png)

1. Review the connected **Hierarchy-Agent** tool, select **Save** and select **⬅**.



#### Task 2.2.2: Implement Work IQ tool calling capabilities for the Communication-Agent
Add the following Work IQ tools to the Communication Agent: 
- Work IQ Mail
- Work IQ Calendar
- Work IQ Teams

1. From the **Agents** list, select **Communication Agent**.



    ![Step 1.png](../../media/image90.png)

1. Under the **Tools** dropdown menu, select **Add**, then select **Browse all tools**.



    ![Step 2.png](../../media/image58.png)

#### Add Work IQ Mail

1. Select **Catalog**, search for `Work IQ Mail` in the search bar, then select **Work IQ Mail**.



    ![Step 3.png](../../media/image89.png)

1. Select **Create**.



    ![Step 4.png](../../media/image91.png)

1. Review the details and select **Connect**.



    ![Step 5.png](../../media/image92.png)

#### Add Work IQ Teams

1. Under the **Tools** dropdown menu, select **Add**, then select **Browse all tools**. 


1. Select **Catalog**, search for `Work IQ Teams` in the search bar, then select **Work IQ Teams**.



    ![Step 6.png](../../media/image93.png)

1. Select **Create**.



    ![Step 7.png](../../media/image94.png)

1. Review the details and select **Connect**.



    ![Step 8.png](../../media/image95.png)

#### Add Work IQ calendar

1. Under the **Tools** dropdown menu, select **Add**, then select **Browse all tools**. 


1. Select **Catalog**, search for `Work IQ calendar` in the search bar, then select **Work IQ calendar**.



    ![Step 9.png](../../media/image4.png)

1. Select **Create**.



    ![Step 10.png](../../media/image5.png)

1. Review the details and select **Connect**.



    ![Step 11.png](../../media/image6.png)

1. Review the connected **Work IQ Mail**, **Work IQ Teams**, and **Work IQ calendar** tools on the Communication-Agent, select **Save**, then select **⬅**.



    ![Step 12.png](../../media/image96.png)

### Task 2.2.3: Implement Work IQ tool calling capabilities for the SOP-Agent

Add the following Work IQ tools to the SOP-Agent: 
- Work IQ Word
- Work IQ OneDrive

1. From the **Agents** list, select **SOP-Agent**.



    ![Step 1.png](../../media/image97.png)

1. Under the **Tools** dropdown menu, select **Add**, then select **Browse all tools**.



    ![Step 2.png](../../media/image58.png)

#### Add Work IQ Word

1. Select **Catalog**, search for `Work IQ Word` in the search bar, then select **Work IQ Word**.



    ![Step 3.png](../../media/image105.png)

1. Select **Create**.



    ![Step 4.png](../../media/image106.png)

1. Review the details and select **Connect**.



    ![Step 5.png](../../media/image107.png)

#### Add Work IQ OneDrive

1. Under the **Tools** dropdown menu, select **Add**, then select **Browse all tools**. 


1. Select **Catalog**, search for `Work IQ OneDrive` in the search bar, then select **Work IQ OneDrive**.



    ![Step 6.png](../../media/image98.png)

1. Select **Create**.



    ![Step 7.png](../../media/image102.png)

1. Review the details and select **Connect**.



    ![Step 8.png](../../media/image103.png)

1. Review the connected **Work IQ Word** and **Work IQ OneDrive** tools on the SOP-Agent, select **Save**, then select **⬅**.



    ![Step 9.png](../../media/image108.png)

### What we learned

- How to create and configure specialized agents with clear personas and system - instructions aligned to specific workflow responsibilities.
- How to integrate **Fabric Data Agent**, **Work IQ Users**, **Work IQ Mail**, **Work IQ Teams**, **Work IQ Calendar**, **Work IQ Word**, and **Work IQ OneDrive** tools to extend agent capabilities.
- How tool and agent mappings establish the foundation for coordinated multi-agent workflows.
- How these connected agents help Ashley quickly understand disruptions, assess business impact, and reduce manual coordination effort for future too.
- How structured agent interactions create the foundation for intelligent, context-aware decision making.


###  Next exercise

In the next exercise, we'll create a multi-agent workflow that brings together the Supervisor, Inventory, Communication, Hierarchy, Summarizer, and SOP agents configured in this exercise. We'll connect them through the Supervisor-Agent as the orchestrator, publish the workflow as an application, and implement an end-to-end workforce disruption scenario from detecting staffing issues and assessing business impact to coordinating actions, notifications, and approvals, thereby helping Zava achieve its business goals.

===
# Exercise 3: Building workflow for multi-agent orchestration

## Summary

In this exercise, you'll bring together the agents you created in Exercise 2 - **Supervisor-Agent**, **Inventory-Agent**, **Work-IQ-Orchestrator-Agent**, **Hierarchy-Agent**, **Communication-Agent**, **SOP-Agent**, and **Summarizer-Agent** - and wire them into a single multi-agent workflow using the YAML workflow editor in Microsoft Foundry. You'll then publish the workflow as a workflow app and validate the end-to-end **Retail** scenario.

## Outcome

- A blank workflow is created in Microsoft Foundry.
- The multi-agent orchestration is defined via YAML.
- The workflow is saved and published as a workflow app.
- The workflow is ready to execute the end-to-end Retail scenario.


### Task 3.1: Create the multi-agent orchestration workflow

1. Select **Workflows**.



    ![Step 1.png](instructions344992/image62.png)

1. Select **Create** and then select **Blank workflow**.



    ![Step 2.png](instructions344992/image63.png)

1. Select **YAML**.



    ![Step 3.png](instructions344992/image64.png)

1. Replace the existing YAML script with the script below, and select **Save**.





kind: workflow
trigger:
  kind: OnConversationStart
  id: trigger_wf
  actions:
    - kind: InvokeAzureAgent
      id: node-1778248476735
      agent:
        name: Supervisor-Agent
      conversationId: =System.ConversationId
      input:
        messages: =System.LastMessage
      output:
        autoSend: false
        messages: Local.Var3365
    - kind: ConditionGroup
      conditions:
        - condition: =Last(Local.Var3365).Text = "Inventory-Agent"
          actions:
            - kind: InvokeAzureAgent
              id: action-1768237934785
              agent:
                name: Inventory-Agent
              input:
                messages: =System.LastMessage
              output:
                autoSend: false
                messages: Local.Var7934
              conversationId: =System.ConversationId
          id: if-action-1768237712578-ma22fceo
      id: action-1768237712578
      elseActions:
        - kind: InvokeAzureAgent
          id: node-1778248101343
          agent:
            name: Work-IQ-Orchestrator-Agent
          conversationId: =System.ConversationId
          input:
            messages: =System.LastMessage
          output:
            autoSend: false
            messages: Local.Var4471
        - kind: ConditionGroup
          id: action-1778248200000
          conditions:
            - condition: =Last(Local.Var4471).Text = "Hierarchy-Agent"
              id: if-action-1778248200000-0
              actions:
                - kind: InvokeAzureAgent
                  id: node-1779703305903
                  agent:
                    name: Hierarchy-Agent
                  conversationId: =System.ConversationId
                  input:
                    messages: =System.LastMessage
                  output:
                    autoSend: false
                    messages: Local.Var9934
                - kind: InvokeAzureAgent
                  id: action-1778248200100
                  agent:
                    name: Communication-Agent
                  conversationId: =System.ConversationId
                  input:
                    messages: =System.LastMessage
                  output:
                    autoSend: false
            - condition: =Last(Local.Var4471).Text = "SOP-Agent"
              id: if-action-1778248200000-1
              actions:
                - kind: InvokeAzureAgent
                  id: action-1778248200200
                  agent:
                    name: SOP-Agent
                  conversationId: =System.ConversationId
                  input:
                    messages: =System.LastMessage
                  output:
                    autoSend: false
                    messages: Local.Var8202
          elseActions:
            - kind: SendActivity
              activity: Local.Var4471
              id: node-1778749061886
    - kind: InvokeAzureAgent
      id: node-1779705250409
      agent:
        name: Summarizer-Agent
      conversationId: =System.ConversationId
      input:
        messages: =System.LastMessage
      output:
        autoSend: true
    - kind: EndConversation
      id: node-1780903631393
id: ""
name: Microsoft-IQ-Workflow
description: ""

    ![Step 5.png](../../media/image112.png)

>[!Note] Read through the YAML carefully so you understand how the **Supervisor-Agent** routes the user query, how the **Work-IQ-Orchestrator-Agent** further routes Work IQ tool requests to the **Hierarchy-Agent**, **Communication-Agent**, or **SOP-Agent**, and how the **Summarizer-Agent** consolidates the final response.

1. Enter the workflow name as `Microsoft-IQ-Workflow` and select **Save**.



    ![Step 6.png](../../media/image114.png)

1. Inside **Microsoft-IQ-Workflow**, select the **Visualizer**. You'll be directed to the visualization area.



	>[!Note] To see the entire workflow, select the vertical display icon next to the visualizer.
    !IMAGE[buh0rhv6.png](../../media/buh0rhv6.png)
    ![Step 7.png](../../media/image115.png)

### Task 3.2: Simulate Robin's sick leave in Microsoft 365

>[!Note] These steps prepare the environment so the workflow in Exercise 4 can detect Robin's absence through email, Teams, and calendar signals.

1. In Microsoft Edge, Select the ellipsis **(…)** in the upper-right corner, and then select **New InPrivate window**.



	!IMAGE[pvwh8v48.png](../../media/pvwh8v48.png)

1. In the new browser, connect to `https://teams.microsoft.com`


1. Sign in as Robin by using the following:



    | Object | Value |
    | -------- | -------- |
    | Email | `@lab.CloudPortalCredential(Robin).Username` |
    | TAP | `@lab.CloudPortalCredential(Robin).AccessToken` |

    >[!Note] You can safely close any pop-up windows that appear.

1. In the upper-right corner, select your **user profile**, and then select **Set status message**.



    !IMAGE[vdo8ci3s.png](../../media/vdo8ci3s.png)

1. At the bottom of the status message panel, select **Schedule out of office**.



    !IMAGE[s1etc6tt.png](../../media/s1etc6tt.png)

1. Switch on the **Turn on automatic replies** toggle, then paste the following message into the **Out of office message** text box and select **Save**:



    
text
    I'll be taking sick leave for 2 days.
    ```

    !IMAGE[et2b719q.png](../../media/et2b719q.png)

1. Back on the upper-right corner, select your user profile again, select the **Available** status, and then choose **Appear offline**.



    !IMAGE[pzqsxsvj.png](../../media/pzqsxsvj.png)

1. On the left menu, select **Chat**.



	!IMAGE[6uzamvr0.png](../../media/6uzamvr0.png)

1. In the search bar at the top of the screen, search for `@lab.CloudPortalCredential(Ashley).Username`, and then select **Ashley**.


1. Send the following message:



    
text
    Hi Ashley, I will be on sick leave for the next 2 days.
    ```

    !IMAGE[um2om0q1.png](../../media/um2om0q1.png)

1. In the upper left, select the **app launcher** (9 dots), and then select **Outlook**.


     !IMAGE[teams.png](../../media/teams.png)

1. In Outlook, select **New mail**, and compose an email with the following details:


   

    - **To:** `@lab.CloudPortalCredential(Ashley).Username`
    - **Subject:** `Sick Leave for 2 Days`
    - **Body:**

        
text
        Hi Ashley,
        I will be on sick leave for the next 2 days due to health reasons.

        Thanks for your understanding.
        ```

1. Select  **Send**.



    !IMAGE[mcpaof4r.png](../../media/mcpaof4r.png)

1. Once the Teams status, chat message, and email have been sent, close the InPrivate browser and return to the Microsoft Foundry browser tab.



### What we learned

- How to create a blank workflow in Microsoft Foundry and switch to the **YAML editor**.
- How to define a multi-agent orchestration by wiring the Supervisor, Inventory, Work-IQ-Orchestrator, Hierarchy, Communication, SOP, and Summarizer agents together via YAML.
- How to save the workflow as a workflow app.


### Next step

In the next section, you'll **validate** the workflow by running the end-to-end Retail scenario: identifying at-risk SKUs, assessing the operational impact of an unavailable team member, scheduling coverage, and capturing the follow-up actions in the SOP document.

===
# Exercise 4: Executing the end-to-end Retail IQ scenario

## Summary

In this exercise, you'll validate the multi-agent workflow you published in Exercise 3 by running the end-to-end **Retail** scenario through the workflow's built-in **Preview** chat. You'll issue a sequence of business queries and confirm that the **Summarizer-Agent** returns the expected consolidated responses, while the underlying agents (Supervisor, Work-IQ-Orchestrator, Hierarchy, Communication, SOP, and so on) work behind the scenes.

## Outcome

- The published **Microsoft-IQ-Workflow** opened in the workflow editor.
- The **Preview** chat opened alongside the workflow canvas.
- Four end-to-end queries executed against the workflow.
- The **Summarizer-Agent** responses validated against the expected output.
- Side effects validated in **Outlook** (email notification) and **Teams Calendar** (calendar block).
- A **Standard Operating Procedure (SOP)** document generated in **OneDrive**.


### Task 4.1: Open the published workflow in Preview

1. In the upper-right corner of the workflow section, select **Preview**. A **chat panel** opens on the right side of the screen. Use the **Message the agent…** box at the bottom of the panel to enter the queries in the next task.



    ![Step 1.png](../../media/image116.png)

### Task 4.2: Execute the end-to-end stockout risk scenario
>[!Note] ** For each query below, you should consider the **Summarizer-Agent** response as the final output. The intermediate agent node outputs (Supervisor, Work-IQ-Orchestrator, Hierarchy, Communication, SOP) are part of the routing and processing flow and are not the final response shown to the user.

1. In the **Preview** chat, enter the following query and select **Enter**:



    
text
    What are my priorities for today?
    ```

    ![Step 1.png](../../media/image117.png)

    >[!Alert] As the workflow runs, it will prompt you for **approval** multiple times to invoke the underlying tools. Select **Approve**, and then select **Always approve all tools**.
    ![Step 2.png](../../media/image118.png)

1. Once the intermediate agents complete the execution, the **Summarizer-Agent**'s consolidated response will appear in the chat panel.



    ![Step 3.png](../../media/image119.png)

	>[!Alert] If you receive the message **No content received from previous agents** or **encounter any error while chatting with the agent**, please **refresh** the Microsoft Foundry **browser tab** and try running the same prompt again.

	 !IMAGE[IQW.png](../../media/IQW.png)
>[!Note] ** Behind the scenes, the **Supervisor-Agent** routes the request to the **Work-IQ-Orchestrator-Agent**, which delegates to the **Hierarchy-Agent** (uses the **Work IQ Users** tool to identify the current user and their direct reports) and then to the **Communication-Agent** (uses **Work IQ Mail**, **Teams**, and **Calendar** to detect absence notifications and review the day's schedule), before the **Summarizer-Agent** consolidates the findings into the final user-facing response.

1. In the **Preview** chat, enter the following query and select **Enter**:



    
text
    What is the impact of Robin-@lab.LabInstance.Id on leave?
    ```

    ![Step 4.png](../../media/image120.png)
>[!Note] ** As shown in step 2, approve any tool prompts the workflow displays during execution.

    >[!Alert] If you receive the message **No content received from previous agents** or **encounter any error while chatting with the agent**, please **refresh** the Microsoft Foundry **browser tab** and try running the same prompt again.

	 !IMAGE[IQW.png](../../media/IQW.png)

1. Once the intermediate agents complete the execution, the **Summarizer-Agent**'s consolidated response will appear in the chat panel.



    ![Step 5.png](../../media/image121.png)
>[!Note] ** Behind the scenes, the **Supervisor-Agent** routes the request to the **Inventory-Agent**, which uses the **Fabric Data Agent** to query the orders assigned to the absent team member and calculate the financial risk across open, in-progress, and unfulfilled statuses, before the **Summarizer-Agent** consolidates the impact analysis and recommends task reassignment in the final user-facing response.

1. In the **Preview** chat, enter the following query and select **Enter**:



    
text
    Proceed with creating an event with Ryan-@lab.LabInstance.Id calendar for the entire day to handle Robin's work and send him an email notification now.
    ```

    !IMAGE[Picture4.png](../../media/Picture4.png)
>[!Note] ** As shown in step 2, approve any tool prompts the workflow displays during execution.

    >[!Alert] If you receive the message **No content received from previous agents** or **encounter any error while chatting with the agent**, please **refresh** the Microsoft Foundry **browser tab** and try running the same prompt again.

	 !IMAGE[IQW.png](../../media/IQW.png)

1. Once the intermediate agents complete the execution, the **Summarizer-Agent**'s consolidated response will appear in the chat panel.



    ![Step 7.png](../../media/image123.png)
>[!Note] ** Behind the scenes, the **Supervisor-Agent** routes the request to the **Work-IQ-Orchestrator-Agent**, which delegates to the **Hierarchy-Agent** (uses the **Work IQ Users** tool to confirm the target team member's reporting relationship) and then to the **Communication-Agent** (uses **Work IQ Calendar** to review the schedule, prepare the day-long calendar block, and stage the email notification), before the **Summarizer-Agent** consolidates the confirmation in the final user-facing response.

1. Validate the side effects of the previous step:


1. In a new browser tab, go to `https://outlook.com`, and then select **Sign in**.


1. Sign in using the following values:



        | Object | Value |
        | -------- | -------- |
        | Email | `@lab.CloudPortalCredential(Ashley).Username` |
        | TAP | `@lab.CloudPortalCredential(Ashley).AccessToken` |

1. Select **Sent Items**. At the top of the list, you'll see the email sent to **Ryan** regarding covering Robin's work. Select it to open and review the message.



    ![Step 8a.png](../../media/image125.png)

1. In a new browser tab, go to `https://teams.microsoft.com`.


1. In Teams, select the **Calendar** icon on the left-hand menu, then expand the **Team-Ashley-@lab.LabInstance.Id** to display the other team member calendars.



	!IMAGE[lz7ddanl.png](../../media/lz7ddanl.png)

1. Select Ryan's calendar and confirm that it has been blocked for the day.



    ![Step 8b.png](../../media/image124.png)

1. Return to the Microsoft Foundry browser tab, enter the following query and select **Enter**:



    
text
    Create a Standard Operating Procedure SOP. If more than 20 orders are impacted, approval is required; if 20 or fewer orders are impacted, the orders can be auto assigned.
    ```
    ![Step 8b.png](../../media/image128.png)
>[!Note] ** As shown in step 2, approve any tool prompts the workflow displays during execution.

    >[!Alert] If you receive the message **No content received from previous agents** or **encounter any error while chatting with the agent**, please **refresh** the Microsoft Foundry **browser tab** and try running the same prompt again.

	 !IMAGE[IQW.png](../../media/IQW.png)

1. Once the intermediate agents complete the execution, the **Summarizer-Agent**'s consolidated response will appear in the chat panel.



    ![Step 10.png](../../media/image129.png)
>[!Note] ** Behind the scenes, the **Supervisor-Agent** routes the request to the **Work-IQ-Orchestrator-Agent**, which delegates to the **SOP-Agent** (uses **Work IQ Word** and **Work IQ OneDrive** to create a new Standard Operating Procedure document capturing the threshold-based approval rules, policy overview, workflow criteria, and implementation details, then saves it to OneDrive and generates a shareable link), before the **Summarizer-Agent** consolidates the confirmation with the document link in the final user-facing response.

1. Select the **link** provided in the Summarizer-Agent response to open the generated **Standard Operating Procedure** Word document. Review the SOP contents and verify that the document has been saved to your personal **OneDrive**.



    ![Step 11.png](../../media/image130.png)

### What we learned

- How to open a published workflow and launch the **Preview** chat panel in Microsoft Foundry.
- How to run an **end-to-end stockout risk scenario** through the multi-agent workflow using natural-language queries.
- How the **Summarizer-Agent** consolidates intermediate agent outputs into a single, user-facing response.
- How to validate the workflow's real-world side effects across **Outlook** (email notification), **Teams Calendar** (calendar block), and **OneDrive** (generated SOP document).


### Conclusion

You've successfully built and executed an end-to-end multi-agent workflow that combines **Microsoft Fabric** data, **Foundry IQ** knowledge, and Microsoft 365 actions (Outlook, Teams, OneDrive) via **Work IQ** to detect a stockout risk, assess operational impact, schedule coverage, notify stakeholders, and capture the procedure as a reusable SOP - all orchestrated through a single conversational interface.

=== 
>[!Alert] **IMPORTANT:** These labs are hosted on the Skillable platform. Completion data is collected and then exported to Success Factors every Monday. SF require another 1-3 days to process that data. The status for this lab will be visible in Viva and Learning Path next week. 
>
Be sure to select "**Submit**" in the bottom right corner to get credit for completing this lab. 

@lab.ActivityGroup(completionsurvey)

>[!Alert] After answering the survey questions, select **submit** to complete and end the lab. **This is required in order to receive credit for lab completion**.

 

