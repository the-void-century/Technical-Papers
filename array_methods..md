# Arrays/List Methods (Python)

- ## Introduction
The aim of this paper is to help the reader get familiar with the standard functions of lists in Python.

- ## Functions

1. `.append()` : This function adds an element at the end of the list , since Python allows the user to add multiple data types to the same list, You can append element of any data type without any errors. **Syntax:**

			list=[1,3]
			new_element=3
			list.append(new_element) #This is the generic syntax
			print(list)
	- The output for the snippet above will be `[1,3,3]`

2. `.clear()` : This function will remove all elements from the list , Be careful while using it. **Syntax:**
	
			list=[1,2,3]
			list.clear() #This is the generic syntax
			print(list)
	- The output for the snippet above will be `[]` (Empty list)

3. `.copy()` : This function will simply return a copy of a list. **Syntax:**

			old_list=[1,2,3]
			new_list=old_list.copy() #This is the generic syntax
			print(new_list)
	- The output for the code above will be `[1,2,3]`

4. `.count()`: Returns the frequency of a given element that is passed as an argument. **Syntax:**

			list=[1,1,1,4]
			element_to_be_counted=1
			frequency=list.count(element_to_be_counted) #This is the generic syntax.
			print(frequency)
	- The output for the snippet above will be `3` (The number of time `1` appears in the list)

5. `.extend()`: Essentially concatenates one list with the other. **Syntax:**

			list1=[1,2,3]
			list2=[4,5,6]
			list1.extend(list2) # This is the generic syntax
			print(list1)
	- The output for the code above will be `[1,2,3,4,5,6]`
	
6. `.index()`: Returns the first index of the element that's passed in the argument. **Syntax**

		 list1=[1,2,3,3,3,4]
		 index=list1.index(3)
		 print(index)
	- The snippet above will print: `2` (The first  "3" appears in the list)

7. `.insert()`: This function will help you out if you want to place a certain element at a certain index, but be careful because it will obviously shift the indexes of all subsequent elements by "1". **Syntax:**

		list=[1,2,3,4]
		index=1
		element=6
		list.insert(index,element) #This is the generic syntax.
		print(list)
	-The above snippet will add `6` at index `1`. The output will be:`[1,6,2,3,4]`

8. `.pop()`: This function will remove an element from a specified index, however the argument is optional, The default value is `-1` , which means the function will remove the last element by default. **Syntax:**

		list=[1,2,3,4]
		index_to_be_removed=2
		list.pop(index_to_be_removed) #This is the generic syntax
		print(list)
	- The output for the above snippet is: `[1,2,4]`
	````
	 list.pop()
	````
	- The code above will further remove the last element , Output: `[1,2]`
9. `.remove()`: This function has the similar functionality as `.pop()` but this function removes by value instead of index, This removes the first occurrence of the specified value. **Syntax:**

		list=[1,2,2,2,3,4]
		element_to_be_removed=2
		list.remove(element_to_be_removed) #This is the generic syntax
		print(list)
	-  The output for the above code will be: `[1,2,2,3,4]`
10. `.reverse()`: This function will simply reverse the given list. **Syntax**

		list=[1,2,3,4,5]
		list.reverse() #This is the generic syntax.
		print(list)
	- The output for the snippet above will be: `[5,4,3,2,1]`
11. `.sort()`: This function will sort the given list,It sorts by ascending order by default , However you can specify the order as an optional argument. You can also customize this function by specifying a key according to which you want the function to sort the elements. **Syntax:**

		list=[3,4,2,1,5]
		list.sort() #This is the generic syntax
		print(list)
	- The snippet above will sort the list by ascending order, Output: `[1,2,3,4,5]`
		````
		list.sort(reverse=True)
		print(list)
		````
	- The snippet above will sort the list by descending order, Output: `[5,4,3,2,1]`
	````
	def function(s):
			return len(s)
	list=["aaaa", "bb" , "c"]
	list.sort(key=function)
	print(list)
	````
	- The code above will sort the list of strings by their lengths instead of their lexicographical order.
	
		


