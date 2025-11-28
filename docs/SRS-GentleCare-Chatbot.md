Software Requirements Specification (SRS)

Project: GentleCare Dental Clinic – AI Chatbot

Version: 1.0

Date: 2025

Prepared by: Kirti Bhalla

1. Introduction
1.1 Purpose

This Software Requirements Specification (SRS) defines all functional and non-functional requirements for the GentleCare Dental Clinic AI Chatbot.
The chatbot provides clinic information, manages appointments, and supports patients with general dental care guidance.

This SRS is intended for stakeholders, business analysts, developers, and testers.

1.2 Scope

The chatbot is an AI-powered system integrated into the dental clinic’s website to:

Provide clinic hours, services, and FAQs

Book, reschedule, and cancel appointments

Offer general dental care tips

Reduce receptionist workload

Improve patient engagement and availability

The system supports walk-in and phone-based workflows currently handled by a receptionist.

1.3 Definitions
Term	Definition
Chatbot	AI-based conversational interface
Appointment ID	Unique identifier for appointments
User	Patient who interacts with the chatbot
Admin/Receptionist	Clinic staff managing appointments


2. Overall Description

2.1 Product Perspective

The chatbot is an independent module embedded in the clinic’s website via Voiceflow widget.

System Components

Chatbot UI (embedded widget)

AI conversation engine

Voiceflow variable-based appointment storage

Mock backend (future integration)

2.2 Product Functions

Primary Features

Provide clinic information

Appointment booking

Appointment rescheduling

Appointment cancellation

Dental care tips

Support Features

Validate user inputs

Identify user via phone number or appointment ID

Generate appointment confirmations

2.3 User Characteristics
Patients

Basic mobile/computer users

Need appointment/services information

Receptionist/Admin

Uses collected data

No technical skills required

2.4 Constraints

Requires stable internet

Accuracy depends on AI responses

Voiceflow free plan limits storage and data persistence

2.5 Assumptions

Phone number uniquely identifies a user

Users enter correct appointment IDs

Voiceflow components behave reliably

3. System Requirements
   
3.1 Functional Requirements

FR1: Provide Clinic Information

The chatbot must respond to information queries.

Sub-requirements

FR1.1 Provide clinic working hours

FR1.2 Provide list of dental services

FR1.3 Provide clinic address

FR1.4 Provide contact information

FR2: Appointment Booking
Workflow

User selects Book Appointment

Provide name

Provide phone number

Provide preferred date & time

Chatbot checks availability

Appointment is created

Appointment ID is generated

Confirmation message is returned

Requirements

FR2.1 Validate phone number input

FR2.2 Validate time slot

FR2.3 Store appointment details in system

FR2.4 Generate appointment ID

FR3: Appointment Rescheduling
Workflow

User selects Reschedule Appointment

Input Appointment ID

System verifies ID

Ask for new date & time

Confirm reschedule

Requirements

FR3.1 Validate appointment ID

FR3.2 Check new slot availability

FR3.3 Update appointment record

FR4: Appointment Cancellation
Workflow

User chooses Cancel Appointment

Enter Appointment ID

System verifies record

Appointment is deleted

Confirmation message sent

Requirements

FR4.1 Validate appointment ID

FR4.2 Remove appointment data

FR4.3 Return final cancellation message

FR5: Dental Care Tips

FR5.1 Provide general safety tips (non-medical)

FR5.2 Tips must not replace medical advice

FR6: Identity Verification

FR6.1 Verify phone number for bookings

FR6.2 Verify Appointment ID for edit/cancellation

3.2 Non-Functional Requirements
NFR1: Performance

Response time ≤ 2 seconds

Handle ~50 concurrent users (simulated)

NFR2: Usability

Simple conversational flow

Mobile and desktop compatible

Clear instructions and error messages

NFR3: Security

User details stored securely in Voiceflow

No sensitive medical data collected

Avoid sharing personal data unnecessarily

NFR4: Reliability

99% uptime target

Handle invalid inputs gracefully

NFR5: Scalability

Ready for integration with real clinic backend

Support multilingual versions in future

4. System Flow & Diagrams
4.1 High-Level Business Process Flow

(Add link to your flowchart image)

4.2 Sequence Diagram

(Add link to your diagram)

4.3 Use Case Diagram

(Optional — add later if created)

5. Future Enhancements

Integration with actual database

OTP verification for user identity

Payment integration for prepaid appointments

WhatsApp bot compatibility

Admin dashboard with analytics

6. Approval
Role	Name	Signature	Date
Business Analyst	Kirti Bhalla
Product Owner			-
