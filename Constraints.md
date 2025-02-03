In the [[Relational Data Model]]constraints encopass rules or conditions applied to the database data, ensuring data integrity, consistency and adherence to [[Business Rules]].

Theoretically,  constraints are boolean expressions. If all constraints evaluate as true, the database is consistent; otherwise, it is inconsistent. If a change to a database's relvars would leave the database in an inconsistent state, that change is illegal and must not succeed.

Constraints are defined in the table ***table_constrains*** in the information scheme

## Types of Constraints

- **Domain Constraints:**

	- Define the valid values that an attribute (column) can hold.
	- Specify the data type (e.g., integer, string, date) and any additional restrictions (e.g., range of values, allowed patterns).

- **[[Keys]] Constraints**
	- [[Primary Keys]]
		- [[Natural Keys]]
		- [[Surrogate Keys]]
	- [[Foreign Key]]

There are other types of constraints such as: 

- Entity Integrity Constraints
- Referencial Integrity Constraints
- Tuple Uniqueness Constraints