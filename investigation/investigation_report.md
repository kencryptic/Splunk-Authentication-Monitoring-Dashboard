# Authentication Investigation Report

## Objective

Investigate Windows authentication activity using Splunk.

---

## Data Source

Windows Security Event Logs

---

## Event IDs

4624 - Successful Authentication

4625 - Failed Authentication

---

## Investigation Summary

Authentication events were analyzed to identify successful and failed logons.

The dashboard highlighted authentication trends, logon types, and user activity.

Most successful logins were service logons (Logon Type 5), which is expected on Windows systems.

A small number of failed interactive logins were identified and validated through raw event inspection.

No evidence of brute-force activity was observed during the analysis period.

---

## Conclusion

The dashboard successfully provides visibility into Windows authentication activity and can assist SOC analysts in identifying abnormal authentication behavior.