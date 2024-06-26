---
Tags: Azure, AZ-400, AZ-204
---
[[Kusto Query Language (KQL)]] utilises an RBAC model where authenticated principal are mapped to roles which determine their roles


bin() is used to group data into bins based on a time interval (time-series)
Example
```KQL
datatable(timestamp: datetime, value: real)
[
    datetime(2023-07-20 12:00), 5,
    datetime(2023-07-20 13:15), 7,
    datetime(2023-07-20 14:30), 9,
    datetime(2023-07-20 15:45), 3
]
| summarize sum(value) by bin(timestamp, 1h)
```

Cheatsheet
![[KQL Cheatsheet A.png]]