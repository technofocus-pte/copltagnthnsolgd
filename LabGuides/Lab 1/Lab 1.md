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

1. Open Copilot Studio Home Page
   
   **Click or visit:**
   ```
   https://copilotstudio.microsoft.com/environments/4a73a65a-10b9-e7a3-aceb-bb9044566c00/home
   ```
2. **Sign In**
   
   Use your Microsoft admin credentials to log in securely.

3. **Select Region**
   
   When prompted, choose United States as your region, then click Next.
![A screenshot of a computer AI-generated content may be
incorrect.](./media/new1.png)

4. Skip Configuration (if prompted)
   On the configuration screen, click Next and then Skip to proceed without custom setup.
   
![A screenshot of a computer AI-generated content may be
incorrect.](./media/New2.png)

5. Navigate to the Dev One Environment
   Once logged in successfully, look at the top-right corner or the environment selector, and switch to the “Dev one” environment to start building or managing       your agents.
   
![A screenshot of a computer AI-generated content may be
incorrect.](./media/new3.png)

6.  Select **“Create”** 🡪 Choose **New Agent**.
    
![A screenshot of a computer AI-generated content may be
incorrect.](./media/image5.png)

7.  From top right corner of the agent creation window, click on **Skip to configure**.

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image6.png)

8.  Enter **Name, Description and Instruction** of the agent as give
    below and click on **Create** button.

    **Name:** Contoso IT Assistant
    
    **Description:** Create an IT support agent that helps users reset
    passwords, request VPN access, and software installation
    
    **Instructions:**

    1. Create the IT Support Copilot Agent
    
    2. Create Topics for Common IT Issues: Password Reset, Request VPN
    Access, Install Software
    
    3. Add Ticket Logging via Power Automate
    
    4. Add Plugin in Copilot Studio
    
    5. Test the Agent
    
    6. Publish and Deploy
       
![A screenshot of a computer AI-generated content may be
incorrect.](./media/image7.png)

9.  Do the following Agent settings: On overview page of **Contoso IT Assistant**

    - **Enable:** the orchestrator for the agent.
    
    - **Disable** the **Allow the AI to use its own general knowledge**
      option.

10.  After making all necessary settings, click **Save**

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image8.png)

11.  From top right corner of the agent, click on the **Settings**
    button.
    
![A screenshot of a computer AI-generated content may be
incorrect.](./media/image9.png)

12.  Go to Generative AI section, select the Generative AI (Preview), set
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

1.  Navigate to **More menu** option on the left side of the navigation pane, then select Power Apps in Copilot Studio.

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image12.png)

![A screenshot of a sign in AI-generated content may be
incorrect.](./media/image13.png)

2.  click on **Sign in** to log in **Powe Apps** **Dev One** environment using the same Microsft Admin credentials

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image14.png)

## Task 2: Setting Up a Dataverse Table

On the power apps home page, from top select the development
environment. In our case its Dev One (prefered), participant can choose their own
environment.

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image15.png)

1.  From the left navigation bar select **Tables 🡪** click on the **+
New table** menu and then select **Create new tables**.

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image16.png)

2.  Select **Import an Excel file or CSV** option to import an Excel or CSV file from your local system.

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image17.png)

3.  Click on the **Select form device** option and then select **Support
Ticket** excel file from your local system and click **Import.**

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image18.png)

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image19.png)

5. Select the uploaded table and click on **View data** option on top bar to update the table with columns with given column name and column type

Column name: Employee ID

Type: Text

Column name: Employee Name

Type: Text

Column Name: Email Address

Type: Email

Column name: Technical Issue Description

Type: multi line text

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image20.png) // change image 

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

7.  From top right side click on **Save and exit** to save the table.

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
    Record** table. Then click on the **Next** and **Add** button
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

3.  click **Test** on the right hand-side of the topic creation window, and
    click refresh button to view the changes

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image33.png)

## Task 3: Create **Reset Password** topic

1.  Go to **Topics** in the top bar of agents overview page to create the **Resset Password** 
    topic for the agent

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

    Name: Request VPN Access
    Description: Help user to Request VPN Access
    
![A screenshot of a computer AI-generated content may be
incorrect.](./media/image41.png)

4.  Click on **+** sign to add a **Question node** and add a agent
    query: **Enter your Email address**

5.  Set **Identify** as **Email**

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
   click on **+** sign, select **Topic management** from the dropdown > click **Go to another topic** and select **End of converstaion** ndoe

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image47.png)

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image48.png)

## Task 5: Create Install Software Topic

1.  Go to Topics window from agent's overview page 🡪 click **+ Add a topic** 🡪 select **Create from
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

   **Question:** “Choose the application you want to install”

   **Identify as:** Multiple choice options

    **Add options:**
    
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

5.  Click on **+ Add a node** 🡪 select **Add a condition** from the dropdown 

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image55.png)

6.  Set the condition as: **Var1 is equal to Power BI**

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image56.png)

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image57.png)

