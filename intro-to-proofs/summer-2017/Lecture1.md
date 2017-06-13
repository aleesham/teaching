### Lecture 1 
###### June 13, 2017

## Welcome 
- Introduce yourself! And how Wash U is weird and starts on the 10 minute intervals (:10 or :40)
- Ask them about their intentions with the class.
- Quickly go over the syllabus.
- Mention Exam Days and Holidays.
- Mention that this class might feel unorganized.
- Read Chapter 1 in Krantz
- Homework: 

## Introduction with Geometry
- Do you remember high school geometry? Let us quickly do a T-chart proof and write it into a paragraph.

<center>
<img src = "http://study.com/cimages/multimages/16/flowproof3.jpg" />

<table style="border: 1px solid white; width: 100%">
    <tr style="border: 1px solid white">
        <th style="border: 1px solid white"> Statement </th>
        <th style="border: 1px solid white"> Reason </th>
    </tr>
    <tr style="border: 1px solid white">
        <td style="border: 1px solid white; text-align: left"> 1. FH perp bis</td>
        <td style="border: 1px solid white;text-align: left"> 1. Given</td>
    </tr>
    <tr style="border: 1px solid white">
        <td style="border: 1px solid white; text-align: left"> 2. < EHF = < GHF </td>
        <td style="border: 1px solid white;text-align: left"> 2. By defn of perp bis</td>
    </tr>
    <tr style="border: 1px solid white">
        <td style="border: 1px solid white; text-align: left"> 3. EH = GH</td>
        <td style="border: 1px solid white;text-align: left"> 3. By defn of perp bis</td>
    </tr>
    <tr style="border: 1px solid white">
        <td style="border: 1px solid white; text-align: left"> 4. tri EHF cong to tri GHF</td>
        <td style="border: 1px solid white;text-align: left"> 4. SAS</td>
    </tr>
    <tr style="border: 1px solid white">
        <td style="border: 1px solid white; text-align: left"> 5. EF = FG</td>
        <td style="border: 1px solid white;text-align: left"> 5. CPCTC</td>
    </tr>
    <tr style="border: 1px solid white">
        <td style="border: 1px solid white; text-align: left"> 6. Iso</td>
        <td style="border: 1px solid white;text-align: left"> 6. Defn</td>
    </tr>
</table>
</center>

Assume that FH is the perpendicular bisector of EG. By definition of perpendicular bisector, the angles EHF and GHF are congruent and right. Furthermore, the segments EH and GH are of the same length, again because FH is the perpendicular bisector of EG. Because FH is of course equal to itself, we can conclude that EHF and GHF are congruent by the side-angle-side congruency law. Hence, EF and FG are of the same length because congruent parts of congruent triangles are congruent. Finally, by the definition of isoceles triangle, our triangle EFG is isoceles.

