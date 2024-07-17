# Search Query language
## Why do we have to learn it?
Since it is important for every user (even if you NEVER write code) and it is widely used. (See following usage section.)

## Usage
When one has to query search box, one uses search query language (as a person who NEVER learn about code may NOT know one uses, in fact we use it every day once we search things on the Internet). Including

+ Search thing on Explorer (such as Google Chrome).
+ Search thing on issuetracker (a kind of Google issue report website).

Now, I believe that every reader the first item is always used. 

That's the reason why I think everyone has to learn search query language. And that's the main purpose to wrote this article for me.

But don't worry about it. I will try to make it as easy as I can.

## Word definition 
1. expression:

 Here an expression consist of one of followings: 

+ ***keyword***  (here a keyword refers solely consist of values) 

+ ***key-value pair*** with separator `:` (such as `status:isOpen`) ) .

2. logical operator:

A logical operator can combine these expression with logic.

Here are a list of atomic (i.e. the smallest part that we can divide it anymore) logical operators

| Atomic logical operator | description | keyword | symbol (in some programming language etc) |
| ----------------------- | ----------- | ------- | ----------------------------------------- |
| not | opposite of an expression | `not` | `!` |
| and | like `and` in English, `and` of two expression is true iff two expressions are **BOTH** true. | `and` | `&&` |
| or | like `or` in English, `or` of two expression is true iff **at least one of** two expressions is true (or both). | `or` | `\|\|` |

## Rule
1. In search box, one can fill in one or more expressions (See the above word definition)
2. One can use logical operator to combine these expressions.


***NOTES***
NOTICE that when there are spaces between two expression, it is usually considered as `and` of two expressions (in most cases, but may differ rarely. Thus, I highly recommend that NOT to do so unless you can ensure thaat it is consider as `and` of two expressions.)

(a key-value consists of a key and a value and seperate with special symbol between them.

## Example
In search query language,

```

```










