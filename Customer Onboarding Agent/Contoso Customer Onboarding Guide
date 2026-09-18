# Contoso USA New Customer Onboarding Guide

## Overview

This guide defines the standard process for onboarding new customers in Business Central for Contoso USA.

---

## Process Summary

When a new customer is created:

1. Determine if customer is US or International
2. Assign salesperson based on rules
3. Set credit limit
4. Set payment terms
5. Assign posting groups
6. Send notification email with Adaptive Card

---

## Salesperson Assignment

### US Customers

- Eastern → Jim Olive (JO)
- Central → Ester Henderson (EH)
- Mountain → Lina Townsend (LT)
- Pacific → Otis Falls (OF)

### International Customers

- All → Robin Bettencourt (RB)

---

## Credit Limits

- US Customers → $25,000
- International Customers → $10,000

---

## Payment Terms

- All customers → NET30

---

## Posting Groups

### Gen. Bus. Posting Group

- US → DOMESTIC
- Europe → EU
- Other → EXPORT

### Customer Posting Group

- All → DOMESTIC

---

## Notification Email

After creation, send email to assigned salesperson.

### Subject

New Customer Assigned for Review: {Customer Name} ({Customer Number})

### Message

Please review the newly created customer record to ensure all information is accurate.

---

## Adaptive Card JSON

```json
{
  "$schema": "http://adaptivecards.io/schemas/adaptive-card.json",
  "type": "AdaptiveCard",
  "version": "1.5",
  "body": [
    {
      "type": "TextBlock",
      "text": "New Customer Assigned for Review",
      "weight": "Bolder",
      "size": "Large"
    },
    {
      "type": "FactSet",
      "facts": [
        { "title": "Customer Name", "value": "${CustomerName}" },
        { "title": "Customer Number", "value": "${CustomerNumber}" },
        { "title": "Country", "value": "${Country}" },
        { "title": "Salesperson", "value": "${SalespersonName}" },
        { "title": "Credit Limit", "value": "${CreditLimit}" },
        { "title": "Payment Terms", "value": "NET30" }
      ]
    }
  ],
  "actions": [
    {
      "type": "Action.OpenUrl",
      "title": "Open Customer",
      "url": "${CustomerLink}"
    }
  ]
}
```

---

## Acceptance Criteria

- Salesperson assigned correctly
- Credit limit applied
- NET30 set
- Posting groups assigned
- Email sent with details and link

