# SQL StrataScratch Practice

My solutions to [StrataScratch](https://platform.stratascratch.com/coding) SQL coding questions, solved on **PostgreSQL**, filtered to the **Free** tier for **Product Analyst** and **Data Analyst** roles.

This repo is where I track my SQL practice end-to-end — writing queries, documenting my approach, and noting recurring patterns (window functions, joins, aggregations, date handling) so I can revisit them before interviews.

## Structure

```
sql-stratascratch-practice/
├── easy/       → Easy questions   (29 total)
├── medium/     → Medium questions (33 total)
├── hard/       → Hard questions   (4 total)
└── notes/
    └── learnings.md   → SQL patterns, gotchas & reusable snippets
```

Each solution file is named after the question (kebab-case) and follows this format:

```sql
/*
Question: <question title>
Company: <company>
Difficulty: <Easy / Medium / Hard>
Link: https://platform.stratascratch.com/coding
*/

-- Approach:
-- (short note on how I solved it)

SELECT ...
```

## Progress Overview

| Difficulty | Total | Solved |
|---|---|---|
| Easy | 29 | 29 |
| Medium | 33 | 33 |
| Hard | 4 | 4 |
| **Total** | **66** | **66** |

---

## Easy (29)

| # | Question | Company | Status | Solution |
|---|----------|---------|--------|----------|
| 1 | Find all posts which were reacted to with a heart | Meta | ✅ | [link](easy/find-all-posts-which-were-reacted-to-with-a-heart.sql) |
| 2 | Finding Updated Records | Microsoft | ✅ | [link](easy/finding-updated-records.sql) |
| 3 | Total Cost Of Orders | Etsy | ✅ | [link](easy/total-cost-of-orders.sql) |
| 4 | Workers With The Highest Salaries | Amazon | ✅ | [link](easy/workers-with-the-highest-salaries.sql) |
| 5 | Average Salaries | Glassdoor | ✅ | [link](easy/average-salaries.sql) |
| 6 | Calculate Samantha's and Lisa's total sales revenue | Amazon | ✅ | [link](easy/calculate-samanthas-and-lisas-total-sales-revenue.sql) |
| 7 | Wine varieties tasted by 'Roger Voss' | Wine Magazine | ✅ | [link](easy/wine-varieties-tasted-by-roger-voss.sql) |
| 8 | Hour Of Highest Gas Expense | Lyft | ✅ | [link](easy/hour-of-highest-gas-expense.sql) |
| 9 | Find all Lyft rides which happened on rainy days before noon | Lyft | ✅ | [link](easy/find-all-lyft-rides-which-happened-on-rainy-days-before-noon.sql) |
| 10 | Lyft Driver Wages | Lyft | ✅ | [link](easy/lyft-driver-wages.sql) |
| 11 | Artist Appearance Count | Spotify | ✅ | [link](easy/artist-appearance-count.sql) |
| 12 | Top Ranked Songs | Spotify | ✅ | [link](easy/top-ranked-songs.sql) |
| 13 | Olympics Events List By Age | ESPN | ✅ | [link](easy/olympics-events-list-by-age.sql) |
| 14 | Find all athletes who were older than 40 years when they won either Bronze or Silver | ESPN | ✅ | [link](easy/find-all-athletes-who-were-older-than-40-years-when-they-won-either-bronze-or-silver.sql) |
| 15 | Order Details | Shopify | ✅ | [link](easy/order-details.sql) |
| 16 | Departments With 5 Employees | Glassdoor | ✅ | [link](easy/departments-with-5-employees.sql) |
| 17 | April Admin Employees | Microsoft | ✅ | [link](easy/april-admin-employees.sql) |
| 18 | First Names With Six Letters Ending in 'h' | Amazon | ✅ | [link](easy/first-names-with-six-letters-ending-in-h.sql) |
| 19 | Find drafts which contains the word 'optimism' | Google | ✅ | [link](easy/find-drafts-which-contains-the-word-optimism.sql) |
| 20 | Number of violations | Yelp | ✅ | [link](easy/number-of-violations.sql) |
| 21 | Inspection For Glassell Coffee Shop | Yelp | ✅ | [link](easy/inspection-for-glassell-coffee-shop.sql) |
| 22 | Churro Activity Date | Yelp | ✅ | [link](easy/churro-activity-date.sql) |
| 23 | Most Profitable Financial Company | Forbes | ✅ | [link](easy/most-profitable-financial-company.sql) |
| 24 | MacBookPro User Event Count | Apple | ✅ | [link](easy/macbookpro-user-event-count.sql) |
| 25 | Contact Information Completeness | Salesforce | ✅ | [link](easy/contact-information-completeness.sql) |
| 26 | Users Missing Phone Numbers | Meta | ✅ | [link](easy/users-missing-phone-numbers.sql) |
| 27 | High Earners in Support Departments | Amazon | ✅ | [link](easy/high-earners-in-support-departments.sql) |
| 28 | Number of Shipments Per Month | Amazon | ✅ | [link](easy/number-of-shipments-per-month.sql) |
| 29 | Unique Users Per Client Per Month | Apple | ✅ | [link](easy/unique-users-per-client-per-month.sql) |

## Medium (33)

| # | Question | Company | Status | Solution |
|---|----------|---------|--------|----------|
| 1 | Users By Average Session Time | Meta | ✅ | [link](medium/users-by-average-session-time.sql) |
| 2 | Acceptance Rate By Date | Meta | ✅ | [link](medium/acceptance-rate-by-date.sql) |
| 3 | Finding User Purchases | Amazon | ✅ | [link](medium/finding-user-purchases.sql) |
| 4 | Risky Projects | LinkedIn | ✅ | [link](medium/risky-projects.sql) |
| 5 | Finding Purchases | Amazon | ✅ | [link](medium/finding-purchases.sql) |
| 6 | Ranking Most Active Guests | Airbnb | ✅ | [link](medium/ranking-most-active-guests.sql) |
| 7 | Number Of Units Per Nationality | Airbnb | ✅ | [link](medium/number-of-units-per-nationality.sql) |
| 8 | Find the number of inspections for each risk category by inspection type | Yelp | ✅ | [link](medium/find-the-number-of-inspections-for-each-risk-category-by-inspection-type.sql) |
| 9 | Find the percentage of shipable orders | Google | ✅ | [link](medium/find-the-percentage-of-shipable-orders.sql) |
| 10 | Meta/Facebook Matching Users Pairs | Meta | ✅ | [link](medium/meta-facebook-matching-users-pairs.sql) |
| 11 | Matching Similar Hosts and Guests | Airbnb | ✅ | [link](medium/matching-similar-hosts-and-guests.sql) |
| 12 | Income By Title and Gender | LinkedIn | ✅ | [link](medium/income-by-title-and-gender.sql) |
| 13 | Top Cool Votes | Yelp | ✅ | [link](medium/top-cool-votes.sql) |
| 14 | Reviews of Categories | Yelp | ✅ | [link](medium/reviews-of-categories.sql) |
| 15 | Top Businesses With Most Reviews | Yelp | ✅ | [link](medium/top-businesses-with-most-reviews.sql) |
| 16 | Find all possible varieties which occur in either of the winemag datasets | Wine Magazine | ✅ | [link](medium/find-all-possible-varieties-which-occur-in-either-of-the-winemag-datasets.sql) |
| 17 | Highest Target Under Manager | Salesforce | ✅ | [link](medium/highest-target-under-manager.sql) |
| 18 | Highest Salary In Department | Asana | ✅ | [link](medium/highest-salary-in-department.sql) |
| 19 | Employee and Manager Salaries | Walmart | ✅ | [link](medium/employee-and-manager-salaries.sql) |
| 20 | Second Highest Salary | Dropbox | ✅ | [link](medium/second-highest-salary.sql) |
| 21 | Titanic Survivors and Non-Survivors | Google | ✅ | [link](medium/titanic-survivors-and-non-survivors.sql) |
| 22 | Duplicate HR Department Employees | Amazon | ✅ | [link](medium/duplicate-hr-department-employees.sql) |
| 23 | Employees With the Same Salary | Amazon | ✅ | [link](medium/employees-with-the-same-salary.sql) |
| 24 | Count Occurrences Of Words In Drafts | Google | ✅ | [link](medium/count-occurrences-of-words-in-drafts.sql) |
| 25 | Make the friends network symmetric | Google | ✅ | [link](medium/make-the-friends-network-symmetric.sql) |
| 26 | Processed Ticket Rate By Type | Meta | ✅ | [link](medium/processed-ticket-rate-by-type.sql) |
| 27 | Top 10 Songs 2010 | Spotify | ✅ | [link](medium/top-10-songs-2010.sql) |
| 28 | Customers with Large Orders | Netflix | ✅ | [link](medium/customers-with-large-orders.sql) |
| 29 | Department Workforce Analysis | Google | ✅ | [link](medium/department-workforce-analysis.sql) |
| 30 | Salary Less Than Twice The Average | Walmart | ✅ | [link](medium/salary-less-than-twice-the-average.sql) |
| 31 | Flags per Video | Netflix | ✅ | [link](medium/flags-per-video.sql) |
| 32 | Maximum of Two Numbers | Deloitte | ✅ | [link](medium/maximum-of-two-numbers.sql) |
| 33 | Share of Active Users | Meta | ✅ | [link](medium/share-of-active-users.sql) |

## Hard (4)

| # | Question | Company | Status | Solution |
|---|----------|---------|--------|----------|
| 1 | Consecutive Days | Netflix | ✅ | [link](hard/consecutive-days.sql) |
| 2 | Best Selling Item | Best Buy | ✅ | [link](hard/best-selling-item.sql) |
| 3 | Rank Variance Per Country | Meta | ✅ | [link](hard/rank-variance-per-country.sql) |
| 4 | Monthly Percentage Difference | Amazon | ✅ | [link](hard/monthly-percentage-difference.sql) |

**Legend:** ✅ Solved · 🟡 In progress · ⬜ Not started

---

## How I work through a question

1. Read the prompt + schema carefully on StrataScratch, sketch the expected output on paper
2. Write the query, test it against the sample data
3. Save the solution in the right folder (`easy/`, `medium/`, `hard/`) with the question comment header
4. Update the status in this README's table
5. If it introduced a new concept/trick, log it in [`notes/learnings.md`](notes/learnings.md)

## Notes

See [`notes/learnings.md`](notes/learnings.md) for recurring SQL patterns (window functions, joins, self-joins, date filtering, string matching, ranking, etc.) picked up while solving these questions.
