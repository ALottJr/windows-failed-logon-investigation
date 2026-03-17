# Windows Failed Logon Investigation (Event ID 4625)

## Overview

This lab demonstrates how to investigate failed authentication attempts using Windows Event Viewer.

Security teams monitor **Event ID 4625** to detect brute force attacks, credential guessing attempts, and unauthorized login activity.

---

## Scenario

Multiple failed login attempts were generated on a Windows system.

The goal of this investigation was to:

• Identify failed authentication events  
• Analyze login attempt details  
• Understand how security logs record authentication failures

---

## Tools Used

- Windows Event Viewer
- Windows Security Logs

---

## Investigation Steps

### Step 1 — Navigate to Security Logs

Open **Event Viewer** and navigate to:

```
Windows Logs → Security
```

Screenshot:

![Security Log](screenshots/step1-security-log.png)

---

### Step 2 — Filter Event ID 4625

Filter the security log to show only **failed logon attempts**.

Event ID:

```
4625
```

Screenshot:

![Filter Event](screenshots/step2-filter-eventid.png)

---

### Step 3 — Review Failed Logon Events

The filtered results show multiple failed authentication attempts recorded by the system.

Screenshot:

![Filter Results](screenshots/step3-filter-results.png)

---

### Step 4 — Analyze Event Details

Event details reveal important authentication information such as:

- Source Network Address
- Authentication Package
- Logon Process
- Account Domain

Screenshot:

![Event Details](screenshots/step4-event-details.png)

---

## Key Findings

- Event ID **4625** represents a failed logon attempt
- Security logs capture detailed authentication information
- Failed login events can indicate:

  - brute force attacks  
  - credential guessing attempts  
  - unauthorized login activity  

---

## Security Insight

Monitoring **Event ID 4625** helps security teams detect potential attacks and investigate suspicious login behavior within an environment.

Regular review of authentication logs is a critical part of **SOC monitoring and threat detection**.
