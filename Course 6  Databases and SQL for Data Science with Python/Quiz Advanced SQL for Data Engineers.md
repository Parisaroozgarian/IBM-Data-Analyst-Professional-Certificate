# Graded Quiz: Advanced SQL for Data Engineers

## Question 1
Consider the following question from the lab:  
“Write and execute a SQL query to list the school names, community names, and average attendance for communities with a hardship index of 98.”
	
Which two of the following statements would be the correct ways to use the Join clause on the required tables from the database to generate this query?  
- [x] `FROM chicago_public_schools RIGHT JOIN chicago_socioeconomic_data ON a.community_area_number = b.community_area_number`  
- [x] `FROM chicago_socioeconomic_data a LEFT JOIN chicago_public_schools b ON a.community_area_number = b.community_area_number`  
- [ ] `FROM chicago_socioeconomic_data a LEFT JOIN chicago_public_schools b ON community_area_number = community_area_number`  
- [x] `FROM chicago_public_schools a RIGHT JOIN chicago_socioeconomic_data b ON a.community_area_number = b.community_area_number`  

---

## Question 2
Consider the following question from the lab:  
“Write and execute a SQL query to list all crimes that took place at a school. Include case number, crime type, and community name.”

How many rows were returned upon execution of this query?  
- [ ] 12  
- [x] 10  
- [ ] 14  
- [ ] 18  

---

## Question 3
Consider the following question from the lab:  
“Write and execute a SQL statement to create a view showing the columns listed in the following table, with new column names as shown in the second column.”

Which of the following is the correct method of creating the required view?  
- [x] `CREATE VIEW SCHOOL_DATA AS SELECT NAME_OF_SCHOOL AS School_Name, Safety_Icon AS Safety_Rating, Family_Involvement_Icon AS Family_Rating, Environment_Icon AS Environment_Rating, Instruction_Icon AS Instruction_Rating, Leaders_Icon AS Leaders_Rating, Teachers_Icon AS Teachers_Rating FROM chicago_public_schools;`  
- [ ] `SELECT VIEW SCHOOL_DATA AS SELECT NAME_OF_SCHOOL AS School_Name, Safety_Icon AS Safety_Rating, Family_Involvement_Icon AS Family_Rating, Environment_Icon AS Environment_Rating, Instruction_Icon AS Instruction_Rating, Leaders_Icon AS Leaders_Rating, Teachers_Icon AS Teachers_Rating FROM chicago_public_schools;`  
- [ ] `CREATE VIEW SCHOOL_DATA AS SELECT NAME_OF_SCHOOL AS School_Name, Safety_Icon AS Safety_Rating, Family_Involvement_Icon AS Family_Rating, Environment_Icon AS Environment_Rating, Instruction_Icon AS Instruction_Rating, Leaders_Icon AS Leaders_Rating, Teachers_Icon AS Teachers_Rating WHERE chicago_public_schools;`  
- [ ] `CREATE VIEW SCHOOL_DATA IN SELECT NAME_OF_SCHOOL IN School_Name, Safety_Icon IN Safety_Rating, Family_Involvement_Icon IN Family_Rating, Environment_Icon IN Environment_Rating, Instruction_Icon IN Instruction_Rating, Leaders_Icon IN Leaders_Rating, Teachers_Icon IN Teachers_Rating FROM chicago_public_schools;`  

---

## Question 4
Consider the following question from the lab:  
“Write and execute a SQL statement that returns just the school name and leaders rating from the view.”

Assuming that the said view was named ‘SCHOOL_DATA,’ which of the following would be the correct query for this question?  
- [x] `SELECT School_Name, Leaders_Rating FROM SCHOOL_DATA;`  
- [ ] `SELECT School_Name, Leaders_Rating FROM chicago_public_schools;`  
- [ ] `SELECT NAME_OF_SCHOOL AS School_Name, Leaders_Icon AS Leaders_Rating FROM chicago_public_schools;`  
- [ ] `SELECT NAME_OF_SCHOOL AS School_Name, Leaders_Icon AS Leaders_Rating FROM SCHOOL_DATA;`  

---

## Question 5
Consider the following question from the lab:  
“Write the structure of a query to create or replace a stored procedure called UPDATE_LEADERS_SCORE that takes a in_School_ID parameter as an integer and a in_Leader_Score parameter as an integer.”

