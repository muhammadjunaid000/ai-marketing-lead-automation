# Workflow Documentation

## 1. Lead Submission

A prospective customer submits their information through the Google Form.

The form collects:

* Full name
* Email address
* Company name
* Company size
* Area of interest
* Business requirements

---

## 2. Lead Capture

The submitted form response is automatically stored in Google Sheets.

Google Sheets acts as the initial lead data store for the automation workflow.

---

## 3. Automation Trigger

Make.com monitors the Google Sheets response data and detects new lead submissions.

When a new lead is detected, the automation scenario begins execution.

---

## 4. AI Lead Analysis

The lead information is passed to an AI analysis module.

The AI evaluates:

* Lead score
* Priority
* Intent
* Lead type
* Sentiment
* Recommended action
* Reason for classification

The AI returns structured information that can be used by downstream automation modules.

---

## 5. Conditional Routing

Make.com's router evaluates the AI-generated priority.

### High Priority

High-priority leads trigger an immediate email notification.

### Medium Priority

Medium-priority leads trigger a follow-up workflow.

### Low Priority

Low-priority leads are recorded without triggering an immediate notification.

### Fallback

Unexpected or unmatched cases are captured through a fallback route for further review.

---

## 6. Data Storage

Processed lead information is stored in a dedicated Google Sheets dataset.

The processed dataset contains both the original lead information and AI-generated classification data.

---

## 7. Analytics

The processed lead data is connected to Looker Studio.

The dashboard provides visibility into:

* Total leads
* Lead priority distribution
* Average lead score
* Lead intent
* Marketing interests
* Recommended actions
