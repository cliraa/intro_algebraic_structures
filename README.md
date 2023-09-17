# Introduction to Algebraic Structures

Defining basic cryptographic concepts:

Today it's time for algebraic structures. Let's begin!

## Let's start from the basics: What is a set?

A set is a collection of elements. We can talk about a set of books, a set of buildings, sets of numbers, etc.

Sets, as you can see, can have finite or infinite elements.

Think for a moment about the set of days of the week (Monday, Tuesday, Wednesday, and so on until Sunday); that would be a finite set, right?

On the other hand, the set of integers (those numbers without decimals) constitutes an infinite set.

## Now, what happens if we somehow relate a set to an operation?

For example, let's relate natural numbers to addition.

If we add two natural numbers (no matter which ones), we will obtain another natural number as a result. Here are some examples:

2 + 7 = 9

1 + 3 = 4

5 + 2 = 7

Since this happens, we say that addition is an 'internal composition law' in natural numbers.

The same cannot be said for subtraction, since if we take two natural numbers and subtract them, it may happen that the result is a negative number:

4 - 6 = -2

... and for this reason, it is said that subtraction is not an "internal composition law" in natural numbers.

On the other hand, in algebraic structures, there is a very particular concept called "neutral element".

## Neutral element:

In the case of working with addition, it is an element e of a set S, such that for any other element a of S, it is satisfied that:

a + e = e + a = a

It's very simple:

In that case, we can say that the neutral element is 0.

For every element a of the natural numbers, we have: a + 0 = 0 + a = a

For example:

7 + 0 = 0 + 7 = 7

If the operation we associate with natural numbers is multiplication, then the neutral element would be 1; since for every a belonging to natural numbers, we have:

a * 1 = 1 * a = a

For example:

7 * 1 = 1 * 7 = 7

## Great! To continue, it is important to remember what the associative property is in mathematics:

If we continue with the example of addition, we say that this operation is associative if it holds that:

(a + b) + c = a + (b + c), for all a, b, and c belonging to the natural numbers.

## With all that said, we can define what a monoid is:

A monoid is an algebraic structure that:

- Relates a set with an associative operation,

- Where that operation is an internal composition law in that set,

- And it has a neutral element.

So far so good, but... when studying cryptography, the concept of a group is more commonly encountered than that of a monoid.

No problem:

## Groups:

A group is nothing more than a monoid that has an 'inverse element' for each element in the set.

## Inverse element?

Let me explain:

Working with integers, if the operation in the group is addition, then the inverse of x would be -x; it is the element that, when added to x, results in 0. 

Since x + (-x) = 0, we say that -x is the additive inverse of x. 

For example, -7 would be the inverse of 7. 

For multiplication, the following happens: 

The multiplicative inverse of x is defined as x ^ -1. 

So, x * (x ^ -1) = 1. 

For example, 7 * (7 ^ -1) = 1. 

At this point, it is worth mentioning that (taking addition as an example) if for two elements in the group, a and b, it holds that: 

a + b = b + a, then the operation is said to be commutative, and the group in question is an abelian group. This is very relevant in cryptography. 

## Some examples of groups are: 

- The set of integers with addition. 

- The set of rational numbers with addition. 

- The set of rational numbers, excluding zero, with multiplication.

In cryptography documents, it is common to come across the concept of a field. What is that?

## Fields:

Well, a field is a non-empty set A that is related to two operations "+" and "*" in the following way:

### - A with addition forms an abelian group.

### - And for multiplication:

- The operation is associative and commutative.

- There exists a neutral element and every element that is not 0 has an inverse.

- Additionally, if a, b, and c belong to A, then a * (b + c) = (a * b) + (a * c).

### Some examples of fields are:

- The set of real numbers with addition and multiplication.

- The set of rational numbers with addition and multiplication.

- Finite fields (highly used in cryptographic systems).

In conclusion, this is a super interesting and fundamental topic to understand how many cryptographic systems work.

I hope you enjoyed this material as much as I did, and above all, I hope it is very useful.

Until next time!
