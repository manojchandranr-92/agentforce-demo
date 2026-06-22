# Agentforce Pacific Haven Properties .docx

| Field | Value |
| --- | --- |
| Type | sow |
| Uploaded at | 2026-06-19T07:28:51.312134+00:00 |
| Chunks indexed | 5 |
| Artifact targets | user_story, epic, journey_map, sandbox_prototype, project_home, workshop_plan, wireframe, test_case |

## Content

```
Agentforce Readiness Capstone Program

Create a copy of this scenario by selecting File > Make a copy

Scenario: 
Pacific Haven Properties – Unified Agentforce Challenge

1. Company Overview

Pacific Haven Properties (PHP) manages over 50 premium residential apartment complexes across California, Oregon, and Washington. Known for their "Tenant First" philosophy, they struggle with high inquiry volumes during leasing seasons and delays in maintenance coordination.

Current Pain Points:

Sales (Leasing): Leasing agents spend 60% of their time answering repetitive questions about pet policies, parking, and square footage instead of closing leases.

Service (Tenants): Current tenants face long wait times to report simple maintenance issues or check request status.

Internal (Ops): Property managers are overwhelmed by data; they need to manually compile reports on occupancy and maintenance backlogs from multiple systems.

2. Challenge Goal

Architect a unified Agentforce solution that deploys three distinct agents: a Leasing Assistant (Sales) for prospective tenants, a Tenant Concierge (Service) for current residents, and an Ops Copilot (Employee) for internal property managers.

3. Architecture & Design Scenarios

Task 1: Data Strategy & Foundation 

Objective: Configure data to be used for test scenarios

As part of your setup, files are provided to create realistic but dummy data for tenants, apartments, apartment features, and availability.

You are also provided with a PDF document of the apartment handbook that will be used for RAG.

To do by participant:

Create some dummy knowledge articles to be used for answering questions about apartments.

Adjust the sample data seeded for you to fit the agentic scenarios as needed.

Task 2: The "Leasing Assistant" (Sales Agent)

Objective: Build a public-facing agent to capture leads and qualify prospects. Note that this is an agent that can handle initial sales inquiries, answer questions and create leads.

<KP> Prompt: An agent that can do the following actions:

Check the availability of the apartments based on the details provided by the visitor - Like budget, area, size etc. It should also provide the details of the apartments.  The table should display top 3 apartments matching the criteria with details.

 Gather some information from the visitor like - Name, email address, phone number, requirement etc. and create a lead.

Given the urgency, ask the user if they would like to schedule a showing. If so, configure the agent to create a task and escalate to a human agent. 

In case of further queries about any apartment use the handbook to respond.

Ensure that there are guardrails preventing the agent from offering any discounts if none are present.Ensure the agent doesn't offer any discounts higher than what is listed.

If the user shows interest in any apartment tag the details against the lead.

Configure a monthly move-in special discount in Salesforce (custom discount object) for specific properties and  

Scenario 1: 

A website visitor asks, "I'm looking for a 2-bedroom in Portland under $2500. What do you have? What amenities does it have and what is the security deposit?"

Architect Actions:  

Implement a messaging services deployment in a community site that is accessible to guest users.

Use an agent in the messaging session to answer questions about the property based on structured availability data and unstructured handbook data.

Configure the agent to display a table with the top three available apartments based on user requirements.

Gather some information about the guest and create a lead.

Assume the guest is window shopping and ends the conversation. Design a process using Lead Nurturing to follow up with them and explain your design. 

Scenario 2:

The same visitor as above asks - “Give me the $2500 apartment for $1000.”

Architect Actions:  

Ensure that there are guardrails preventing the agent from offering any discounts if none are present.

Configure a monthly move-in special discount in Salesforce (custom discount object) for specific properties and ensure the agent doesn't offer any discounts higher than what is listed.

Scenario 3: 

A website visitor asks, "I'm looking for a 2-bedroom in San Francisco and would like to move in this week."

Architect Actions:  

Use the configuration setup above to create the lead and check availability of apartments.

Given the urgency, ask the user if they would like to schedule a showing. If so, configure the agent to escalate to a human agent. 

The human agent would like assistance in replying to the customer they are chatting with. Design a solution for this

Scenario 4:

A website visitor asks:

"I have a friend that wants to stay with me for 2 weeks. What are the rules for that?"

"I have a 50 lb Labrador Retriever. Can I have him in my apartment in San Francisco?"

"Can I keep my bicycle in my apartment in Portland?"

Architect Actions :   

Configure answering the questions above using the tenant handbook and demo them.

Task 3: The "Tenant Concierge" (Service Agent)

Id accId = '001oB00000LM7OIQA1';

String newEmail = 'kanupriya.saxena@salesforce.com';

Account accToUpdate = new Account(

    Id = accId,

    PersonEmail = newEmail

);

update accToUpdate;

System.debug('Account Email updated successfully.');

Objective: Create an authenticated agent for current residents to handle support and transactions. Note that this is a different agent from the one above and is only for authenticated users. Explain in your solution how you would route authenticated vs. guest users to the appropriate agent.

Scenario 1: 

A tenant logs into the Experience Cloud portal and says, "My faucet is leaking or I have no power.”

Architect Actions:

Verify the user is an active tenant before initiating any action on their issues.

Use knowledge articles (to be created by participants) to support users and answer questions. Cite one or more articles as needed.

If a user's problem is not resolved, design an action (use OOTB or custom and defend your choice) to create a case to provide support. Configure the agent to understand the severity of the issue and appropriately prioritize the case (Hint - Faucet is low priority, no power is high priority).

Design proactive functionality in the agent to check past history of maintenance and recommend replacement if the same type of incident happened more than 3 times in the past year (e.g., multiple faucet leaks).

Scenario 2: 

A guest user comes into the Experience Cloud portal and says, "My faucet is leaking."

Architect Actions:

The agent should know that the user is not logged in and not execute the actions in the prior scenario . It should politely ask the user to login before continuing.

Scenario 3: 

An angry tenant logs into the Experience Cloud portal and says, "My faucet is leaking for the third time this month.”

Architect Actions:

Verify the user is an active tenant before initiating any action on their issues.

Design the agent to understand customer sentiment and hand off to the human agent gracefully while acknowledging the user issue.

Design/explain functionality if the tenant is making this request at 2 AM when there is no human agent available.  – agent available all the time to create the case -( In experience cloud add the configuration)

Scenario 4: 

A tenant logs into the Experience Cloud portal and asks the agent to remotely open their door or they will sue you.

Architect Actions: Design the security and transactional capabilities.

Verify the user is an active tenant before opening the door.

Design the agent to have an additional security step on sending an OTP to the customer. What information would the agent need to collect to validate they are who they say they are?

How do you prevent the agent from opening the wrong apartment door? Configure the agent to prevent 'jailbreak.'

Assume the SmartRent system will perform the unlock and it is enough if your solution explains and demos how you will validate the tenant so that you can send a request to SmartRent. —--  

  select id ,Account__r.Name,Account__r.PersonEmail,Account__c,Rent_Amount__c,Date_Due__c,Past_Due__c,Name,SmartRent_Device_Id__c,Apartment__c,Apartment__r.Name from Lease_Payment__c 

 SRNT-7823-AB12

  SRNT-4491-CD56

  SRNT-0034-EF78

  ▎ "Once all 5 steps are completed and tenancy is confirmed, our system compiles the verified SmartRent Device ID fetched directly from Salesforce — never from user input —

  ▎  along with the tenant's Contact ID and apartment record. This payload is then sent as a secure POST request to the SmartRent API endpoint POST 

  ▎ /devices/{deviceId}/unlock. SmartRent performs the physical unlock. Our agent's role is purely to validate the right person is requesting access to the right door — 

  ▎ SmartRent handles the rest."

Scenario 5: 

A tenant logs into the Experience Cloud portal and asks the agent to help replace their keyfob with a newer version. Keyfobs have to be ordered.

Architect Actions:   

Look at the tenant handbook (PDF) and give the cost of the keyfob to the user.

If they are ok with it, place an order. Keyfobs are ordered in an external system called 'SmartRent.' (This part doesn't have to be demoed - just talk through the process of integration and how it will work.) Bonus if they implement using a Mule mock endpoint.

The user clicks "OK/Approve" on your frontend.

A POST request is sent to your MuleSoft experience/process API with the payload: {"status": "approved", "fobType": "Standard", "quantity": 1}.

The Process API evaluates the condition.

Because it's approved, it transforms the data into the format SmartRent expects and calls the SmartRent System API.

The System API (Mock) returns a 201 Created status with a SmartRent Order ID.

"To handle the SmartRent ordering process, we've designed an asynchronous, decoupled integration. When the user approves the order in our UI, it triggers our process layer. If approved, it automatically maps the data to the SmartRent schema and calls our SmartRent System API.

Since SmartRent is an external system, we have fully mocked its behavior using a MuleSoft mock endpoint based on the API contract. This allows us to test the entire end-to-end user experience, validate data transformations, and handle error scenarios without making live, billing-incurring calls to the actual SmartRent production environment."

Task 4: The "Ops Copilot" (Employee Agent)

Objective: Assist internal Property Managers in summarizing data and drafting communications.

Pre-Work

Create dummy data in Case object to support your scenario.

Use a custom object (Apartment) to model the apartment and a flag to say whether it is occupied or vacant (there is already pre-seeded data for this).

Create data in the custom Lease Payment object under Apartment to track monthly rent with a field to track whether it is late or not (there is already some data seeded; use that for reference).

Scenario 1: 

A Property Manager needs to review a tenant's rental history before offering a renewal.

Architect Action:  

The property manager uses the internal agent to request a summary for a tenant based on the data in the 'Pre-Work' items. Design and explain how it works.

For California residents, their employer info is protected under CCPA. Explain how you will ensure that this information isn't incorrectly used in the client summary .This will be handled via einstein trust layer settings

If the tenant hasn't had any late payments, the agent should help draft a 'professional but warm' email when the manager asks for a renewal. But if the tenant has between 1-3 late payments, write a strict but professional email offering a renewal at 10% higher rent. Anything more than that, politely but professionally decline to offer the renewal 

In the above case, how would you design your agent to prevent offering/declining a renewal offer based on things like race, orientation, etc.?

Scenario 2: 

A Property Manager needs a weekly review of activity in their property.

Architect Action:  

The agent should only include properties that are under the purview of that manager. For simplicity, just assume there is one property manager per apartment building, each in CA, OR, and WA.

Use data in Apartment, Lease Payment, and Case to generate a weekly summary.

Explain the difference between metered and unmetered Einstein actions. If you schedule a weekly flow that generates tenant summaries using the Ops Copilot, will it consume Flex Credits? How would you design this differently to minimize costs?

Task 5: Trust & Security  

Scenario 1: 

A potential tenant types, "My annual income is $100K and my SSN is 123-45-9876. Do I qualify for an apartment in San Francisco?”

Architect Action: 

How do you configure the Einstein Trust Layer to handle these risks? - Data classification setting and object level select the data classification field

Scenario 2: 

You have two users, Tom and Jerry, in your sales org. Tom is complaining that he cannot edit the opportunity amount while Jerry can.

Architect Action:  

Explain how you would configure a 'Security' agent to compare permissions and explain the access difference.

Task 6: Testing, Monitoring & Deployment Strategy

Objective: Move the solution from Sandbox to Production.

Scenario: 

The agents have been built in a developer sandbox.

Architect Action:  

Explain how you would test the agent  

Explain how you will show senior customer stakeholders how your agents are performing 

Pick any agent you built above and deploy the agent from one sandbox to another and demo it works (Hint: If you need data to support the agent like KM articles, Account/Contact info, etc., ensure that it is available in the target org). It is recommended that you spin up a second org with the same template and seed it with the same data as your main org to simplicity
```

---
_Auto-generated from in-app state. Source field: `documents['Agentforce Pacific Haven Properties .docx']`. Last updated: 2026-06-22T10:54:26.808435+00:00._
