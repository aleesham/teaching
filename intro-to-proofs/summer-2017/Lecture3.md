### Lecture 3 
###### June 20, 2017

## Objectives
- Questions for HW
## Reminders
- Read Chapter 2 in Krantz
- Homework 1 and 2: Posted on BB.
- First Exam: Next Tuesday. Advice: Copy the homework you turn in Thursday as I will provide solutions ASAP. Furthermore, start/finish HW 2 before the exam since it will help as a study guide. 
#
# Chapter 1 

Questions for the homework?

#
# Chapter Two: Methods of Proof

## Section 1: What is a proof?

Read this section. It tells you how mathematics is different than any other science.

The difference between mathematicians and other scientists is the fact that we will only take something as fact if it is one-hundred percent true. We construct proofs. As it turns out, we have discovered that there exist statements that can neither be proved true or false. This is a manifestation of G\"odel's incompleteness theorem: that any sufficiently complex logical system will contain such statements. However, for this class and much of undergraduate mathematics, we concentrate on statements which are provable or disprovable. 

Here, we will learn of different methods of proof. 

## Aside 2.2 of Campbell: Existence Proofs and Counterexamples:

Here we will prove there exist statements and disprove some for all statements.

__Example:__ Prove that there exists a real number such that x/(x+1) = 5. Can we write this as an if-then statement? Not really. However, if we already know which real number x satisfies x/(x+1) = 5, we can write an if-then as follows: If x = -5/4 then x/(x+1) = 5. 

__Proof:__ Suppose x = -5/4. Then (-5/4)/((-5/4)+1)=(-5/4)/(-1/4)=5. This completes the proof.

__Note:__ Sometimes with there exist statements, it is easier to work backward. If I am told to prove there is a real number x such that x/(x+1) = 5, I would first find x, and then write the proof. Let us redo this problem.

There exists a real number x such that x/(x+1)=5. 

Okay, if such an x exists, I can solve the equation x/(x+1) = 5 for x. Then x = 5(x+1)=5x+5. Thus, -4x = 5 implying that x = -5/4. Checking my answer, I see that (-5/4)/((-5/4)+1)=(-5/4)/(-1/4)=5. Now, we are ready to construct the proof. 

__Proof:__ Let x = -5/4. Then x/(x+1)=(-5/4)/((-5/4)+1) =5. Therefore, there exists a real number x such that x/(x+1) = 5. This completes the proof. 

__In class activity:__ Prove that there exists an integer x > 2 such that x^2-5x+6 =0.

__Outline:__ What can we do here. First of all, we can rewrite x^2-5x+6 by factoring. Then we want x>2 such that x^2-5x+6=(x-2)(x-3)=0. Clearly, 2 is not greater than itself. However 3>2, so x=3 satisfies x>2 and x^2-5x+6=0. Now, let us write this as a proof.

__Proof:__ Let x = 3. Then x > 2 and furthermore, x^2-5x+ 6 = (3)^2-5(3)+6=9-15+6=-6+6=0. Hence, there exists an integer x>2 such that  x^2-5x+6=0.

__Recall:__ If x is a real number, then x is an intger. We said this was false because not all real numbers are integers. For example, 1/2 is a real number that is not an integer. Therefore, we provided a counterexample to show that the statement was false.

__Defintion:__ An example which demonstrates a statement false is called a *counterexample.* 

Let us explore some false statements and think of some counterexamples:
__In class activcity:__ (Write as math statements)
- For every x in the integers, x/3 is in the integers.
    - x = 1.
- For every x in the integers, \sqrt(x) is in the integers.
    - x = 2.
- For every x in the integers, 1/x is in the reals. 
    - x = 0.

Now, we have used specific examples to prove existence statements and disprove for every statements. Why does this work? It is obvious why for existence statements: we just need to find one example where the statement is true. Then such an object exists. Furthermore, disproving a for every statement is the same as proving a there exists statement, which is why providing a counterexample is enough to disprove a for every statement. 

What if we want to prove a for every statement or disprove a there exists statement? We need more machinery and mathematical maturity. This will turn our attention to the idea of direct proofs (and then further to other methods of proof.)

### Back to the Krantz Book

## Section 2: Direct proof

