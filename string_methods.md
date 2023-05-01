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
2. `.find() and .index()`: The reason I have grouped these two together is because they serve almost the same functionality, both of these functions will return the first index of where a specified value is found , however when they fail to find the value, `.index()` raises a **ValueError** exception and `.find()` returns -1. **Syntax:**

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
4.  `.isalpha()`: This function returns a boolean value after checking if all characters in a string are alphabets or not. **Syntax:**

		text1="Company"
		text2="Company10"
		check_alpha1=text1.isalpha()
		check_alpha2=text2.isalpha()
		print(check_alpha1,check_alpha2)

	- The above snippet prints `True` and `False` respectively.

5. `.replace`: This function replaces a given character or a phrase with another one. An optional argument can be added , specifying the number of existing phrases the user wants to remove. **Syntax:**

		text="I like Bananas"
		current_phrase="Bananas"
		new_phrase="Oranges"
		modified_text=text.replace(current_phrase,new_phrase) #This is the generic syntax
		print(modified_text)

6. `.upper() and .lower()`: Both of these functions have similar functionality, `.upper()` changes all characters in a string to uppercase and `.lower()` changes all the characters to lowercase. **Syntax:**

		text="AaAbC"
		upper_text=text.upper()
		lower_text=text.lower()
		print(upper_text,lower_text)

	- The snippet above prints `AAABC` and `aaabc` respectively.

7. `.split()`: This function splits the string on the basis of the given argument which is space by default. **Syntax:**

		text1="This is a sentence"
		new_list=text1.split()
		print(new_list)
	
	- The above snippet will print `["This","is","a","sentence"]` splitting the above string by space

8. `.strip()`: This function removes the leading and trailing occurrences of a specified string, the default argument is space.  **Syntax:**

		text1="  abcd    "
		new_text1=text1.strip()
		print(new_text1)

	- The above snippet will print `abcd` removing all instances of spaces from the right and the left end.

9. `.join()`: This function is the polar opposite of the `.split()` function , This function will help you out if you want to join a list to make a string based on a separator.  **Syntax:**

		list=["This","is","a","sentence"]
		separator="  "
		answer=separator.join(list)
		print(answer)

	- The snippet above will print `This is a sentence` creating a space will adding the specified separator between the words.

10. `isdigit()`: Returns `True` if all characters in the given string are digits , else returns `False`. **Syntax:**

		digit="10273"
		non_digit="adefre13"
		print(digit.isdigit())
		print(non_digit.isdigit())

	- The snippet above prints `True` and `False` respectively.
		

