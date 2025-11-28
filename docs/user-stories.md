User Stories & Acceptance Criteria

Project: GentleCare Dental Clinic – AI Chatbot

Version: 1.0

EPIC: Appointment Management Chatbot


As a patient, I want to interact with a chatbot so that I can get clinic information and manage my dental appointments easily.

* User Story List

US-01 – View Clinic Information

US-02 – Book Appointment

US-03 – Reschedule Appointment

US-04 – Cancel Appointment

US-05 – Receive Dental Care Tips

* User Stories with Acceptance Criteria
  
US-01: View Clinic Information

User Story:
As a patient, I want to ask the chatbot for clinic information so I can know the timings, services, and address.

Acceptance Criteria

Scenario: User requests clinic details

Given the chatbot is active

When the user asks for “clinic hours”, “services”, “address”, or “contact details”

Then the chatbot must display the correct clinic information

US-02: Book Appointment

User Story:

As a patient, I want to book an appointment through the chatbot so I can visit the clinic at a convenient time.

Acceptance Criteria

Scenario: Successful appointment booking

Given the user selects Book Appointment

When the chatbot collects name, phone number, date & time

Then the chatbot must validate availability

And generate an appointment ID

And display a confirmation message

Scenario: Time slot unavailable

Given the user enters an unavailable time slot

When the chatbot validates it

Then it must display “Slot unavailable”

And prompt the user to pick another slot

US-03: Reschedule Appointment

User Story:

As a patient, I want to reschedule my appointment so I can choose a more convenient time if my plans change.

Acceptance Criteria

Scenario: Successful reschedule

Given the user has a valid appointment ID

When they enter a new date and time

Then the chatbot must verify the appointment

And update the appointment in the system

And show a reschedule confirmation

US-04: Cancel Appointment

User Story:

As a patient, I want to cancel my appointment so that the clinic frees up the time slot.

Acceptance Criteria

Scenario: Successful cancellation

Given the user enters their appointment ID

When the chatbot verifies the ID

Then it must delete the appointment

And show a cancellation confirmation

US-05: Receive Dental Care Tips

User Story:

As a patient, I want to receive helpful dental care tips so I can maintain good oral hygiene.

Acceptance Criteria

Scenario: Display tips

Given the user requests tips

When the chatbot responds

Then tips must be general, safe, and non-medical

And should not replace professional dental advice
