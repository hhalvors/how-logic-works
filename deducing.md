---
title: "[How Logic Works: Exercises](index.html)"
author: "Hans Halvorson"
css: "pandoc2.css"
---

# Chapter 2

The proofs in Chapter 2 should *not* use dependency numbers, as they
are only introduced in Chapter 3. Thus, a correctly written proof will
consist of two columns: the first column contains a line number (n)
and a formula, the second column contains a justification. For
example:

---------------   ---------  -------------
(1) $P$                      A
(2) $P\wedge P$              1,1 $\wedge$I
---------------   ---------  -------------


**Exercise 2.1**

1.  Prove that $Q\wedge P$ follows from $P\wedge Q$. That is, write
    $P\wedge Q$ on line $(1)$, then use the rules ($\wedge$
    introduction and elimination) repeatedly until you obtain $Q\wedge
    P$.

2.  Prove that $P\wedge (Q\wedge R)$ follows from $(P\wedge Q)\wedge R$.


**Exercise 2.2** Prove the following sequents.

1.  $P\wedge Q\:\vdash\:Q\vee R$

2.  $P\wedge Q\:\vdash (P\vee R)\wedge (Q\vee R)$

3.  $P\:\vdash\:Q\vee (P\vee Q)$

4.  $P\:\vdash\: (P\vee R)\wedge (P\vee Q)$


**Exercise 2.3** Prove that the following argument forms are valid.
  You may use the rules $\wedge$E, $\wedge$I, $\vee$I, and MP.
  
1. $P\to (Q\to R),\,P\to Q,\,P\:\vdash\: R$

2. $(A\vee B)\to T,\,Z\to A,\,T\to W,\,Z\:\vdash\:W$ 

3. $(A\to B)\wedge (C\to A),\,(C\wedge (W\to Z))\wedge
  W\:\vdash\:(B\vee D)\wedge (Z\vee E)$
  
4. $P\to (P\to Q),\,P\:\vdash\: Q$

5. $P\wedge (P\to Q)\:\vdash\: P\wedge Q$

6. $P\to (Q\to R),P\wedge Q\:\vdash\: R$


**Exercise 2.4** Prove that $Q\to (P\to R),\neg R\wedge Q\:\vdash\:
\neg P$.


**Exercise 2.5** Prove the following sequents. Here the double
turnstile means that you should prove the sequents in both directions.

1. $P\wedge (Q\wedge R)\:\dashv\vdash\: (P\wedge Q)\wedge R$ 

2. $P\:\dashv\vdash\: P\wedge P$


<!--- Pospesel and Marans have many translation problems http://humbox.edshare.ac.uk/id/eprint/5509 -->

**Exercise 2.6** As we mentioned before, there is only an approximate
match between symbolic logic and arguments in the wild. Nonetheless,
to develop your intuitions, it helps sometimes to look at an argument
in the wild, and to try to represent it symbolically. To that end,
let's try our hand at representing the logical form of some
sentences. Here's how we do it. First of all, identify the overall
logical structure of the sentence. Ask yourself: what does the
sentence assert? Is it an atomic sentence in the sense that there is
no internal logical complexity? Does it assert the conjunction of two
other sentences? Does it assert the disjunction of two other
sentences? Etc.

For example, the sentence, "The cat is on the mat," is atomic. In this
case, the best we can do is to represent it with a single letter such
as $P$. On the other hand, "The cat is on the mat, and the dog is in
the kennel," asserts a conjunction of two atomic sentences. Thus, it's
best represented as something like $P\wedge Q$.

For the following sentences, give the most perspicuous representation
you can of their inner logical form. First identify the component
atomic sentences, and abbreviate each with a (distinct) letter. Then
translate the original sentence using the symbols $\vee ,\wedge ,\neg
,\to$ for the logical words "or", "and", "not", "if...then...". (We
have suggested letters for the atomic sentences at the end of each
sentence.)

1.  It's not true that if Ron doesn't do his homework then Hermione will
    finish it for him. $R,H$

2.  Harry will be singed unless he evades the dragon's fiery breath.
    $S,E$

3.  Aristotle was neither a great philosopher nor a great scientist.
    $P,S$

4.  Mark will get an A in logic only if he does the homework or bribes
    the professor. $A,H,B$

