Answer all questions

```
Submit seperate code files for first 4 questions.
You can write in C or Java or Python.  
File names for Q3 answer:
q3.py or q3.c or q3.java

note: 
With these lower case file names only. 
Wrong file names will be ignored. 

note:
Just the code for the required method only.
```

### PART - 01

---

Q1
  
Write a recursive method to add an array of numbers.      

---

Q2  
  
Given a binary tree, print the factors of the maximum number in the left-sub tree. You may assume that both left and right sub-tree exists.  

```
e.g:
  16  
  / \  
 14 18  
 / \  
12 15  

Output:
1 3 5 15
```
---
  
Q3  
  
Given a binary search tree, find if the difference between the minimum of right sub-tree and maximum of left sub-tree is prime or not. You may assume that both left and right sub-tree exists. You can use is_prime method where needed, no need to implement it.  

```
e.g:
   16  
   / \  
  14 18  
 / \  
12 15  
  
Output:
The difference 3 is prime.
```
---

Q4

A crosswords puzzle sub-problem. Given 3 words of 3 length each. Find out in which order when you place these 3 words in 3 rows. The word formed by the middle collumn is one of the given 3 words.

```
e.g:
i/o:
Given 3 words: cat bet aee
o/p:
The order you can place is:
cat
bet
aee

i/o:
Give 3 words: cat bat ate
o/p:
Not possible
```

---

### PART - 02

```
write answers in a text file and submit it.

```

Q5
```python
1   def process(number):
2      if number < 1:
3>>       return 0        ### break point
4
5     part = number//3
6     part_result = 1 + process(part)
7     part_result += 2 + process(part * 2)
8     return part_result
9
10  print(process(5))
```

When the break point is hit for the first time.
+ What is the call stack?
+ Draw the stack frames and it's contents.  
  
What is the output of the program?

---

Q6

```python
1   def do_this(number):
2      if number < 1:
3>>        return 0          # break point
4 
5      part = number//3
6      part_result = 1 + you_do_this(part)
8      part_result += 2 + you_do_this(part * 2)
9      return part_result
10
11
12  def you_do_this(number):
13     return 5 * do_this(number//2)
14 
15  print(do_this(15))
```

What is the call-stack when the break point is hit for the first time?  
How many times do_this function is called?
What is the output?  

---

Q7

```python
def process(number):
    if number < 1:
        return 0

    part = number//3
    part_result = 1 + process(part)
    part_result += 2 + process(part * 2)
    return part_result
```

What is the time complexity and space complexity of process function?

```python
def depth(number):
    result = 0
    for step in range(1, number):
        for element in range(1, step):
            result += element * step

    if result > 100:
        return result

    result = result * 2
    result = result // 5

    for step in range(1, number*2):
        result += step * 5

    return result
```

What is the time complexity and space complexity of depth function?

---


Q8

Given a weighted graph G and it's minimum spanning tree MST. Now a new edge e of weight c is inserted into G to form G'. Design an algorithm to determine if the MST in G is also an MST in G'. You may assume all edge weights are distinct. V is the number of the vertices. State the algorithm and what is the complexity of it?