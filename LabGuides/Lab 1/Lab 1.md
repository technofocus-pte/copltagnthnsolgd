![link](./media/cover6.1.png)

# Project 1 Lab Guide: Smart IT Helpdesk Agent for Employee Self-Service 

_**Scenario:** Smart IT Helpdesk Agent_ <br>
_**Version**: 25 June, 2025_ <br>
_**Estimated Time:** 120–140 minutes_  <br>
_**Platform:** Microsoft Copilot Studio + Microsoft Teams + Power Automate_ <br>

# Introduction

![A screenshot of a phone AI-generated content may be
incorrect.](./media/image2.png)

The **Contoso IT Assistant** is a virtual support agent built using
Microsoft Copilot Studio. It helps employees quickly resolve common IT
issues, such as password resets, VPN access, software installation, and
connectivity troubleshooting.

Available 24/7 in Microsoft Teams, the assistant empowers users with
self-service options and automates routine support tasks, reducing wait
times and IT workload.

# Objectives

Build a Copilot Studio agent that can: 

1.  Help employees reset passwords 

2.  Request VPN or software access 

3.  Escalate unresolved issues to human IT support 

4.  Be deployed on Microsoft Teams ![Shape](./media/image3.png) 

# Pre-Requisites 

1.  Access to Microsoft Copilot Studio 

2.  A Microsoft 365 tenant with Teams and SharePoint 

3.  Power Automate access with basic flow permissions 

# Architecture Diagram 

![A screenshot of a phone AI-generated content may be
incorrect.](./media/arch.png)

# Key Personas 

**Olivia Chen**
- *Role:* (Not specified)
- *Goals:* Improve ticket response times, reduce manual workload
- *Pain Points:* High number of simple repetitive tickets; SLA breaches

**Diego Morales**
- *Role:* Employee (Sales Division)
- *Goals:* Quickly reset password and request VPN access
- *Pain Points:* Waiting 24–48 hours for basic IT help

**Priya Nair**
- *Role:* IT Business Analyst
- *Goals:* Implement user-friendly IT automation solutions
- *Pain Points:* Poor user experience with current helpdesk portal

**YOU (Learner)**
- *Role:* Agent Developer (Contoso IT Team)
- *Goals:* Build and deploy a smart, scalable, self-service agent
- *Pain Points:* Must balance functionality, governance, and usability


# Step-by-Step Instructions 

# Exercise 1: Creating the Contoso IT Assistant Agent 

This exercise focuses on logging into Microsoft Copilot Studio and
creating a customized Copilot agent tailored for IT support operations
at Contoso. Participants will gain hands-on experience navigating
Copilot Studio, configuring environments, and building an AI-powered
agent to streamline IT workflows.

## Task 1: Creating and Configuring Contoso IT Assistant Agent

1.  Sign in to Microsoft Copilot Studio with Dev One environment

[Home - Microsoft Copilot
Studio](https://copilotstudio.microsoft.com/environments/Default-70d9ca6c-eefa-4403-bcbd-325818744ce2/home)

![](./media/image4.png)

2.  Select **“Create”** 🡪 Choose **New Agent**. 

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image5.png)

3.  From top right corner click on **Skip to configure** button.

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image6.png)

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image7.png)

4.  Enter **Name, Description and Instruction** of the agent as give
    below and click on **Create** button.

    **Name:** Contoso IT Assistant
    
    **Description:** Create an IT support agent that helps users reset
    passwords, request VPN access, and software installation
    
    **Instruction:**

    1. Create the IT Support Copilot Agent
    
    2. Create Topics for Common IT Issues: Password Reset, Request VPN
    Access, Install Software
    
    3. Add Ticket Logging via Power Automate
    
    4. Add Plugin in Copilot Studio
    
    5. Test the Agent
    
    6. Publish and Deploy

5.  Do the following Agent settings: On overview page of **Contoso IT Assistant**

    - **Enable:** the orchestrator for the agent.
    
    - **Disable** the **Allow the AI to use its own general knowledge**
      option.

6.  After making all necessary settings, click **Save**

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image8.png)

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image9.png)

7.  From top right corner of the agent, click on the **Settings**
    button.

