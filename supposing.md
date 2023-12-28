---
title: "[How Logic Works: Exercises](index.html)"
author: "Hans Halvorson"
css: "pandoc2.css"
---

# [Supposing](supposing.html)

The proofs in this chapter require the use of dependency
numbers. Thus, a correctly written proof consists of three columns
with a list of dependency numbers in the first column, a line number
and a formula in the second column, and a justification in the third
column. For example:


------   -----------------------------  ---------------
1        (1) $P$                        A            
2        (2) $Q$                        A            
1,2      (3) $P\wedge Q$                1,2 $\wedge$I
1        (4) $Q\to (P\wedge Q)$         2,3 CP       
------   -----------------------------  ---------------


**Exercise 3.1** Prove the following sequents. (You should not use
reductio ad absurdum in any of these problems, although you might be
tempted to do so in 3.1.8, 3.1.9, and 3.1.10. The hints explain how
the other rules can be used to derive the same things as RA, albeit in
a much more roundabout way. For the philosophically minded: MT is an
"impure" rule since its application requires the presence of different
connectives.)

1.  $P\:\vdash\: Q\to (P\wedge Q)$

2.  $(P\to Q)\wedge (P\to R)\:\vdash\: P\to (Q\wedge R)$

3.  $P\to (Q\to R)\:\vdash\: Q\to (P\to R)$

4.  $P\to Q\:\vdash\: (Q\to R)\to (P\to R)$

5.  $P\to (P\to Q)\:\vdash\: P\to Q$

6.  $P\to (Q\to R)\:\vdash\: (P\wedge Q)\to R$

7.  $(P\vee Q)\to R\:\vdash\: P\to R$

8.  $\neg P\:\vdash\: \neg (P\wedge Q)$ (Hint: For any sentences
      $\phi$ and $\psi$, if you can derive $\psi\vdash\phi$ then you
      can derive $\neg\phi\vdash\neg \psi$. Indeed, apply CP to
      $\psi\vdash\phi$ to derive $\vdash \psi\to \phi$. Now assume
      $\neg \phi$ and apply MT.)

9.  $\neg (P\vee Q)\:\vdash\: \neg P\wedge\neg Q$ (Hint: If you can
      prove $\neg (P\vee Q)\vdash \neg P$ and $\neg (P\vee Q)\vdash
      \neg Q$ individually, then you can use $\wedge$I and you're
      done. )
	  
10. $P\to \neg P\:\vdash\:\neg P$ (Hint: First prove that $P\vdash
      (P\to \neg P)\to \neg P$, resulting in a proof with first line
      "$1\: (1)\,P\: \mathrm{A}$" and last line "$1\: (n)\,(P\to \neg
      P)\to \neg P$". Now use line 1 again to derive $\neg\neg P$ and
      apply MT.)
	  
11. $P\to (Q\to R),P\to Q\:\vdash \: P\to R$

12. $P\to (Q\to R)\:\vdash\: (P\to Q)\to (P\to R)$

13. $P\to Q\:\vdash \:\neg Q\to\neg P$ 

14. $(P\wedge Q)\to R\: \vdash \: P\to (Q\to R)$

15. $P\to (Q\to R)\:\vdash\: P\to (\neg R\to \neg Q)$

16. $P\to (Q\to R)\:\vdash\: \neg R\to (Q\to \neg P)$

17. $(P\to Q)\to P\:\vdash\: (P\to Q)\to Q$ (Hint: Not as difficult as
    it looks. Assume $(P\to Q)\to P$ and $P\to Q$. The latter can be
    used both as the antecedent of a conditional, and as a conditional
    itself.)


**Exercise 3.2** Prove the following sequents. (Do not use reductio ad
absurdum, which is only introduced in a subsequent section.)

1.  $\vdash\:(P\wedge Q)\to (Q\wedge P)$

2.  $\vdash\:(P\wedge Q)\to P$

3.  $\vdash\:Q\to (P\to Q)$

4.  $\vdash\:Q\to (P\to P)$ 

5.  $\vdash \:P\vee \neg P$ (Hint: This *can* be proven with the rules
    we have so far! One possibility is to use 3.1.10, but replace $P$
    with $P\vee \neg P$. In particular, use the fact that $\neg (P\vee
    \neg P)\vdash P$ to derive $\vdash \neg (P\vee \neg P)\to \neg\neg
    (P\vee \neg P)$.)
	
6. $\neg P\: \vdash \: P\to Q$ (Hint: Prove $\neg P\vdash \neg Q\to \neg P$
   and then use the contrapositive maneuver.)
   
7. $\vdash\: (P\to Q)\to (\neg Q\to \neg P)$

8. $(P\to Q)\to P,Q\:\vdash \: P$	
	
9. $(P\to Q)\to P\: \vdash \: \neg P\to P$



**Exercise 3.3** Prove the following sequents. (Still do not use
RA. It is good to learn to prove directly when you can!)

1.  $(P\to R)\wedge (Q\to R)\:\vdash\: (P\vee Q)\to R$

2.  $P\vee (Q\vee R)\:\dashv\vdash\: (P\vee Q)\vee R$

3.  $P\vee Q,\neg P\:\vdash \: Q$ (Hint: Recall that $\neg P\vdash
    P\to Q$.)

4.  $P\wedge (Q\vee R)\:\dashv\vdash\: (P\wedge Q)\vee (P\wedge R)$

5.  $P\vee (Q\wedge R)\:\dashv\vdash\: (P\vee Q)\wedge (P\vee R)$

