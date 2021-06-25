# Rule Set #1 - Row Counts
[![License: CC0](https://img.shields.io/badge/License-CC0-red)](LICENSE "Creative Commons Zero License by DataResearchLabs (effectively = Public Domain")
[![YouTube](https://img.shields.io/badge/YouTube-DataResearchLabs-brightgreen)](http://www.DataResearchLabs.com)
## Data Validation Examples - Oracle

## Table of Contents
 - <a href="#introduction">1. Introduction</a>


* [T001 - FullRowCount()](#T001)
* [T002 - PartialRowCount()](#T002)
* [T003 - RelativeRowCount()](#T003)
* [T004 - RecentRowCount()](#T004)
<br>

<a name="TOO1"></a>
### T001 - FullRowCount()
  Verify full row count for a table or view.  For example, table X must have at least 10,000 rows.
  ```sql
  -- "RS-1 Row Counts" #1 - Verify FullRowCount() = 25 at table [countries]
  SELECT CASE WHEN COUNT(*) <> 25 THEN 'FAIL' ELSE 'P' END AS status 
  FROM demo_hr.countries;
  ```
<br>


<a name="TOO2"></a>
### T002 - PartialRowCount()
Verify partial row count for a subset of a table or view.  For example, there must be 50+ rows in Table X having value "Y" in Field Z.
```sql
  -- "RS-1 Row Counts" #2 - Verify PartialRowCount() = 8 where [region_id] = 1 (Europe) in table [countries]
  SELECT CASE WHEN COUNT(*) <> 8 THEN 'FAIL' ELSE 'P' END AS status   
  FROM demo_hr.countries
  WHERE region_id = 1;
```
<br>


<a id="introduction" class="anchor" href="#introduction" aria-hidden="true"> </a>
### T003 - RelativeRowCount()
Verify relative row counts between tables or views.  For example, table X must be 5 times or more larger than table Y.
```sql
  -- "RS-1 Row Counts" #3 - Verify RelativeRowCount() table [countries] row count >= 5x table [regions] row count
  SELECT CASE WHEN countries_count < 5 * regions_count THEN 'FAIL' ELSE 'P' END AS status
  FROM (
    SELECT (SELECT COUNT(*) AS row_count FROM demo_hr.countries) AS countries_count 
    , (SELECT COUNT(*) AS row_count FROM demo_hr.regions)   AS regions_count
    FROM dual
  );
```
<br>


<a name="TOO4"></a>
### T004 - Verify RecentRowCount()
Verify recent row counts.  For example, the table row count where DateCreated is within past 10 days.
```sql
  -- "RS-1 Row Counts" #4 - Verify RecentRowCount() >= 5 in table [countries] where [date_last_updated] in past
  SELECT CASE WHEN row_count < 5 THEN 'FAIL' ELSE 'P' END AS status
  FROM (
    SELECT COUNT(*) AS row_count 
    FROM demo_hr.countries
    WHERE date_last_updated >= SYSDATE - 10
  );
```