8.  Go to Generative AI section, select the Generative AI (Preview), set
    content moderation as **Medium** and click on **Save** to save the
    setting.

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image10.png)

### Conclusion

By completing this exercise, participants will learn:

1. How to access and set up Microsoft Copilot Studio.

2. Steps to create and configure a custom Copilot agent.

3. Practical skills in enabling generative AI and orchestrator settings

**Note:** The agent is now named "Contoso IT Assistant" and is set up to
help users with password resets, VPN access requests, and software
installations.

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image11.png)

# Exercise 2: Getting Started with Power Apps

This exercise introduces participants to Power Apps and Dataverse. The
goal is to log in to Power Apps, set up a working environment, and
create a Dataverse table by importing data from an Excel file.
Participants will learn essential skills for working with data-driven
applications.

## Task 1: Logging into Power Apps

1.  Navigate to **Tools** and select **Power Apps** from Copilot Studio

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image12.png)

![A screenshot of a sign in AI-generated content may be
incorrect.](./media/image13.png)

2.  Click Sign in and provide the Sign in details

3.  Sign in to the **Dev One** environment

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image14.png)

## Task 2: Setting Up a Dataverse Table

On the power apps home page, from top select the development
environment. In our case its Dev One, participant can choose their own
environment.

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image15.png)

2.  From the left navigation bar select **Tables 🡪** click on the **+
New table** and then select **Create new tables**.

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image16.png)

3.  Select **Import an Excel file or CSV** option to create a new
table.

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image17.png)

4.  Click on the select form device option and select **Support
Ticket** excel file from your local system and click **Import.**

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image18.png)

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image19.png)

5.  Select the table and click on **View data** to see the table.

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image20.png)

**Note:** In my case, the table is named **Employee Technical Support
Record**. The name may vary with each execution. Please save the table
name for future reference.

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image21.png)

6.  Go to table data, select **Technical Issue Description down arrow**

    select **Edit column,** set the data type as **Text** -\> Multipl
line of Text -\> **Plain Text** and click on the **Update.**

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image22.png)

7.  From top right side click on **Save and exit**to save the table.

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image23.png)

## Conclusion

By completing this exercise, participants will learn:

1. How to access and navigate Power Apps using admin tenant / work or
  school credentials.

2. Steps to create and configure a Dataverse table by importing data.

3. Practical knowledge of setting up an environment to support app
  development workflows.

# Exercise 2: Enhancing Bot Capabilities

This exercise focuses on enhancing the capabilities of the Contoso IT
Assistant Agent by adding a knowledge base and customizing bot topics
for improved interaction.

## Task 1: Add Knowledge Base to the Agent

1.  On **Contoso agent overview page**, scroll down and click on **+ Add
    Knowledge** button.

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image24.png)

2.  Select **Click to browse** button to add the lab file **Contoso IT
    Support Issue** from Lab Files folder and then click on **Add** to
    save the file.

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image25.png)

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image26.png)

3.  Again, go to agent overview page, scroll down and click on **+ Add
    knowledge.**

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image27.png)

4.  Select **Dataverse (preview)** option as data source.

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image28.png)

5.  In top right corner search bar, enter and search
    for **Employee** and select **Employee Technical Support
    Record** table. Then click on the **Next, Next** and **Add** button
    to add the knowledge source.

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image29.png)

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image30.png)

## Task 2: Customize the Conversation Start Topic

1.  From the top bar option click on **Topics** and then click and
    open **Conversation Start** topic.

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image31.png)

2.  Scroll down and go to message node. Update the message after bot
    name as given below:

    > **Hello! I'm your virtual IT assistant.** I'm here to help you with
    > the following common requests:
    >
    > 🔐 **Reset password**
    >
    > 🌐 **Request VPN access**
    >
    > 💻 **Install software**
    >
    > Please choose an option to get started.

![A screenshot of a chat AI-generated content may be
incorrect.](./media/image32.png)

3.  Navigate to Test agent on the right hand-side of the window and
    click refresh button to view the changes

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image33.png)

## Task 3: Create **Reset Password** topic

1.  Go to **Topics** in the top bar of agents overview page to create
    topics for the agent

