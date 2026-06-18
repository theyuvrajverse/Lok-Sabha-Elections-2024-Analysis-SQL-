# Lok-Sabha-Elections-2024-Analysis-SQL-
Description: SQL analysis of India's 2024 general election results — alliance classification, seat distribution by state, and constituency-level winner/runner-up identification using window functions

# Lok Sabha Elections 2024 Analysis (SQL)

## Business Problem

Election datasets contain large volumes of constituency-level, party-level, and state-level information that can be difficult to analyze without a structured data model. The objective of this project was to transform raw election data into meaningful political insights by analyzing alliance performance, constituency outcomes, voting patterns, and state-level election statistics using SQL.

## Dataset Structure

The analysis was performed on multiple related election datasets containing:

* Constituency information
* Candidate details
* Party information
* State information
* Vote distribution data

The tables were linked through primary and foreign key relationships to enable constituency-level and state-level analysis.

## SQL Analysis

Developed analytical SQL queries to answer key election questions:

* Alliance-wise seat distribution across India
* State-wise seat breakdown for NDA, I.N.D.I.A, and Other alliances
* Winning and runner-up candidate identification for every constituency
* Vote distribution analysis between EVM and postal ballots
* Party performance across states
* Constituency-level election outcomes
* State-level election summaries and statistics

### Data Transformation

Implemented custom political alliance classification by:

* Modifying schema using `ALTER TABLE`
* Creating alliance classification fields
* Mapping 30+ political parties into:

  * NDA
  * I.N.D.I.A
  * OTHER

using business-rule-based SQL logic.

## Key Insights

* Successfully classified 30+ political parties into their respective alliances using SQL-based transformation logic.
* Generated alliance-wise seat counts to evaluate overall coalition performance.
* Identified winners and runners-up across all constituencies using window functions and ranking techniques.
* Analyzed constituency-level vote distribution between EVM and postal ballots.
* Produced state-wise election summaries including seat counts, candidate participation, party representation, and voting statistics.
* Enabled drill-down analysis from national-level alliance performance to individual constituency results.

## SQL Concepts Demonstrated

* Multi-Table Joins
* Window Functions (`ROW_NUMBER()`)
* Aggregate Analysis (`GROUP BY`, `HAVING`)
* CASE Statements
* Data Transformation & Classification
* Schema Modification (`ALTER TABLE`)
* Subqueries
* Common Reporting Queries
* Business Rule Implementation in SQL

## Files

* `loksabha_2024_analysis.sql` — Complete SQL analysis, alliance classification logic, constituency ranking, and election reporting queries

## Tools & Technologies

* MySQL
* SQL Window Functions
* Relational Data Modeling
* Data Transformation
* Election Data Analytics
