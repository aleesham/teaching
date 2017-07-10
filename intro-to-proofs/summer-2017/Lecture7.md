### Lecture 7 
###### July 6, 2017

## Objectives
- Academic Integrity.
- Finish Chapter 3.
- Review Chapter 3.
- Start Chapter 4.
- Will probably not finish this today. Finish Tuesday and visit more examples. You will also visit some examples on Thursday before the exam.
- Mention Structure of the Exam.

## Reminders and Announcements
- Read Chapters 3 and 4 in Krantz
- Homework 3 and 4 are posted and have been updated.
- Homework 3 due 7/11.
- Homework 4 due 7/13.
- Midterm  Exam 2 7/13.

#
# Chapter 3: Set Theory

### Section 3.5: Indexing and Extended Operations

Often we want to manipulate infinitely many sets or some arbitrary number of sets. We could get away with using dotdotdot notation *sometimes*, but instead we will define suitable notation similar to that of a summation as follows:

__Definition:__ If S_1,S_2,\dots are sets, the we define the union and countable intersection as follows:
- Union: \cup_{i=1}^\infty S_j = {x : \exists j such that x\in S_j}
- Intersection: \cap_{i=1}^\infty S_j = {x : \forall j, x\in S_j}

__Examples:__ (3.5.1,2) __Refer to Notes__
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


#
# Chapter 4: Relations and Functions

### Section 1: Relations

__Defn:__ Let S and T be sets. A *relation* on S and T is a subset of S\times T. If \curly{R} is a relation, then we write either (s,t)\in\curly{R} or sometimes s\curly{R}t to indication that (s,t) is an element of the relation. We will also write s\sim t when the relation is clear from context.  

__Example:__ (4.1.1) Let S=\NN and T=\RR. Define \curly{R} on S and T by (s,t)\in\curly{R} if s < \sqrt{t} < s+1. What are some elements of this relation? (2,5), (4,17). So we say 2 is related to 5, and 4 is related to 17. What are some elements not in the relations? (Some elements in ^c\curly{R}?) (5,10), (3,\pi).

__Defn:__ 
- The *domain* of a relation is the set of s\in S such that there exists a t\in T with (s,t)\in \curly{R}. 
- The *image* of the relation is the set of t\in T such that there exists an s\in S with (s,t)\in\curly{R}. 
- It is sometimes convient to refer to the entire set T as the *range* (*codomain*) so we know that it is distinct from the image.  
- __NOTE:__ (So, the way you think of domains/codomains/ranges/images with functions is the same. We will talk about functions later. They are special kind of relations, which is why the way we define a domain is the same.) The image 


__Example:__(4.1.2)
- Let S=T=\NN and define \curly{R} = {(s,t) : s^2 < t.} We claim that the domain is all of \NN. How do we see this? Well, let s\in S and consider t=s^2+1. We know that s^2+1 \in \NN by properties of the natural numbers and that s^2 < s^2+1, so s^2 < t. We constructed a t\in\NN for any s such that s^2< t. So, by definition, the domain must be all of \NN. We can say that s is related to s^2+1 since (s,s^2+1)\in\curly{R}
Now, we consider the image. We know that 1 is not in the image because there is no natural numbers s such that s^2 < 1. However, every other natural number is in the image because if t\in \NN is greater than 1, then letting s=1, we know s^2 = 1< t. Since we have shown that there is an s for all t>1 such that s^2 < t, we have that t is in the image of the relation. We can say if t>=2 then 1 is related to t since 1^2 < 2 <=t.
- The example above? The domain is all of S. How can we see this? the real numbers are dense. There is a real number (infinitely many, in fact) between any two integers, so there certainly exists a real number between two consecutive integers. The image are all positive numbers greater than 1 excluding the naturals that are perfect squares. Therefore, the image of \curly{R} is {t\in\NN : t>=2}.
- Read example 4.1.3. It is about Pythagorean triples and is pretty interesting. To me at least.

__Terminology:__ If S and T are equal sets, say A, then a relation on S and T can be simply said to be a relation on A. 
(
__Example:__ (4.1.4)
Let \ZZ be the integers. Define \curly{R} = {(s,t) : s-t is divisible by 2.)} What is the domain? What is the range? We will also note the following:
if s is an even element, then s is related to t if and only if t is even. Similiar if s is odd, then s is related to t if and only if t is odd. To put it breifly, s is related to t if and only if s and t have the same parity. 

__Note:__  We notice that the last relation created a division into two disjoint sets: all even integers are related to each other and all odd integers are related to one another. This is a special kind of relation:

__Defn:__  (4.1.5) Let \culry{R} be a relation set on A. We say that \curly{R} is a *equivalence relation* if the following properties hold:
- \curly{R} is reflexive: if x\in A, then (x,x)\in\curly{R}.  
- \curly{R} is symmetric: if (x,y)\in \curly{R}, then (y, x)\in\curly{R}. 
- \curly{R} is transitive: if (x,y)\in \curly{R} and (y,z)\in \curly{R}, then (x, z)\in\curly{R}.  

