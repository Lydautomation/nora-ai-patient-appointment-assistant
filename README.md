# NORA — AI Patient Appointment Assistant

NORA is an AI-powered patient appointment assistant built to simplify appointment management and reduce repetitive administrative work in healthcare settings.

It allows patients to manage appointments conversationally while connecting each interaction to the underlying appointment workflow.

## The Problem

Appointment management can involve repetitive administrative tasks such as checking available dates and times, recording patient information, creating appointments, handling rescheduling or cancellations, retrieving appointment details, and sending reminders.

These processes can take up staff time and create unnecessary back-and-forth for both patients and healthcare teams.

## The Solution

NORA provides a conversational interface through which patients can manage common appointment-related tasks.

The system identifies what the patient wants to do, retrieves the required information, interacts with appointment data, completes the appropriate action, and triggers relevant notifications.

NORA supports the appointment journey from initial scheduling through pre-appointment reminders.

## Core Capabilities

- Book new appointments
- Check available appointment dates and time slots
- Reschedule existing appointments
- Cancel appointments
- Retrieve appointment information
- Retrieve appointments using alternative patient information when an appointment ID is unavailable
- Capture required patient information
- Send appointment confirmation emails
- Notify the relevant department about new appointments
- Send automated patient reminders 24 hours before scheduled appointments

## How It Works

A typical booking flow follows this process:

1. The patient tells NORA they want to book an appointment.
2. NORA collects the required appointment information, including the department.
3. The system checks the appointment database for available dates and time slots.
4. The patient selects an available slot.
5. NORA collects the required patient details.
6. The appointment is created and stored.
7. The patient receives an appointment confirmation.
8. The relevant department receives a notification.
9. Twenty-four hours before the scheduled appointment, the patient automatically receives a reminder.

NORA also supports separate conversational flows for appointment retrieval, rescheduling, and cancellation.

## System Design

The system design documentation provides a visual overview of NORA's architecture and appointment-management process.

[View NORA System Design](docs/nora-system-design.pdf)

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

## Human Oversight

NORA is designed to automate repetitive appointment-management tasks while keeping healthcare staff involved where human review, intervention, or decision-making is required.

The system supports healthcare operations rather than replacing professional judgment or clinical decision-making.

## Monitoring & Reliability

The project includes supporting monitoring workflows for:

- Error monitoring and alerts
- Daily system health checks

These help identify workflow failures and verify that important system components remain operational.

## Tech Stack

**Automation & Orchestration:** n8n  
**AI / LLM Access:** OpenRouter  
**Appointment Data:** Supabase  
**Notifications:** Email  
**Monitoring:** n8n error monitoring and daily health checks

## Privacy & Data Handling

Public demonstrations and documentation for NORA use fictional or test information only.

No real patient information, private credentials, API keys, authentication tokens, or other sensitive healthcare data are included in the public project documentation.

---

**Built by [Lydia Ogbene Odey](https://github.com/Lydautomation)**
