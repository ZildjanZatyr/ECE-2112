# Programming Assignment 1: Introduction to Python Programming
##### This repository contains three problems emphasizing different aspects of Python programming, including string manipulation, list handling, and conditional logic. Each problem presents unique challenges that enhance understanding of data structures and algorithmic thinking in Python.

## 1. Alphabet Soup Problem
###### This code creates a function that takes a string and returns a string with its letters in alphabetical order.
```Ruby
# Defines function "alpabetize_string" and prompts user input then stores in variable "s"
def alphabetize_string():
    s = input("Enter a word: ")
    return "".join(sorted(s))

# Recalls the function and prints the result
print(alphabetize_string())
```

## 2. Emoticon Problem
###### This code creates a function that changes specific words into emoticons.
```Ruby
# Defines function "emotify" and creates a dictionary "emotify_lib" that maps words to their corresponding emoticons
def emotify():
    emotify_lib = {
        "smile": ":)",
        "grin": ":D",
        "sad": ":((",
        "mad": ">:("
    }

# Prompts user input and stores input in variable "sentence"
    sentence = input("Enter a sentence: ")

# Iterates each key-value pair in the dictionary and replaces all occurences of the word with its corresponding emoticon
    for word, emoticon in emotify_lib.items():
        sentence = sentence.replace(word, emoticon)
    return sentence

# Recalls the function and prints the result
print(emotify())
```

## 3. Unpacking List Problem
###### This code unpacks the list and write your code here into three variables: First, middle, and last.
```Ruby
# Defines function "unpack_list" and prompts input user and stores into variable "user_input"
def unpack_list():
    user_input = input("Enter a list (separated by spaces): ")
    elements = user_input.split()

# Checks if the list has less than 3 elements, if so, then it prints and error message and returns from the function
    if len(elements) < 3:
        print("Please enter at least 3 elements")
        return

# Unpacks the list into three variables
    first, *middle, last = elements

# Prints the values for the first, middle, and last
    print("First:", first)
    print("Middle:", middle)
    print("Last:", last)

# Recalls the function
unpack_list()
```
