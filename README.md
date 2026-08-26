# ECE-2112-PA-1
**Made By: Myk Zachary Marcian M. San Miguel | 2ECE-D '26-'27**

This repository contains the content for Programming Assignment 1 for our Advanced Computer Programming Course this S.Y. 2025-2026. This project covers three Python problems on Base Computing.

## Part A: Word Rotation Problem
This function, which we will name `rotate word(),` accepts a non-empty string. It moves the first character of the string to the end while keeping all remaining characters in their original order. This function preserves the capitalization of every character.


```python

```

## Part B: Username Builder Problem
This function, which we will name `make_username()`, accepts two strings: `first_name` and `last_name`. Moreover, this function also converts all letters to lowercase and removes all spaces from the first and last names. After this, the function joins the processed first and last names with a single period.

The following methods were used in this function:
- `.lower()` - transforms all the letters inside a variable into lowercase.

example: `"wHAt Are thOSE".lower()` ---> 'what are those'


- `.replace()` - replaces your chosen character with a new character that you want.

example: `"I the best".replace("I","u")` ---> 'u the best' 

Now in order to define and make our own function, we will use the given functions above to achieve the function that we want to make.
```python
def make_username(first_name, last_name): #this defines the name of the function and the 2 variables that we will be using

    #makes all of the letters within the FIRST variable in lower case and removes all the spaces
    newfirst=first_name.lower().replace(" ","")

    #makes all of the letters within the SECOND variable in lower case and removes all the spaces
    newlast=last_name.lower().replace(" ","")

    #this prints the new 1st and 2nd variables, seperated by a period
    print(newfirst+"."+newlast)
```
Now, the function that we will use for this problem will be:  
```python
make_username(input("Enter first name: "), input("Enter family name: ")) #calls out the function and lets us input the first name and the family name
```

## Part C: Bookend Swap Problem
This function makes a function named `swap_bookends()` that accepts two elements and unpacks them into three variables, which are: first - the first element; middle - a list that contains the elements between the first and last elements; and last - the last element.



```python

```


#### README File Version History:
August 24, 2026 - Initial README output is uploaded

August 26, 2026 - Revisions were made in the README file
