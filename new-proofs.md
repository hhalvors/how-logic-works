---
title: "[How Logic Works: Exercises](index.html)"
author: "Hans Halvorson"
css: "pandoc2.css"
---

# [New Proofs from Old](new-proofs.html)


**Exercise 4.1** Which of the following formulas is a substitution
  instance of the formula $P\to \neg Q$?  In cases where you answer
  affirmatively, show how to reconstrue $P$ and $Q$ to get the
  resulting formula.  
  
1. $\neg Q\to \neg P$ 

2. $(P\to \neg Q)\to R$ 

3. $(P\to \neg Q)\to \neg (P\to \neg Q)$


**Aside.** A formula $\psi$ is a substitution instance of another
formula $\phi$ if and only if $\phi$ provides a set of instructions
for disassembling $\psi$ into subformulas. For example, if $\phi$ is
of the form

```haskell
And(IfThen(P,Q),Not(R)) 
```

for atomic sentences $P,Q,R$, then any substitution instance of $\phi$
is of the form 

```haskell
And(IfThen(X,Y),Not(Z))
```

where $X,Y$ and $Z$ are well-formed formulas.


**Exercise 4.2** Do you think the following claims are true or false?
Explain your answers.

1. If $\phi$ is not provable, then no substitution instance of $\phi$
is provable.

2. The sentence $(P\wedge Q)\to R$ has a substitution instance that
can be proven.


**Exercise 4.3** Prove the following sequents.  You may invoke cut
with any named sequent that you have already proven (e.g. excluded
middle, positive paradox, negative paradox).
   
1. $P\leftrightarrow Q\:\vdash\: Q\leftrightarrow P$     

2. $\vdash\: (Q\to P)\vee (P\to R)$     

3. $P\leftrightarrow Q\:\dashv\vdash\: (P\wedge Q)\vee (\neg P\wedge \neg Q)$

4. $\neg (P\leftrightarrow P)\:\vdash\: Q\wedge\neg Q$

5. $P\leftrightarrow Q, Q\leftrightarrow R\:\vdash\: P\leftrightarrow R$

6. $\neg (P\leftrightarrow Q)\:\dashv\vdash\: (P\leftrightarrow \neg Q)$

7. $\vdash\: (P\leftrightarrow Q)\vee (P\leftrightarrow R)\vee
 (Q\leftrightarrow R)$ 
 

**Exercise 4.4** Identify each equivalence used in the following
proof.

---  ----------------------------------------      ---------
1    (1) $(P\to Q)\vee (Q\to P)$                   A
1    (2) $(\neg P\vee Q)\vee (\neg Q\vee P)$       1 RE
1    (3) $\neg P\vee (Q\vee (\neg Q\vee P))$       2 RE
1    (4) $\neg P\vee ((Q\vee \neg Q)\vee P)$       3 RE
1    (5) $\neg P\vee (P\vee (Q\vee\neg Q))$        4 RE
1    (6) $(\neg P\vee P)\vee (Q\vee \neg Q)$       5 RE
1    (7) $(P\vee\neg P)\vee (Q\vee \neg Q)$        6 RE
---  ----------------------------------------      ---------


**Exercise 4.5** Use replacement-style reasoning to convert the
following sentences to disjunctive normal form.  You might wish to
consult the equivalences on page ??.

1. $(P\to Q)\vee (Q\to R)$

2. $(P\leftrightarrow Q)\vee (P\leftrightarrow R)\vee
   (Q\leftrightarrow R)$
