# Graded Quiz: Views, Stored Procedures, and Transactions

## Question 1
A stored procedure can:  
- [x] Be written in different languages  
- [x] Accept information  
- [x] Return results  
- [x] All of the above  

---

## Question 2
What does ACID stand for?  
- [ ] Atomic, Consistent, Initiated, Duplicated  
- [ ] Asynchronous, Complete, Individual, Direct  
- [x] Atomic, Consistent, Isolated, Durable  
- [ ] Alternative, Creative, Isolated, Durable  

---

## Question 3
Which of the following SQL statements will create a view named EMP_VIEW with an employee’s First name, last name, and ID, based on the EMPLOYEES tables?  
- [x] `CREATE VIEW EMP_VIEW (EMP_ID, FIRSTNAME, LASTNAME) AS SELECT EMP_ID, F_NAME, L_NAME FROM EMPLOYEES;`  
- [ ] `CREATE VIEW EMP_VIEW (EMP_ID, FIRSTNAME, LASTNAME) AS SELECT EMP_ID, F_NAME, L_NAME;`  
- [ ] `NEW VIEW EMP_VIEW (EMP_ID, FIRSTNAME, LASTNAME) AS SELECT EMP_ID, F_NAME, L_NAME FROM EMPLOYEES;`  
- [ ] `CREATE VIEW EMP_VIEW (EMP_ID, FIRSTNAME, LASTNAME) FROM EMPLOYEES;`  

---

## Question 4
Which of the following SQL statements will create a view that lists only the employees in department number 7?  
- [x] `CREATE VIEW EMP_VIEW (EMP_ID, FIRSTNAME, LASTNAME) AS SELECT EMP_ID, F_NAME, L_NAME FROM EMPLOYEES WHERE DEP_ID = 7;`  
- [ ] `CREATE VIEW EMP_VIEW (EMP_ID, FIRSTNAME, LASTNAME) WHERE DEP_ID = 7 AS SELECT EMP_ID, F_NAME, L_NAME FROM EMPLOYEES;`  
- [ ] `CREATE VIEW EMP_VIEW (EMP_ID, FIRSTNAME, LASTNAME) AS SELECT EMP_ID, F_NAME, L_NAME WHERE DEP_ID = 7;`  
- [ ] `CREATE VIEW EMP_VIEW (EMP_ID, FIRSTNAME, LASTNAME) AS SELECT EMP_ID, F_NAME, L_NAME FROM EMPLOYEES IF DEP_ID = 7;`  

---

## Question 5
You are developing an application that helps users transfer money from one bank account to another. In tests, the source account is debited, but the target account is not credited. Which of the following SQL commands undoes all the changes made during the transfer to leave the database in a stable state?  
- [ ] DROP  
- [x] ROLLBACK  
- [ ] COMMIT  
- [ ] BEGIN  

---
