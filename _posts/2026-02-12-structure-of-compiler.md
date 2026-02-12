---
title: "[Compiler]: The Structure of compiler"
date: "2026-02-12 22:34:30 +0200"
author: Ahmed Nour
category: Compiler 
---

Here, we’re disecting compiler components.

# <span style="color:blue">The structure of compiler(Front End focus)</span>

Compiler consists of three main components: 

1. Front end:  Deals with source language and transforms source code into an Intermediate representation(IR) 
2. Middle End: Performs transformations on Ir with goal of either improving performance or reducing the size of code
3. Backend: Produces machine code from Intermediate representation (IR)


## <span style="color:blue">Front End</span>

Usually the input to front end is text file which then is processed with the three following components:

1. Lexer: which identifies language words such as numbers and identifiers which are usually called tokens so it basically generate tokens 
 
2. Parser: syntactical structure formed by tokens is analyzed and generates AST (abstract syntax tree)
 
3. Semantic analyzer: Check if rules of programming language is obeyed then if no errors found Then AST is transformed to IR and handed over to middle end 