7.  Set another condition as **Var1 is equal to Zoom**

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image58.png)

8.  If both conditions are not satisfied, then add the **Fallback**
    response for all other conditions

![A screenshot of a chat AI-generated content may be
incorrect.](./media/image59.png)

9.  click on + sign to add a new node, go to **Topic management** 🡪 click **Go to another topic** 🡪 and select
    **Fallback**

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image60.png)

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image61.png)

10. Configure the **Condition 1: Var1 is equal to Poer BI** node:
    
    Click on **+** add a new node sign, select **Send a message** option to add message node and enter the sgent repsonse in the message node as:
    
   **Messgae**: Steps to Install Power BI
   
            1. Go to the Official Site
            Visit: https://powerbi.microsoft.com/desktop
            
            2. Click on ‘Download Free’
            Click the Download Free button and follow the prompts.
            
            3. Install the Downloaded File
            Once the .msi installer downloads, double-click it.

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image62.png)

11. Similarly, add a message node after **Condition 2: Var1 is equal to Zoom** and enter the agent response to install Zoom app

      **Message:** Steps to install Zoom
    
                  1. Visit the Zoom Download Page
                  Go to: https://zoom.us/download
                  
                  2. Choose the Right Version for Your Device
                  For Desktop (Windows/Mac/Linux):
                  Download "Zoom Desktop Client" by clicking the Download button.
                  
                  For Mobile (Android/iOS):
                  Use your device’s app store:
                  
                  Google Play Store for Android
                  
                  App Store for iOS
                  
                  Search for "Zoom Cloud Meetings"
                  
                  3. Download and Install
                  Desktop: Run the downloaded .exe (Windows) or .pkg (Mac) file and follow the on-screen instructions.
                  
                  Mobile: Tap Install (Android) or Get (iOS) and wait for it to complete.
                  
                  4. Launch Zoom
                  Open Zoom from your Start Menu, Applications folder, or Home Screen.
                   You can now sign in, join a meeting, or host a meeting.
    
![A screenshot of a computer AI-generated content may be
incorrect.](./media/image63.png)

12. After all the necessary configurations, add **End of conversation** over closing all the conditional nodes:
    
**To add End of conversation node**: click on **+** sign Add a node, select **Topic management** > select **Go to another topic** and, finally select **End of conversation** node 

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image64.png)

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image65.png)

13. click on **Save** button to save the configuration for **Install Softwrae** topic

## Task 6: Add Escalation Topic 

1.  From agent's overview page Create a new topic **From blank**

2. Configure the Escalation topic:
   
  **Name: Talk to IT Support**
  
  **Message:  “You can reach our IT support team**  <br>
   *Email us at: admin@M365x09815490.onmicrosoft.com*
   
 **Trigger phrases: “speak to a person”, “this didn’t help”.**

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image89.png)

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image90.png)

3.  click on **Describe what the topic does** node and enter the trigger phrases:

   - “speak to a person”,
     
   - “this didn’t help”. 

4.  Now, click on **+** sign and select **Send a message** option to add a message node and enter the Message:

    “You can reach our IT support team.
    
    **Email us at:** admin@M365x09815490.onmicrosoft.com”

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image91.png)

![Shape](./media/image3.png)

### Conclusion

By completing this exercise, participants will learn:

1. How to upload and integrate a knowledge base to enhance the bot's
functionality.

2. Steps to customize conversation start messages for a more engaging
user experience.

3. Techniques to update fallback responses for better handling of
unsupported queries.

4. Escalation to human support added 

# Exercise 4: Automating Support Ticket Creation with Power Automate

This exercise demonstrates how to automate support ticket creation using
**Power Automate** and integrate it with the **Contoso IT Assistant**.
Participants will create a flow to streamline issue reporting, record
data in **Dataverse**, and notify support engineers via email.

## Task 1: Create a Flow to Streamline Issue Reporting

1.  Go to **Contoso IT assistant** agent's overview page, naviagte to **Tools** section and click on 
    the **+ Add tool.** button

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image66.png)

2.  In the **Add tool** window, navigate to the **Flows** tab and click on **+ New tool**. From the options, select **Agent flow**. The Power Automate flow configuration window will then open.

![A screenshot of a chat AI-generated content may be
incorrect.](./media/image67.png)

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image68.png)

3.  In Power automate flow, you will see the autogenerated **When an agent calls the flow** trigger. Click on the trigger and configure the parameters:
When an agent calls a flow trigger collects the user input , it sends the collected user inputs to a Power Automate flow. The flow then processes the data (e.g., saves it, sends emails) and can return a response to the agent.

4.  Click on **+ Add input** button from the parameters window

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image69.png)

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image70.png)

5.  Select **Text** as data type of input and rename the input as Name, follow the same and configure the remianing paremters:
   Name: Text
   ID: Text
   Emial: emial
   Details: details

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image71.png)

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image72.png)

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image73.png)

6.  With same procedure create more input as per given details.
   **Input parameter:**
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