Here, we assume we know that the natural numbers \N = \{0,1,2,3,...\}. 
In this book, we define even and odd natural numbers as follows:

__Defintion:__ A natural number is said to be even if, when it is divided by two, there is no remainder. 
__Defintion:__ A natural number is said to be eveoddn if, when it is divided by two, the remainder is one.

Thus, by defintion (and the Euclidean algorithm), every natural number is either even or odd.

__Note:__ if a natural number n is even, we can write n=2k for some natural number k. Similarly if a natural number n is odd, we can write n=2k+1 for some natural number k.  

__Some terminology:__ Formal mathematical statements are refered to as theorems, propositions, and lemmas. Theorems are significant results, propositions of lesser importance, and lemmas are normally just needed to prove something larger.

Let us write our first direct proof:

__Propostion:__ The square of an even number is even. (Rewrite as an if-then.) If a number n is even, then its square n^2 is even.

__Proof:__ Let n be an even natural number. Then there is a natural number k such that n = 2k. Hence, n^2 = n(n) = (2k)(2k)=4k^2=2(2k^2). Therefore, n^2 can be written as 2 times the natural number 2k^2. Hence, n^2 is even. 

Why can't we use a truth table here? How can we use one? The truth table for A->B shows that if A is true, B must also be true, which is what we showed in our proof. 

__Proposition:__ The square of an odd number is odd. (Rewrite as if-then.) If a number n is odd, then its square n^2 is odd.

__Proof:__ Let n be an odd natural number. Then there is a natural number k such that n = 2k+1. Hence, n^2 = n(n) = (2k+1)(2k+1)=4k^2+4k+1=2(2k^2+2k)+1. Therefore, n^2 can be written as 2 times the natural number 2k^2+2k, added to 1. Hence, n^2 is odd. 

__Proposition:__ Prove that if n is a positive integer, then the quantity n^2+3n+2 is even. 


__Proof:__ K = n^2+3n+2 = (n + 1)(n + 2). Note that either n+1 = 2k for some integer k or n+2= 2k for some integer k because consecutive numbers are even, odd pairs.
Therefore, K = 2(k(n +2)) or K = 2(k(n + 1)). In either case, K is even, so we have completed the proof. 

### __Mention proving by cases__
<!-- Another way to prove this is by using cases which we will explore in section 2.5. -->

__Proposition:__ The sum of two odd natural numbers is even. (Rewrite as if-then.) (In class activity. Give five minutes.)

__Proof:__ Suppose that n and m are two odd natural numbers. Then there are integers r and s such that n = 2r + 1 and m = 2s +1. Therefore, n+m=2r+1+2s+1=2r+2s+2=2(r+s+1). Therefore, n+m can be written as 2 times the natural number r+s+1; hence, n + m is even. 

__Proposition:__ The sum of an even natural number and an odd natural number is odd. (Rewrite as if-then.) (In class activity. Give five minutes.)

__Proof:__ Suppose that n is even and m is odd. Then there exist natural numbers r and s such that n = 2r and m =2s +1. Thus, n + m =2r +2s +1 = 2(r+s) +1. Thus, n + m is odd.

__Proposition:__ The sum of two even numbers is even. (Rewrite as if-then.) (In class activity. Give five minutes.)

__Proof:__ 2m + 2n = 2(m+n)

__Example:__ Prove that every even integer can be written as the sum of two odd integers. 

__Proof:__ Suppose we have the even integer n = 2m. If m is odd, then 2m = m + m is the sum of two odd integers. If m = 2k is even, then 

2m = 2m + 1 - 1 = (m + 1) + (m - 1) = (2k+1) +(2k-1)

is the sum of two odd integers. 

__Example:__ Prove the Pythagorean theorem.

<!-- Look in the book at page 34-36 -->
## __Refer to pages 34 to 36 in Krantz.__
#

## Section 3: Proof by Contradiction


### Aside 2.6 of Campbell:

__Definition__: a *contradiction* is a statement which can never be true. 

__Defintion__: A *proof by contradiction* is a proof in which you assume the negative of your statement is true and then show that it is a contradition. If you show that the negation of the statement cannot under any circumstances be true, then it must be false. Hence, you will have shown the original statement. 

Let us begin an example:

