
I've been contemplating about why I don't like programming in python. 
I don't mind using python for shell scripting; it's more elegant than bash scripting and when use with PyPi it is super fast.
**But**, for general programming, it is difficult to read and write.

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
This makes it difficult, when reading new code or debugging new code, to quickly identify the conditions and the function parameters.

There is a reason we have full stops and commas. Look at this sentence:
> The core of extensible programming is defining functions. Python allows mandatory and optional arguments, keyword arguments, and even arbitrary argument lists.

And compare with this:
>The core of extensible programming is defining functions   Python allows mandatory and optional arguments  keyword arguments  and even arbitrary argument lists  

It looks cleaner but it is harder to identify the clauses.

Whitespace and minimalism is good but not when it sacrifices understanding.  

**EDIT**: I know the print statement has changed in python 3.
Yes, I know that this issue is made irrelevant with syntax highlighting. 
