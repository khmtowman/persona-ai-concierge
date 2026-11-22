# Testing and Validation

## 1. Introduction

This document describes the manual testing and validation performed on Persona AI Concierge.

The purpose of testing was to evaluate whether the publicly accessible AI agent could communicate in Bangla and English, present the supplied salon services accurately, guide customers through appointment preferences, and direct them to the official appointment portal.

Testing focused on observable customer-facing behavior rather than automated software testing or backend integration.

## 2. Testing Objectives

The main objectives were to verify that:

- The published AI agent is accessible without requiring an Agentplace login.
- Customers can start a conversation successfully.
- The agent supports both Bangla and English.
- All four salon service categories are represented.
- The supplied service names are presented correctly.
- Customers can follow the guided appointment-preference workflow.
- The agent handles an unspecified preferred outlet appropriately.
- The agent does not falsely claim appointment availability or confirmation.
- Customers receive the correct official appointment portal link.

## 3. Testing Approach

Testing was conducted manually through the publicly published customer-facing interface.

The following approach was used:

1. Open the public agent URL.
2. Verify that the welcome interface loads.
3. Start conversations in Bangla and English.
4. Explore the service categories and their listed services.
5. Test the guided appointment-preference conversation.
6. Observe how the agent responds to missing information.
7. Verify the appointment portal handoff.
8. Open the agent through an incognito browser to check public accessibility.

No automated test framework, performance-testing suite, or backend integration-testing environment was used.

## 4. Functional Test Cases

| Test ID | Test scenario | Expected behavior | Observed result |
|---|---|---|---|
| TC-01 | Open the public agent URL | Customer-facing interface loads | Passed |
| TC-02 | Start a new conversation | Agent provides a welcome message and accepts input | Passed |
| TC-03 | Interact in Bangla | Agent communicates in Bangla | Passed |
| TC-04 | Interact in English | Agent communicates in English | Passed |
| TC-05 | Explore Facial services | Relevant supplied services are presented | Passed |
| TC-06 | Explore Hair Treatments | Relevant supplied services are presented | Passed |
| TC-07 | Explore Top Haircuts | Relevant supplied services are presented | Passed |
| TC-08 | Explore Makeup services | Relevant supplied services are presented | Passed |
| TC-09 | Select a specific service | Agent recognizes the selected service | Passed |
| TC-10 | Provide an unknown preferred outlet | Agent accepts the response and continues | Passed |
| TC-11 | Provide a preferred appointment date | Agent acknowledges the preference | Passed |
| TC-12 | Provide a preferred appointment time | Agent acknowledges the preference | Passed |
| TC-13 | Review appointment preferences | Agent summarizes the provided information | Passed |
| TC-14 | Continue toward appointment booking | Agent directs the customer to the official portal | Passed |
| TC-15 | Open the public agent in an incognito browser | Agent is accessible without an Agentplace login | Passed |

*Passed indicates that the described behavior was observed during manual testing. It does not imply exhaustive testing across every possible conversation.*

## 5. Bilingual Service Knowledge Validation

The agent was tested in both supported languages.

The supplied knowledge base contains 20 services across four categories.

### Facial

1. Bright Nourishing Facial
2. Oxy CollagenA
3. Persona Special Facial
4. Detoxify Brightening Facial
5. Hydro Transformation Facial

### Hair Treatments

1. Hot Oil Massage
2. Absolute Hair Care
3. Protein
4. Hair Spa
5. Heena

### Top Haircuts

1. Front Layer (U)
2. Long Layer
3. Blunt Cut
4. Persona Special Layer
5. Butterfly

### Makeup

1. Special Party Makeover
2. Bridal Makeover By Kaniz Almas Khan
3. Gorgeous Makeover
4. Hair Do
5. Mehendi

**Validation focus:** The agent should present the supplied service names without inventing additional services.

## 6. Appointment Workflow Validation

A manual conversation was conducted to validate the appointment-preference workflow.

The tested scenario involved a customer requesting a bridal makeover.

The conversation covered:

1. Customer requests a bridal makeover.
2. Agent identifies Bridal Makeover By Kaniz Almas Khan.
3. Customer selects the service.
4. Agent asks for the preferred outlet.
5. Customer responds that they do not know.
6. Agent accepts the missing outlet preference.
7. Customer provides a preferred date: 25 November 2026.
8. Customer provides a preferred time: 4:00 PM.
9. Agent summarizes the collected preferences.
10. Agent directs the customer to the official appointment portal.

### Expected validation outcome

The agent should maintain a natural conversational flow and distinguish between customer preferences and actual booking confirmation.

**Observed outcome:** The guided workflow was completed, including the handling of an unspecified outlet and the final portal handoff.

## 7. Public Accessibility Validation

The published agent was opened through a separate incognito browser session.

The following behaviors were observed:

- The public agent URL opened successfully.
- The welcome interface loaded.
- A conversation could be started.
- The customer did not need to sign in to Agentplace to access the public agent.

This confirmed basic public accessibility at the time of testing.

It does not establish continuous uptime, scalability, or availability under heavy traffic.

## 8. Appointment Portal Handoff Validation

The official appointment portal was opened to inspect the initial customer-facing form.

The initial page displayed fields for:

- Full Name
- Phone Number
- E-Mail

A Next button was also visible.

The agent's responsibility ends at directing customers to this official portal.

No appointment was submitted as part of this testing, and no booking confirmation was obtained.

## 9. Responsible AI and Information Accuracy

The agent was designed to avoid unsupported business claims.

Important validation boundaries include:

- No invented service prices.
- No fabricated ingredients or treatment benefits.
- No unsupported service durations or results.
- No invented outlet names or locations.
- No claims of real-time appointment availability.
- No false appointment confirmations.
- No claims of successful booking submission.

These boundaries are important because the agent is intended to represent a real business to its customers.

## 10. Testing Limitations

The following testing activities were not performed:

| Testing area | Status |
|---|---|
| Automated unit testing | Not performed |
| Automated integration testing | Not performed |
| API and webhook testing | Not applicable to the current implementation |
| Live booking availability testing | Not implemented |
| Actual appointment submission | Not performed |
| Booking confirmation retrieval | Not implemented |
| CRM integration testing | Not implemented |
| Load and stress testing | Not performed |
| Security penetration testing | Not performed |
| Cross-device compatibility testing | Not comprehensively tested |
| Long-term uptime monitoring | Not performed |

These limitations reflect the current scope of the project.

## 11. Overall Testing Outcome

The manual validation demonstrated that the published Persona AI Concierge can:

- Open through its public customer-facing URL.
- Communicate in Bangla and English.
- Present the supplied salon service categories and services.
- Guide customers through a basic appointment-preference workflow.
- Handle an unspecified preferred outlet.
- Summarize customer preferences.
- Direct customers to the official appointment portal.
- Maintain clear boundaries around appointment availability and confirmation.

The project therefore demonstrated its intended customer-facing conversational assistance capabilities within the tested scope.

Further testing would be required before deploying a production system with live booking, CRM, or other business-system integrations.

## 12. Project Links

- **Live AI Agent:** https://lowb4k5vhfca.run.agentplace.io/
- **Official Appointment Portal:** https://appointment.persona.com.bd/
- **GitHub Repository:** https://github.com/khmtowman/persona-ai-concierge

---

*Testing note: Results represent manual observations from the project validation process. They should not be interpreted as a certification of production readiness or comprehensive software quality assurance.*
