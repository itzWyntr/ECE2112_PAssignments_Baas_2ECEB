# Ryan Baas Programming Assignments

My Programming Assignments on the course 2112 are compiled in this repository.

## Programming assignments

PA1: https://github.com/itzWyntr/ECE2112_PAssignments_Baas_2ECEB/blob/main/PA1.ipynb

### Programming Assignment 1
#### Alphabet Soup Problem
In this project, we are tasked to arrange the letters of a word in alphabetical order

1. I started with naming the function and having a blank array for each letter
```python
def alphabet_sort(s):
    letter_sort = []
```

2. Then, I created a loop that will check if each character of the string is in the alphabet
```python
for char in s: #loop through each character of the string
        if char.isalpha(): #check if the character is a letter
            letter_sort.append(char)
```

3. Then, I sorted each letter alphabetically
```python
sorted_letter = sorted(letter_sort, key=lambda x: x.lower()) #sort collected letters
    return ''.join(sorted_letter)
```

4. I used "Hello World" as a test
```python
print(alphabet_sort("Hello World")) 
```
