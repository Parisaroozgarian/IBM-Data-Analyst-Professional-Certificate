# Graded Assignment: Final Exam

## Question 1
The ______ statement is called a query, and the output we get from executing the query is called a result set.  
- [ ] DROP DATABASE  
- [x] SELECT  
- [ ] ALTER  
- [ ] CREATE TABLE  

---

## Question 2
Which of the following SQL statements will delete the customers where the Country is Italy?  
- [ ] DELETE ‘ITALY’ FROM CUSTOMERS  
- [x] DELETE FROM CUSTOMERS WHERE COUNTRY = ‘ITALY’  
- [ ] DELETE FROM CUSTOMERS WHERE COUNTRY IS ‘ITALY’  
- [ ] DELETE COUNTRY ‘ITALY’ FROM CUSTOMERS  

---

## Question 3
What uniquely identifies each row in a table?  
- [ ] The columns  
- [ ] The textual data  
- [x] The primary key of a relational table  
- [ ] The secondary key of a relational table  

---

## Question 4
The basic categories of the SQL commands based on functionality are ________ and Data Manipulation Language (DML).  
- [x] Data Definition Language (DDL)  
- [ ] Data Entry Language (DEL)  
- [ ] Data Update Language (DUL)  
- [ ] Data Input Language (DIL)  

---

## Question 5
When querying a table called Author that contains a list of authors and their city of residence, which of the following queries will return the number of authors from each city?  
- [x] SELECT City, COUNT(City) FROM Author GROUP BY City  
- [ ] SELECT DISTINCT(City) FROM Author  
- [ ] SELECT City, COUNT(City) FROM Author  
- [ ] SELECT City, DISTINCT(City) FROM Author GROUP BY City  

---

## Question 6
You want to retrieve a list of books that have between 450 and 600 pages. Which clause would you add to the following SQL statement: SELECT Title, Pages FROM Book ________________________________  
- [ ] WHERE Pages = 450  
- [ ] IF Pages >= 450 and Pages <= 600  
- [ ] WHERE Pages 450 – 600  
- [x] WHERE Pages >= 450 and Pages <= 600  

---

## Question 7
Which of the following queries will retrieve the HIGHEST value of PRICE in a table called PRODUCTS?  
- [ ] SELECT MOST(PRICE) FROM PRODUCTS  
- [ ] SELECT MIN(PRICE) FROM PRODUCTS  
- [x] SELECT MAX(PRICE) FROM PRODUCTS  
- [ ] SELECT HIGHEST(PRICE) FROM PRODUCTS  

---

## Question 8
Which of the following queries will retrieve the PRODUCT NAME that has the highest price?  
- [ ] SELECT PRODUCT_NAME FROM PRODUCTS WHERE UNIT_PRICE = MAX  
- [x] SELECT PRODUCT_NAME FROM PRODUCTS WHERE UNIT_PRICE = (SELECT MAX(UNIT_PRICE) FROM PRODUCTS)  
- [ ] SELECT PRODUCT_NAME FROM PRODUCTS WHERE UNIT_PRICE IS HIGHEST  
- [ ] SELECT MAX(UNIT_PRICE) FROM PRODUCTS  


---

## Question 9
A ____________ is a control structure that enables traversal over the records in a database.  
- [x] Database cursor  
- [ ] Connection  
- [ ] Import  
- [ ] Primary key  

---

## Question 10
What is missing in the following statement, that is meant to load the information of a dataframe to a table in a database? “df.to_sql(‘Sample’,__________)  
- [ ] Reference to dataframe  
- [ ] Data cursor  
- [ ] Table name  
- [x] Connection object  

---
