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
**Appointment Data:** Google Sheets  
**Notifications:** Email  
**Monitoring:** n8n error monitoring and daily health checks
## Privacy & Data Handling

Public demonstrations and documentation for NORA use fictional or test information only.

No real patient information, private credentials, API keys, authentication tokens, or other sensitive healthcare data are included in the public project documentation.

---

**Built by [Lydia Ogbene Odey](https://github.com/Lydautomation)**
