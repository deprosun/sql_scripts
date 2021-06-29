# Multiple Platform Data Validation Scripts
[![License: CC0](https://img.shields.io/badge/License-CC0-red)](LICENSE "Creative Commons Zero License by DataResearchLabs (effectively = Public Domain")
[![YouTube](https://img.shields.io/badge/YouTube-DataResearchLabs-brightgreen)](http://www.DataResearchLabs.com)

## What is Data Validation Testing?
<img align="right" src="https://github.com/DataResearchLabs/sql_scripts/blob/main/img/04_data_validation_scripts.png" width="500px">
"Data Validation Testing" ensures that the data you work with is accurate and complete, that any necesary transformations occur without loss, that your processes can handle incorrect data, and the final output is correct.<br>
<br>

## How Can You Use Data Validation Testing?

- **Test/Stage Regression**: You could setup a more extensive set of data validation tests and schedule them to run daily.  If it take 45 minutes to run 1,200 tests to thoroughly exercise the business logic of an entire schema, running it daily is a good trade-off.  You'll be surprised at the number of times where out-of-the-blue you catch some odd application bug based on data rules.
- **Manual QA**: When it makes sense, you can build a data validation test script that you manually run during the QA process at the appropriate gates/milestones.
- **Dev BVTs**: You could setup a lean/fast validation script that runs as a Build Verification Test every time developers check-in code...a baseline set of rules that should never be violoated.
- **Production Checkouts**: You can use data validation testing for after prod deplosy using carefully crafted read-only SELECTs so as to not impact performance.  
- **Baked Into Applications**: Where appropriate, you can build data validation tests directly into your ETL or data pipeline code.
<br>

## Note
Because each database platform has its own unique flavor of SQL, this page is just a central landing page to redirect you to the appropriate database platform's specific pages.<br>
<br>

<table>

<tr>
<td align="center" valign="top" rowspan=3>
  <br>
  <img align="enter" src="https://github.com/DataResearchLabs/sql_scripts/blob/main/img/db_icons/gp_icon.png" width="96px">
</td>
<td rowspan=3 width=325>

## Greenplum
* Rule Set 01 - Row Counts<br>
* Rule Set 02 - Keys<br>
* Rule Set 03 - Heuristic Thresholds<br>
* Rule Set 04 - Numeric Values<br>
* Rule Set 05 - Date Values<br>
* Rule Set 06 - Text Values<br>
* Rule Set 07 - Regular Expressions<br>
* Rule Set 08 - Diff Checks<br>
* Rule Set 09 - Defect Regression<br>
* Best Practices<br>
* Basic Validation Script<br>
* Advanced Validation Script<br>
</td>
 
<td>
  1. Basic<br>Table Level<br>Tests<br>Tutorial<br>(TODO)
</td>
<td>
  2. Advanced<br>Table Level<br>Tests<br>Tutorial<br>(TODO)
</td>
<td>
  3. Basic<br>Field Level Tests<br>Tutorial<br>(TODO)
</td></tr>
<tr><td>
  4. Advanced<br>Field Level<br>Tests<br>Tutorial<br>(TODO)
</td>
<td>
  5. Best Practices<br>for<br>Tests<br>Tutorial<br>(TODO)
</td>
<td>
  6. How to<br>Use<br>Basic<br>Validation<br>Script<br>(TODO)
</td></tr>
<tr><td>
  7. How to<br>Use<br>Advanced<br>Validation<br>Script<br>(TODO)
</td></tr>


<tr>
<td align="center" valign="top" rowspan=3>
  <br>
  <img align="enter" src="https://github.com/DataResearchLabs/sql_scripts/blob/main/img/db_icons/mssql_icon.png" width="96px">
</td>
<td rowspan=3 width=325>

## MS SQL Server
* Rule Set 01 - Row Counts<br>
* Rule Set 02 - Keys<br>
* Rule Set 03 - Heuristic Thresholds<br>
* Rule Set 04 - Numeric Values<br>
* Rule Set 05 - Date Values<br>
* Rule Set 06 - Text Values<br>
* Rule Set 07 - Regular Expressions<br>
* Rule Set 08 - Diff Checks<br>
* Rule Set 09 - Defect Regression<br>
* Best Practices<br>
* Basic Validation Script<br>
* Advanced Validation Script<br>
</td>
 
<td>
  1. Basic<br>Table Level<br>Tests<br>Tutorial<br>(TODO)
</td>
<td>
  2. Advanced<br>Table Level<br>Tests<br>Tutorial<br>(TODO)
</td>
<td>
  3. Basic<br>Field Level Tests<br>Tutorial<br>(TODO)
</td></tr>
<tr><td>
  4. Advanced<br>Field Level<br>Tests<br>Tutorial<br>(TODO)
</td>
<td>
  5. Best Practices<br>for<br>Tests<br>Tutorial<br>(TODO)
</td>
<td>
  6. How to<br>Use<br>Basic<br>Validation<br>Script<br>(TODO)
</td></tr>
<tr><td>
  7. How to<br>Use<br>Advanced<br>Validation<br>Script<br>(TODO)
</td></tr>
  

  
<tr>
<td align="center" valign="top" rowspan=3>
  <br>
  <img src="https://github.com/DataResearchLabs/sql_scripts/blob/main/img/db_icons/mysql_icon.png" width="105px">
</td>
<td rowspan=3 width=325>

## MySQL
* Rule Set 01 - Row Counts<br>
* Rule Set 02 - Keys<br>
* Rule Set 03 - Heuristic Thresholds<br>
* Rule Set 04 - Numeric Values<br>
* Rule Set 05 - Date Values<br>
* Rule Set 06 - Text Values<br>
* Rule Set 07 - Regular Expressions<br>
* Rule Set 08 - Diff Checks<br>
* Rule Set 09 - Defect Regression<br>
* Best Practices<br>
* Basic Validation Script<br>
* Advanced Validation Script<br>
</td>
 
<td>
  1. Basic<br>Table Level<br>Tests<br>Tutorial<br>(TODO)
</td>
<td>
  2. Advanced<br>Table Level<br>Tests<br>Tutorial<br>(TODO)
</td>
<td>
  3. Basic<br>Field Level Tests<br>Tutorial<br>(TODO)
</td></tr>
<tr><td>
  4. Advanced<br>Field Level<br>Tests<br>Tutorial<br>(TODO)
</td>
<td>
  5. Best Practices<br>for<br>Tests<br>Tutorial<br>(TODO)
</td>
<td>
  6. How to<br>Use<br>Basic<br>Validation<br>Script<br>(TODO)
</td></tr>
<tr><td>
  7. How to<br>Use<br>Advanced<br>Validation<br>Script<br>(TODO)
</td></tr>  
  
  
  
<tr>
<td align="center" valign="top" rowspan=3>
  <br>
  <img src="https://github.com/DataResearchLabs/sql_scripts/blob/main/img/db_icons/oracle_iconX.png" width="102px">
</td>
<td rowspan=3 width=325>

## Oracle
* Rule Set 01 - Row Counts<br>
* Rule Set 02 - Keys<br>
* Rule Set 03 - Heuristic Thresholds<br>
* Rule Set 04 - Numeric Values<br>
* Rule Set 05 - Date Values<br>
* Rule Set 06 - Text Values<br>
* Rule Set 07 - Regular Expressions<br>
* Rule Set 08 - Diff Checks<br>
* Rule Set 09 - Defect Regression<br>
* Best Practices<br>
* Basic Validation Script<br>
* Advanced Validation Script<br>
</td>
 
<td>
  1. Basic<br>Table Level<br>Tests<br>Tutorial<br>(TODO)
</td>
<td>
  2. Advanced<br>Table Level<br>Tests<br>Tutorial<br>(TODO)
</td>
<td>
  3. Basic<br>Field Level Tests<br>Tutorial<br>(TODO)
</td></tr>
<tr><td>
  4. Advanced<br>Field Level<br>Tests<br>Tutorial<br>(TODO)
</td>
<td>
  5. Best Practices<br>for<br>Tests<br>Tutorial<br>(TODO)
</td>
<td>
  6. How to<br>Use<br>Basic<br>Validation<br>Script<br>(TODO)
</td></tr>
<tr><td>
  7. How to<br>Use<br>Advanced<br>Validation<br>Script<br>(TODO)
</td></tr>  
    
  
  
<tr>
<td align="center" valign="top" rowspan=3>
  <br>
  <img src="https://github.com/DataResearchLabs/sql_scripts/blob/main/img/db_icons/pgsql_icon.png" width="125px">
</td>
<td rowspan=3 width=325>

## PostgreSQL
* Rule Set 01 - Row Counts<br>
* Rule Set 02 - Keys<br>
* Rule Set 03 - Heuristic Thresholds<br>
* Rule Set 04 - Numeric Values<br>
* Rule Set 05 - Date Values<br>
* Rule Set 06 - Text Values<br>
* Rule Set 07 - Regular Expressions<br>
* Rule Set 08 - Diff Checks<br>
* Rule Set 09 - Defect Regression<br>
* Best Practices<br>
* Basic Validation Script<br>
* Advanced Validation Script<br>
</td>
 
<td>
  1. Basic<br>Table Level<br>Tests<br>Tutorial<br>(TODO)
</td>
<td>
  2. Advanced<br>Table Level<br>Tests<br>Tutorial<br>(TODO)
</td>
<td>
  3. Basic<br>Field Level Tests<br>Tutorial<br>(TODO)
</td></tr>
<tr><td>
  4. Advanced<br>Field Level<br>Tests<br>Tutorial<br>(TODO)
</td>
<td>
  5. Best Practices<br>for<br>Tests<br>Tutorial<br>(TODO)
</td>
<td>
  6. How to<br>Use<br>Basic<br>Validation<br>Script<br>(TODO)
</td></tr>
<tr><td>
  7. How to<br>Use<br>Advanced<br>Validation<br>Script<br>(TODO)
</td></tr>  
</tr>     
</table>
<br>
<br>


***If you like these scripts, be sure to click the "Star" button above in GitHub.*** <br>
<br>
***Also, be sure to visit or subscribe to our YouTube channel*** www.DataResearchLabs.com!<br>
<br>
<br>