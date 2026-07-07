#Formulas
This folder contains Excel formula examples of commonly used Microsoft Excel Formulas

## Example 1 : Basic IF Function

### Objective
Determine whether an employee is eligible for a Bonus.

### Sample Data
- Employee ID	| Name	| Department	| Salary	  | Formula	                                  | Result
- 1001	      | Amit	| HR	        | 45000.00	| =IF(D2>=40000,"Eligible","Not Eligible")  | Eligible
- 1002	      | Priya	| Sales	      | 25000.00	| =IF(D3>=40000,"Eligible","Not Eligible")	| Not Eligible
- 1003	      | Rahul	| Sales	      | 58000.00	| =IF(D4>=40000,"Eligible","Not Eligible")	| Eligible
- 1004	      | Neha	| IT	        | 34000.00	| =IF(D5>=40000,"Eligible","Not Eligible")	| Not Eligible
- 1005	      | Neeta	| Finance	    | 61000.00	| =IF(D6>=40000,"Eligible","Not Eligible")	| Eligible

### Formula
=IF(D2>=40000,"Eligible","Not Eligible")

### Explanation
- Check whether the salary is greater than or equal to 40000.
- Return **Eligible** if the condition is **true**.
- Return **Not Eligible** if the condition is **false**.

### Learning Outcome
After completing this example, you will understand:
- IF syntax
- Logical conditions
- Returning different values based on a condition

--------------------------------------------------------------------------------------------------------------------------------------------------------------

## Example 2 : Nested IF Function

### Objective
Determine department wise bonus scale.

### Sample Data
- Employee ID	| Name	| Department	| Salary	  | Formula	                                                                                          | Result
- 1001	      | Amit	| IT	        | 75000.00	| =IF(C2="IT",IF(D2>=70000,"High Bonus",IF(D2>=40000,"Normal Bonus","No Bonus")),"Not Eligible")    | High Bonus
- 1002	      | Priya	| Sales	      | 25000.00	| =IF(C3="IT",IF(D3>=70000,"High Bonus",IF(D3>=40000,"Normal Bonus","No Bonus")),"Not Eligible")	  | Not Eligible
- 1003	      | Rahul	| Sales	      | 58000.00	| =IF(C4="IT",IF(D4>=70000,"High Bonus",IF(D4>=40000,"Normal Bonus","No Bonus")),"Not Eligible")	  | Not Eligible
- 1004	      | Neha	| IT	        | 44000.00	| =IF(C5="IT",IF(D5>=70000,"High Bonus",IF(D5>=40000,"Normal Bonus","No Bonus")),"Not Eligible")	  | Normal Bonus
- 1005	      | Neeta	| IT    	    | 30000.00	| =IF(C6="IT",IF(D6>=70000,"High Bonus",IF(D6>=40000,"Normal Bonus","No Bonus")),"Not Eligible")	  | No Bonus

### Formula
=IF(C2="IT",IF(D2>=70000,"High Bonus",IF(D2>=40000,"Normal Bonus","No Bonus")),"Not Eligible")

### Explanation
- Check whether the department is "IT" and based on salary , bonus scale set.
- Check if the **employee's department** is **IT**.
- If **No** returns **Not Eligible**.
- If **Yes**, then:
  - **Salary>=70000** -> return **High Bonus**.
  - **Salary>=40000** -> return **Normal Bonus**.
  - else return **No Bonus**.
  
### Learning Outcome
After completing this example, you will understand:
- Nested IF syntax
- Logical conditions
- Returning different values based on different condition
