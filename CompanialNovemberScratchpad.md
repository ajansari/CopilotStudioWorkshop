# Instructions

# Purpose
- You are an agent working for Contoso USA that will work with Business Central data, answering questions about customers, creating customers, providing aged accounts receivable information, emailing the team about customer details, and answering questions about Business Central functionality.

# General Guidelines
- Do not use emojis
- Always show list data as a table
- Always provide citations with your answers

# Process: Show Customer Lists from Business Central
- When showing a list of customers from Business Central, display as a table with just these columns: No., Name, Salesperson Code, Balance Due. Sort the list by descending order of Balance Due, and filter out customers with Balance Due of $0.

---------

# Description for BC documentation Knowledge Source:
This knowledge source is the official documentation for Microsoft Dynamics 365 Business Central on the Microsoft Learn portal.

# Purpose of our agent before lunch
Connect to Business Central
- Be able to pull a list of customers from Business Central
- Create a new customer in Business Central 
- Report on Aged Accounts receivable in Business Central
- Send an email
- Always show a link to the Customer record in Business Central.
- Connect to a knowledge source that is BC documentation

# BC API v2.0 Documentation:
https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/api-reference/v2.0/resources/dynamics_customer

# Prompting Cornerstones
- Task
- Context
- Format
- Persona

# Get URL v3 Description for Customer Deeplink
This tool generates a bookmark (aka Deeplink, Deep Link, or URL) for the desired Customer record in Business Central.

# Improve AI Fill:
This input is to be populated with the SystemId (or id) of the customer record in question.
I want to build an adaptive card v1.5 in Copilot Studio to create a new customer. Have a title in bold: Create Customer. Have the following input fields: Name (text), Salesperson Code (text), Credit Limit (decimal), Address (text). Add a Submit button.
I want this as a JSON payload.

# Article: How to get Page level citations for PDF docs on Knowledge Sources
https://microsoft.github.io/mcscatblog/posts/pdf-page-level-citations/

# Video: How to set up Pay As You Go in Copilot Studio
https://www.youtube.com/watch?v=0cnBT61Hc9c

# Video: How to create Adaptive Cards in Copilot Studio
https://www.youtube.com/watch?v=HvUGUQrpHJQ
https://www.youtube.com/watch?v=RhIlzYHPCXo << Adaptive Card with Dynamic Data (for example, dynamic data in drop down lists)


# My prompt
I want to onboard Customers into Business Central via this agent. This will happen either as a file upload, or as an incoming email (trigger). The process will be in this order:
For each customer:
1. Check if the customer already exists in Business Central by matching the name (match on lower case). If there is an exact match, do not import the customer, but notify the user after all good records as imported. If there is not an exact match but very similar match, ask the user if the record should be imported or not. Otherwise, import the customer (all fields except Contact Name)
2. Check if the customer is US or international
3. Assign salesperson code based on the following rules: US customers: JO (Jim Olive), International customer: OF (Otis Falls)
4. Set credit limit: US customers: $50,000; International: $45,000
5. Assign posting groups: Gen Bus Posting: US: DOMESTIC, International: EU; Customer Posting Group: All: DOMESTIC
6. Update the customer record with the Contact Name.
7. Send a welcome email to the Salesperson and to the Customer Contact.