6.  $\neg P\vee Q\:\dashv\vdash\: P\to Q$

7.  $\neg P\vee \neg Q\:\vdash\: \neg (P\wedge Q)$


**Exercise 3.4** Prove the following sequents.

1.  $P\to Q\:\vdash\: \neg (P\wedge \neg Q)$

2.  $\neg (P\wedge Q)\:\vdash\: \neg P\vee \neg Q$

3.  $\neg (P\to Q)\:\vdash\: P\wedge \neg Q$ 

4. $\vdash (P\to Q)\vee (Q\to P)$ 

5. $P\to (Q\vee R)\:\vdash\: (P\to Q)\vee (P\to R)$

6.  $(P\wedge Q)\to \neg Q\:\vdash\:P\to \neg Q$

7. $P\wedge\neg Q\:\vdash\: \neg (P\to Q)$

8. $\vdash\: ((P\to Q)\to P)\to P$ (Hint: One possibility is to first
   prove $\vdash P\vee \neg P$, and then argue by cases. The first
   case is easy if you remember "positive paradox". For the second
   case, remember "negative paradox", i.e. that $\neg P$ implies $P\to
   Q$.)
   
9. $P\to (Q\vee R)\:\vdash \: \neg R\to (\neg Q\to \neg P)$

10. $P\to \neg Q\:\vdash\: (P\wedge Q)\to R$

11. $P\to \neg Q\:\vdash\: P\to (Q\to R)$

12. $\neg (P\to Q)\:\vdash \: P\to \neg Q$

13. $P\:\dashv\vdash\: (P\wedge Q)\vee (P\wedge\neg Q)$

14. $P\to (Q\to R)\:\dashv\vdash \: (P\to Q)\to (P\to R)$

15. $P\to\neg P\:\dashv\vdash\:\neg P$

16. $P\to (Q\to \neg Q)\:\dashv\vdash\: P\to \neg Q$
	  
17. $(P\to Q)\to (P\to \neg Q)\:\dashv\vdash\: P\to \neg Q$	  

18. $P\:\dashv\vdash\: P\wedge (Q\vee\neg Q)$

19. $P\:\dashv\vdash\: P\vee (Q\wedge\neg Q)$

20. $(P\to Q)\to Q\:\vdash\: (Q\to P)\to P$

21. $(P\to Q)\to R\:\vdash\: (P\to R)\to R$

22. $(P\to R)\to R\:\dashv\vdash\: P\vee R$ (Hint for $\vdash$: it's
    easy to derive $\neg P\to R$ from the sentence on the left.)
	
23. $(P\to Q)\to P\:\dashv\vdash \: P$ (Hint for $\vdash$: assume
    $\neg P$ and derive $P\to Q$.)



**Exercise 3.5** People who reject DN elimination also tend to reject
the law of excluded middle.[^1] This exercise explains why. Use the
law of excluded middle and EFQ to re-derive DN elimination. That is,
show that $\neg\neg P\vdash P$, without using DN, but where you're
allowed to insert $P\vee\neg P$, and where you're allowed to infer
anything from a contradiction.

For discussion: is the law of excluded middle more obviously correct
than the DN rule?

**Exercise 3.6** An earlier exercise shows that the following sequent
is provable: $\vdash (P\to Q)\vee (Q\to P)$. Give an example of
English sentences $P$ and $Q$ where it does *not* seem correct to say
that either $P\to Q$ or $Q\to P$ is true. Discuss what this means
about the relationship of propositional logic to rational thinking.

**Exercise 3.7** Show that $\Gamma\vdash \neg (\neg \phi\wedge
\neg\psi )$ can be derived from $\Gamma\vdash\phi$ without using the
$\vee$ rules at any step.


**Exercise 3.8** Consider the following scenario:

If $a$ is at home then so is $b$.

Either $d$ or $e$, or both are at home.

Either $b$ or $c$, but not both are home.

$d$ and $c$ are either both at home or both not at home.

If $e$ is at home then $a$ and $d$ are also at home.

Using the letter $X$ for the sentence "$x$ is at home", write these
conditions in propositional logic notation. Then prove that there is a
unique scenario that satisfies these conditions. (Hint: Assume $E$ for
RA.)


**Exercise 3.9** Show that the rule MT can be derived from the other
rules.


**Exercise 3.10** Show that the rule of DN introduction can be derived
from the other rules.


**Exercise 3.11** We say that a proof is *intuitionist* if it does
*not* use DN elimination --- but it can use the derived rule EFQ. Show
that the following two schema are intuitionistically equivalent: 

1. $\vdash \: \psi\vee \neg \psi$

2. $\vdash ((\phi \to \neg \phi )\to \phi)\to \phi$

By calling them "schema", we mean that one is allowed to replace the
Greek letters with any sentence whatsoever (not just atomic
sentences). So a schema is an infinite collection of axioms with the
same form. (All of our inference rules are actually schematic in this
sense.)


**Exercise 3.12** Show that there is a formula $\chi$ such that for
every formula $\phi$, $\vdash \phi\leftrightarrow (\chi\to \phi )$.


**Exercise 3.13** Show that there is an intuitionistic derivation of
$\vdash P\vee\neg P$ from the schema $\phi\to (\psi\vee \theta )\vdash
(\phi\to \psi )\vee (\phi\to \theta )$. Hint: use $Q\vee \neg Q$ for
$\phi$. Supposing that there is no intuitionist proof of $\vdash P\vee
\neg P$, argue that there is no intuitionist proof of $P\to (Q\vee
R)\vdash (P\to Q)\vee (P\to R)$. 


