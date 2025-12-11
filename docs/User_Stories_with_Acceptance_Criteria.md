USER STORIES FOR SMILEBOT

  User Story 1: Book Appointment
  
  Story:
  
   As a patient, I want to book an appointment through the chatbot so that I can schedule a visit without        calling the clinic.

  Acceptance Criteria:
  
   Chatbot collects name, phone number, service type, and preferred date/time.
   Chatbot confirms availability before finalizing.
   Chatbot generates Appointment ID and confirms booking.

  User Story 2: Cancel Appointment

  Story:
  
   As a patient, I want to cancel my appointment through the chatbot so that I can avoid calling the clinic.

  Acceptance Criteria:
  
   Chatbot verifies patient identity using phone number and Appointment ID.
   Chatbot confirms cancellation and updates the schedule.
   Chatbot notifies patient if the Appointment ID is invalid.

  User Story 3: Reschedule Appointment

  Story:
  
   As a patient, I want to reschedule an existing appointment so that I can choose a time that works better      for me.

  Acceptance Criteria:

   Chatbot verifies identity using phone number and Appointment ID.
   Chatbot asks for new date/time and checks availability.
   Chatbot confirms updated appointment or suggests alternatives if unavailable.

  User Story 4: FAQs / General Information

  Story:
  
     As a patient, I want to get answers to frequently asked questions so that I can know clinic hours,            services, and dental care tips instantly.

  Acceptance Criteria:
  
     Chatbot provides answers to predefined FAQs.
     If question is not recognized, chatbot suggests contacting receptionist.

  User Story 5: Verify Patient Identity

  Story:
  
    As a patient, I want the chatbot to verify my identity before canceling or rescheduling appointments so       that my data and appointments remain secure.

  Acceptance Criteria:
  
     Chatbot checks phone number + Appointment ID against existing records.
     If valid, allow the action.
     If invalid, prompt for correct details or escalate to receptionist.
