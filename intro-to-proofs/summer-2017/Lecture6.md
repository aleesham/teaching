### Lecture 6 
###### June 29, 2017

## Objectives
- Go over exam questions?
- Start (and Finish) Chapter 3.
- Visit Chapter 3 Examples
- Start Chapter 4

## Reminders and Announcements
- Read Chapters 3 and 4 in Krantz
- Homework 3 and 4 are posted and have been updated.

#
# Chapter 3: Set Theory

### Section 3.1: Undefinable Terms

__Note:__ I suggest you read this. It talks about how we have to stop defining things at some point. For example, saying "the shortest path between two points." What is a path? What is a point? What do we mean by shortest path? 

So, basically, there are certain terms we consider undefinable. 

In modern mathematics, it is customary to use "set" and an "element of" a as undefinables. A set is declared to be a collection of objects. 

__Notation:__ 
- If S is a set and x is an element of S, we write x\in S or S \ni x.

__Definition:__ We say that two sets S and T are precisely __*equal*__ when they have the same elements. We write S = T. 

__Example:__ {x in N such that x^2>3} = {x in N: x>2}


### Section 3.2: Elements of Set Theory

__Defintion:__ Let S and T be sets. We say that S is a __*subset*__ of T and we write S \subset T or T \containing S if x\inS implies x\in T

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

__Exercise:__ Let S = {x\in N x>=4} and T={x\in N: x<9}. Prove/disprove containments.

__Proposition:__ Let T and S be sets. Then S=T if and only if S subset T and T subset S. (Write A => B and B => A.)

__Proof:__ Read pages 59-60. If S=T then by definition S and T have precisely the same elements. In particular this means that x\inS implies x\in T and x\in T implies x\in S. That is, S\subset T and T\subset S. 

Now, suppose that S\subset T and T\subset S. Seeking a contradiction, suppose that S\not\eq T. Then either there is some element of S that is not in T or that there is some element of T not in S. The first eventuality contradicts the fast that S\subset T and the second contradicts T\subset S. Hence, the original statement holds. Thus, the biconditional holds. 

__Definition:__ (3.2.6) We let \emptyset denote the set that contains no elements. That is, for every x, x\not\in\emptyset. We call it the __*empty set*__. Another notation:{}. 

__Example:__ (3.2.7) It may seem strange to consider a set with no elements, but it is a set that arises naturally. Let S = {x in R such that x^2 < 0}. This set is defined perfectly legally, however, there is no real number whose square is <0. Therefore, S=\emptyset. 

__Note:__ If S is any set, then \emptyset\subset S. 

__Example:__ (3.2.8) S = {x\in N : x+2>= 19 and x<3} (Read the book.)

__Defintion:__ (3.2.9) Let S and T be sets. We say that x is an element of S\cap T if both x\in S and x\in T. It is useful and enlightening to write x\in S\cap T <=> x\in S \wedge x\in T. We call this set the __*intersetion*__ of S and T.

__Defintion:__ (3.2.9)  Let S and T be sets. We say that x is an element of S\cup T if x\in S or x\in T. Again, it is useful and enlightening to write x\in S\cup T <=> x\in S \vee x\in T. We call this set the __*union*__ of S and T.

__Example:__ (3.2.10,12,13,14) 
- 12 in class
- 10 as exercise
- 13 in class
- 14 in class

__Defintion:__ Let S and T be set. We say that X\in S\T if both x\in S and x\not\in T. We may write this logically as x\in S\T the __*set-theoretic difference*__ of S and T. Other notation: S-T.

__Example:__ (3.2.16)

