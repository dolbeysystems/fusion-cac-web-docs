+++
title = 'Query Impact'
weight = 60
+++

## How does the impact of a query get recorded?

The impact for inpatient cases is captured by the natural actions a CDS takes, therefore no manual data
entry needs to be tracked by the CDS. The impact of the query is calculated by using the working DRG
calculated within the same session in which you created the physician query for. Then once the
physician replies to the query the CDS will then close the query as agreed, disagreed or no opinion. The
same session that a CDS closes the query the system will then capture the working DRG that was
calculated during this session. A session is closed by saving the chart.

```
Query Impact = Pre-Query Working DRG Weight – Post-Query Working DRG Weight
```

If physician query shifts the assigned DRG, diagnosis, procedures, CC/MCC/HAC/ROM/SOI or Quality
metrics, the shift reason is automatically calculated by the system. The shift reason is captured by the
system looking at the difference between the last working DRG to the Current Working DRG and Code
Sets the difference in the most current working DRG and code sets will be automatically captured for
reporting.
