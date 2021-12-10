# Visdown

**Make visualisations using only markdown**

Write visualisation using a simple declarative markup like you would write code. Just wrap it in fenced block (three backticks) and mark the language as `vis`.

*Make simple static visualisations*

```vis
data:
  url: ../data/covid19-public-main/epidemic/cases_malaysia.csv
mark: point
encoding: 
  x: 
    field: date
    type: quantitative
  y: 
    field: cases_new
    type: quantitative
```