For creating this stored procedure, which of the following will be a requirement?  
- [x] Changing the delimiter before the Stored Procedure is initiated and changing it back after the code is complete.  
- [ ] All of them are required.  
- [x] BEGIN and END statements between which the procedure commands will be written.  
- [x] Specifying the data type of each input argument to the stored procedure.  

---

## Question 6
Consider the following question from the lab:  
“Inside your stored procedure, write a SQL statement to update the Leaders_Score field in the CHICAGO_PUBLIC_SCHOOLS table for the school identified by in_School_ID to the value in the in_Leader_Score parameter.”

Which one of the following is the correct query that goes in the stored procedure statement?  
- [ ] `UPDATE CHICAGO_PUBLIC_SCHOOLS SET in_Leader_Score = "Leaders_Score" WHERE in_School_ID = "School_ID";`  
- [x] `UPDATE CHICAGO_PUBLIC_SCHOOLS SET "Leaders_Score" = in_Leader_Score WHERE "School_ID" = in_School_ID;`  
- [ ] `ALTER CHICAGO_PUBLIC_SCHOOLS SET in_Leader_Score = "Leaders_Score" WHERE in_School_ID = "School_ID";`  
- [ ] `ALTER CHICAGO_PUBLIC_SCHOOLS SET "Leaders_Score" = in_Leader_Score WHERE "School_ID" = in_School_ID;`  

---

## Question 7
Consider the following question from the lab:  
“Inside your stored procedure, write a SQL IF statement to update the Leaders_Icon field in the CHICAGO_PUBLIC_SCHOOLS table for the school identified by in_School_ID using the following information.”

Which of the following code snippets can be a part of the IF structure created for this stored procedure?  
- [x] `ELSEIF in_Leader_Score < 80 THEN UPDATE CHICAGO_PUBLIC_SCHOOLS SET "Leaders_Icon" = 'Average';`  
- [ ] `ELSEIF in_Leader_Score < 60 THEN UPDATE CHICAGO_PUBLIC_SCHOOLS SET "Leaders_Icon" = 'Strong';`  
- [ ] `ELSEIF in_Leader_Score < 40 THEN UPDATE CHICAGO_PUBLIC_SCHOOLS SET "Leaders_Icon" = 'Weak';`  
- [ ] `IF in_Leader_Score > 10 AND in_Leader_Score < 20 THEN UPDATE CHICAGO_PUBLIC_SCHOOLS SET "Leaders_Icon" = 'Very Weak';`  

---

## Question 8
Consider the following question from the lab:  
“Write a query to call the stored procedure, passing a valid school ID and a leader score of 50, to check that the procedure works as expected.”

Assuming that the school ID is “610281”, which of the following is the correct way to execute the stored procedure “UPDATE_LEADERS_SCORE”?  
- [ ] `UPDATE_LEADERS_SCORE(610281, 50)`  
- [ ] `RUN UPDATE_LEADERS_SCORE(610281, 50)`  
- [x] `CALL UPDATE_LEADERS_SCORE(610281, 50)`  
- [ ] `EXEC UPDATE_LEADERS_SCORE(610281, 50)`  

---

## Question 9
Consider the following question from the lab:  
“Update your stored procedure definition. Add a generic ELSE clause to the IF statement that rolls back the current work if the score did not fit any of the preceding categories.”

What will be the nature of the edit that will be done to the stored procedure?  
- [x] A generic ELSE clause is added with the statement “ROLLBACK WORK” to the IF ELSE structure.  
- [ ] A generic ELSE clause is added with the statement “ROLL_BACK WORK” to the IF ELSE structure.  
- [ ] A generic ELSE clause is added with the statement “ROLL BACK” to the IF ELSE structure.  
- [ ] A generic ELSE clause is added with the statement “ROLLBACK” to the IF ELSE structure.  


---

## Question 10
Consider the following question from the lab:  
“Update your stored procedure definition again. Add a statement to commit the current unit of work at the end of the procedure.”

What will be the nature of the edit that will be done to the stored procedure?  
- [ ] Add the statement “COMMIT” before the IF ELSE statement structure.  
- [ ] Add the statement “COMMIT WORK”.  
- [ ] Add the statement “COMMIT WORK” before the IF ELSE statement structure.  
- [x] Add the statement “COMMIT WORK” after the IF ELSE statement structure.  

---
