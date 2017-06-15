### Lecture 2 
###### June 15, 2017

## Objectives
- Recall last class
- Finish Chapter 1
- Summary and More Examples of Chapter 1
- Begin Chapter 2
## Reminders
- Read Chapter 1 in Krantz
- Homework: Posted on BB.

#
# Chapter 1 (Continued)

## Recalling Last Class
- Atomic statements
- Statements
- Proof
- Negation
- Conjunction
- Disjunction
- Logical Equivalence (Do an example with two seperate truth tables. ~(A^B) and ~A V ~B)


## Section 1.5: "If - Then"

__Definition:__ A statement of the form "If __A__, then __B__" asserts that whenever __A__ is true, then __B__ is also true. However, when __A__ is false, the statement claims nothing, so the statement is true. We use "__A__ -> __B__" to denote "If __A__, then __B__". This statement is sometimes referred to as a *conditional* where __A__ is the *hypothesis* and __B__ is the *conclusion*. Let us do the truth table:

<center>
<table style="border: 1px solid white">
    <tr style="border: 1px solid white">
        <th style="border: 1px solid white"> A </th>
        <th style="border: 1px solid white"> B </th>
        <th style="border: 1px solid white"> A -> B</th>
    </tr>
    <tr style="border: 1px solid white">
        <td style="border: 1px solid white; text-align: left"> T</td>
        <td style="border: 1px solid white;text-align: left"> T</td>
        <td style="border: 1px solid white;text-align: left"> T</td>
    </tr>
    <tr style="border: 1px solid white">
        <td style="border: 1px solid white; text-align: left"> T</td>
        <td style="border: 1px solid white;text-align: left"> F</td>
        <td style="border: 1px solid white;text-align: left"> F</td>
    </tr>
    <tr style="border: 1px solid white">
        <td style="border: 1px solid white; text-align: left"> F</td>
        <td style="border: 1px solid white;text-align: left"> T</td>
        <td style="border: 1px solid white;text-align: left"> T</td>
    </tr>
    <tr style="border: 1px solid white">
        <td style="border: 1px solid white; text-align: left"> F</td>
        <td style="border: 1px solid white;text-align: left"> F</td>
        <td style="border: 1px solid white;text-align: left"> T</td>
    </tr>
</table>
</center>


__Examples:__
- The following are all true. Why?
    - "If 2=7, then I'm a giraffe."
    - "If cars are invisible, then chickens are not invisble."
    - "If 2=2, then all integers are real numbers.
- The following are all false. Why?
    - "If the sky is blue, then the sky is neon green."
    - "If I am Aleesha, then I am tall."

## Aside 1.5 (1.3 in Campbell): Logical Equivalences

Let us revisit the truth table. Noticing that __A__ -> __B__ is only false in only one particular area, can we make any guesses at a logical equivalence? What if we revisit the definition? (~A V B is equivalent to A->B. Prove this. )

__In class activity:__ page 13 of Campbell (Logical deduction)
 <!-- Notes -->

__In class activity:__ page 14 of Campbell
 <!-- Notes -->

## Section 1.5 (Continued): More Examples

__Examples:__ 
- Assuming "`x`" is a real number, determine if the following statements are true or false:
    - "If `x` is negative, then `-5x` is postive."
    - "If `x>0` and `x^2<0`, then `x>=10.`"
    - "If `x>0`, then `x^2<0` or `2x<0`."

So, why do we care so much about this? Suppose that we know __A__ and __A__->__B__ are both true. What did we decide in our class activity about __B__? This will turn out to be the most commonly used practice in proof writing, known as direct proof. Some other ways to say "If A, then B" include:

<!-- (Include a list here. Page 15 of Cambell.) -->

__In class activity:__ Page 15 of Campbell.
 <!-- Notes --> 

Now, let us explore some statements related to "A implies B."

## Section 1.6: Contrapositive, Converse, and "IFF"

__Definition:__ We call the statement "B -> A" the *converse* of "A -> B." 

It turns out these two statements are logically distinct; that is they are not logically equivalent. We can see this in their truth table:

<!-- Enter truth table -->

And furthermore, we will illustrate this in the following examples: 

<!-- Enter Examples -->

The second example leads us into the next statement related to the conditional "A -> B":