## Introduction with Logic Puzzles
- Now, let us do some logic puzzles.  
    - 1. [The Liar and the Truth Teller:](https://brilliant.org/wiki/truth-tellers-and-liars/)
    - 2. [The Tweleve Pills Problem:](http://mathforum.org/library/drmath/view/55618.html) 
    - 3. There are three boxes in front of you. One box has only apples, one has only oranges, and the last has both apples and oranges. The first box has the label "apples," the second "oranges," and the third "apples and oranges." Unfortunately, all of the boxes are labeled wrong, and you are tasked with fixing them. You aren't allowed to peek inside any of the boxes, but you are able to ask for a single sample from any box. That is, someone will show you just one item from one box of your choosing. Which box can you choose from that will guarantee enough information to fix the labels?

## Section 1.0: A Remark from Aleesha.  
Note that I will be referencing both texts for the majority of Chapter One (in Krantz). Having Krantz's book will be sufficient, but I find some of the wording in Campbell's book to be a bit easier. 

## Section 1.1: Principles of Logic

__Definition:__ An *atomic* or *elementary statement* is a sentence that can be taken as true or false that has with a subject, a verb, and sometimes an object, but has no connectives (such as "And", "Or", "Not", "If-Then", "If-And-Only-If").  

__Examples:__
- Mary has bread.
- Six is greater than seven.
- John is good.

__Definition:__ A *statement* is a sentence or group of atomic statements connected by connectives that can be taken to be true or false, exclusively.

__Examples:__ 
- Six is greater than seven or seven is greater than six.
- If six is greater than five, then five is less than six.

## Section 1.2: Truth  

In everyday conversation, we could argue if the statement "John is good" is true or false. In mathematics, there is nothing to argue about. Either John is good, or he isn't. We have no room for opinion. But how do we decide what is true or false? Krantz states that "the modern methodology in mathematics works as follows,"
- We *define* certain terms.
- We *assume* that there terms have certain properties or truth attributes (these assumptions are called axioms.)
- We specify certain rules of logic.
We use the axioms and definitions along with these rules to obtain new statements that we prive to be true or false. 

__Definition:__ A written arguement which demonstrates the truth of a statement, using only logic and well-established facts is called a *proof*.

On the other hand, if a statement is false, then assuming it is true can lead to a contradiction. Alternatively, if a statement __P__ is false, then it's negation __~P__ (show other notation) can be proven to be true. This is our first of five connectives, and it will lead into our next section.

## Section 1.4: "Not"

Suppose that __A__ is an atomic statement. The statement "not __A__," written ~__A__ (show other notation) is true whenever __A__ is false. 

__Example:__ "Charles is not happily married" is true provided that "Charles is happily married" is false. 

We can summarize these asserations with a truth table:

<center>
<table style="border: 1px solid white">
    <tr style="border: 1px solid white">
        <th style="border: 1px solid white"> A </th>
        <th style="border: 1px solid white"> ~A</th>
    </tr>
    <tr style="border: 1px solid white">
        <td style="border: 1px solid white; text-align: left"> T</td>
        <td style="border: 1px solid white;text-align: left"> F</td>
    </tr>
    <tr style="border: 1px solid white">
        <td style="border: 1px solid white; text-align: left"> 
        F</td>
        <td style="border: 1px solid white;text-align: left"> T</td>
    </tr>
</table>
</center>

It turns out truth tables really allow us to organize our work, and we will see this as we gain experience with them. One helpful note is that if we have `n` distinct atomic statements, then we should have `2^n` rows in our truth table. 

## Section 1.3: "And" and "Or"

Let __A__ and __B__ be atomic statements. The statement "__A__ and __B__" is true when *both* __A__ is true and __B__ is true. For example, conisder __Zach is tall__ and __Zach is fat__. If Zach is both tall and fat, then our statement __A__ and __B__ is true. In all other cases, it is false. 

__Notation:__ We deonte the phrase "__A__ and __B__" with "__A__ ^ __B__" (Note that this text editor does not allow for perfect mathematical symbols. Think "^" for "A.") We often call "__A__ and __B__" the *conjuction* of __A__ and __B__.

Now, let us draw the truth table:
- Note we must list all possible truth vales of __A__ and __B__ along with the corresponding values of the conjuction. 
- Because __A__ and __B__ are two distinct atomic sentences, how many rows should our table have?


Moving onto the "Or" statement. We must add that in mathematics, "Or" is taken by convention to be the *inclusive* "Or" unless noted otherwise. That is, the statement "__A__ or __B__" is true provided either __A__ is true or __B__ is true or both __A__ and __B__ are true. 

__Notation:__ We call "__A__ or __B__" the *disjunction* of __A__ and __B__ and we denote it "__A__ V __B__."

Truth table:
- How many rows do we need to exhaust all possibilities of combinations of truth for our atomic statements?
- When can __A__ V __B__ be false?

__Examples:__
- "x>2 and x<5" is true for the number x = 3 and false for the number x = 6. Why?

- "x is odd and x is a perfect cube" is true for x = 27, and false for x = 7, x = 8, and x = 10. Why?

- "x<3 or x>3" is true for what values of x? Is it false for any values of x? Why or why not.

- Truth Table Practice:
    - (__A__ V __B__) ^ B
    - What do we notice about the above and the __B__ column?

In the next section, we will talk about logical equivalence, which is the idea of column in a truth table being identical. 

## Aside 1.4: (1.3 in Campbell): Logical Equivalence

__Definition:__ Two statements are said to be *logically equivalent* if they contain the same atomic statements and no matter what the truth values of the atomic statements of these two statements are, the two statements have the same truth value.

__Example:__
    - ~(__A__ ^ __B__)
    - (~__A__) V (~__B__)
    - What do we notice about the last two truth tables?

The two above statements are logically equivalent. In fact, this is one of the famous equivalences of the *de Morgan's laws.*

We will get back to logical equivalences as we go on.

## Section 1.5: "If - Then"

## Aside 1.5 (1.3 in Campbell): Logical Equivalences

## Section 1.6: Contrapositive, Converse, and "IFF"

## Aside 1.6 (1.3 in Campbell): Logical Equivalences

## Section 1.7: Quantifiers
## Section 1.8: Truth and Provability



