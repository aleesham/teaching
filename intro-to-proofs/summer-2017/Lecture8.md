### Lecture 8
###### July 11, 2017

## Objectives
- Academic Integrity.
- Finish(?) Chapter 4.
- Summarize(?) Chapters 3 and 4.
- Examples(?) from Chapters 3 and 4.

## Reminders and Announcements
- Read Chapters 3 and 4 in Krantz.
- Homework 4 due 7/13.
- Midterm  Exam 2 7/13.

#
# Chapter 4: Relations and Functions

## Section 1

Review:
__Defn:__ (Equivalence Relation) Let R be a relation on A.  (4.1.5) Let \curly{R} be a relation set on A. We say that \curly{R} is a *equivalence relation* if the following properties hold:
- \curly{R} is reflexive: if x\in A, then (x,x)\in\curly{R}.  
- \curly{R} is symmetric: if (x,y)\in \curly{R}, then (y, x)\in\curly{R}. 
- \curly{R} is transitive: if (x,y)\in \curly{R} and (y,z)\in \curly{R}, then (x, z)\in\curly{R}.  

We finished with the following prop:
__Prop:__ Let \curly{R} be an equivalence relation opn a set A. If x\in A, then define Ex={y\in A: (x,y)\in \curly{R}}. We call the sets Ex the *equivalence classes* induced by the relation \curly{R}. If now s and t are any two elemen ts of A, then either Es\cap Et=\emptyset or Es=Et. In summary, the set A is the pairwise disjoint union of the equivalence classes induced by the equivalence relation \curly{R}.

Now, let us visit some examples.
__Examples:__ Read the other examples 7, 12:
- Example 4.1.8
- Example 4.1.9
- Example 4.1.10
- Example 4.1.11
 
### Section 2: Order Relations
We will skip this section for now. Read it. 

### Section 3: Functions

We will define a function in terms of a relation. Read Krantz to figure out why.

__Defn:__ Let S and T be sets. A function $f$ from S to T is a relation on S and T such that:
- (i) Every s\in S is in the domain of f;
- (ii) If (s,t)\in $f$ and (s,u) \in $f$ then t=u. 

Another way to say this: for every s\in S there is a unique t\in T such that (s,t)\in f.

__Notes:__ 
- Note that because $f$ is a relation by definition, the domain, range, and image are as defined before. We also sometimes denote the image as f as f(S).
- Condition one mandates that each element of S is associated to some element of T.
- Condition two mandates that each element of S is associated to only one memeber of T. This is the idea of a function being "well-defined." (A function MUST be well-defined to be a function. "Is this function well-defined?" basically translates to "Is this *actually* a function?") (Another way to think of this, in terms of \RR^2, is that f it passes "the vertical line test" if we relate the two sets as axes.)

__Example:__
- __notes__ (4.3.2) Let S = {1,2,3} and T = {a,b,c}. Set f = {(1,a), (2,a), (3,b)}. Is this a function?  Prove or disprove.
- __notes__ Let S = {1,2,3,4,5} and T = {a,b,c}. Set f = {(1,a), (2,a), (3,b), (4,b), (5,c)}. Is this a function? Yes.

