# PACCAR
<ins>Repository for solution of PACCAR Data validation assignment</ins>

This repository contains the solution for the Data Validation assessment. The problem statement is about validating the output of a Data processor that receives input files and processes them as per a predefined logic and produces 2 output files. The expectation is to write python code to validate the entries produced by the data processor and produce a test results file that would contain information about the validity of each entry produced by the Data processor.

For this I have utilized pandas library for data processing. A sample of data processing using Pandas library is given below.

Let's consider one of the logic points of the Data processor which says that if any player does not have any data for runs and wickets, he would not figure in the output. 

Using pandas, it can be done in a single line as below.

```
from_json = from_json.dropna(subset=['runs','wickets'],how='all')
```

