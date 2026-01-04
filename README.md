# AI Lead Follow-Up & Qualification System

This repository documents a reusable AI-powered system designed to automatically handle business enquiries from first contact to follow-up.

The system ensures no leads are missed, responses are sent instantly, follow-ups are consistent, and higher-priority enquiries are highlighted for human attention.

---

## What This System Does

- Captures new leads via Google Forms  
- Sends an instant, professional AI-generated reply  
- Classifies leads as priority or normal based on budget and urgency  
- Sends automated follow-up emails if the lead does not reply  
- Stops all follow-ups automatically when a lead replies or books  
- Notifies the business about new, priority, and replied leads  
- Can be cloned and deployed quickly for multiple businesses  

---

## Tools Used

- Google Forms  
- Google Sheets  
- Gmail  
- OpenAI (ChatGPT API)  
- Make.com  

No CRM, dashboards, or unnecessary third-party tools are used.

---

## System Structure

### 1. Google Form
Captures lead details such as:
- Name
- Email
- Phone
- Service required
- Budget range
- Urgency

---

### 2. Google Sheet

**Leads Tab**
- Stores all lead data
- Tracks follow-up stage
- Tracks next follow-up time
- Detects replies and booking status

**Settings Tab**
- Business name
- Sender email
- Notification email
- Booking link
- Priority lead rules
- Editable AI prompt variables

All key values are controlled from this tab to ensure reusability.

---

## Automation Scenarios (Make.com)

### Scenario 1 – Lead Capture & Initial Reply
- Triggered by Google Form submission
- Saves lead to Google Sheets
- Sends instant AI-generated reply
- Flags priority vs normal leads
- Notifies the business

---

### Scenario 2 – Automated Follow-Ups
- Runs on a scheduled interval
- Sends follow-up emails at defined delays
- Stops automatically if the lead replies or booking is detected
- Updates the lead status in the sheet

---

### Scenario 3 – Reply Detection & Stop Logic
- Monitors incoming email replies
- Matches replies to leads in Google Sheets
- Disables follow-ups when a reply is detected
- Updates lead status automatically

---

## Demo Videos

### Video 1 – System Overview & Structure
(Explains the form, sheet structure, priority logic, and reusability)

👉 Loom link: **https://www.loom.com/share/ff3602d9e00c47f385e458c5a3d9c85f**

---

### Video 2 – Live Demo & Testing
(Shows live form submission, follow-ups, reply detection, and stop logic)

👉 Loom link: **https://www.loom.com/share/119a45ec6a9e4fd7910527e47f1dfccb**

---

## Key Design Principles

- Fully reusable and cloneable  
- No hard-coded values  
- Clear separation of logic and settings  
- Business-focused outcomes, not technical complexity  

---

## Use Case

Ideal for:
- Service businesses
- Agencies
- Consultants
- Lead-driven businesses
- Anyone who wants faster response times and consistent follow-up without manual effort

---

## Notes

- Follow-up delays can be adjusted (used shorter intervals for testing)
- Booking integration is optional and can be added easily
- Designed for fast onboarding of new clients

---

## Author

Built and documented by **Usman** as part of a real-world Upwork client project.