__Defn:__ Let f be a function with domain S and range T. We often write such a function as f: S->T. We say that f is *one-to-one* or *injective* if whenever (s,t)\in f and (s',t)\in f, then s = s'.  (f injective iff f(s)=f(s') implies s=s'.) We sometimes refer to such a mapping as an injection.


__Example:__
-  __notes__ (4.3.6) Let S=T=\RR and let f be the set of all ordered pairs {(x,x^2) : x\in\RR}. We may also write this function as f(x)=x^2. Verify that f is a function, but that it is not injective. 
- (4.3.7) Let S=T=\RR and let f be the function f(x)=x^3+x-5. Then f'(x)=3x^2+1 > 0. So f is strictly increasing, implying that if s < t then f(s) < f(t). It particular, f(s)\neq f(t). So f is one-to-one. 

__Defn:__ Let f be a function with domain S and range T. If, for each t in T there is an s in S such that f(s) = t, then we say that f is *onto* or *surjective.* We sometimes refer to such a mapping as a surjection. 

__Note:__ A function is surjective when its image and its range coincide. 

__Defn:__ A function that is both one to one and onto is a bijection, sometimes called a set-theoretic isomorphism. We will talk more about this later.

__Examples:__ 
-  __notes__ (4.3.9) Let S=T=\RR f:S -> T be defined by f(x)=x^2. Consider t=-1\in T. There is no real number s such that f(s)=s^2 = -1. This is not a surjection. What if T is non-negative reals?
-  __notes__ (4.3.10) Let S = \RR and T=[1,\infty). Let g:S->T be given by g(x)=x^2+1. Prove this is a surjection. 


### Section 4: Combining Functions
__Note:__ We will now write our functions as f(x) = (formula) as we have before this class. However, we should note it is not always easy to write an elegant formula.

__Defn:__ Let f and g be functions with the same domain S and the same range T. Assume that T is a set in which the indicated arithmetic operations make sense:
- (f+g)(x) = f(x) + g(x)
- (f-g)(x) = f(x) - g(x)
- (f\cdot g)(x) = f(x)g(x)
- (f/g)(x) = f(x)/g(x) provided g(x)\neq zero.

__Note:__ There are defining new functions in terms of the component functions that have domain S but possibly a different image/range. (Why possibly a different range? S=T=\ZZ. f/g has \QQ as a range/image) 

Now, to get used to writing these as relations in the normal sense, we will practice with (a). 

- f is a collection of all order pairs in S \times T that satisfy the conditions for a function as is g. Then:
since (f+g)(s) = f(s) + g(s), we have that if f(s) = t and g(s) = t', then
(f+g)(s)=t+t'. Furthermore, (s,t)\in f, (s,t')\in g, and (s, t+t')\in (f+g). Hence, 
f + g = {(s, t+t') :  (s,t)\in f and (s,t')\in g}.

You will have to do the remainder on your homework.

__Example:__ __notes__ (Example 4.4.2) 

__Definition:__ Let f:S->T be a function, and let g:T->U be a function. Then we define, for s\in S, the composite function (g\circ f)(s) = g(f(s)) we call g\circ f the *composition* of the functions g and f. 

__Example:__
- __notes__ (Example 4.4.4)
- __notes__ (Example 4.4.5)

__Definition:__ Let S and T be sets. Let f:S->T and g:T->S. We say that f and g are mututally inverse provided that both (f\circ g)(t) = t for all t in T and (g\circ f)(s) =s for all s in S. We write g=f^{-1} and f=g^{-1} and refer to functions f and g as invertible; we call g the inverse of f and f the inverse of g.

__Note:__ It is also worth noting that if a function is invertible, its inverse function is unique. However, we will not explicitly prove this. It can be very complicated. 


__Example:__  __notes__ 4.4.7


__Defintion:__ Not every function has an inverse. You can read more about this on page 85. It turns out that f:T->S has an inverse if and only if f is bijective. 

__Example:__
- __notes__ (4.4.9) Prove that the function f:\RR->\RR given by f(x) = x^3 is bijective. This is equivalent to proving it is injective. 


<!----------------------------------------->

## Section 5: Cantor's Notion of Cardinality.
One of the most profound and uncomfortable ideas in modern mathematics is the ideas of inifinites. As I talked about before, the interval (0,1) is the same size as the interval (0,2). In fact, they are both the same size as all of \RR. But they are bigger than the naturals, integers, and rationals. 

__Defn:__ Let A and B be sets. We say that A and B a have the same cardinality if there is a bijective function from A to B. We write card(A)=card(B).


__Example:__ (4.5.2)

__Note:__ If card(A) = card(B) via f_1 and card(B)=card(C) via f_2 then card(A)=card(C) via f_2\circf_1. That is "=" is transitive for cardinalities.

__Defn:__ Let A and B be sets. If there is a one-to-one function from A to B, but no bijection between A and B, then we will write
card(A) < card(B). This notation is read "A has a smaller cardinality than B." Why? We don't want to say less than in the idea of the infinities. Furthermore, card(A)<=card(B) is what you think it is. 

__Note:__ Note that < is transitive with cardinalities, as expected. Further, if A \subset B card(A)\leq card (B). Just consider the inclusion map i:A->B where i(a)=a. This function is certainly one-to-one (but not necessarily bijective) so by definition of "<" in the se3nse of cardinalities, either card(A)< card(B) or card(A)=card(B), so,<=. 



__Example:__ (4.5.4)

__Theorem:__ (Schroder-Bernstein) Let A,B be sets. If there is a one-to-one function f:A->B and  a one-to-one function g:B->A, then A and B have the same cardinality. 

__Proof:__ Omitted, but in the book. This is a pretty complicated proof, and not really worth our time. However, if you are planning on taking many more proof classes, it is worth reading to get a feel fore more "complicated" proofs.

__Defn:__ An infinite set is said to be *countable* if it has the same cardinality as \NN. Note however, that MOST mathematicians use "countable" to mean either infinitely countable or finite. If an infinite set us not countable, that is, if an inifinite set does not have a bijection with \NN, then it is said to be *uncountable.*




__Examples:__
- 4.5.7
- 8
- 9
- 10

__Note__: 10 shows n\times n is countable. We can use similar arguments to show z times z is countable. read. 


__Defn:__ A set S is called *finite* if it is either empty or else there is a bijection of S with a set of the form In={1,2,\dots, n} for some positive integer n. If S is not empty and no such bijection exists, then it is called *infinite*.

__Note:__ Mathematicians define infinite-ness differently. For example, one approach defines an infinite set to be one which can be put in a one-to-one correspondence with a proper subset of itself. For example, we can find a one-to-one correspondence between \ZZ and evens. We can also find a one to one correspondance with \RR and (0,1). By contrast, a finite set cannot be in a one-to-one correspondence with a proper subset of itself. 

<!-- We can probably? stop here. Depends how much time is left. -->

__Note:__ We will take some properties of the naturals for granted although we may return to study them later (chapter 6). For example, we will assume that N is ordered and any nonempty subset of N has a least element

__Prop:__ (4.5.13) If S is countable and R \subset S, then R is either empty, finite, or countable. 

__Proof:__ (We need to adjust this a bit.) Assume S is ordered (we can order it by putting it into correspondence to N and imposing that order.)


__Example:__ Page 93 (\QQ is countable.)

__Theorem:__ (4.5.14) Let S_1 and S_2 be countable sets. Set \curly{S}=S_1\cup S_2. Then S is countable.


__Proof:__

__Prop:__ (4.5.15) If S and T are each countable sets, then so is S\times T. 

__Proof:__

__Corollary:__ (4.5.16) If S1, S2, ..., Sk are each countable sets, then so it S1\times S2\times\cdots\times Sk. 

__Proof:__ Read this proof. Can you prove this inductively? We may revisit this. :)

__Corollary:__ (4.5.17) The countable union of countable sets is countable. 

__Proof:__ Read.



__Example:__ (4.5.21) (This is going to be a difficult example.)

__Example:__ (4.5.22) (This is going to be a difficult example.)



__Prop:__ (4.5.24) Let S be any infinite set. Then S has a subset T that is countable. 

__Proof:__

__Note:__ A natural question that arises, is there a cardinality in bewteen card(N), countable, and card(\RR), which we call the cardinaility of the continuum? It turns out that there is not. Furthermore, there is no "biggest" cardinality, which we will see in the next Theorem.

__Theorem:__ (Cantor's Theorem.) Let S be any set. Then the power set \curly{P}(S), consisting of all subsets of S, has a cardinality greater than the cardinality of S. That is, card(S) < card(\curly{P}(S)).

__Proof:__

__Prop:__ Let S be a set. The set S is infinite if and only if it can be put in a one-to-one correspondence with a proper subset of itself. 

__Proof:__ Outlined in the exercise 4.41. Try this.

<!-- I don't think we will get this far. If we do, take questions or end the day.  -->


#
# Chapter 3: Set Theory (Review of Sections 1 through 4)

__Prop:__ Recall that two sets are equal if the contain precisely the same elements.

__Defn:__ S\subset T iff "x\in S implies x\in T" is true

__Prop:__ S=T iff S\subset T and T\subset S.

__Defn:__ empty set is the set with no elements.

__Defn:__ intersection x\in S\cap T iff x\in S \wedge x\in T

__Defn:__ union x\in S\cup T iff x\in S \vee x\in T

__Defn:__ S\times T ={(s,t): s\in S and t\in T}

__Defn:__ \script{P}(S) is the set of all subsets of S.

<!-- Add Sections 5 -->

### Examples:
Exercises: 1acf, 2, 5bf, 3bf, 4c, 18ghijkl, 21ab, 26(HW)

#
# Chapter 4: Relations and Functions (Review Sections 1, 3 through 5)

### Examples: 
Exercises: 20aci, 25 <!-- need to add stuff -->

