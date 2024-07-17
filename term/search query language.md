# Search Query language
## Why do we have to learn it?
Since it is important for every user (even if you NEVER write code) and it is widely used. (See following usage section.)

## Usage
When one has to query search box, one uses search query language (as a person who NEVER learn about code may NOT know one uses, in fact we use it every day once we search things on the Internet). Including

+ Search thing on Explorer (such as Google Chrome).
+ Search thing on issuetracker (a kind of Google issue report website).
+ Search thing on Logcat.

Now, I believe that every reader the first item is always used. 

That's the reason why I think everyone has to learn search query language. And that's the main purpose to wrote this article for me.

But don't worry about it. I will try to make it as easy as I can.

## Word definition 
1. expression:

 Here an expression consist of one of followings: 

+ ***keyword***  (here a keyword refers solely consist of values) 

+ ***key-value pair*** with separator `:` or `=`

2. key-value pair:

a key-value pair consists of a key and a value and seperate with special symbol between them. .

3. logical operator:

A logical operator can combine these expression with logic.

Here are a list of atomic (i.e. the smallest part that we can divide it anymore) logical operators

| Atomic logical operator | description | keyword | symbol (in some programming language etc) | keyword in query search language in issuetracker | symbol in query search language in issuetracker|
| ----------------------- | ----------- | ------- | ----------------------------------------- | -------------------------------- | ----------------------- |
| not | opposite of an expression | `not` | `!` | `NOT` | `-` |
| and | like `and` in English, `and` of two expression is true iff two expressions are **BOTH** true. | `and` | `&&` | `AND` | `\ ` |
| or | like `or` in English, `or` of two expression is true iff **at least one of** two expressions is true (or both). | `or` | `\|\|` | `OR` | `\|` |

***NOTES***
In **query search language**, the keywords in logical operator must be capital (for example `AND`).

## Rule
1. In search box, one can fill in one or more expressions (See the above word definition)
2. One can use logical operator to combine these expressions.

***NOTES***
NOTICE that when there are spaces between two expression, it is usually considered as `and` of two expressions (in most cases, but may differ rarely. Thus, I highly recommend that NOT to do so unless you can ensure thaat it is considered as `and` of two expressions.)

## Example
In search query language,

One can easily guess that

```
status:isOpen
```

will find all records that satisfies the status is opened.

One can also easily guess that

```
level:debug && tag:MainActivity 
```

will find all records that satisfies both the message is generate when debugging and tag is `MainActivity`.

## Conclusion
I have simply introduce the core concepts and rule of query search language. However, for brief, I didn't disccuss the details on it. For more details, see [query search language](https://developers.google.com/issue-tracker/concepts/search-query-language).



## Ref
[query search language](https://developers.google.com/issue-tracker/concepts/search-query-language)
