# budget-planner
a net pay calculator with an expenditure input that gives the user the amount of money they remain with after every deduction is made
# here are the rates used
# 1 nhif
Employee's Monthly Gross Salary(Kshs)	Monthly NHIF Contribution (Kshs)
5,999	150
6,000 - 7,999	300
8,000 - 11,999	400
12,000 - 14,999	500
15,000 - 19,999	600
20,000 - 24,999	750
25,000 - 29,999	850
30,000 - 34,999	900
35,000 - 39,999	950
40,000 - 44,999	1,000
45,000 - 49,999	1,100
50,000 - 59,999	1,200
60,000 - 69,999	1,300
70,000 - 79,999	1,400
80,000 - 89,999	1,500
90,000 - 99,999	1,600
100,000 and above	1,700

# nssf
To find the Kenya NSSF Rate  using 6% of the Gross Salary. BUT ONLY A MINIMUM OF 18,000 Gross Salary CAN BE USED IN NSSF. 

# nhdf
NHDF = gross_salary *  0.015

# taxable_income

taxable_income = gross salary - (NSSF + NHDF + NHIF) 

# payee
Monthly Bands of Taxable Income (KES)	Tax Rate
0 – 24,000	10%
On the next 8,333	25%
On the next 467,667	30%
On the next 300,000	32.5%
On amounts over 800,000	35%
Personal Relief: KES 2,400.00 per month
Minimum Taxable Income: KES 24,001.00 per month

# net pay
 net_salary = gross_salary - (nhif + nhdf +  nssf + payee-relief)

# remnant
net pay -expenditure