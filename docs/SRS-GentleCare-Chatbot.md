Software Requirements Specification (SRS)

Project: GentleCare Dental Clinic – AI Chatbot

Version: 1.0

Date:10/12/2025

Prepared by: Kirti 

1. Introduction
   
   1.1 Purpose

      This Software Requirements Specification (SRS) defines all functional and non-functional requirements        for the GentleCare Dental Clinic AI Chatbot.The chatbot provides clinic information, manages                 appointments, and supports patients with general dental care guidance.This SRS is intended for               stakeholders, business analysts, developers, and testers.

   1.2 Scope

      The chatbot is an AI-powered system integrated into the dental clinic’s website to:

      * Provide clinic hours, services, and FAQs

      * Book, reschedule, and cancel appointments
      
      * Offer general dental care tips

      * Reduce receptionist workload

      * Improve patient engagement and availability

      * The system supports walk-in and phone-based workflows currently handled by a receptionist.

   1.3 Definitions:
   
      Term	Definition:
   
      i. Chatbot:> AI-based conversational interface
   
      ii. Appointment ID:> Unique identifier for appointments
   
      iii. User:> Patient who interacts with the chatbot
   
      iv. Admin/Receptionist:> Clinic staff managing appointments


3. Overall Description

   2.1 Product Perspective

      The chatbot is an independent module embedded in the clinic’s website via Voiceflow widget.

    * System Components

      i. Chatbot UI (embedded widget)

      ii. AI conversation engine

      iii. Voiceflow variable-based appointment storage

      iv. Mock backend (future integration)

   2.2 Product Functions

      Primary Features

      1. Provide clinic information
      2. Appointment booking
      3.  Appointment rescheduling
      4.  Appointment cancellation
      5.  Dental care tips
      6.  Support Features
      7.  Validate user inputs
      8.  Identify user via phone number or appointment ID
      9.  Generate appointment confirmations

   2.3 User Characteristics:
   
      Patients: Basic mobile/computer users and Need appointment/services information.

      Receptionist/Admin: Uses collected data.
   
      No technical skills required

   2.4 Constraints

      1. Requires stable internet.
      2. Accuracy depends on AI responses
      3. Voiceflow free plan limits storage and data persistence

   2.5 Assumptions

      1. Phone number uniquely identifies a user
      2. Users enter correct appointment IDs
      3. Voiceflow components behave reliably

3. System Requirements:>
   
   3.1 Functional Requirements:

      FR1: Provide Clinic Information

      The chatbot must respond to information queries.

    !Sub-requirements!

      FR1.1 Provide clinic working hours

      FR1.2 Provide list of dental services

      FR1.3 Provide clinic address

      FR1.4 Provide contact information

   FR2: Appointment Booking Workflow

      Step 1. User selects Book Appointment
   
      Step 2. Provide name
   
      Step 3. Provide phone number
   
      Step 4. Provide preferred date & time
   
      Step 5. Chatbot checks availability
   
      Step 6. Appointment is created
   
      Step 7. Appointment ID is generated
   
      Step 8. Confirmation message is returned

   !Requirements!

      * FR2.1 Validate phone number input

      * FR2.2 Validate time slot

      * FR2.3 Store appointment details in system

      * FR2.4 Generate appointment ID

FR3: Appointment Rescheduling:>

   {Workflow}
   
   Step 1. User selects Reschedule Appointment
   
   Step 2. Input Appointment ID
   
   Step 3. System verifies ID
   
   Step 4. Ask for new date & time

   Step 5. Confirm reschedule

!Requirements!

   * FR3.1 Validate appointment ID

   * FR3.2 Check new slot availability

   * FR3.3 Update appointment record

   * FR4: Appointment Cancellation
     
      { Workflow}

        Step 1. User chooses Cancel Appointment
     
        Step 2. Enter Appointment ID
     
        Step 3. System verifies record
     
        Step 4. Appointment is deleted
     
        Step 5. Confirmation message sent

 !Requirements!

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

   * Response time ≤ 2 seconds

   * Handle ~50 concurrent users (simulated)

   NFR2: Usability

   * Simple conversational flow

   * Mobile and desktop compatible

   * Clear instructions and error messages

   NFR3: Security

   * User details stored securely in Voiceflow

   * No sensitive medical data collected

   * Avoid sharing personal data unnecessarily

   NFR4: Reliability

   * 99% uptime target

   * Handle invalid inputs gracefully

   NFR5: Scalability

   * Ready for integration with real clinic backend

   * Support multilingual versions in future

4. System Flow & Diagrams
   
   4.1 High-Level Business Process Flow

      [High-Level Business Process Flow](images/high_level_business_process_flow.drawio.png)

   4.2 Sequence Diagram

      [Workflow Diagram](images/workflow_Diagram.drawio.png)

   4.3 Use Case Diagram

      [TO-BE Improved Workflow](images/TO-BE_flow.drawio.png)

5. Future Enhancements

   1. Integration with actual database

   2. OTP verification for user identity

   3. Payment integration for prepaid appointments

   4. WhatsApp bot compatibility

   5. Admin dashboard with analytics

6. Approval

   Role : Business Analyst

   Name: Kirti

   Date: 10/12/2025