__Statement:__ If a and b are integers and ab is odd, then either a is odd or b is odd. 

__Proof:__ Suppose the statement is not true. That is suppose that a and b are integers, ab is odd, a is even, and b is even. Then there are r and s such that a = 2r and b = 2s. Note then that ab= (2r)(2s)=2(2rs) so ab is even. However, we have assumed ab is odd, so this is not possbile. Therefore, we have reached a contradiction so the original statement must be true. That is, it must be true that if a and b are integers and ab is odd, then either a is odd or b is odd. 

Let us explore the most popular example for this type of proof method. First, we need to discuss the idea of rational numbers.

### Back to Krantz

Rational numbers: what are they? Any number that can be represented as p/q where p,q are integers and q is non-zero.

__Lemma:__ if n^2 is even, then n is even.

__Proof:__ We actually proved this already (by contraposition which we will talk about later)!

__Theorem:__ There is no rational number with the property that x^2 = 2.

In symbols, this is ~(there exists x, x in Q and x^2 = 2) so its negation, which we will assume is, (there exists x, x in Q and x^2=2.)

__Proof:__ Assume there is a rational number x such that x^2 = 2. We may write x = p/q where q is non-zero. Furthermore, we may assume that p/q is in lowest terms. That is, we may assume p and q have no common divisor. Then, x^2 = (p/q)^2 = p^2/q^2 =2. Hence, p^2 = 2q^2 implying that p^2 is even. 
Because p^2 is even, p is also even (by lemma). Therefore, there exists an integer k such that p = 2k. Thus, p^2=4k^2=2q^2. Therefore, 2k^2 = q^2. Hence, q^2 is even implying that q is even. So there exists l such that q = 2l. Therefore, p and q are both divisible by 2. However, we had assumed that p and q have no common divisors, so p=2k and q=2l is a contradiction. Therefore, our original statement is true. That is, there is no rational number with the property that x^2 = 2.

__Theorem:__ The pigeonhole principle: Suppose that n+1 pieces of mail are delivered to n mailbozes. Then some mailbox contains at least two pieces of mail. 

__Proof:__ Seeking a contradiction, assume the contrary. Then each mailbox contains zero or one pieces of mail. But then the amount of mail cannot exceed 1+1+...+1 (one added n times). In other words, there are at most n pieces of mail. This contradicts the fact that there are n+1 pieces of mail, so the original statement must be true. That is, if there are n+1 pieces or mail being delivered to n mailboxes, then some mailbox contains at least two pieces of mail. 

This seems pretty obvious, but proving the fact is necessary if we'd like to use it in mathematics. The pigeonhole principle is incredibly important in mathematics, and you will hear it being used through your mathematical undergraduate career (although I cannot currently think of any examples....)

