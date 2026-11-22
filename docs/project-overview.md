# Project Overview — Persona AI Concierge

## 1. Introduction

Persona AI Concierge is a bilingual AI-powered customer service and appointment-assistance agent developed for Persona, a beauty and salon business in Bangladesh.

The project was built using Agentplace, with GPT-6 Luna configured as its customer-facing AI model.

The agent provides conversational assistance in Bangla and English, helping customers explore salon services, select their preferred options, communicate appointment preferences, and navigate the official appointment-request process.

This project represents a practical implementation of Agentic AI and AI-assisted application development through a real-world business use case.

## 2. Business Context

Persona offers beauty and salon services across several categories.

The project incorporates four owner-supplied service categories:

- Facial Services
- Hair Treatments
- Top Haircuts
- Makeup Services

Each category contains five listed services, resulting in a knowledge base of 20 supplied service options.

The agent uses this information to help customers navigate the service menu through natural conversation.

## 3. Problem Identification

Customers exploring beauty and salon services may need assistance with:

- Discovering available services.
- Navigating different service categories.
- Identifying their preferred service.
- Communicating appointment preferences.
- Finding the appropriate appointment-request channel.

The project addresses these customer-interaction challenges through a conversational AI interface.

## 4. Project Goals

The primary goals were:

1. Develop a functional AI-powered customer-service agent.
2. Support both Bangla and English conversations.
3. Integrate verified business service information.
4. Provide conversational service discovery.
5. Implement structured appointment-preference collection.
6. Guide customers to the official appointment portal.
7. Maintain accuracy and responsible AI behaviour.
8. Deploy a publicly accessible customer-facing agent.

## 5. Target Users

The primary target users are:

- Existing Persona customers.
- Potential customers exploring salon services.
- Bangla-speaking customers.
- English-speaking customers.
- Customers seeking guidance before submitting an appointment request.

## 6. Core Capabilities

### 6.1 Conversational Customer Support

The agent responds to customer questions and helps them explore the available service menu.

### 6.2 Bilingual Interaction

Customers can communicate in Bangla or English. The agent follows the customer's language.

### 6.3 Service Discovery

The agent presents the four available service categories and their supplied service names.

### 6.4 Appointment Preference Collection

The agent follows a structured conversational workflow:

- Identify the selected service.
- Ask for the preferred outlet, if known.
- Ask for the preferred appointment date.
- Ask for the preferred appointment time.
- Summarize the collected preferences.

### 6.5 Official Booking Portal Handoff

The agent directs customers to:

https://appointment.persona.com.bd/

Customers enter their own contact information and submit their appointment requests through the official portal.

## 7. Responsible AI and Information Accuracy

A key design principle is to prevent unsupported claims.

The agent is instructed not to:

- Invent service prices.
- Assume treatment ingredients or benefits.
- Fabricate outlet information.
- Predict treatment outcomes.
- Claim appointment availability without verification.
- Submit or confirm bookings without an actual authorized booking integration.

Customer-provided appointment dates and times are treated as preferences rather than verified available slots.

## 8. Development Approach

The project followed an iterative AI-assisted development approach.

The main stages were:

1. Business research and requirement identification.
2. Service information collection and organization.
3. Agent configuration and instruction design.
4. Customer-facing conversational workflow development.
5. Bilingual testing and refinement.
6. Appointment handoff testing.
7. Public deployment and accessibility verification.

Agentplace's AI-assisted Builder was used to develop and refine the agent through natural-language instructions.

## 9. Project Scope

The current implementation focuses on customer assistance, service discovery and appointment-request guidance.

It does not currently provide:

- Direct access to Persona's booking database.
- Live appointment availability.
- Automated booking submission.
- Booking-status verification.
- External CRM or calendar synchronization.
- Automated payment processing.

These capabilities would require authorized business-system access and additional integrations.

## 10. Project Outcome

The project resulted in a publicly deployed bilingual AI customer-service and appointment-assistance agent.

The published version was tested in Bangla and English, including service discovery, preference collection and the official booking-portal handoff.

Public accessibility was also verified using an incognito browser session.

## 11. Learning Outcomes

This project provided practical experience in:

- Agentic AI application development.
- Prompt engineering and agent instructions.
- AI-assisted development and vibe coding.
- Business knowledge integration.
- Bilingual conversational design.
- Customer journey and workflow design.
- Responsible AI behaviour.
- Testing and iterative refinement.
- Public AI application deployment.

---

**Project:** Persona AI Concierge  
**Platform:** Agentplace  
**Customer-facing model:** GPT-6 Luna  
**Languages:** Bangla and English  
**Live Demo:** https://lowb4k5vhfca.run.agentplace.io/  
**GitHub:** https://github.com/khmtowman/persona-ai-concierge
