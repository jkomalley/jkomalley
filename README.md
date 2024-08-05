```python
# me.py

class Developer:
  def __init__(self):
    self.name = "Kyle"
    self.pronouns = ["he", "him"]
    self.code = ["Python", "C", "C++", "Rust"]
    self.degree = "B.S. Computer Science"
    self.almaMater = "University of Pittsburgh"
    self.numCats = 2

  def greet(self):
    print(self)

  def __str__(self):
    out = f"My name is {self.name}"
    out += f" ({'/'.join(self.pronouns)}).\n"
    out += f"I love writing code in  "
    out += f"{', '.join(self.code[:-1])} and {self.code[-1]}.\n"
    out += f"I earned my {self.degree} degree from the {self.almaMater}.\n"
    out += f"I have {self.numCats} cats that love sitting on my keyboAAAAAAAASAQWQSQQQ"
    return out

me = Developer()
me.greet()
```
```console
user@github $ python me.py
My name is Kyle (he/him).
I love writing code in  Python, C, C++, and Rust.
I earned my B.S. Computer Science degree from the University of Pittsburgh.
I have 2 cats that love sitting on my keyboAAAAAAAASAQWQSQQQ
```
