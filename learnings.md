# Learnings & Patterns

Running notes on SQL concepts and patterns picked up while solving StrataScratch questions. Updated as I go — each entry links back to the question that taught it.

---

## Window Functions

- `RANK()` vs `DENSE_RANK()` vs `ROW_NUMBER()`
  - `RANK()` leaves gaps after ties (1,1,3), `DENSE_RANK()` doesn't (1,1,2), `ROW_NUMBER()` never ties.
  - Use `DENSE_RANK()` for "Nth highest salary" style questions where ties should count once (see *Second Highest Salary*).
- `PARTITION BY` resets the window per group — essential for "top N per group" questions (see *Highest Salary In Department*, *Ranking Most Active Guests*).
- `LAG()` / `LEAD()` for comparing a row to the previous/next row — useful for "percentage difference month over month" type questions (see *Monthly Percentage Difference*).

## Joins & Self-Joins

- **Self-joins** for comparing rows within the same table (e.g. matching pairs, finding duplicates) — see *Meta/Facebook Matching Users Pairs*, *Duplicate HR Department Employees*, *Employees With the Same Salary*.
- **INNER vs LEFT JOIN** for "missing data" style questions — LEFT JOIN + `IS NULL` finds rows with no match (see *Users Missing Phone Numbers*).
- Watch out for **fan-out** when joining one-to-many tables before aggregating — aggregate first or use `DISTINCT` carefully.

## Aggregation & Grouping

- `GROUP BY` + `HAVING` for filtering on aggregated values (e.g. "departments with 5 employees") — see *Departments With 5 Employees*.
- `COUNT(DISTINCT ...)` vs `COUNT(...)` — matters a lot for "unique users per month" style questions (see *Unique Users Per Client Per Month*).
- Conditional aggregation with `SUM(CASE WHEN ... THEN 1 ELSE 0 END)` to pivot categories into columns (see *Titanic Survivors and Non-Survivors*).

## Date & Time Handling

- `EXTRACT(HOUR FROM ...)` / `DATE_PART()` to pull out hour/day/month from a timestamp (see *Hour Of Highest Gas Expense*).
- `DATE_TRUNC('month', ...)` to bucket rows by month (see *Number of Shipments Per Month*, *Department Workforce Analysis*).
- Careful with timezone assumptions when filtering "before noon" style conditions (see *Find all Lyft rides which happened on rainy days before noon*).

## String Matching

- `LIKE '%word%'` / `ILIKE` for case-insensitive substring search (see *Find drafts which contains the word 'optimism'*).
- `~` (regex) in Postgres for pattern-based filtering, e.g. names ending in a specific letter (see *First Names With Six Letters Ending in 'h'*).

## CTEs & Query Structure

- Breaking a query into multiple `WITH` CTEs makes multi-step logic (filter → aggregate → rank) much easier to debug than one giant nested query.
- Naming CTEs clearly (`filtered_orders`, `ranked_users`) instead of `cte1`, `cte2` — makes solutions easier to revisit later.

## Common Gotchas

- `NULL` breaks equality checks — always use `IS NULL` / `IS NOT NULL`, never `= NULL`.
- Integer division truncates in Postgres — cast to `NUMERIC` or multiply by `1.0` before dividing when computing percentages (see *Find the percentage of shipable orders*, *Acceptance Rate By Date*).
- `ORDER BY` inside a window function's `OVER()` clause is independent of the query's outer `ORDER BY`.

---

*This file grows as I solve more questions — each new pattern gets added here with a link back to the question that introduced it.*
