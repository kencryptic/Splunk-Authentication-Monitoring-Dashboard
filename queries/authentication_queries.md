# Authentication Queries

## Successful vs Failed Logins

```spl
index=* sourcetype=XmlWinEventLog (EventCode=4624 OR EventCode=4625)
| eval Login_Result=if(EventCode=4624,"Successful","Failed")
| stats count by Login_Result
```

---

## Failed Logins by User

```spl
index=* sourcetype=XmlWinEventLog EventCode=4625
| stats count by TargetUserName
| sort -count
```

---

## Logon Type Distribution

```spl
index=* sourcetype=XmlWinEventLog EventCode=4624
| stats count by Logon_Type
| sort -count
```

---

## Failed Authentication Trend

```spl
index=* sourcetype=XmlWinEventLog EventCode=4625
| timechart span=1d count
```

---

## Interactive User Logons

```spl
index=* sourcetype=XmlWinEventLog EventCode=4624 Logon_Type=2
| timechart span=1d count by TargetUserName
```