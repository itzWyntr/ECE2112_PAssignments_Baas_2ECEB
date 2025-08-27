# Programming Assignment 1

My Programming Assignments 1 in explained in this repository

## Table of Contents
Alphabet Soup Problem: https://github.com/itzWyntr/ECE2112_PAssignments_Baas_2ECEB/blob/main/README.md#alphabet-soup-problem

Emoticon Problem: https://github.com/itzWyntr/ECE2112_PAssignments_Baas_2ECEB/blob/main/README.md#emoticon-problem

Unpacking Problem: https://github.com/itzWyntr/ECE2112_PAssignments_Baas_2ECEB/blob/main/README.md#unpacking-list

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

#### Emoticon Problem
In this project, we are tasked to change words into emoticons. Specifically, smile, grin, sad, and mad.

1. I started with naming the function and creating a map of words with their equivalent emojis
```python
def emoticon_replace(sentence):
    emoticons = { "smile" : ":)", "grin" : ":D",  "sad" : ":((", "Mad" : ">:(" } #emoticon map
```

2. Then, I split each word in the sentence
```python
  words = sentence.split() #split sentence into words
    new_words = []
```

3. Then, I create a function that will check each word if it's in the map and replace it. If not, it'll keep the word as is
```python
 for word in words: 
        if word in emoticons: #check if word is in emoticon list
            new_words.append(emoticons[word]) #replace the word
        else: 
            new_words.append(word) #keep if not on list
    return ' '.join(new_words)
```

4. I used "Try to smile and grin instead of being mad or sad" as a test
```python
sentence = "Try to smile and grin insted of being mad or sad"
print(emoticon_replace(sentence))
```

#### Unpacking List
In this project, we are tasked to split a collection of numbers into three variables, namely first, middle, and last. With the middle being everything between first and last

1. I started with a sample list
```python
writeyourcodehere = [25, 14, 1, 7, 8]
```

2. Then, I unpacked the list and split it for each variable
```python
first, *middle, last = writeyourcodehere #unpacking list
```

3. Then, I print each result
```python
print("First: ",first)
print("Middle: ",*middle)
print("Last: ", last)
```

