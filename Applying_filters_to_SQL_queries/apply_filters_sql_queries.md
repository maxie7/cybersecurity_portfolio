## Apply filters to SQL queries

### Project description

As part of my role, I oversee bolstering the security protocols within my organization's digital infrastructure. My responsibilities include safeguarding the system, surveying for potential vulnerabilities, and administering requisite updates to employee devices. The following examples demonstrate how I leverage SQL queries and filters to execute security-related tasks.

### Retrieve after hours failed login attempts

An incident with potential security implications occurred outside of normal business hours, specifically post 18:00. An investigation into all unsuccessful login attempts that transpired during this after-hours period is necessitated.

The provided code snippet showcases how I constructed an SQL query to isolate failed login attempts post 18:00. The screenshot exhibits two segments: the initial portion displays the query utilized, while the latter section previews a sample of the resultant output.

![failed_login_attempts](https://github.com/maxie7/cybersecurity_portfolio/assets/15796607/39409440-39c6-4f67-9c03-f74af8b7ddcf)

The query aims to filter unsuccessful login attempts post 18:00. To accomplish this, I started by drawing all data from the 'log_in_attempts' table. Next, I integrated a WHERE clause employing an AND operator to refine the data. This refinement ensured solely login attempts satisfying two criteria were surfaced: attempts post 18:00 and unsuccessful attempts. The first standard, 'login_time > '18:00'', filters for attempts post 18:00, while the second criterion, 'success = FALSE', isolates failed login attempts.

### Retrieve login attempts on specific dates

An incident arousing suspicion materialized on May 9, 2022. To thoroughly investigate the matter, scrutinizing login activities on this explicit date and the preceding day, May 8, 2022, is imperative.

The provided code excerpt demonstrates how I constructed an SQL query to identify login attempts occurring on the particular dates in question. The screenshot encompasses two segments: the initial portion displays the query formulation, while the subsequent section exhibits a snippet of the resultant output.

![login_on_specific_dates](https://github.com/maxie7/cybersecurity_portfolio/assets/15796607/8fb9373b-4c97-432d-801d-e21ef385b3c7)

The query primarily aims to retrieve all login attempts on May 9, 2022 or May 8, 2022. The procedure commenced by extracting comprehensive data from the ‘log_in_attempts’ table. Subsequently, I utilized a WHERE clause integrating an OR operator to refine the findings. This refinement process ensured solely the presentation of login attempts satisfying two criteria: attempts on May 9, 2022 (‘login_date = ‘2022-05-09’’) and attempts on May 8, 2022 (‘login_date = ‘2022-05-08’’).

### Retrieve login attempts outside of Mexico

Upon examining the organization’s login attempt data, I identified an issue regarding login activities originating externals Mexico. Investigating these particular login attempts is imperative.

The provided code snippet demonstrates the methodology utilized to construct an SQL query isolating login attempts beyond Mexico’s borders. The screenshot includes two segments: the first section displays the query formulation, while the second presents an output sample.

![attempts_outside_0f_mexico](https://github.com/maxie7/cybersecurity_portfolio/assets/15796607/a5c46006-4389-40ef-988e-66615dd17e38)

The query primarily aims to retrieve all login attempts transpiring outside of Mexico. The procedure began by extracting comprehensive data from the ‘log_in_attempts’ table. Subsequently, I employed a WHERE clause with the NOT operator to refine the results based on the stipulated criterion. To identify non-Mexican countries, I leveraged the LIKE operator coupled with the pattern ‘MEX%’, since the dataset denotes Mexico by both ‘MEX’ and ‘MEXICO’. Here, the ‘%’ wildcard matches any unspecified sequence of characters when used alongside the LIKE operator.

### Retrieve employees in Marketing

My team aims to update computers for specific Marketing department employees. This necessitates aggregating data concerning which employee devices require updates.

The provided code excerpt demonstrates my approach for constructing an SQL query that pinpoints Marketing department employees situated in the East building. The screenshot contains two segments: the first portion displays the query formulation, while the second previews sample output.

![marketing_employees](https://github.com/maxie7/cybersecurity_portfolio/assets/15796607/e6a9091b-1b38-47b0-9b6e-b2b215b44e98)

The query’s core objective is retrieving details of Marketing employees in the East building. I initiated the process by extracting comprehensive data from the ‘employees’ table. Subsequently, I integrated a WHERE clause with an AND operator to refine the results per stipulated criteria. To isolate Marketing employees in the East building, I utilized the LIKE operator with the pattern ‘East%’ to correspond to the ‘office’ column data, within which the East building is denoted alongside a unique office number. The first criterion, ‘department = ‘Marketing’’ filters for Marketing employees, while the second criterion ‘office LIKE ‘East%’’ narrows results to those in the East building.

### Retrieve employees in Finance or Sales

Moreover, updating machines utilized by Finance and Sales department employees is necessary. Given the distinct security update necessitated, exclusively aggregating data pertaining to employees of these two specific departments is essential.

The provided code excerpt demonstrates the methodology utilized to construct an SQL query aimed at identifying employee machines affiliated with either the Finance or Sales departments. The screenshot includes two segments: the first portion displays the query construction, while the second previews resulting output.

![finance_and_sales_employees](https://github.com/maxie7/cybersecurity_portfolio/assets/15796607/e064154a-0817-4504-bf54-04c626f95b52)

The query’s primary objective is retrieving data about employees in the Finance or Sales departments. The procedure began by comprehensively extracting from the ‘employees’ table. Subsequently, I introduced a WHERE clause with an OR operator to refine results per the specified criteria. The OR operator usage here is critical, as it ensures the inclusion of all employees of either department. The first criterion, ‘department = ‘Finance’’ isolates Finance department employees, while the second criterion ‘department = ‘Sales’’ refines the results to encompass Sales department employees.

### Retrieve all employees not in IT

Moreover, my team must deploy an additional security update for employees unaffiliated with the Information Technology department. As preparation, the initial step involves aggregating information exclusively regarding these non-IT employees.

The provided content demonstrates the methodology utilized to construct an SQL query for filtering employee machines of individuals external to the Information Technology department. The screenshot contains two sections: the first segment displays the query formulation, while the second provides output sample.

![not_IT_employees](https://github.com/maxie7/cybersecurity_portfolio/assets/15796607/87afa331-dd1d-47bd-87d5-e3e5f601f80f)

The query’s chief objective is extracting details of employees outside the Information Technology department. The process began by comprehensively selecting data from the ‘employees’ table. Subsequently, I introduced a WHERE clause integrating the NOT operator to refine results to employees not affiliated with the stipulated department.

### Summary

Utilizing filtering mechanisms within SQL queries, I extracted precise data concerning login attempts and employee machines. By leveraging distinct tables—specifically, ‘log_in_attempts’ and ‘employees’—I took advantage of operators including AND, OR, and NOT to curate results per specific goals. Furthermore, I employed the LIKE operator alongside the ‘%’ wildcard to potentiate effective filtering per particular patterns in the data.

