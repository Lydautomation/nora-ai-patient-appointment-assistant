## Project Screenshots

### Workflow Overview

The n8n workflow orchestrates NORA's conversational appointment-management process and connects the AI assistant with the supporting appointment services.

![NORA n8n Workflow Overview](screenshots/nora-workflow-overview.png.jpg)

### Patient Interaction

Patients interact with NORA through n8n Web Chat to manage their appointments conversationally.

![NORA Web Chat](screenshots/nora-web-chat.png.jpg)

### Appointment Availability

NORA checks appointment availability against the appointment slots stored in Supabase before presenting available options to the patient.

![Appointment Slots in Supabase](screenshots/appointment-slots-supabase.png.png)

### Appointment Records

Confirmed appointments are stored and managed in Supabase for subsequent retrieval, rescheduling, and cancellation.

![Appointments in Supabase](screenshots/appointments-supabase.png.png)

### Appointment Confirmation

After a successful booking, the patient automatically receives an appointment confirmation email.

![NORA Appointment Confirmation Email](screenshots/appointment-confirmation-email.png.jpg)

### 24-Hour Appointment Reminder

NORA automatically sends the patient a reminder 24 hours before the scheduled appointment.

![NORA Appointment Reminder Email](screenshots/appointment-reminder-email.png.png)