[Pigeon Hole Examples](http://mathforum.org/mathimages/index.php/Pigeonhole_Principle)


__Theorem:__ There exist infinitely many primes. 

__Proof:__ Suppose the contrary. That is, suppose that there are only finitely many primes, p1,p2, dots, pn. Let P = p1p2p3dotspn + 1. If we divide P by pj tgere us a remainder of 1. (Show this using long division.) Now P is either prime or compositio. Since we know no pj divides P it cannot be composite. So P is prime. However, this is a contradiction because P is a prime not contained in the list p1,p2,...,pn. Hence, the original statement must be true. That is, there exist infinitely many primes. 

__Example 2.3.6:__ Show that there are no positive integer solutions to the equation x^2-y^2=1.

__Proof:__ What do we assume? Try this yourself, and read the book (page 39) if you get stuck. 

Next: we will explore other methods of proof before coming back to section 2.4 on mathematical induction.

<!--
## Section 4: Proof by Induction (We will come back to this)
-->

## Section 5: Other methods of proof

### Secition 5.1: Proof by cases.

Sometimes it is easier to prove a statemet down if we break down the hypothesis first. In the beginning of the direct proofs, we proves the following:

__Proposition:__ Prove that if n is a positive integer, then the quantity n^2+3n+2 is even. 

by arguing that n^2+3n+2=(n+1)(n+2) is a multiple of two consecutive numbers, and one of these numbers must be even. This seems kind of hand-wavy to some, but we can use the technique of proving by cases to make this more precise. 

We restate the problem as follows:

__Propostion:__ If n is even, then n^2+3n+2 is even, OR if n is odd, then n^2+3n+2 is even. This statement is equivalent to the way we previous stated it (which we could argue using a truth table -- but we won't. :) ).

So let us rewrite the above proof using cases.

__Proof:__ Let n be a natural number. Either n is even or n is odd. (Case 1: if n is even, then n = 2k for some natural number k. Thus, n^2+3n+2=2k(2k)+3(2k)+2=2(2k^2+3k+2). Therefore, n^2+3n+2 is even. (Case 2: What is n is odd?) Suppose instead that n is odd. Then n=2k+1 for some natural number k. Thus, n^2+3n+2=(2k+1)(2k+1)+3(2k+1)+2=4k^2+4k+1+6k+3+5=4k^2+10k+6=2(2k^2+5k+3). Therefore, n^2+3n+2 is even. In either case, n^2+3n+2 is even; this completes the proof.


Let us do a couple more examples:

### Aside Campbell Section 2.4: Using cases:

<!-- Page 44 in Campbell -->
__In class activities:__
- If x is any integer, then x^2 + x is even.
    - Proof 1: x^2+x = x(x+1). Either x is even or x+1 is even, so x^2+x is even.
    - Proof 2: Suppose x=2k is even. Then x^2+x=4k^2+2k=2(2k^2+k) is even. Suppose that x=2k+1 is odd. Then (2k+1)^2+(2k+1)=4k^2+4k+1+2k+1=4k^2+6k+2=2(2k^2+3k+1) is even. This completes the proof. 
- Define absolute value. |x|=x if x>=0 and -x if x<0.
- Let a,b \in \RR. Then |ab| = |a||b|.
    - a>=0 and b>=0. ab >= 0 |a||b|=ab=|ab|
    - a>=0 and b<0. |a||b| = a(-b) = -(ab) = |ab|
    - a<0 and b>=0. |a||b| =(-a)b = -(ab) = |ab|
    - a<0 and b<0. |a||b| = (-a)(-b) = ab = |ab|

### Back to Krantz:

__Example 2.5.1:__ Show that every integer n which is a perfect cube is either:
1. A multiple of 9,
2. one less than a mutliple of 9, or
3. one more than a multiple of 9.

Although it may not be immediately obvious, we have three cases. 
1. n = (3k)^3, n is a perfect cube of a multiple of 3.
2. n = (3k+1)^3, n is a perfect cube of one more than a multiple of 3.
3. n = (3k+2)^3, n is a perfect cube of two more than a multiple of 3. 

Why do these exhaust all perfect cubes? Well, there are "three congruency classes" modulo three. We don't have the tools to give a precise reasoning. But we can agree that every integer is either a multiple of three, one more than a multiple of three (3k + 1) or two more than a multiple of 3 (3k + 2). [Krantz does this proof differently, so I suggest reading it.] Now, we are ready to write the proof:

__Proof:__ Suppose first that n = (3k)^3. Then n=27k^3 = 9(3k^3), which is a multiple of 9. Therefore, n is either a multiple of nine, one less than a multiple of 9, or one more than a multiple of 9.

Now, suppose that n = (3k+1)^3. Then n = (3k+1)(9k^2+6k+1) = 27k^3+18k^2+3k+9k^2+6k+1 = 27k^3+27k^2+9k+1 = 9(3k^3+ 3k^2 + k) + 1, so n is one more than a multiple of 9. Therefore, n is either a multiple of nine, one less than a multiple of 9, or one more than a multiple of 9.

Finally, suppose that n = (3k+2)^3. Then n = (3k+2)(9k^2+12k+4) = 27k^3+36k^2+12k+18k^2+24k+8 = 27k^3+54k^2+36k+8 = 9(3k^3+6k^2 + 4k) + 8. Note that 
we can rewrite 9(3k^3+6k^2 + 4k) + 8 = 9(3k^3+6k^2 + 4k) + 9 + (8 - 9) = 9(3k^3+6k^2 + 4k + 1) = 1. Therefore, n is one less than a multiple of 9. Therefore, n is either a multiple of nine, one less than a multiple of 9, or one more than a multiple of 9.

Since we have exhausted the cases, we have completed the proof. 


__Example:__ (Skip if running out of time): Show that if n is an integer, then 3n^2+n+14 is even.

__Proof:__ Case 1: n is even; Case 2: n is odd. 

__Proposition:__ The triangle inequality. For any real numbers x and y, |x+y|<=|x|+|y|. (Page 47 of Krantz)

__Proof:__ Cases:
- x,y >= 0
- x>=0, y<0
- x<0, y>=0
- x,y <0.

### Section 2.5.2: Proof by Contrapositive

Recall the lemma we used to prove that \sqrt(2) is irrational. 

__Lemma:__ if n^2 is even, then n is even.

Recall from truth tables that an implication and its contrapositive are logically equivalent. So proving the lemma above is equivalent to proving:

__Lemma:__ if n is not even, then n^2 is not even.

since not even is the same as odd, we have

__Lemma:__ if n is odd, then n^2 is odd.

which we proved in the beginning of the direct proofs section.

It turns of that sometimes it is easier or clearer to argue the contrapositive, which is why proof by contraposition is a useful method. Let us visit some examples:

__Example:__ Prove that if x,y\in \ZZ, and x+y even, then x,y have the same parity. That is x and y are both even or x and y or both odd.

__Contrapositive:__ Suppose x,y\in\ZZ and x,y do not have the same parity. Then x+y is odd. 

__Proof:__ Suppose (WLOG) x is even and y is odd. Then there exist integers r,s such that x = 2r and y = 2s+1. Then x + y = 2r+2s+1=2(r+s)+1. Hence, x+y is odd. This completes the proof. 

__In class activity:__

- __Example:__ Prove that if k\in\ZZ and 3k+1 even, then k is odd. 
    - __Contrapositive:__ If k is even, then 3k+1 is odd.
    - _Proof_: Five minutes.
- __Example:__ Let x,y\in\RR. Prove that if x+y is irrational, then either x is irrational or y is irrational.
    - __Contrapositive:__ If x,y are rational, then x+y is rational.
    - _Proof_: Five minutes.

### Section 2.5.3: Counting Arguments

These are often important in combinatorics, graph theory, probability. Counting can pretty pretty hard in the abstract world or in a world where there are, although finitely many, a lot of possibilities. I will provide two examples:

__Example:__ Show that if there are 23 people in the room then the odds are better than even two of them having the same birthday. 

__Proof:__ Instead, let us calculate the probability that no two people share the same birthday. If this is less than 50%, then we have shown our claim. Now, we count:

The number of ways 23 people can have different birthdays is:

365* 364 * 363 * ... * 343. 

The number of ways 23 people can have unrestricted birthdays is:

365 * 365 * ... * 365 = 365^(23)

The probility that all 23 people have different birthdays is then

p = ()/() \approx 0.4927 < .5

Therefore, it is more likely that at least 2 out of 23 people share the same birthday than all 23 people having different birthdays.

Explain choose notation: n choose k = n!/(k!(n-k)!). Take this with a grain of salt. I can talk about this more if you'd like later on or I can send resources, but I'm not sure how much we will need this so I am just going to wave my hands a bit. You would see this in a probability class normally (which you can take after calculus 3 normally).

__Example:__ Jill is dealt a poker hand out of a standard deck of 52 cards. What is the probability that she holds a four of a kind?

__Proof:__ To calculate this probability, we need to count the number of hands with four of a kind, the number of possible hands, and take the quotient. If we have 4 aces, then the fifth card can be any of the remaining 48 cards. Hence, that there are 48 ways to have a four of a kind of aces. Similiarly, there are 48 ways to have a four of a king of kings, queens, jacks, etc. Because there are 13 different types of cards (aces, 2,3, etc.) and each has 48 ways of being drawn as a four of a kind, we have a total of

13 * 48 = 624 ways a four of a kind can be drawn. 

Furthermore, there are (52 choose 5) = 2598960 ways to have five cards. 

Hence, the probability that she holds a four of a kind is 624/2598960 \approx 0.00024.



<!--
## Section 4: Proof by Induction (We will come back to this)
-->

## Section 2.4: Proof by Induction:









(265 lines)