5.  Dumbledore will be killed, and either McGonagal will become
    headmistress and Hogwarts will flourish, or else it won't flourish.
    $K,M,F$

6.  Harry and Dumbledore are not both right about the moral status of
    Professor Snape. $H,D$
	
7. The spell will work only if Hermione concentrates and Ron doesn't
   interrupt. ($W,C,I$)
   
8. Draco will apologize or not get dessert, but he won't do
   both. ($A,D$)
   
9. The Quidditch match will be canceled if it rains, unless the field
   can be magically dried. ($C,R,M$)
   
10. If Taylor Swift expresses support for environmental policies, then
    she will also advocate for renewable energy, unless she
    prioritizes economic concerns. ($E,A,P$)
	
11. If Elon Musk innovates in electric car technology or develops new
    space exploration methods, then he will be recognized as a pioneer
    in technology. However, if he fails to achieve progress in either
    field, he will not be recognized as such. ($I,D,R$)
	
12. If it is not sunny then we will not go to the beach. ($S,B$)

13. Either it's sunny or we will not go to the beach. ($S,B$)

14. We will not go to the beach if it's not sunny. ($S,B$)

15. We will go to the beach only if it's sunny. ($S,B$)

16. It's being sunny is a necessary but not sufficient condition for
    our going to the beach. ($S,B$)
	
17. A society does not have free speech unless it allows peaceful
    protests. ($F,P$)
	
18. Professor Plum is the murderer unless the weapon was a candlestick
    or the crime occurred in the library. ($P,C,L$)
	
19. Professor Plum is the murderer only if the weapon was the
    candlestick and the crime occurred in the library, or the weapon
    was the dagger and the crime didn't occur in the
    library. ($P,C,L,D$)
	
20. Provided, but only provided, that the French Fleet is sailed
    forthwith for British harbors, His Majesty's Government give their
    full consent to an armistice for France. ($S,C$)
	
21. For the tenability of the thesis that mathematics is logic it is
    not only sufficient but also necessary that all mathematical
    expressions be capable of definition on the basis solely of
    logical ones.
	
	
	
**Exercise 2.6.1** Display the propositional form of the following
argument. Does it seem valid to you? Does it convince you that God
does not exist? 	
	
Premise 1: If God exists then he is all good and all powerful. 

Premise 2: If God is all good and all powerful then there would be no
suffering.

Premise 3: There is suffering. 

Conclusion: Therefore, God does not exist.


**Exercise 2.6.2** Display the propositional form of the following
argument. Does it seem valid to you?

Premise 1: If the murder happened in the kitchen, then the weapon was
either a knife or a revolver.

Premise 2: The murder did not happen in the kitchen.

Conclusion: Therefore, the weapon was neither a knife nor a revolver.
	
	
**Exercise 2.6.3** Display the propositional structure of the
following argument.

Premise 1: The greatest genius of our time must have made
groundbreaking contributions in multiple advanced fields.

Premise 2: Elon Musk has made groundbreaking contributions in multiple
advanced fields, such as space exploration with SpaceX, electric
vehicles with Tesla, and neural technology with Neuralink.

Conclusion: Therefore, Elon Musk is the greatest genius of our time.


**Exercise 2.7** Prove that the following argument forms are
valid. Each line of your proof must either be one of the premises
given, or it must be justified from previous lines by one of our rules
of inference: MP, MT, DN, $\wedge$I, $\wedge$E, or $\vee$I.

1. $\neg \neg Q\to P,\,\neg P\:\vdash\:\neg Q$

2. $P\to (P\to Q),\,P\:\vdash\: Q$

3. $(P\wedge P)\to Q,\, P\:\vdash\: Q$

4. $P\:\vdash\: Q\vee (\neg\neg P\vee R)$

5. $\neg P\to \neg Q,Q\:\vdash\: P\wedge Q$

6. $P\to \neg (Q\vee R),Q\:\vdash \: \neg P$




**Exercise 2.8** Demonstrate that the following argument forms are
*invalid* by providing a counterexample, i.e. give English sentences
for $P,Q,R$ such that the premises are obviously true but the
conclusion is obviously false.

1.  $P\to \neg Q,\neg P \: \vdash \: Q$

2.  $P\to R\:\vdash \: (P\vee Q)\to R$

3. $P\to Q\:\vdash \: Q\to P$

4. $P\to Q\: \vdash \: P\to (Q\wedge R)$
