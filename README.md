SmileBot – AI Chatbot for Dental Clinics (Business Analysis Project)

This repository contains a complete end-to-end Business Analysis case study for the SmileBot AI chatbot built for a dental clinic.

* Project Includes

  1. Problem Statement

  2. Stakeholder Analysis

  3. Business Requirements

  4. Functional & Non-Functional Requirements

  5. AS-IS and TO-BE Process Flows

  6. Use Case Documentation

  7. User Stories with Acceptance Criteria

  8. Wireframes

  9. Chatbot Demo Link & Screenshots

* Purpose

This project demonstrates core business analyst skills, including:requirements gathering, documentation, process modeling, structured thinking,
and communication with stakeholders.

* Chatbot Demo Link

#()

* Status

Documentation is being prepared step by step as part of a full BA  project.

* Tools Used

> GitHub

> Voiceflow

> Draw.io / Excalidraw

> Google Docs / Markdown

* Folder Structure

()

* Created by
Kirti Bhalla


## 12. Feature List

### 1. Customer-Facing Features
- Provide clinic timings, address, and available services.
- Answer FAQs like pricing, procedures, insurance, and doctor availability.
- Assist patients in booking appointments.
- Collect patient details (name, phone, service).
- Confirm or modify appointments.
- Guide walk-in patients on peak hours and waiting time.
- Provide emergency assistance guidance.

### 2. System Logic / Functional Features
- Detect intent: FAQ, appointment, follow-up.
- Slot filling for appointment booking.
- Error handling if user enters invalid data.
- Conditional flows based on clinic hours.
- Provide fallback message when intent not recognized.

### 3. Integration & Backend Features (Current + Future Scope)
- (Current) Fully functional conversation flow built in Voiceflow.
- (Current) Data captured within Voiceflow for demo purposes.
- (Future Scope) API integration to clinic calendar.
- (Future Scope) Auto-confirmation via WhatsApp or SMS.
- (Future Scope) Store appointments in a customer database or CRM.



## 13. Non-Functional Requirements (NFRs)

### 1. Usability
- The chatbot should be easy to use for patients of all age groups.
- Conversations must be simple, clear, and guided.
- The chatbot must provide quick reply options for faster navigation.

### 2. Performance
- Responses should be generated within 1–2 seconds.
- The system should handle multiple users at the same time without crashing.

### 3. Reliability
- The chatbot should maintain consistent responses across all supported platforms.
- All conversation flows should have fallback handling to avoid dead ends.

### 4. Availability
- The chatbot should be available 24/7 for answering patient questions.
- If using website embedding, the bot should load even during high-traffic hours.

### 5. Scalability
- System should support adding new intent categories (e.g., cosmetic dentistry, pediatric dentistry).
- Architecture should allow integration with CRM, website, and appointment calendar in future.

### 6. Security
- The chatbot must not store sensitive customer data without encryption.
- Communication between integrations (future API calls) must use HTTPS.
- Any personally identifiable information collected must follow GDPR/DPDP compliance guidelines.

### 7. Maintainability
- Conversation steps should be modular in Voiceflow for easy updates.
- Documentation should be updated whenever flows change.

### 8. Compatibility
- The chatbot should work across laptop, mobile browsers, and embedded website modes.
- The browser-based demo should run without requiring installation.


## 14. User Stories with Acceptance Criteria

### **User Story 1: View Clinic Information**
As a patient, I want to view basic clinic information so that I know the clinic hours, location, and services.

**Acceptance Criteria**
- Given a patient opens the chatbot, when they ask for clinic hours, then the bot must show correct operational hours.
- When the patient asks for services, the bot must show a list of available dental services.
- When the patient asks for location, the bot should display the clinic address and Google Maps link (if available).

---

### **User Story 2: Book an Appointment**
As a patient, I want to book an appointment so that I can visit the clinic at a suitable time.

**Acceptance Criteria**
- Given a patient chooses “Book Appointment,” the bot must ask for name, phone number, and preferred time.
- Bot must validate the phone number.
- Bot must confirm if the chosen time is available.
- Bot must show a “Booking Confirmed” message with appointment ID.

---

### **User Story 3: Reschedule Appointment**
As a patient, I want to reschedule my existing appointment so that I can come at a more convenient time.

**Acceptance Criteria**
- Bot must ask for appointment ID and phone number.
- If ID is valid, bot allows selection of a new time.
- Bot must update the appointment.
- Bot must send a confirmation message with new appointment details.

---

### **User Story 4: Cancel Appointment**
As a patient, I want to cancel my appointment so that I can free up my schedule.

**Acceptance Criteria**
- Bot must ask for appointment ID and phone number.
- If ID matches existing record, appointment is canceled.
- Bot must display: "Your appointment has been canceled successfully."

---

### **User Story 5: Ask General Dental Care Questions**
As a patient, I want to ask general dental care questions so that I can get instant knowledge without visiting the clinic.

**Acceptance Criteria**
- Bot should answer common queries like brushing tips, tooth pain, post-treatment care.
- If the bot does not understand the query, it must show a fallback message.
- Bot should offer a menu of topics.

---

### **User Story 6: Receptionist Productivity Tracking**
As a clinic manager, I want the chatbot to handle routine questions so that the receptionist is free for high-value tasks.

**Acceptance Criteria**
- Bot should answer at least 60% of FAQs without human help.
- Bot should log conversations for analytics.
- Bot should reduce receptionist query load during peak hours.


## 15. High-Level Process Flow (Business Workflow)

This diagram shows how the patient, chatbot, receptionist, and appointment system interact end-to-end during booking, rescheduling, information queries, or cancellation.

### Actors:
- **Patient**
- **Chatbot (SmileBot)**
- **Receptionist / Clinic Staff**
- **Appointment Management System**

### Process Summary:
1. Patient opens chatbot and selects the required service.
2. Chatbot collects all required information.
3. Chatbot validates inputs.
4. Chatbot processes the request or routes information to the receptionist.
5. Receptionist reviews (if needed) and updates the appointment system.
6. Appointment system confirms booking/reschedule/cancellation.
7. Chatbot sends final confirmation message to the patient.

