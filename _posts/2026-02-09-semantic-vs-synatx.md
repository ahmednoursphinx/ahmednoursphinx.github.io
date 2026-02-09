---
title: "[Misc]: Semantic Vs syntax"
date: "2026-02-09 10:46:30 +0200"
author: Ahmed Nour
category: Misc 
---

# <span style="color:blue">What is Semantics</span>
Short version first: semantics = meaning 😄 

In programming languages, semantics describes what a program actually does when it runs, not how it looks or how it’s written.

## <span style="color:blue">Layers of programming language</span>

When we talk about a programming language, there are usually three layers:

1. Syntax → How it’s written  
2. Semantics → What it means / what happens  
3. Pragmatics → How people actually use it

for example: 
```c++
 a = b + c;
```

**Syntax**:
Is this written in a way the compiler understands?
(Yes: assignment, +, identifiers, semicolon)

**Semantics**:
What does this mean?

Take the value of b
Take the value of c
Add them
Store the result in a

If b = 2 and c = 3, the semantic result is a = 5.

## <span style="color:blue">Why syntax alone is not enough?</span>

For example :

```c++
x = x + 1;
```

vs

```c++
x += 1;
```

**Syntax**: different 

**Semantics**: the same (increment x by 1)

Now compare:

```
x = x++;
```

**Syntax**: valid (in C/C++)

**Semantics**: tricky / undefined (depends on language rules)

So semantics answers:

“What exactly happens here?”

## <span style="color:blue">Semantics vs behavior across languages</span>

```c++
int x = 1 / 2;
```

C/C++ semantics → x = 0

Python semantics → x = 0.5

Swift semantics → compile error (type mismatch)

Same text, different meaning.

## <span style="color:blue">Summary</span>

**Syntax** is how code looks.

**Semantics** is what the code means and what it does when executed.