__Defintion:__ Suppse that we are studying subsets of a fixed set X. If S\subset X, then we use the symbol ^cS (S^c, \overline{S}, S') to denote X/S. We sometimes refer to X as the __*universal*__ set. And we call ^cS the __*complement of S (in X)*__

__Examples:__ (3.2.18)

__Proposition:__ Let X be the universal set and S \subset X, T \subset X, then 
- ^c(S\cup T) = ^cS \cap ^cT
- ^c(S\cap T) = ^cS \cup ^cT

__ASIDE__ Section 3.3 on Venn Diagrams. This section is just a couple paragraphs. I would read it to check it out. It basically just says that we sometimes use a Venn Diagram to aid in our understanding. Let use do a few examples

__Examples:__ Let A,B,C be sets (contained in a universal set X.) (Refer to paper notes)


__Note:__ Recall that a picture is not a proof, but it can help make your proof clearer or help you think more clearly. 

__Proposition:__ Let X be the universal set and S \subset X, T \subset X, then 
- ^c(S\cup T) = ^cS \cap ^cT
- ^c(S\cap T) = ^cS \cup ^c

__Proof:__ (Read) We will prove (a) in class and I will let you read (b) or try (b) on your own (or I will revisit at the end of class).

It is often best to treat the proof of equality of two sets as two separate proofs of containment. That is, to show that  ^c(S\cup T) \subset ^cS \cap ^cT and  ^cS \cap ^cT \subset  ^c(S\cup T). Recall the defintion of subset. (A\subset B) if (x\inA \implies x\in B). 

We will first show forward containment. ( ^c(S\cup T) \subset ^cS \cap ^c) Suppose that x \in  ^c(S\cup T). Then by definition x\not\in S\cap T. Thus, x is neither an element of S nor is it an element of T. If x is not an element of S, then x\in ^cS by defintion. Similarly, if x\is not an element of T, x\in^cT by defintion. Since x\in ^cT and x\in^cS, x\in their intersection. Thus, we have shown  ^c(S\cup T) \subset ^cS \cap ^c.

Now, we will show backward containment. (^cS \cap ^cT \subset  ^c(S\cup T)) Suppose that x\in^cS \cap ^cT. Then x\in ^cS and x\in ^cT by definition of intersection. Hence, x\not\in S and x\not\in T. In words, x is neither an element of S nor is it an element of T. That is, x \not\in S\cup T. Therefore, by definition of  complement, x\in ^c(S\cup T). Therefore, we have shown ^cS \cap ^cT \subset  ^c(S\cup T).

Because both containments hold, the sets are equal.


### Section 3.4: Further Ideas in Elementary Set Theory

__Definition:__ Let S and T be sets. We define S\times T to be the set of all ordered pairs (s,t) where s\in S and t\in T. The set S\times T is called the __*set-theoretic product*__ (product, or cartesian product) of S and T. 

__Example:__ Let S = {1,2,3} and T = {a,b}. Then S\times T consists of what elements?

__Note:__ It is not a coincedence that S has 3 elements, T has two elements, and S\times T has 2\cdot 3 = 6 elements. In fact, if we have two finite sets S and T with k and \ell elements respectively S\times T will have k\cdot\ell elements. I will prove this (Exericse 3.20) at the end of class if time permits. 


__Note:__ This next idea can get confusing, so it is good to practice writing power sets. I suggest to try Exercises 18 and 19.

__Definition:__ If S is a set, then the __*power set*__ of S is the set of all subsets of S. We denote the power set by script P(S). We may write X\subset S iff X\inP(S).

__Example:__ Let S={1,2,3}. What is P(S)? P(S) = { {1}, {2}, {3}, {1,2}, {1,3}, {2,3}, {1,2,3}, {} }.

__Propostion 3.4.4.:__ Let S={s_1, s_2, \dots, s_k} be a set where k\in\NN. Then \scriptP(S)= 2^k. 

__Proof:__ We will proceed by induction on k. Note that P(k) is the statement that a set S with k elements has a power set with 2^k elements.

Base case: Suppose k=1. Then \scriptP(S)={{},{s_1}}. The base case holds. 

P(j)impliesP(j+1): Suppose that S={s_1,\dots,s_j} elements and that \scriptP(S) has 2^j elements.  Now consider S'= S\cup {s_{j+1}}. Certainly, \scriptP(S)\subset\script(S') since S\subset S' (because every subset of S is a subset of S' by transitivity.) But \scriptP(S') also contains the set X\cup {s_{j+1}} where X\in\scriptP(S). Thus, the total number of elements of \scriptP(S') is 2^j+2^j=2(2^j)=2^{j+1}.

(This is a bit handwavy, but you can read the book for more clarity.)

__Example:__ (Exercise 19) In this exercise, you will be asked to write out the power set of each set, but for now, let us just count the number of elements that will be in the power set:
- {1,\emptyset,{a,b}}
- {\bullet, \triangle, \partial}
- {\emptyset, {\emptyset}, {{\emptyset}}}

### Section 3.5: Indexing and Extended Operations

Often we want to manipulate infinitely many sets or some arbitrary number of sets. We could get away with using dotdotdot notation, but instead we will define suitable notation similar to that of a summation as follows:

__Definition:__ If S_1,S_2,\dots are sets, the we define the union and countable intersection as follows:
- Union: \cup_{i=1}^\infty S_j = {x : \exists j such that x\in S_j}
- Intersection: \cap_{i=1}^\infty S_j = {x : \forall j, x\in S_j}

__Examples:__ (3.5.1,2)
- (3.5.1) Let Q be the rational numbers and let S_j={x\in Q : 0 < x < 1+1/j}
for j=1,2,3\dots. What does \cup S_j look like? \cap S_j?
    - Note that S_1 = (0,2)\cap Q, S_2 = (0, 3/2)\cap Q, S_3=(0,4/3)\cap Q,.... That is, these sets are nested. so S_1 contains S_j for all j. Therefore, their union must be S_1.
    - Look in the __book/notes__ for this. Prove \cap S_j = (0,1].
- (3.5.2) Note it is possible for nested, nonempty sets. Consider instead S_j={x\in Q : 0 < x <1/j}}. Similar to the last example... \cup S_j = S_1 and
\cap S_j = {x\in Q : 0< x<=0}=\emptyset.

__Definition/Note:__ An __*index set*__ is a set in which our indices range over. In the examples so far, we let the index j range over {1,2,3,\dots}. It is often useful to use a "larger" index set, such as the real numbers, or some unspecified index set. Usually, in these cases, we will call our index set A and index by alpha.

__Example:__ (3.5.3) __notes__

__Proposition 3.5.4:__ Fix a universal set X. Let A be an index set and for each alpha in A, let S\alpha be a subset of X. Then
- ^c(\cap_{\alpha\inA}S_\alpha) = \cup_{\alpha\in A} ^cS\alpha
- ^c(\cup_{\alpha\inA}S_\alpha) = \cap_{\alpha\in A} ^cS\alpha

__Proof:__ (a) is very similar to Prop 3.2.19 (b), which we have not shown (though it is in the book.) So lets prove this one.

(a) __proof in notes__.


TALK MORE ABOUT 26.

### Examples:
Exercises: 1acf, 2, 5bf, 3bf, 4c, 18ghijkl, 21ab, 26(HW)
