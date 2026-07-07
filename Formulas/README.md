#Formulas
This folder contains Excel formula examples of commonly used Microsoft Excel Formulas

## Example 1 : IF Function

### Objective
Determine whether an employe is eligible for a Bonus.

### Sample Data
Employee ID	| Name	| Department	| Salary	| Formula	                                  | Result
1001	        Amit	  HR	          45000.00	=IF(D2>=40000,"Eligible","Not Eligible")    Eligible
1002	        Priya	  Sales	        25000.00	=IF(D2>=40000,"Eligible","Not Eligible")	  Not Eligible
1003	        Rahul	  Sales	        58000.00	=IF(D2>=40000,"Eligible","Not Eligible")	  Eligible
1004	        Neha	  IT	          34000.00	=IF(D2>=40000,"Eligible","Not Eligible")	  Not Eligible
1005	        Neeta	  Finance	      61000.00	=IF(D2>=40000,"Eligible","Not Eligible")	  Eligible

### Formula
=IF(D2>=40000,"Eligible","Not Eligible")

### Explanation
-Check whether the salary is greater than or equal to 40000.
-Return **Eligible** if the condition is true.
-Return **Not Eligible** if the condition is false.

### Learning Outcome
After completing this example, you will understand:
-IF syntax
-Logical conditions
-Returning different values based on a condition
