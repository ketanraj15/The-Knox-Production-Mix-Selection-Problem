# The-Knox-Production-Mix-Selection-Problem-
## The Knox Production-Mix Selection Problem - A Fuzzy Approach
<br /> Supervisor:Dr Prabhjot Kaur
<br /> Authored By:
<br />Pravahan Jaivili   	(IMH/10046/18)
<br />Ketan Raj 		(IMH/10015/18)

## Abstract 
In problems of classical system analysis, it is ubiquitous to treat imprecision by the use of probability theory. It is becoming increasingly clear, however, that in the case of many real world problems involving large scale systems such as economic systems, social systems, mass service systems, etc., the major source of imprecision should more properly be labeled ‘fuzziness’ rather than ‘randomness.’ By fuzziness, we mean the type of imprecision which is associated with the lack of sharp transition from membership to nonmembership, as in tall men, small numbers, likely events, etc. In our approach, the emphasis is on mathematical programming and the use of the concept of a level set to extend some of the classical results to problems involving fuzzy constraints and objective functions.

## The Knox production-Mix Selection Problem (Verdegays Model)
Let us consider a product-mix selection problem . Suppose that the Knox Mix company has the option of using one or more of four different types of production processes. The first and second processes yield items of product A, and the third and fourth yield items of product B. The inputs for each process are labor measured in man-weeks, pounds of material Y, and boxes of material Z. Since each process varies in its input requirements, the 81 profitabilities of the process differ, even for processes producing the same item. The manufacturer's decision on a week's production schedule is limited in the range of possibilities by the available amounts of manpower and both kinds of raw materials.

![alt text](Images/Problem_image.PNG)

## Formulation of Optimization Problem

With production levels in processes 1, 2, 3, 4 as x1, x2, x3, x4 respectively. The problem can then be formulated as <br />
z = 4x1 + 5x2 + 9x3 + 11x4			(Profit)<br />
       Max z subject to constraints <br />
g1(x)  =   x1 + x2 + x3 + x4   <  15			(Man Weeks) <br />
g2(x)  =   7x1 + 5x2 + 3x3 + 2x4  <  120		(Material Y) <br />
g3(x)  =   3x1 + 5x2 + 10x3 + 15x4  < 100		(Material Z) <br />

We then solve this linear programming problem by use of the Simplex Method - (using Tora Software) . The optimal solution is: 

![alt text](Images/Simplex_image.PNG)

```x* = (50 / 7, 0, 55 / 7, 0)  =  (7.14, 0, 7.86, 0) and z* = $ 695 / 7 = $99.29. The actual resources used are  15, 73.57 and 100 units for manweeks, material Y and material Z, respectively``` 

Let us assume that the available  constraints in the above problem are imprecise with a tolerance of 25%. Then the membership function of fuzzy constraints are

```
                     1					if g1(x)  <  15
μ1(x) =    1 - [ (g1(x) - 15) / 4]        		if 15 <  g1(x)  <  1
                     0					if g1(x)  >  19
              
```
![alt text](Images/graph1.PNG)

```
                     1				      	if g2(x) < 120
μ2(x) =     1 - [ (g2(x) - 120) / 30]        	       if 120 <  g2(x)  <  150
	              0					if g2(x) > 150
              
```
![alt text](Images/graph2.PNG)

``` 
      	       1				     	if g3(x) < 100
μ3(x) =    1 - [ (g3(x) - 100) / 25]        	if 100 <  g3(x)  <  125
	       0				   	if g3(x) > 125

```
![alt text](Images/graph3.PNG)

