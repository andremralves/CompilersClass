
### Intermediate code 
Representation:
- abstract syntax trees
- sequence of "tree-adresses"
fig. 2.4

## 2.2 Syntax Definition 

### Context-free grammar

if (expression) statement else statement
-->
stmt -> if ( expr ) stmt else stmt

- -> may be read as "can have the form"
- the rule is called production
- if and (): terminals
- expr and stmt: sequence of terminals/nonterminals

### 2.2.1 Definition of Gramamar

### 2.2.2 Derivations

### 2.2.3 Parse Trees

- The process of finding a parse tree for a given string of terminals is called parsing that string.

### 2.2.5 Associativity of Operators

- add, sub, mult and div are left-associative
- a=b=c and exponentiationis are right-associative

```
right -> letter = right | letter
letter -> a|b|...|z
```
fig. 2.7

### 2.2.6 Precedence of Operators

```
factor -> digit | (expr)

term -> term * factor
      | term / factor
      | factor

expr -> expr + term
      | expr - term 
      | term 
```

## 2.3 Syntax-Directed Translation

Syntax-directed translation is done by attaching rules or program fragments to
pro ductions in a grammar.

2 concepts:

- Atributes:
  - An attribute is any quantity asso ciated with a programming
construct.

- (Syntax-directed) translation schemes:
  - A translation scheme is a notation for attaching program fragments to the productions of a grammar.

## 2.3.1 Posfix Notation

infix: (9-5)+2
posfix: 95-2+

