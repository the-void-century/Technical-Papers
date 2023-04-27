# String Methods (Python)

- ## Introduction
The aim of this paper is to help the reader get familiar with the standard functions of strings in Python.

- ## Functions

1. `.count()`: This function returns the count of a specific value inside a string , the value is passed as an argument. **Syntax:**

		s="aabbzzz"
		character_to_be_counted='z'
		frequency=s.count(character_to_be_counted) #This is the generic syntax
		print(frequency)
	- The snippet above prints the number of time **"z"** appears in the string **"s"** which is `3`
2. `.find() and .index()`: The reason I have grouped these two together is because they serve almost the same functionality, both of these functions will return the first index of where a specified value is found , however when they fail to find the value, `.index()` raises a **ValueError** exception and `.find()` returns -1. **Syntax**

		s="aabbcc"
		answer=s.find("a")
		answer2=s.index("a")
		print(answer,answer2)

	- Both of these functions will return `0` (The first occurrence of **"a"**)
3. `.format()`: This function places text inside given string, The user needs to define a  placeholder inside the string so the function knows where to place specific values. **Syntax:**

		text="The price of {fruit} is {price}"
		modified_string=text.format(fruit="mango",price=35")
		print(modified_string)
	
	- The output for the snippet above is `The price of mango is 35` 
	-  `format` maps the values to their respective placeholders.
		