7.  After **When an agent calls the flow** action, click on **(+)** sign and
    select **Add a new action**.

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image74.png)

8.  In Add an action search bar, enter **Add a new row** then select
    **Add a new row** from **Microsoft Dataverse** section.
    
The "Add a new row" action in Power Automate inserts data into a selected Dataverse table. You map user inputs from the agent or form to the table columns to store the information.

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image74.png)

9. click on the **Add a new row** trigger box and configure the trigger: search and select the **Table name** from Table name section and configure the advanced parameters for the trigger:
    
   **Table:** Employee technical Support Record
       
   **Advanced parameters:** set up dynamic variables to each input parameter
    
       **Email Address:** /Email
    
       **Technical Support Description:** /Details
    
       **Employee ID:** /ID
    
       **Employee Name:** /Name
       
![A screenshot of a computer AI-generated content may be
incorrect.](./media/image75.png)

10.  Below table name select **Show all**, then click on the particular
    field and add input with the help of dynamic content button (Thunder
    bolt) as per the below given field.
    
    **Advanced Parameters:** set up dynamic variables to each input parameter
    
       **Email Address:** /Email
    
       **Technical Support Description:** /Details
    
       **Employee ID:** /ID
    
       **Employee Name:** /Name
    
**Note:** click on the thunderbolt icon or press / to select the dynamic value

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image76.png)

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image76.png)

11. Below **Add a new row** action, click on **(+)** sign and select **Add an
    action**.

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image76.png)

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image77.png)

12. In add an action section, search **Send an email (V2)** in the search bar
    and select **send an email (V2)** from **office 365 outlook
    section**.

13. To Configure **Send an email** trigger enter the below given detail in the
    respected section:
    
   **To:** Enter support engineer email (MOD Admin)
    
   **Subject:** New Technical Support Ticket Raised
    
   **Body:** Dear HR,

      A new technical support ticket has been raised and requires your attention. Please find details below:
      
      Employee Name: @{triggerBody()?['text']}
      
      Employee ID:  @{triggerBody()?['text_1']}
      
      Technical Issue: @{triggerBody()?['text_3']}
      
      Thank you for your prompt attention to this matter.
      
      Best Regards,
      Contoso IT Support Team
      
14. Now, configure the The **Respond to the agent** action sends data or a confirmation message back to the agent. It lets the agent display a reply to the user after the flow completes.

![A screenshot of a computer AI-generated content may be
incorrect.](./media/agent1.png)

15. click on the **+ Add input** option, select **Text** as the output type in the parameters window and configure it for the given input values 
    
   **Enter Name:** Confirmation Message
   
   **Enter a Value:** Your travel request has been received. Thank you!
   
   **Enter a Decsription:** Acknowledgement!

![A screenshot of a computer AI-generated content may be
incorrect.](./media/agent2.png)

![A screenshot of a computer AI-generated content may be
incorrect.](./media/agent3.png)

16. Click on **Save draft** and **Publish** to save all the action configurations done for the agent flow. 

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image79.png)

17.  Once the agent flow is published navigate to the agent flow overview page and click on Edit button to view the flow details
   
18.  Then, change the flow name as  **LogITTicket** on the
    **Details** page and click **Save** and **Publish**

**Note:** Update the other details such as : **primary owner,
description** and **click Save.**

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image80.png)

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image81.png)

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image82.png)

19. After all the configurations are saved successfully, click on the **Publish** button from top right corner of the agent flow window.

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image83.png)

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image84.png)

## Task 2: Run and test the flow 

1.  Go to **Flows**, select **LogITTicket** Overview page 🡪 click
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

3.  Go to Microsoft Outlook and sign in with the MOD Admin credential and verify the email triggered
    after a successful run of ITLogTicket flow.

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image88.png)

4. Also, open the Dataverse table created in Power Apps and verify the input logged in Employee Technical Support Record table
   
![A screenshot of a computer AI-generated content may be
incorrect.](./media/table.png)

**Note:** your flow is now ready ran successfully.

## Task 3: Test and Publish the Agent 

1.  Use the **Test bot** in Copilot Studio to simulate sample flows. 

![A screenshot of a computer AI-generated content may be
incorrect.](./media/image92.png)

2.  Enter the prompt: Reset password and verify the response

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

4.  Final test demo completed 

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

1. **Trigger** :
A trigger is an event that starts a workflow or process.
In this project, the trigger is initiated when a user submits a travel request form through the Copilot Studio agent. This sends the request data to Power Automate, where the flow begins execution.

Example:

- “When a Power Virtual Agents (Copilot Studio) topic sends a request to Power Automate.”

2.**Tool** :
A tool in Microsoft Copilot Studio refers to external integrations or flows added to an agent topic.
These are typically Power Automate flows that the agent can invoke to perform backend operations like sending an approval email or logging data to SharePoint.

Example:

- “Call a tool” → Select the Power Automate flow named TravelRequestsApprovalFlow to process and log the request.

3. **Action** :
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