2.  Click on **+ Add a topic** 🡪 select **Add from description with
    Copilot** and enter the following details and click **Create.**

    **Name your topic:** Reset password
    
    **Create a topic to:** Instruct user to reset their password

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image34.png)

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image35.png)

3.  Scroll to the message node and update the agent response with the
    given instructions:

    To reset your password, please follow these steps:
    
    - Go to the login page.
    
    - Click on the 'Forgot Password' link.
    
    - Enter your registered email address.
    
    - Check your email for a password reset link.
    
    - Follow the instructions in the email to reset your password.

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image36.png)

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image37.png)

4.  To end the conversation of the specific topic add a conversation
    node: click **+ Add node** -\> go to **Topic management** -\> select
    **Go to another topic** -\> select **End of conversation**.

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image38.png)

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image39.png)

## Task 4: Create Request VPN Access topic

1.  Navigate back to Topics page, click on **+ Add a topic 🡪** select
    **From blank**

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image40.png)

2.  Enter the topic name: **Request VPN Access** and provide the
    description.

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image41.png)

3.  Click on **+** sign to add a **Question node** and add a agent
    query: **Enter your Email address**

4.  Set **Identify** as **Email**

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image42.png)

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image43.png)

5.  Again, click on **+ sign** and add a question node to update the
    agent query:

   **Question:** “Why do you need VPN access?”

6.  Select **Identify** as **Multiple choice options,** click on **+ New
    option** and add following options for the user to select:

    - Remote Desktop
    
    - Team Collaboration

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image44.png)

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image45.png)

7.  Now add the agent response in the **Message node**, click **+ Add a
    node 🡪** select **Message node**

> Message: **Response**: To request VPN access, follow these steps:
>
> **Identify the VPN Requirements**: Determine the specific VPN service
> you need access to and any requirements or prerequisites for access.
>
> **Contact IT Support**: Reach out to your organization's IT support
> team. This can usually be done via email, phone, or through a
> dedicated support portal.
>
> **Provide Necessary Information**: When contacting IT support, include
> the following details:
>
> Your full name and job title.
>
> Your department or team.
>
> The reason for requesting VPN access.
>
> Any specific resources or systems you need to access via the VPN.
>
> **Follow Security Protocols**: Ensure you follow any security
> protocols or guidelines provided by your IT department. This may
> include verifying your identity or completing a security training.
>
> **Wait for Approval**: After submitting your request, wait for
> approval from the IT team. They may need to verify your information
> and ensure you meet the requirements for VPN access.
>
> **Install VPN Software**: Once your request is approved, you will
> receive instructions on how to install and configure the VPN software.
> Follow these instructions carefully.
>
> **Test the VPN Connection**: After installation, test the VPN
> connection to ensure it is working correctly. If you encounter any
> issues, contact IT support for further assistance.

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image46.png)

8.  Add **End of conversation** node 🡪 click **Save**

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image47.png)

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image48.png)

## Task 5: Create Install Software topic

1.  Go to Topics window 🡪 click **+ Add a topic** 🡪 select **Create from
    description with Copilot**

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image40.png)

2.  Enter the following details, and click **Create**

    **Name your topic**: Install Software
    
    **Create a topic to**: Help user to install Zoom and Power BI software
    applications

**Note**: We are limiting the software installation for Zoom and Power
BI applications.

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image49.png)

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image50.png)

**Note**: Delete both the message nodes generated by default, right
click on the **Message** **node** and select **delete**.

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image51.png)

3.  Now, click on **+ Add a node** to add a question node 🡪 enter the
    agent query :

    “Choose the application you want to install”

    Add options:
    
    - Zoom
    
    - Power BI

**Note**: select Identify as Multiple choice options to add options
Power BI and Zoom.

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image52.png)

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image53.png)

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image54.png)

4.  Add a condition node to verify the user response for the given
    options

5.  Click on **+ Add a node** 🡪 select **Add a condition**

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image55.png)

6.  Set the condition as: **Var 1 is equal to Power BI**

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image56.png)

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image57.png)

7.  Set another condition as **Var 1 is equal to Zoom**

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image58.png)

8.  If both conditions are not satisfied, then add the **Escalate**
    response for all other conditions

![A screenshot of a chat AI-generated content may be
incorrect.](./media/image59.png)

