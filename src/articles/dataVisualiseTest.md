# Visdown

**Make visualisations using only markdown**

Write visualisation using a simple declarative markup like you would write code. Just wrap it in fenced block (three backticks) and mark the language as `vis`.

*Make simple static visualisations*

```vis
data:
  url: "../data/covid19-public-main/epidemic/cases_malaysia.csv"
mark: point
encoding: 
  x: 
    field: date
    type: quantitative
  y: 
    field: cases_new
    type: quantitative
```
Visdown is based on the grammar of interactive graphic (vega-lite) which allows you to specify the visualisation including interactions in a declarative fashion.

*Make interactive visualisations*

Select the circles with the mouse

```vis
data:
  url: "../data/covid19-public-main/epidemic/cases_malaysia.csv"
mark: circle
selection:
  brush:
    type: interval
encoding:
  x:
    type: quantitative
    field: date
    scale:
     domain: [12,25]
  y:
    type: quantitative
    field: cases_new
    scale:
     domain: [0,25000]
  color:
    condition:
      selection: brush
      field: type
      type: nominal
    value: grey
width: 450
height: 300
```
[Home Page](../../index.md)
<div style="text-align: right"><a href="../../index.md" >Next Chapter</a> </div>