__Definition:__ The statement "A if and only if B", denoted 
"A <-> B" is a brief way of saying "(A->B) ^ (B->A)". We call this statement the *biconditional* of A and B. "if-and-only-if" is often abbreviated "iff." WARNING FOR TALKS: if there are non-mathematicians in the audience, do not abbreviate because it will look like a typographical error. 

<!-- Enter truth table -->

And furthermore, we will illustrate this in the following examples: 

<!-- Enter Examples -->

Finally, we move on to contrapositive, which will be one of our main proof methods in the next chapter.

__Defintion:__ Given "A -> B", the *contrapositive* statement is defined to be "~B -> ~A."

__Example:__ Prove using two truth tables that an implication and it's contrapositive are logically equivalent.

<!-- Enter truth table -->

__Example:__
Here is an example of when we used contrapositives in Calculus I.
<!-- CAmpbell page 12 -->
- If f(x) is differenetiable at x, then f(x) is continuous at x. 
- If f(x) is not continuous at x, then f(x) is not differentiable at x. 

<!-- Krantz page 13 -->
Example 1.6.7 Read this out loud to the class. 


## Aside 1.6 (1.4 in Campbell): "~(A -> B)"

What is the negation of an implication? We need to recall several things: 
- A -> B is logically equivalent to ~A V B
- ~(~A V B) is logically equivalent to A ^ ~B.

__In Class Activity:__ Campbell page 19
<!-- Stuff -->
Write the contrapositive, converse, and negation of the following:
- If x is even, then x^2 is even.
- If x is a real number, then x>0 or x<= 0.
- If x is a multiple of 6, then x is divisible by 2 and x is divisibe by 3. 


## Section 1.7: Quantifiers
This section, like much of the class thus far, is going to be very example driven. We have two basic quantifiers: "For all", often denoted as an upside down A, and "There exists", denoted with a backward E. Note. There exists unique?

__Examples:__ I will explain these
- All automobiles have wheels. 
    - This makes a claim about *every* automobile, not just sedans, or trucks, etc. Furthermore, this claim is true.
- There exists a woman who is blonde.
    - This statement is vastly different from the last. Although it does consider *every* woman, we only make a claim about this universe. We say that considering *every* woman, at least one is blonde. Since there are blonde when, this is true. 
- All women are blonde.
    - This is very different than the last, and is false as not all women are blonde.

__Examples:__ I will guide these
- True or False? Why? Give a counterexample when false.
    - All positive real number are integers.
    - The square of any real number is positive
    - There is a man who is at least ten feet tall.

Note that in the first two, we proved these using a counterexample. A counterexample is saying that "there exists an object that disagrees with your asseration." In the third, we needed to argue that *every* man is less than ten feet tall. Hence,

"There exists" is the negation of "For all" and "For all" is the negation for "There exists." Let us revisit the previous Examples and take their respecitve negations:

__Examples:__ I will guide these
- There exists a real number that is not an integer.
- There exists a real number whose square is not positive.
- Every man is shorter than ten feet tall.

Let's move more into real notation used in mathematics. We will deal with the first two examples above again. Or that x\in \RR

__Examples:__ Assume our universe is the real numbers 
- All positive real number are integers.
    - For every x in R, x in Z.
- There exists a real number that is not an integer.
    - There exists x in R, x in Z.
- The square of any real number is positive.
    - For every x in R, x^2>0
- There exists a real number whose square is not positive.
    - There exists x in R, x^2 <= 0

__NOTE:__ Sometimes the universe is not stated explicility in the statement, but is rather clear from context. For now, assume our universe is the real numbers.

__Example: 1.7.5__
 <!-- Notes -->

__Logical Equivalences:__
 Pages 16 and 17 of Krantz
 <!-- Notes -->

 Mention why we do not really use truth tables here.
We don't often use truth tables since "for all" statements can be thought of infinitely many conjunctions. For example: for every non-zero integer n, n^2 >0. That would be like writing A - n is one, B - 1^2 >0, C n is 2, D 2^2 >0,.... which is not feasible. 

Similarly, we don't use truth tables for "there exists" statements since they can be thought of inifinitley many disjunctions. For example, there exists an integer n such that p(n)=2n^@-5n+2 = 0 is like saying
p(1)=0 or p(-1)=0 or p(2)=0 or p(-2)=0  or ...., which again is not feasible. 


