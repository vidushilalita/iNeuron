## Assignment Part-1
Q1. Why do we call Python as a general purpose and high-level programming language?


Python is called a general purpose programming language due to the large numbers of modules and libraries offered that provide a wide range of
 functionalities as per the field where it is being used. 
It is easier to learn as compared to other Object Oriented Programming languages such as Java , C++, etc .
It is also called high level programming as it easier to understand and the semantics are closer to human language (English) than machine readable 
language (binary).

Q2. Why is Python called a dynamically typed language?

Python is called dyally typed language because it allows you to declare and assign a variable as you code.
 The data type of the variable is determined during runtime 


Q3. List some pros and cons of Python programming language?

Pros:

1.	Python is open source  and is beginner friendly.It is verbose language and reading python is similar to reading English
2.	It has a large community which makes it easier to seek out help from experienced developers and professionals
3.	Embeddable. There can support implementation of other languages e.g. Cython(C,C++) , Jython(Java)
4.	Extensive Libraries : It features extensive libraries containing code for various purposes like document-generation , 
	regular expressions ,web browsers etc .One doesn’t need to write code for every purpose manually
5.	Highly scalable
6.	Python is WORA(Write Once Run Anywhere) ie it is platform independent

Cons:

1.	 It is a slower language than other compiled languages
2.	It is not 100% secure . There is no concept of private , public, secured functions.
3.	It has high memory usage and garbage collection
4.	Being Dyally typed language,it is prone to human and logic error
5.	Python is unsuitable for complicated designs 



Q4. In what all domains can we use Python?



Python is most commonly used in the following domains due to extensive libraries it features:-

Data Science
Data Analysis and Visualization
Web Development
Testing and Automation
DataWarehousing
Game Development
Machine Learning
Natural Language Processing
Search Engine Optimisation

Q5. What are variable and how can we declare them?

Variable is a name given to be memory location where user wants to store a value.
In  python we can declare and assign the variable at the same time and the data type of the variable will be determined during runtime
For eg :

a = 10
b = float(input())



Q6. How can we take an input from the user in Python?


We can take input from user in Python using input() function which returns the value entered by the user and store it in a variable
The input value is treated as String by default

For eg :

a = input()    	#input is string
b = float(input())	#input is float


Q7. What is the default datatype of the value that has been taken as an input using input() function?



The default datatype of any value take using input() is String.


Q8. What is type casting?


Type casting refers to explicitly changing the data type  of a value.
For eg :
rollNo = int(input(‘enter your rollno”)    #typecasting input rollNo from String to int data type
 a = 9
print(float(a))			# typecasting a from int to float



Q9. Can we take more than one input from the user using single input() function? If yes, how? If no, why?

The input that user enters is considered as one string by python interpreter . However, we can use split() function in order to extract multiple input 
values from the entered string and assign them to multiple variable .

For eg 
 firstName, middleName , lastName = input('Enter full name').split()
 print('The first name is {} , the middle name is {}, the last name is {}'.format(firstName, middleName , lastName))



Q10. What are keywords?

Keywords are the predefined reserved words in python language that can/should not be used as variables as they hold a special meaning . These are used to denote predefined methods
boolean literals etc 



Q11. Can we use keywords as a variable? Support your answer with reason.

We can not use keywords as variables as they hold a specific meaning in the language. Using these keywords as variables will result in 'invalid syntax' error. 


Q12. What is indentation? What's the use of indentaion in Python?


Indentation means space on the left ie beginning of the code line . 
Python uses identation to denote a block of code 

Q13. How can we throw some output in Python?

 We can throw some output in python using print() function . This function accept the values to be shown as output as a parameter
 which can be any literal values or values in the form of a variable/ expressions
 We can also print multiple values by passing them in print function separated by comma.
 
 
 For eg 
 print(5)  ---> 5
 print('Hello') ---> Hello
 a = 15 
 b = 3
 print (a,b) ---> 15 3
 print(a+b) ---> 18

Q14. What are operators in Python?

Operators are the special symbols in python used to computations  on data.
There are various types of operators available in python:
Assignment operator ( = )
Arithmatical operators ( +,-,*,/,//,%,**)
Comparison operators( ==,!=,>,<,>=,<=)
Bitwise (&,|,~,^,>>,<<)
Identity (is )

Q15. What is difference between / and // operators?

'/' returns the dividend as float value ie integer + fractional part of the dividend
'//' is used for integer division ie it returns only the integer part of the dividend . The type of dividend is also int 

Q16. Write a code that gives following as an output.
```
iNeuroniNeuroniNeuroniNeuron
```

print('iNeuron' * 3)


Q17. Write a code to take a number as an input from the user and check if the number is odd or even.

num = int(input('Enter a number))
if num == 0 : print ('Enter a non zero number)
elif num % 2 == 0 : print(num + ' is an even number')
else :  print(num + ' is an odd number')


Q18. What are boolean operator?

There are three logical operators that are used to compare values. 
They evaluate expressions down to Boolean values, returning either True or False 



Q19. What will the output of the following?
```
1 or 0 :  True

0 and 0 :  True

True and False and True : False

1 or 0 or 0 :True
```

Q20. What are conditional statements in Python?

Conditional statements in python are used to make decision based on if a particular condition is met or not.

for eg 
if n%2 == 0 :
	print ('even no')
else :
	print('odd no')


Q21. What is use of 'if', 'elif' and 'else' keywords?


'if' keyword is used to provide condition and subsequent code block to be followed if the condition is true.
'elif' keyword is used in combination with 'if' keyword if there are multiple alternative conditions 
'else'keyword is used in combination with 'if' keyword to provide instructions if  none of the other previously given conditions are not true

for eg 	

if num == 0 : print('Number is 0)
elif num < 0 : print ('Number is positive')
else print('Number is negative'


Q22. Write a code to take the age of person as an input and if age >= 18 display "I can vote". If age is < 18 display "I can't vote".



age = int(input('Enter age))

if age >= 18 : print("I can vote")
else : print("I can't vote")


Q23. Write a code that displays the sum of all the even numbers from the given list.
```
numbers = [12, 75, 150, 180, 145, 525, 50]
```

total = 0
for i in numbers :
	if i % 2 == 0 :
		total+= i

print('Sum of even number = ', total  )



Q24. Write a code to take 3 numbers as an input from the user and display the greatest no as output.


a = int(input())
b = int(input())
c = int(input())
def largest(a,b,c):
	if a > b and a > c :
		return a 
	elif b > a and b > c:
		return b
	else : 
		return c

print ('largest number = ', largest(a,b,c))


Q25. Write a program to display only those numbers from a list that satisfy the following conditions

- The number must be divisible by five

for i in numbers:
  if i % 5 == 0 : print(i)


- If the number is greater than 150, then skip it and move to the next number


for i in numbers :
	if i > 150: continue 
	if i % 5 == 0 : print(i)

- If the number is greater than 500, then stop the loop


for i in numbers :
	if i > 500 : break
	if i > 150: continue 
	if i % 5 == 0 : print(i)

```
numbers = [12, 75, 150, 180, 145, 525, 50]
```