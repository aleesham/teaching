### Lecture 4 
###### June 22, 2017

## Objectives
- Finish Chapter 2.
- Start (?) Chapter 3.
- OR do more examples.

## Reminders
- Read Chapter 2 in Krantz
- Homework 2: Posted on BB.
- First Exam: Next Tuesday. 
- Advice: Copy the homework you turn in Thursday as I will provide solutions ASAP. Furthermore, start/finish HW 2 before the exam since it will help as a study guide. 
- Mention editing HW2.

#
# Chapter 2: Methods of Proof

### Section 2.5.1: Proof by Cases (Continued)

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

__Extra:__ How would we do this by contradiction? It is essentially the same thing as above. Contradiction however does not guarantee that we contradict the hypothesis although in this case it does. 

__Proof:__ Suppose not. Then x,y\in\ZZ, x+y even, and exactly one of x,y even. Assume WLOG x=2r and y=2s+1 for some r,s\in\ZZ. Then x+y=2(r+s)+1 is odd; we have reached a contradiction. 

__Extra:__ How would we do this directly? Either x is even or x is odd. We want to show that if x and x+y is even, then y is even and if x is odd and x+y is even, then y is odd. 

__Proof:__ x= 2r and x+y = 2s implies y=(x+y)-x = 2s-2r=2(s-r) is even. x = 2r+1 and x+y = 2s implies y=(x+y)-x = 2s-(2r+1)=2(s-r)-1=2(r-s-1)+1 is odd.

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

### Aside: Campbell 2.8 Regular Induction:

__Defintion:__ (Weak) induction is a type of argument in which you show that the statement is true for some staring value, and then we go on to show that if the statement is true for some arbitrary k, then it must be true for k+1. This method is often referred to as "the domino effect." Further, it shows the statement is true for all integers greater than or equal to your starting value. 

__Note:__ This proof method relies on the construction and the well-ordering principle in chapter 6. However, it fits here, so we explain it now. 


__Note:__ Read this section to get a better grasp. Pages 40-41 at least.

__Steps in a (Weak) Inductive Proof:__
1. Enunciate the inductive statement, denoted P(n). This should be a simple declarative sentence about the positive integer n. 
1. Verify the case n = 1. (Verify the base case n = starting value).
1. Verify that the case j implies the case j+1. IH: p(j) true.

Let us outline this with an example.

__Example:__ For every natural number n, the number n^2+5n+6 is even.

__Outline:__
1. Enunciate P(n). P(n) is the statement "The number n^2 + 5n + 6 is even."
2. Verify the case n=1.  
When n=1, n^2+5n+ 6 = 1^2+5(1)+6 = 12. Hence, P(1) holds.
3. Verify P(j) implies P(j+1).  
We assume that j^2+5j+6 is even. Furthermore, we see that (j+1)^2+5(j+1)+6 = j^2+2j+1+5j+5+6 = (j^2+5j+6) + 2j + 6, which is even. Hence, P(j) implies P(j+1).


__Proof:__ Let n\in\NN. We want to show that n^2+5n+6 is even. We will proceed by induction. The base case clearly holds as 1^2+5(1)+6 = 12 is even. Now, assume that j^2+5j+6 is even for some fixed j\in\NN. We want to show that (j+1)^2+5(j+1)+6 is even. Because j^2+5j+6 is even, there is some integer m such that j^2+5j+6 =2m. Now, we expand our expression (j+1)^2 + 5(j+1) + 6 which gives j^2+2j+1+5j+5+6 = (j^2+5j+6) + 2j + 6 = 2m+2j+6 = 2(m+j+6). Therefore, the RHS is even, so the LHS is even. Hence, (j+1)^2 + 5(j+1) + 6 is even, which completes our inductive argument. 



__Proof:__ (Directly?) n^2+5n+6 = (n+2)(n+3)

__Proof:__ (Cases) n=2k implies n^2+5n+6 = 4k^2+10k+6 , n=2k+1 implies 4k^2+4k+1+5k+5+6.


__Proposition:__ If n is any natural number, 1+2+dots+n = n(n+1)/2