__In Class Activities__: Page 22.
- Write the following statements using quantifiers:
    - If x,y are real numbers, then x+y is a real number. 
    - a_i > 3 for some i in N
    - a_i > 3 for all i in N
- Determine the truth value. Explain.
    - In class activity 2: 1,3,4,5 <!-- -->



## Summary of Chapter One
- Atomic Statement
- Statement
- Proof
- Truth tables
- Five connectives (Symbolizes Table page 7 of Campbell, add the actual words in the table)
    - "Not"
    - "And"
    - "Or"
    - "If-Then"
    - "If-and-Only-If"
- Logical equivalences
- Quantifiers
    - "For all"
    - "There exists"

<!-- I will try to post a sheet of some tables from Campbell about negations, equivalences, etc. -->

## More Examples
- Truth Tables:
    - Krantz: 1b,
    - Campbell: (1.2) 2 and 5,

- Rewrite English into If-Then:
    - Campbell: (1.3) 16,21, 24

- Translating English into Logic
    - Krantz: 2 Negate each sentence, a,b,f,

- Translating Logic into English
    - Krantz: 3 Negate each secntence, adg; 10f

- Converse, Contrapositive and Negation:
    - Krantz: 4af; Just Negate 13cgm

- Determining Truth Value with Quantifiers:
    - Krantz: 5ach

- Find a logically equivalent statement using S,T, ~ V. Use a truth table or other means to explain why they are logically equivalent. 
    - Krantz: 6bd

- Logical Equivalence (Table on page 13)
    - Campbell: Prove 3rd and 4th Lines.

- Other:
    - Campbell: (1.3) 13, 11

#
# Work on Some Homework for 30 Minutes:

<!--

#
# Chapter Two: Methods of Proof

## Section 1: What is a proof?

The difference between mathematicians and other scientists is the fact that we will only take something as fact if it is one-hundred percent true. We construct proofs. As it turns out, we have discovered that there exist statements that can neither be proved true or false. This is a manifestation of G\"odel's incompleteness theorem: that any sufficiently complex logical system will contain such statements. However, for this class and much of undergraduate mathematics, we concentrate on statements which are provable or disprovable. 

Here, we will learn of different methods of proof. 

## Section 2: Direct proof

Here, we assume we know that the natural numbers \N = \{0,1,2,3,...\}. 
In this book, we define even and odd natural numbers as follows:

__Defintion:__ A natural number is said to be even if, when it is divided by two, there is no remainder. 
__Defintion:__ A natural number is said to be eveoddn if, when it is divided by two, the remainder is one.

Thus, by defintion (and the Euclidean algorithm), every natural number is either even or odd.

__Note:__ if a natural number n is even, we can write n=2k for some natural number k. Similarly if a natural number n is odd, we can write n=2k+1 for some natural number k.  

__Some terminology:__ Formal mathematical statements are refered to as theorems, propositions, and lemmas. Theorems are significant results, propositions of lesser importance, and lemmas are normally just needed to prove something larger.

Let us write our first direct proof:

__Propostion:__ The square of an even number is even. (Rewrite as an if-then.)

Proof on page 31

Why can't we use a truth table here? How can we use one? The truth table for A->B shows that if A is true, B must also be true, which is what we showed in our proof. 

__Proposition:__ The square of an odd number is odd. 

__Proposition:__ Prove that if n is a positive integer, then the quantity n^2+3n+2 is even. 


__Proposition:__ The sum of two odd natural numbers is even (Exercise)

__Proposition:__ The sum of an even natural number and an odd natural number is odd.

__Proposition:__ The sum of two even numbers is even. (Exercise)

__Proposition:__ Let n be a natural number. Then either n>6 or n<9.
 
Rewrite an if-then. Show that we assumed that if n is not greater than 6 it must be less than 9. 

__Example:__ Prove that every even integer can be written as the sum of two odd integers. 

__Example:__ Prove the Pythagorean theorem.


### Aside 2.2 of Campbell: Existence Proofs and Counterexamples:

__Example:__


## Section 3: Proof by Contradiction

Rational numbers: what are they?

Again, in mathematics a statement is either true or it is false. If we can prove that A could not possibly be false, then it must be true. Similarly, if we can prove that A could not be true, then it must be false. We will explore a very popular example:

__Theorem:__ There is no rational number with the property that x^2 = 2.
## Section 4: Proof by Induction (We will come back to this)
## Section 5: Other methods of proof

-->
