# Copilot Studio Workshop Scratchpad

## New Agent Description:

The purpose of this agent is to assist employees by answering questions related to their own HR benefits, company HR policies, personal HR information, and customer information stored in Business Central. The agent can also retrieve, create, and update customer records in Business Central, as well as answer questions related to expense report policy and check uploaded expense receipts for compliance.

----

## OData Filter examples:

```
email eq 'xyz@abc.com'
tolower(email) eq tolower('xyz@abc.com')
balancedue gt 5500
balancedue lt 5500
contains(username,'ansari')
contains(tolower(username),tolower('ansari')
```

An ODATA filter query that filters employee records by email. If the user's email xyz@abc.com, then the filter is:
```
tolower(email) eq tolower('xyz@abc.com')
```

-----

## Raw proprt to build out Instructions:

I'm building a mega awesome Copilot Studio agent to handle onboarding of a new customer at Contoso USA. When a user creates a new customer from the agent, follow the steps in the Contoso USA New Customer Creation SOP document. Then, send a welcome email to the new customer, and CC the salesperson. Introduce the salesperson to the customer with their name and their contact info (all info from the Salesperson card). Tell the customer about their credit limit, payment terms, how to remit pay Contoso USA (information available the Company Information record in BC). Include our main email, address, website, etc. and invite them to ask any questions. Apply HTML formatting to the email, use tables where appropriate, use formal but cordial language, don't use emojis or emoticons.Then, send a separate email to the salesperson asking if we should offer the customer an introductory Sales Invoice discount with choices of 10, 20, or 30%, and when discount should be valid through (15, 30, or 45 days). When the salesperson replies, implement their recommendation in Business central and let the customer know that you of our welcome discount by email. As for the email sent to the customer with salesperson on CC: if the customer responds, review the email and respond accordinlgnly. If they ask for a change in payment terms, credit limit, etc., and the ask is within 10% of current credit limit or within 15 days of current payment terms, accept their request and reply back that you are able to extend them this couresty. If it excceeds this, forward the request to the salesperson for their thoughts and separatrely reply to the customer acknowledging their request but letting them know this is outside the range of what you can do so you have escalated this for review and approval. Make sure all parties on the email remain on the response as TO or CC. When salesperson replies to this with approval, denial, or alternate offer, implement any changes needed in BC and notify the customer of what you were able to do for them. If we are unable to offer them what they're asking for, be gracious while notifying them. When responding to emails, always use the Reply with All Messages (full thread, and keeping all parties on the email). When forwarding emails, using the Forward tool. Always apply your signature as Contoso New Accounts Agent. For dates, use MM/DD/YYYY formatting, for amounts, add $ sign as prefix. For all numerical values, use thousands and decimal separators with two decimail digits. For nagative numbers, use parantheses. You will create a basic starter instruction set in markdown with general guidelines, and then you will point to the main Onboarding Skill guide which will contain all the above stuff. Lastly, back in the instructions, you will add a section for addendum or overrides to the SOP or this onboarding process. Make both starter and skill as markdown files.

-----

## Prompt to create customer

Create a new customer in BC called Dem Tractors, located at 2455 Eastling Ave, Houston TX 77056. Contact is Ginny Dem, email is ginny@contoso.com, phone is +1-832-605-2134



