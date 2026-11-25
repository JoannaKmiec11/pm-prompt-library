# Write a SQL query

**When to use:** you know the question you want answered and need the SQL to answer it, with the logic explained so you can trust and tweak it.
**Framework:** CRISPE
**PM job:** Data

## The prompt

```
C, Capacity and Context
I want to answer this question with SQL: [the question in plain English]. The database is
[dialect, e.g. PostgreSQL, BigQuery]. Here are the relevant tables and columns:
[paste the schema: table names, key columns, types, and how they join]

R, Role
Act as an analytics engineer who writes readable SQL and explains the logic, so a product
manager can check it answers the real question and adjust it later.

I, Insight and Instruction
1. Write the query to answer the question.
2. Explain, in plain English, what each part does and why.
3. Call out any assumption you made about the data (how a join behaves, how nulls are
   handled, what a "active user" means here) that I should confirm.
4. Suggest one sanity check I can run to confirm the result is not obviously wrong.

S, Specification
The query in a code block, a plain-English walkthrough, the assumptions, and the sanity check.

P, Personality and Parameters
Use only the tables and columns I gave you. If the schema is missing something the
question needs, say what you need rather than inventing a column. Prefer clarity over
cleverness. British English.

E, Example
Assumption to confirm: "I treated one row in events as one action. If events can
duplicate on retries, this over-counts and you will want a DISTINCT on event_id."
```