__Examples:__
- Let S=\NN and T=\RR. Define \curly{R} on S and T by (s,t)\in\curly{R} if s < \sqrt{t} < s+1. This CANNOT be an equivalence relation because S\neq T.
- Let S=T=\NN and define \curly{R} = {(s,t) : s^2 < t.} This is not an equivalence relation because (1,1)\not\in\curly{R} (there are other counter examples)
- Let \ZZ be the integers. Define \curly{R} = {(s,t) : s-t is divisible by 2.)} How can we prove this? We verify each property:
    - Let x\in \ZZ. Clearly, x-x=0 is divisble by two. Therefore (x,x)\in\curly{R}.
    - Let (x,y)\in\curly{R}. Then x-y = 2k for some integer k by definition of \curly{R}. Then y-x =2(-k) so (y,x)\in]\culry{R}.
    - Let (x,y) and (y,z) \in \curly{R}. Then x-y = 2m and y-z = 2n for some integers m,n. Thus, x-z = (x-y)+(y-z) = 2m+2n = 2(m+n) is divisible by two, so (x,z)\in\curly{R}.
    - This completes the proof. 

__Note:__ The most important property of equivalence relations is that the relation divides the set into disjoint subsets. Like above, we have the set of even integers, which are all related to each other, and the set of all odds. These are called equivalence classes, which we will no define formally in a proposition. 

__Prop:__ Let \curly{R} be an equivalence relation on a set A. If x\in A, then define E_x = {y in A : (x,y)\in\curly{R}}. We call the sets E_x the equivalence classes unduced by the relations \curly{R}. If now s and t are any two elements of A, then either Es\capEt is empty or identical. In summary, the set A is the pairwise disjoint union of the equivalence classes induced by the equivalence relation \curly{R}

__Note:__ What does this summary mean? It means every element in a\in A is in exactly one equivalence class. It is certainly in Ea since an equivalence relation contains (a,a) for all A. However, it may not be immiediately obvious that these sets are pairwise disjoint and form a partition. (A pairtition of a set A is a pairwise disjoint set whose union is the whole set.) It is cler that \cup Ea = A though. Let us revist the example from before:

__Example:__ Let \ZZ be the integers. Define \curly{R} = {(s,t) : s-t is divisible by 2.)} Here, we said the equivalence classes were the even integers E_{2k}=\curly{E} and the odd integers E_{2k+1}=\curly{O}. This certainly forms a parition. 

__Proof of Prop:__ page 75. __Notes__:

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

__Notes:__ 
- Note that because $f$ is a relation by definition, the domain, range, and image are as defined before. We also sometimes denote the image as f as f(S).
- Condition one mandates that each element of S is associated to some element of T.
- Condition two mandates that each element of S is associated to only one memeber of T. (That is, it passes "the vertical line test" if we relate the two sets as axes.)

__Example:__
- Let S = {1,2,3} and T = {a,b,c}. Set f = {(1,a), (2,a), (3,b)}. Is this a function?  Prove or disprove. __book notes (pg 80)__ 
<!--Written Notes Stop Here -->
- Let S = {1,2,3,4,5} and T = {a,b,c}. Set f = {(1,a), (2,a), (3,b), (4,b), (5,c)}. Is this a function? Yes

__Defn:__ Let f be a function with domain S and range T. We often write such a function as f: S->T. We say that f is *one-to-one* or *injective* if whenever (s,t)\in f and (s',t)\in f, then s = s'.  (f injective iff f(s)=f(s') implies s=s'.) We sometimes refer to such a mapping as an injection.

__Example:__
- Let S=T=\RR and let f be the set of all ordered pairs {(x,x^2) : x\in\RR}. We may also write this function as f(x)=x^2. Verify that f is a function, but that it is not injective. 
- Let S=T=\RR and let f be the function f(x)=x^3+x-5. Then f'(x)=3x^2+1 > 0. So f is strictly increasing, implying that if s < t then f(s) < f(t). It particular, f(s)\neq f(t). So f is one-to-one. 

__Defn:__ Let f be a function with domain S and range T. If, for each t in T there is an s in S such that f(s) = t, then we say that f is *onto* or *surjective.* We sometimes refer to such a mapping as a surjection. 

__Note:__ A function is surjective when its image and its range coincide. 

__Defn:__ A function that is both one to one and onto is a bijection, sometimes called a set-theoretic isomorphism. We will talk more about this later.

__Examples:__ 
- Let S=T=\RR f:S -> T be defined by f(x)=x^2. Consider t=-1\in T. There is no real number s such that f(s)=s^2 = -1. This is not a surjections. __book notes (page 82)__
- Let S = \RR and T=[1,\infty). Let g:S->T be given by g(x)=x^2+1. Prove this is a surjection. 




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

__Example:__ (Example 4.4.2)

__Definition:__ Let f:S->T be a function, and let g:T->U be a function. Then we define, for s\in S, the composite function (g\circ f)(s) = g(f(s)) we call g\circ f the *composition* of the functions g and f. 

__Example:__
- (Example 4.4.4)
- (Example 4.4.5)

__Definition:__ Let S and T be sets. Let f:S->T and g:T->S. We say that f and g are mututally inverse provided that both (f\circ g)(t) = t for all t in T and (g\circ f)(s) =s for all s in S. We write g=f^{-1} and f=g^{-1} and refer to functions f and g as invertible; we call g the inverse of f and f the inverse of g.

__Note:__ It is also worth noting that if a function is invertible, its inverse function is unique. However, we will not explicitly prove this. It can be very complicated. 

__Example:__ 4.4.7

__Defintion:__ Not every function has an inverse. You can read more about this on page 85. It turns out that f:T->S has an inverse if and only if f is bijective. 

__Example:__
- Prove that the function f:\RR->\RR given by f(x) = x^3 has an inverse. __4.4.9__ It turns out the inverse function is g(x)=x^{1/3}.




<!-- Finish Section 5 Next Time -->
Do some of these exercises if time permits:

Exercises: 2, 4, 9abc, 10bdf, 17, 18,


