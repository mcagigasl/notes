ACID stands for Atomicity, Consistency, Isolation and Durability, the four key properties that ensure reliable transaction processing in **database management systems ([[Database Management Systems]])**, particularly in traditional **relational databases**. These properties guarantee that database transactions are processed reliably and ensure data integrity, even in the event of errors, power failures, or crashes.

Here’s what each letter in **ACID** stands for:

### 1. **A - Atomicity**

- **Definition**: A transaction is an atomic unit of work. This means that either **all operations** in a transaction are completed successfully, or **none** are applied. If any part of the transaction fails, the entire transaction is **rolled back** to its previous state, ensuring that no partial updates are made to the database.
- **Example**: If you are transferring money from one bank account to another, the transaction will ensure that either the **entire transaction** (debit from one account and credit to another) is successful or **neither action** occurs if there is an error.

### 2. **C - Consistency**

- **Definition**: A transaction must take the database from one **valid state** to another. It ensures that any transaction will bring the database into a consistent state, adhering to all the defined rules, constraints, and integrity checks (e.g., foreign keys, unique constraints, etc.).
- **Example**: If a database enforces that the total balance of all accounts must always equal a specific value, a transaction should maintain this consistency rule. If an account balance is debited and credited, the sum of all balances should still be consistent with this rule.

### 3. **I - Isolation**

- **Definition**: Transactions are executed in isolation from one another. Even if multiple transactions occur simultaneously, the intermediate state of one transaction is **invisible** to others. This prevents issues such as **dirty reads**, where a transaction reads uncommitted data from another transaction.
- **Example**: If two people try to withdraw money from the same bank account at the same time, isolation ensures that one transaction completes before the other can proceed, preventing both from accessing the same balance simultaneously.

### 4. **D - Durability**

- **Definition**: Once a transaction is **committed**, its changes are permanent, even in the event of a system crash or failure. The data is written to persistent storage (like a disk) and will not be lost.
- **Example**: If you transfer money and the transaction is successfully completed, the updated balances will be stored in the database. Even if the system crashes immediately after the transaction completes, the changes (e.g., the debited and credited amounts) will persist after the system is restored.