9.  Go to **Topic management** 🡪 **Go to another topic** 🡪 and select
    **Fallback**

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image60.png)

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image61.png)

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image62.png)

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image63.png)

10. Add End of conversation over closing all the conditional nodes.

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image64.png)

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image65.png)

### Conclusion

By completing this exercise, participants will learn:

1. How to upload and integrate a knowledge base to enhance the bot's
functionality.

2. Steps to customize conversation start messages for a more engaging
user experience.

3. Techniques to update fallback responses for better handling of
unsupported queries.

# Exercise 4: Automating Support Ticket Creation with Power Automate

This exercise demonstrates how to automate support ticket creation using
**Power Automate** and integrate it with the **Contoso IT Assistant**.
Participants will create a flow to streamline issue reporting, record
data in **Dataverse**, and notify support engineers via email.

## Task 1: Create a Flow to Streamline Issue Reporting

1.  Go to overview page of the agent, scroll down **Tools** and click on
    the **+ Add tool.**

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image66.png)

2.  In a **Add tool** window, navigate to **Flows** tab and click on **+
    New tool** power automate flow window will open.

![A screenshot of a chat AI-generated content may be
incorrect.](./media/image67.png)

3.  Select **Agent** **flow**

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image68.png)

4.  In Power automate flow, click on **When an agent calls the flow**
    and

    then select **Add an Input**

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image69.png)

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image70.png)

5.  Select **Text** as data type of input and rename the input as

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image71.png)


![A screenshot of a computer AI-generated content may be
incorrect.](./media/image72.png)

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image73.png)

5.  With same procedure create more input as per given below details.

    Input type: Name <br>
    Date type: Text
       
    Input type: Email <br>
    Date type: Email
       
    Input type: ID <br>
    Date type: text
       
    Input type: Details <br>
    Date type: Text

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image73.png)

6.  Below **When an agent calls the flow**, click on **(+)** sign and
    select **Add an action**.

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image74.png)

7.  In Add an action search bar, enter **Add a new row** then select
    **Add a new row** from Microsoft Dataverse section.

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image74.png)

8. Configure the **Add a new row** action
9. On **Table Name** section search and select **Employee Technical
    Support Record**.

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image75.png)

9.  Below table name select **Show all**, then click on the particular
    field and add input with the help of dynamic content button (Thunder
    bolt) as per the below given field.

    **Table:** Employee technical Support Record
    
    **Parameters:** set up dynamic variables to each input parameter
    
       **Email Address:** /Email
    
       **Technical Support Description:** /Details
    
       **Employee ID:** /ID
    
       **Employee Name:** /Name

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image76.png)

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image76.png)

10. Below **Add a new row** action click on (+) and select **Add an
    action**.

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image76.png)

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image77.png)

11. In add an action section, enter **Send an email** in the search bar
    and select **send an email (V2)** from **office 365 outlook
    section**.

12. In send an email section, Enter the below given detail in the
    respected section:

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image78.png)

13. Click on **Save draft**

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image79.png)

14. Select the flow created Rename the flow as **ITLogTicket** on the
    **Details** page and click **Save** and **Publish**

**Note:** Update the other details such as : **primary owner,
description** and **click Save.**

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image80.png)

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image81.png)

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image82.png)

15. From top bar right corner click **Publish.**

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image83.png)

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image84.png)

## Task 2: Run and test the flow 

1.  Go to **Flows**, select **ITLogTicket** Overview page 🡪 click
    **Run**

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image85.png)

2.  Enter the Demo input on **Run flow** window and click **Run flow**

    - Name: sadhana
    
    - ID: 102
    
    - Email: MODadmin
    
    - Details: Reset password

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image86.png)

![A screen shot of a computer AI-generated content may be
incorrect.](./media/image87.png)

3.  Open Outlook with the MODadmin Id and verify the email triggered
    after the flow

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image88.png)

**Note:** your flow is now ready ran successfully**.**

## Task 3: Add Escalation Topic 

1.  Create a topic called **Talk to IT Support**. 

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image89.png)

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image90.png)

2.  Add trigger phrases: “speak to a person”, “this didn’t help”. 

