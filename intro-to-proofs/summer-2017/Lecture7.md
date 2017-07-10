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

__Prop:__ Let \curly{R} be an equivalence relation opn a set A. If x\in A, then define Ex={y\in A: (x,y)\in \curly{R}}. We call the sets Ex the *equivalence classes* induced by the relation \curly{R}. If now s and t are any two elements of A, then either Es\cap Et=\emptyset or Es=Et. In summary, the set A is the pairwise disjoint union of the equivalence classes induced by the equivalence relation \curly{R}.



<!-- Finish Section 5 Next Time -->
Do some of these exercises if time permits:

Exercises: 2, 4, 9abc, 10bdf, 17, 18,


