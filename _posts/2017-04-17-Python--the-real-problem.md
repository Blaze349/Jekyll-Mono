
I've been contemplating about why I don't like programming in python. 
I don't mind using python for shell scripting, its much better than bash scripting and with PyPi is super fast.
But for general coding I find it difficult to read and write.

Look at this code below:
```python
>>> x = int(input("Please enter an integer: "))
Please enter an integer: 42
>>> if x < 0:
...     x = 0
...     print('Negative changed to zero')
... elif x == 0:
...     print('Zero')
... elif x == 1:
...     print('Single')
... else:
...     print('More')
...
More
```
Compared to this:
```javascript
let x = 4
if (x < 0) {
  x = 0
  console.log("Changed to zero")
} //and more stuff...
```
The top code is python and the second is javascript.
Immediately what jumps out is the braces. Python has no braces. But this isn't the problem. 
The lack of braces can actually increase focus on code.

## The Real Problem
The real problem with Python is the lack of brackets. No brackets at all.
Even for a print statement.
```python
print "Hi universe!"
```
This makes it hard for me, when reading new code or debugging new code, to quickly identify the conditions and the function parameters.
Python, whitespace and minimalism is good but not when it sacrifices understanding. There is a reason we have full stops. 
So we can easily identify when a sentence starts an stops.
