# Programming Assignment 1: Introduction to Python Programming
##### This repository contains three problems emphasizing different aspects of Python programming, including string manipulation, list handling, and conditional logic. Each problem presents unique challenges that enhance understanding of data structures and algorithmic thinking in Python.

## 1. Alphabet Soup Problem
###### This code creates a function that takes a string and returns a string with its letters in alphabetical order.
```Ruby
def alphabetize_string():
    s = input("Enter a word: ")
    return "".join(sorted(s))

print(alphabetize_string())
```

## 2. Emoticon Problem
###### This code creates a function that changes specific words into emoticons.
```Ruby
def emotify():
    emotify_lib = {
        "smile": ":)",
        "grin": ":D",
        "sad": ":((",
        "mad": ">:("
    }

    sentence = input("Enter a sentence: ")

    for word, emoticon in emotify_lib.items():
        sentence = sentence.replace(word, emoticon)
    return sentence

print(emotify())
```

## 3. Unpacking List Problem
###### This code unpacks the list and write your code here into three variables: First, middle, and last.
```Ruby
def unpack_list():
    user_input = input("Enter a list (separated by spaces): ")
    elements = user_input.split()

    if len(elements) < 3:
        print("Please enter at least 3 elements")
        return

    first, *middle, last = elements

    print("First:", first)
    print("Middle:", middle)
    print("Last:", last)

unpack_list()
```
