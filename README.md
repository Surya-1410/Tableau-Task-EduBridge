# Tableau-Task-EduBridge

Step 1: Import the excel dataset which we are going to workout

In Excel the Attributes and Values be  

                     Emp_name	Id      Salary
                     Ravish	  10	  1000
                     Suresh	  101	  20000
                     Priya	  1010	50000
                     Neha   	10101	70000
                     Nitin	 1101 	15000
                     
Step 2: After importing the Excel file. Go to sheet 1

Step 3: Drag and drop the Table Attributes/features to the Rows to display table in the workbook page to start a new calculation

Step 4: After Inserting the required values and select the Create Calculated Field.

Step 5: In that dialogue box we can name it as Employee Id (Id) and the syntax for the calculation is

        LEFT('0000000',( 7 - LEN(STR([Emp id]))))
        +
        STR([Emp Id])
 
 Step 6: We can also add that calculation to the table by drag n drop to the Rows

             Emp_name	Id	Employee_Id	Salary
             Ravish	10	0000010 	1000
             Suresh	101	0000101 	20000
             Priya	1010	0001010 	50000
             Neha	10101	0010101 	70000
             Nitin	1101	0001101         15000
             
all Employee Id (Id) a 7-digit number in Tableau.
