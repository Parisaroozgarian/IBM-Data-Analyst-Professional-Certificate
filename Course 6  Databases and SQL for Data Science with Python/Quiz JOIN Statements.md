# Graded Quiz: JOIN Statements

## Question 1
An INNER JOIN returns only the rows that match. (T/F)  
- [x] True  
- [ ] False  

---

## Question 2
A LEFT OUTER JOIN displays all the rows from the right table and combines matching rows from the left table. (T/F)  
- [ ] True  
- [x] False  

---

## Question 3
When using an OUTER JOIN, you must explicitly state what kind of OUTER JOIN you want - a LEFT JOIN, a RIGHT JOIN, or a FULL JOIN. (T/F)  
- [x] True  
- [ ] False  

---

## Question 4
Which of the following are valid types of JOINs?  
- [x] LEFT OUTER JOIN  
- [x] RIGHT OUTER JOIN  
- [x] FULL OUTER JOIN  
- [ ] FULL LEFT JOIN  

---

## Question 5
A FULL JOIN returns only the rows that match. (T/F)  
- [ ] True  
- [x] False  

---

## Question 6
Which of the following is true about INNER JOINS?  
- [x] Return relevant entries from multiple tables based on corresponding columns between them.  
- [ ] Return all rows from multiple tables based on primary key columns between them.  
- [ ] Return all rows from multiple tables.  
- [ ] Return all rows from multiple tables with matching rows.  

---

## Question 7
Consider the following query:  

```sql
SELECT COLUMN1, COLUMN2
FROM TABLE1 A
LEFT JOIN TABLE2 B
ON A.COLUMN_NAME = B.COLUMN_NAME
```

What is the expected output?  
- [ ] Only COLUMN1 and COLUMN2 from the 2 tables are retrieved for corresponding entries of COLUMN_NAME in TABLE1 and TABLE2  
- [x] All relevant entries from TABLE1 are retained, along with a few entries from TABLE2 with matching entries in COLUMN_NAME for TABLE1 and TABLE2  
- [ ] All relevant entries from TABLE2 are retained, along with a few entries from TABLE1 with matching entries in COLUMN_NAME for TABLE1 and TABLE2  
- [ ] All entries of COLUMN1 and COLUMN2 from TABLE1 and TABLE2 are retrieved.  


---

## Question 8
In MySQL, how is a FULL OUTER JOIN implemented?  
- [ ] Using the keyword FULL JOIN  
- [x] Using a UNION of LEFT and RIGHT JOINS  
- [ ] Using the keyword JOIN  
- [ ] Using the keyword FULL OUTER JOIN  

---

## Question 9
For Joins to work, which of the following is a valid statement about the columns with corresponding values?  
- [ ] The columns in the two tables must have the same names.  
- [ ] The columns in the two tables must have different names.  
- [x] The columns in the two tables may have the same or different names.  
- [ ] The columns in the two tables must have exact the same values.  

---

## Question 10
If the rows in the joined tables do not match, the result set of the full outer join contains _____ values for every column of the table that lacks a matching row.  
- [x] NULL  
- [ ] Zero  
- [ ] NAN  
- [ ] random  

---
