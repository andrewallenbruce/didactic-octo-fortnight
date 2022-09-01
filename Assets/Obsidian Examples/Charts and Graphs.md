
```chart
type: radar
labels: [Pay Per Visit,New Patients,No Shows,Visits Per Patient]
series:
  - title: January
    data: [29,26,29,24]
  - title: February
    data: [24,29,26,30]
  - title: March
    data: [18,23,25,19]
  - title: April
    data: [14,15,22,13]	
tension: 0
width: 100%
labelColors: true
fill: false
beginAtZero: false
```
---
```chart
type: bar
labels: [Monday,Tuesday,Wednesday,Thursday,Friday, Saturday, Sunday, "next Week", "next Month"]
series:
          - title: Title 1
            data: [1,2,3,4,5,6,7,8,9]
          - title: Title 2
            data: [5,4,3,2,1,0,-1,-2,-3]
tension: 0
width: 91%
labelColors: true
fill: false
beginAtZero: false
```
---
```chart
type: line
labels: [Pay Per Visit,New Patients,No Shows,Visits Per Patient]
series:
  - title: January
    data: [29,26,29,24]
  - title: February
    data: [24,29,26,30]
  - title: March
    data: [18,23,25,19]
  - title: April
    data: [14,15,22,13]	
tension: 0
width: 100%
labelColors: true
fill: false
beginAtZero: false
```

``` tracker
searchType: table
searchTarget: RCM/Tables[0][0], RCM/Tables[0][1]
xDataset: 0
fixedScale: 0.8
margin: 10, 10, 10, 10
line:
	title: Clean Claim Distribution
	yAxisLabel: PCC
	yAxisUnit: %
	lineColor: red, yellow
	yAxisLocation: left, right
```

```chart
type: bar
labels: [UHC,Horizon,Oxford,Aetna,Medicare,Cigna]
series:
          - title: Clean Claim Distribution by Payers (%)
            data: [82,73,64,59,59,51]
tension: 0
width: 100%
labelColors: true
fill: true
beginAtZero: false
```