__Outline:__
1. P(n) is the statement summation k = n(n+1)/2
1. P(1) is the statement 1 = 1(1+1)/2 which is true. 
1. Assume P(j) is true. Then 1+dots+j = j(j+1)/2. Add j+1 to both sides. Then 1+dots+j+(j+1) = j(j+1)/2 + (j+1) = (j+1)((j/2)+1)=((j+1)(1/2)(j+2)) = (j+1)((j+1) + 1 ) /2. 

__Proof:__ Let n\in\NN. We want to show that sum k = n(n+1)/2. We will proceed by induction. The base case is obvious as 1=1. Now, assume the inductive hypothesis. That is, assume that sum k = j(j+1)/2. Adding j+1 to both sides of the equation gives us the following strings of equalities. <!-- Stuff! --> Therefore, assuming sum k = stuff implies that sum k = otherstuff, which completes our inductive argument. 

__Proof:__ (Directly with counting argument! Gauss! Yay.)

__Note:__ recall that in the steps of an induction proof I mentioned we show a "base case." This is our starting value because often times, starting at a different integer. Observe:

__Example:__ For n>=4, 3^n > 2n^2+3n.

__Outline:__  
1. Statement: P(n) 3^n > 2n^2+ 3n
1. Base Case: P(4) 3^4 = 81, 2(4^2) + 3(4) = 32+12 = 44; 81 > 44.
1. Inductive Hypothesis: P(j). Then:  
3^j > 2j^2+3j. Multiplying both sides by 3 preserves the inequality and we conclude that 3(3^j) > 3(2j^2+3j) implying that 3^(j+1) > 6j^2 + 9j. 
Now we have the following:

LOOK IN THE BOOK PAGE 44. 

Hence, we are done. 

__Example:__ FIbonacci stuff

__Proof:__ In class (Page 44)

__Example:__ (Page 63 of Campbell)

__Example:__ sum of first n odd is n^2 

__Proof:__ (If there is time. Otherwise suggest that they read.)


__Complete (Strong) Mathematical Induction:__ (Page 45):

__Example:__ Every number > 1 is prime or a product of primes. (Page 46.)

#
# More Examples from Chapter
3, 4, 5, (Examples below), 12, 13, 21, 25, 34

__Example:__ Let a be an integer. If p a prime divdes a^2, then p divides a.
__Note:__ You need this fact for your homework.

__Example:__ Show that sqrt(3) is irrational.

#
# Chapter 3: Set Theory

### Section 3.1: Undefinable Terms

__Note:__ I suggest you read this. It talks about how we have to stop defining things at some point. For example, saying "the shortest path between two points." What is a path? What is a point? What do we mean by shortest path? 

So, basically, there are certain terms we consider undefinable. 

In modern mathematics, it is customary to use "set" and an "element of" a as undefinables. A set is declared to be a collection of objects. 

__Notation:__ 
- If S is a set and x is an element of S, we write x\in S or S \ni x.

__Definition:__ We say that two sets S and T are precisely equal when they have the same elements. We write S = T. 

__Example:__ {x in N such that x^2>3} = {x in N: x>2}


### Section 3.2: Elements of Set Theory

__Defintion:__ Let S and T be sets. We say that S is a subset of T and we write S \subset T or T \containing S if x\inS implies x\in T

__Example:__ 
- Page 59. Is S a subset of T or is T a subset of S? S of T, but not T of S.
- S = {x in N : x>3} and T = {x in N: x^2 > 4}
- S of T: Proof
- T of S: Counterexample.

__Example:__ 
- Page 59. Is S a subset of T or is T a subset of S? S of T, but not T of S.
- S = {-2, 3} and T = {x in Z : x^3-x^2-6x = 0}
- S of T: Proof
- T of S: Counterexample.

__Exercise:__ Let S = {x\in N x>=4} and T={x\in N: x<9}. Prve/disprove containments.

__Proposition:__ Let T and S be sets. Then S=T if and only if S subset T and T subset S. 

__Proof:__ Read pages 59-60.

__Definition:__ We let \emptyset denote the set that contains no elements. That is, for every x, x\not\in\emptyset. We call it the empty set. Another notation:{}. 

__Example:__ S = {x in R such that x^2 < 0}

__Note:__ If S is any set, then \emptyset\subset S. 

__Example:__ (3.2.8) <!-- Start reading again here. -->

### Section 3.3: Venn Diagrams
### Section 3.4: Further Ideas in Elementary Set Theory
### Section 3.5: Indexing and Extended Operations




