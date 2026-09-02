# ECE-2112-PA-1
**Made By: Myk Zachary Marcian M. San Miguel | 2ECE-D '26-'27**

This repository contains the content for Programming Assignment 1 for our Advanced Computer Programming Course this S.Y. 2026-2027. This project covers three Python problems on Base Computing.

## Part A: Word Rotation Problem
The objective of this function, which we will name `rotate word()`, is to accept a non-empty string. It moves the first character of the string to the end while keeping all remaining characters in their original order. This function preserves the capitalization of every character.

The following methods were utilized in this function:

- `return` - this statement is used inside a function to exit the function and send a specified value back to the code that called it.

**string splicing** - this will allow us to extract a specific portion of a string using the syntax `string[start:stop:step]`. Where:
- `start` - is the index where the slicing begins. It usually defaults to `0`, which is the index of the first letter.
- `stop` - is the index where the slice ends. Leaving it blank will default to the end of the string.
- `step` - refers to how many increments the value will take between the characters.

**Using the index to call characters of a string**
- for example, the syntax `z[1::1]`. Inside the bracket, there were integers separated by a colon. The first integer `1`(integer beside the opening bracket) tells the compiler to start at the 2nd character of the string stored in the given arbitrary variable `z`.
- Then it is followed by the first colon and a _blank_, which tells the compiler to stop at the last letter of the string.
- After that, it is followed by a 2nd colon and the last integer beside the closing bracket, which is `1` in this scenario. Since it is `1`, it tells the compiler to take the character every 1 step.

With all of the functions discussed, the final function will look like this:
```python
def rotate_word(z): #defines the function named "rotate_word" with an arbitrary variable "z"
    return z[1::1] + z[0] #takes the first letter of the string and moves it to the end

#calls out the funcion and outputs the result of the said function
print (rotate_word("Python"))
```

## Part B: Username Builder Problem
This function's objective, which we will name `make_username()`, accepts two strings: `first_name` and `last_name`. After that, this function also converts all letters to lowercase and removes all spaces from the first and last names. After this, the function joins the processed first and last names with a single period.

Example:
If you were input the first_name as `"RonALD"`, and the last name as `"Mc Donald"`, it will output `ronald.mcdonald`


The following methods were used in this function:
- `.lower()` - transforms all the letters inside a variable into lowercase.\
example: `"wHAt Are thOSE".lower()` ---> 'what are those'


- `.replace()` - replaces your chosen character/s with a new character that you will declare.\
example: `"I the best".replace("I","u")` ---> 'u the best' 

Now, in order to define and make our own function, we will use the given functions above to achieve the function that we want to make.
```python
def make_username(first_name, last_name): #this defines the name of the function and the two variables that we will be using

    #makes all of the letters within the FIRST variable in lower case and removes all the spaces
    newfirst=first_name.lower().replace(" ","")

    #makes all of the letters within the SECOND variable in lower case and removes all the spaces
    newlast=last_name.lower().replace(" ","")

    #this prints the new 1st and 2nd variables, seperated by a period
    return print(newfirst+"."+newlast)

#calls out the function and displays the first name and the family name 
make_username("Ana Maria","De Leon")
```

## Part C: Bookend Swap Problem
This function makes a function named `swap_bookends()` that accepts two elements and unpacks them into three variables, which are: first - the first element; middle - a list that contains the elements between the first and last elements; and last - the last element.

The following methods were utilized in this function:

A sample list was given: `items = [1,2,3,4,5,6]`

Using manual slicing, relevant values from the list were assigned to their respective variables and displayed.
```python
def swap_bookends(items): #defines the name of the function and the arbitrary variable that stores the elements 
    
    first = items[0] #takes the first element and assigns it to an arbitrary variable named "first"
    middle = items [1:-1] #takes the second element to the second to the last element and assigns it to an arbitrary variable named "middle"
    last = items [-1] #takes the last element and assigns it to an arbitrary variable named "last"

    #switches the place of the first and last elements while maintaining the order of the middle element and assigns these to a new variable
    newitems = last,*middle,first

    #closes the function and outputs the contents of the new variable
    return print (newitems)

#calls and executes the user-defined fucntion
swap_bookends([1,2,3,4,5,6])
```

Thank you so much for taking the time to read! If you wish to download the file, download it [here](https://github.com/mykzacharysanmiguel/ECE-2112-PA-1/blob/fc320caaf14070587e4824b1ec7b6f03fb919c66/Programming%20Assignment%201.ipynb)

#### README File Version History:
August 24, 2026 - Initial README output is uploaded

August 26, 2026 - Revisions were made in the README file, and the .ipynb file was attached

August 27, 2026 - Final revisions were made in the .ipynb file as well as the README file

September 2, 2026 - School year is corrected on Line 4 of the README file
