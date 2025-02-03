In [[Pandas]], a **data offset** allows you to manipulate `datetime` objects by shifting them based on specific time intervals or business rules.

## Common types of Offsets 

- `DateOffset`: A general offset to shift dates by a specific amount (e.g., add 5 days).
- `MonthEnd`, `MonthBegin`: Shift to the end or beginning of the month.
- `BMonthEnd`, `BMonthBegin`: Similar to `MonthEnd`/`MonthBegin`, but for business months.
- `BusinessDay`: Shifts by a certain number of business days (ignores weekends/holidays).
- `Week`: Shifts by full weeks, and so on.