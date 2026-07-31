# Splunk Authentication Monitoring Dashboard

## Overview

This project demonstrates a Security Operations Center (SOC) authentication monitoring dashboard built using Splunk Enterprise.

The dashboard monitors Windows Security authentication events, helping analysts identify successful logins, failed logins, authentication trends, and suspicious login activity.

---

## Technologies

- Splunk Enterprise
- SPL (Search Processing Language)
- Windows 11
- Windows Security Event Logs

---

## Event IDs

| Event ID | Description |
|----------|-------------|
| 4624 | Successful Logon |
| 4625 | Failed Logon |

---

## Dashboard Features

- Authentication Overview
- Failed Authentication by User
- Successful Logons by Logon Type
- Failed Authentication Trend
- Interactive User Logons
- Recent Failed Authentication Events
- Authentication Success vs Failure Trend

---

## Skills Demonstrated

- Windows Event Log Analysis
- Authentication Monitoring
- Security Investigation
- SPL Query Development
- Dashboard Development
- Incident Triage
- Log Analysis

---

## Key Findings

- Analyzed Windows Security authentication events collected in Splunk.
- Observed that Logon Type 5 (service logons) represented the majority of successful authentications.
- Investigated failed authentication events for the local user account and verified them through raw event analysis.
- Correlated dashboard visualizations with Windows Security logs to validate findings.


---

## Future Improvements

- Brute Force Detection
- Password Spray Detection
- Interactive Dashboard Filters
- Risk Score Panel
- Email Alerting