3.  Add a Message node to provide the support with contact info:

    “You can reach our IT support team.  
    **Email us at:** admin@M365x09815490.onmicrosoft.com”

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image91.png)

![Shape](./media/image3.png)

## Task 4: Test and Publish the Agent 

1.  Use the **Test bot** in Copilot Studio to simulate sample flows. 

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image92.png)

2.  Ente the prompt: Reset password and verify the response

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image93.png)

3.  Enter the prompt: Request VPN Access and verify the response

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image94.png)

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image95.png)

4.  Click **Publish** and then **Share to Microsoft Teams**. 

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image96.png)

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image97.png)

5.  Go to **Channels** on the top bar and select **Teams** form the list
    of channels

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image98.png)

6.  Select **See agent in teams** on **Teams and Microsoft 365 Copilot
    page**

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image99.png)

7.  Select **Use the web app instead**

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image100.png)

8.  On your Team’s web app, if you don’t see your Copilot agent
    **Contoso IT Assistant**, search for **Contoso IT Assistant** on the
    search bar on top and open the agent listed.

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image101.png)

9.  Start Interacting with the Agent

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image102.png)

![A screenshot of a chat AI-generated content may be
incorrect.](./media/image103.png)

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image104.png)

![Shape](./media/image3.png)

# Submission Checklist 

1.  Agent created and deployed to Teams 

2.  Password reset, VPN, and software request topics configured 

3.  Plugin action integrated with Power Automate 

4.  Escalation to human support added 

5.  Final test demo completed 

![Shape](./media/image3.png)

# Key Learnings and Summary 

This lab guide provided participants with a hands-on experience in
deploying an Autonomous Copilot Agent for Contoso Solutions' IT support
service desk. By following the step-by-step exercises, participants were
able to:

1.  **Set Up Copilot Studio**: Participants learned how to log into
    Copilot Studio, create and configure the IT support agent, and
    enable essential settings like generative AI and orchestrator for
    effective troubleshooting and ticket automation.

2.  **Navigate Power Apps**: Participants gained practical knowledge in
    logging into Power Apps, setting up a Dataverse table, and importing
    data from Excel to track and manage support tickets efficiently.

3.  **Enhance Bot Capabilities**: The exercises focused on adding a
    knowledge base to the bot, customizing the conversation start, End
    of conversation, Fallback, and Escalate topics to improve user
    interaction, and ensuring the bot could handle a wide range of IT
    support scenarios.

4.  **Agent created and deployed to Teams:** participants learned to
    Publish the Agent and share the Agent Contoso IT Assistant for team
    on Teams app for continuous automated IT support.

5.  **Automate IT Support Tasks**: Participants also learned how to
    automate the creation of support tickets using Power Automate,
    enhancing the bot's capability to manage unresolved issues and
    improve IT team workflows.
    
# Key Definitions

1. **Trigger**
A trigger is an event that starts a workflow or process.
In this project, the trigger is initiated when a user submits a travel request form through the Copilot Studio agent. This sends the request data to Power Automate, where the flow begins execution.

Example:

- “When a Power Virtual Agents (Copilot Studio) topic sends a request to Power Automate.”

2.**Tool**
A tool in Microsoft Copilot Studio refers to external integrations or flows added to an agent topic.
These are typically Power Automate flows that the agent can invoke to perform backend operations like sending an approval email or logging data to SharePoint.

Example:

- “Call a tool” → Select the Power Automate flow named TravelRequestsApprovalFlow to process and log the request.

3. **Action**
An action is an individual step within a Power Automate flow that performs a specific function.
Actions execute tasks such as sending an email, creating a SharePoint list item, or posting a Teams message based on data passed from the agent.

Examples of actions in this project:

- “Send an email (V2)” – Notifies the travel approver.
- “Create item” – Stores travel request data in a SharePoint list.
- “Get response details” – Extracts information from the Copilot Studio form submission
  
# Conclusion

By completing these exercises, participants were able to implement a
robust autonomous support system that improves response times, reduces
manual workload, and enhances overall productivity for IT support
operations. The integration of Copilot Studio, Power Apps, and Dataverse
ensures a seamless flow of information, automates routine tasks, and
optimizes support workflows, providing immediate troubleshooting
solutions to employees and automated ticket management for unresolved
issues.
