USE CASES FOR SMILEBOT

* Use Case 1: Book Appointment

    ID: UC-001

    Actor: Patient

    Description: Patient books an appointment via chatbot

    Preconditions: Patient has a valid phone number

    Trigger: Patient selects “Book Appointment”

    Main Flow:
      Chatbot asks for name
      Chatbot asks for phone number
      Chatbot asks for service type
      Chatbot asks for preferred date/time
      Chatbot checks availability
      Chatbot confirms appointment and generates Appointment ID

Alternate Flow:
If requested slot unavailable → Chatbot suggests next available time

Postconditions: Appointment recorded and ID generated

Use Case 2: Cancel Appointment

ID: UC-002

Actor: Patient

Description: Patient cancels existing appointment

Preconditions: Patient has valid Appointment ID

Trigger: Patient selects “Cancel Appointment”

Main Flow:
Chatbot asks for phone number + Appointment ID
Chatbot verifies identity
Chatbot cancels appointment
Chatbot confirms cancellation

Alternate Flow:

Incorrect Appointment ID → Chatbot asks again or escalates to receptionist

Postconditions: Appointment removed from schedule

Use Case 3: Reschedule Appointment

ID: UC-003

Actor: Patient

Description: Patient reschedules an appointment

Preconditions: Patient has valid Appointment ID

Trigger: Patient selects “Reschedule Appointment”

Main Flow:
Chatbot asks for phone number + Appointment ID
Chatbot verifies identity
Chatbot asks for new date/time
Chatbot checks availability
Chatbot confirms updated appointment

Alternate Flow:

If new slot unavailable → Chatbot suggests alternative times

Postconditions: Appointment updated

Use Case 4: FAQs / General Info

ID: UC-004

Actor: Patient

Description: Patient asks common questions about the clinic

Preconditions: None

Trigger: Patient selects “FAQ”

Main Flow:
Chatbot provides answers about hours, services, pricing, dental tips

Alternate Flow:

If question unknown → Chatbot escalates to receptionist or suggests contact

Postconditions: Patient receives answer

Use Case 5: Verify Patient Identity

ID: UC-005

Actor: Patient

Description: Chatbot verifies identity before cancel/reschedule

Preconditions: Appointment exists

Trigger: Patient provides phone number + Appointment ID

Main Flow:
Chatbot cross-checks phone number and Appointment ID
If valid → allow cancel/reschedule

Alternate Flow:
If invalid → ask again or escalate to receptionist

Postconditions: Only verified patients can modify appointments
