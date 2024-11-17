**<h1 align="center">MATHEMATICAL STATISTICS I</h1>**

**CONTENTS:**
- [2.0 The Fundamental Counting Principle](#2.0)
	- [Theorem 2.1: Fundamental Counting Rules](#2.1)
	- [Theorem 2.2: Generalized Fundamental Counting Principle (GFCP)](#2.2)
		- [Factorial Function](#FF)
	- [Theorem 2.3: Linear Arrangements](#2.3)
	- [Theorem 2.4 : Linear Arrangement with Indistinct Elements](#2.4)
	- [Theorem 2.5 : Circular Arrangements](#2.5)
- [3.0 Probability Theory](#3.0)
	- [Theorem 3.1: The Probability of a Complement](#3.1)
	- [Theorem 3.2: The Probability of the Empty Set](#3.2)
	- [Theorem 3.3: The Probability Concerning Subsets](#3.3)
	- [Theorem 3.4: The Probability of Every Event](#3.4)
	- [Theorem 3.5: The Probability of a Union of Two Events](#3.5)
	- [Theorem 3.6: The Probability of a Union of Three Events](#3.6)
	- [Definition of Probability](#DefProbab)
	- [Conditional Probability](#ConditionalProb)
	- [Multiplication Rule](#MultRule)
	- [Independent Events](#IndepEve)


---

# <a name="2.0">2.0 The Fundamental Counting Principle

## <a name="2.1"><u>**Theorem 2.1** : *Fundamental Counting Rules*</u></a>

Suppose there are two experiments, the first one having $m$ possible outcomes and the second having $n$ possible outcomes. Then, together, both experiments have $mn$ possible outcomes.

>***Proof:***
>Let $S_1 = {x_1, x_2, x_3, · · · , x_m}$ be the sample space of the first sub experiment and $S_2 = {y_1, y_2, y_3, · · · , y_n}$ be the sample space of the second experiment. Then, the sample space of doing both sub experiments is given by $S1 × S2 = {(x, y)|x ∈ S1, y ∈ S2}$. From Set Theory, we know that $|S1 × S2| = |S1||S2|$. Therefore, $|S1 × S2| = mn$.

## <a name="2.2"><u><a name="Theorem2.2">**Theorem 2.2 :** *Generalized Fundamental Counting Principle (GFCP)*</a>

If **$r$** experiments have $n_1, n_2, · · · , n_r$ possible outcomes, respectively, then altogether, there are $n_1n_2 · · · n_r$ possible outcomes.

### <a name="FF"><u>Factorial Function</u></a>
For a nonnegative integer n, we define the factorial of n, denoted n! by:

$$n!= \begin{cases} 1 &\text{if }  n=0  \\ n(n-1)! &\text{if } n > 0 \end{cases} $$


## <a name="2.3"><u><a name="Theorem2.3">**Theorem 2.3** : *Linear Arrangements*</a>

There are $n!$ ways to rearrange $n$ distinct objects

> ***Proof:*** Let there be n distinct objects in the set $S = {x1, x2, · · · , xn}$. Then there are $n$ possible objects that can placed in the first position. Since this object cannot be placed again in the next position, there are $n − 1$ remaining possible objects that can be placed second. There are $n − 2$ on the next, and so on. This manner continues until the last position in which only one object can possibly be placed. By [GFCP](#2.2) we find that there are:
> 
> |$n$|$n − 1$| $n − 2$|$· · ·$| $1$ |
>|-|-|-|-|-|
>
> $$n(n − 1)(n − 2)· · ·(1) = n!$$

## <a name="2.4"><u>**Theorem 2.4** : *Linear Arrangement with Indistinct Elements*</u></a>

Let there be n distinct objects, each object appearing $r_1, r_2, ··· , r_n$ times, respectively. Then, there are

$$\frac{(r_1 + r_2 + r_3 + ··· + r_n)!}{r_1!r_2!r_3! ··· r_n!}$$

possible ways to rearrange them.

## <a name="2.5"><u>**Theorem 2.5** : *Circular Arrangements*</u></a>
There are $(n_1)!$ ways to arrange $n$ objects around a circle. (assuming rotations are indistinct)


# <a name="3.0">**3.0 Probability Theory**</a>

Probability is a real-valued set function $P$ that assigns, to each event $A$ in the sample space $S$ , a number $P(A)$ , called the probability of the event $A$ , such that the following properties are satisfied:

|Axiom|Definiton|
|-|-|
|Axiom 1| $P(A) ≥ 0$|
|Axiom 2| $P(S) = 1$|
|Axiom 3|if $A_1, A2, _A3, · · ·$ are events and $A_i ∩ A_j = ∅$ , $i \neq j$ , then $P(A_1 ∪ A_2 ∪ A_3 ∪ · · · ∪ A_k) = P (A_1) + P (A_2) + P (A_3) + · · · + P (A_k)$ for each $k ∈\mathbb{Z}^+$ and $P (A_1 ∪ A_2 ∪ A_3 ∪ · · · ) = P (A_1) + P (A_2) + P (A_3) + ...$ for an infinite, but countable number of events.|



## <a name="3.1">**Theorem 3.1** : _Complement Rule_</a>

$$P(A) = 1 − P(A')$$

> ***Proof:***
> 
> Using the [Axiom 2]() of the definition of probability stating that $P(S)=1$ , we can have
> 
> $\implies P(A) = P(S) - P(A')$
> 
>  $\implies P(A)  + P(A')= P(S)$
>  
>  Since $A \cap A' = ∅$ , we can use Axiom 3 of the definition of probability
>  
>  $\implies P(A \cup A')= P(S)$
>  
>  Using "Compliment Laws" in Set Theory, we can have $A \cup  A' = S$ , then
>
>  $\implies P(S)= P(S)$ □

## <a name="3.2">**Theorem 3.2** : _The Probability of the Empty Set_</a>
$$P(∅) = 0$$
> 
> ***Proof:***
> 
> Using Theorem 3.1, Let $A=∅$
> 
> $\implies P(∅) = 1− P(∅')$
> 
> Using Axiom 2 of the definition of probability and by the definition of sets, we can write $P(S)=1$ and $∅' = S$
> 
> $\implies P(∅)= P(S) - P(S)$
> 
> $\implies P(∅) = 0$ □



## <a name="3.3">**Theorem 3.3** : _The Probability Concerning Subsets_</a>
 If events $A$ and $B$ are such that $A \subseteq B$ , then:
 
 $$P(A) ≤ P(B)$$

> ***Proof:***
> 
> 
> 
> 
> 
> 
> 
> 
> 
> 
> 




## <a name="3.4">Theorem 3.4: *The Probability of Every Event*</a>
For each event A, 

$$P(A) ≤ 1$$

> ***Proof:***
> 
> 
> 
> 
> 
> 
> 
> 
> 
> 
> 
> 
> 


## <a name="3.5">Theorem 3.5: *The Probability of a Union of Two Events*</a>
If $A$ and $B$ are two events, then

$$P(A ∪ B) = P(A) + P(B) − P(A ∩ B)$$

> ***Proof:***
> 
> Using Distributing Law, we can get $A \cup (A' \cap B)$ from $A \cup B$
> 
> >***Proof:***
> >$$A \cup B = A \cup (A' \cap B) $$
> >$\implies S \cap (A \cup B)$
> >$\implies (A \cup A') \cap (A \cup B)$
> >$\implies A \cup (A' \cap B)$ □
> 
> Thus we can re-write $P(A \cup B)$
> 
> $\implies P(A \cup (A' \cap B))$
>
> Since $P(A \cup (A' \cap B))=\varnothing$ , with the help of Axiom 3 of the definition of probability, we can re-write
> 
> $\implies P(A) + P(A' \cap B)$
> 
> Using ***Set Identity***, we can get $P(B) - P(A \cap B)$ from $P(A' \cap B)$
> >***Proof:***
> > $$P (A' \cap B) = P(B) - P(A \cap B)$$
> > 
> > $\implies P (A' \cap B) + P(A \cap B)= P(B)$
> > 
> > Since $(A' \cap B) \cap (A \cap B)= \varnothing$ , with the help of Axiom 3 of the definition of probability, we can re-write $P (A' \cap B) + P(A \cap B)$ to
> > 
> > $\implies P (A' \cap B) \cup (A \cap B)) = P(B)$
> > 
> > $\implies P (B \cap ( A' \cup A)) = P(B)$
> > 
> > $\implies P (B \cap (S)) = P(B)$
> > 
> > $\implies P (B ) = P(B)$
> 
> Then it is safe to re-write $P(A) + P(A' \cap B))$
> 
> $\implies P(A) + P(B) − P(A ∩ B)$
> 
> Thus, $P(A ∪ B) = P(A) + P(B) − P(A ∩ B)$ □



## <a name="3.6">Theorem 3.6: *The Probability of a Union of Three Events*</a>
If $A, B$ and $C$ are any three events, then 

$$P(A ∪ B ∪ C) =P(A) + P(B) + P(C) − P(A ∩ B) − P(A ∩ C)− P(B ∩ C) + P(A ∩ B ∩ C)$$

> ***Proof:***
> Let $B \cup C = D$
> 
> $\implies P(A \cup D)$
> 
> Using Theorem 3.5, we can re-write $P(A \cup D)$ to
> 
> $\implies P(A) + P(D) - P(A \cup D)$
> 
> Since $B \cup C = D$ , we can re-write $P(A) + P(D) - P(A \cup D)$ to
> 
> $\implies P(A) + P(B \cup C) - P(A \cap (B \cup C))$
> 
> $\implies P(A) + P(B) + P(C) - P(B \cap C) - P((A \cap B) \cup (A \cap C))$
> 
> $\implies P(A) + P(B) + P(C) - P(B \cap C) - (P(A \cap B) + P(A \cap C) - P(A \cap B \cap C))$
> 
> $\implies P(A) + P(B) + P(C) - P(B \cap C) - P(A \cap B) - P(A \cap C) + P(A \cap B \cap C)$ □




## <a name="DefProbab"></a><u>**Definition of Probability**</u>
Let a probability set function be defined on a sample space $S$. Let $S = {e_1, e_2, ..., e_m}$, where each $e_i$ is a possible outcome of the experiment. The integer $m$ is called the <u>total number of ways in which the random experiment can terminate</u>. If each of these outcomes has the same probability of occurring, we say that the $m$ outcomes are equally likely. That is:

$$P({e_i}) = \frac{1}{m}$$
$$\text{where }i = 1, 2, 3, ..., m$$

If the number of outcomes in an event $A$ denoted by $h$, then the integer $h$ is called the <u>number of ways that are favorable to the event $A$.</u> In this case, $P(A)$ is equal to the number of ways favorable to the event $A$ divided by the total number of ways in which the experiment can terminate. That is, under this assumption of equally likely outcomes, we have 

$$P(A) = \frac{h}{m} = \frac{N(A)}{N(S)}$$

where $N(A) =$ is the <u>number of ways that A can occur</u> and $N(S) =$ is the <u>total number of ways that S can occur.</u>

## <a name="ConditionalProb"><u>**Conditional Probability**</u></a>

Event $A$, given that event $B$ has occurred, is defined by $$P (A|B) = P (A ∩ B) P (B)$$  where $$P (A ∩ B) = N(A ∩ B) N(S),$$ $$P (B) = N(B) N(S)$$ provided that $P(B) > 0$
> **NOTE:** $P(A|B)$ read as the probability of $A$ given that $B$ has occured.

## <a name="MultRule"><u>**Multiplication Rule**</u></a>

The probability that two events, $A$ and $B$, both occur is given by the multiplication rule

$$P(A ∩ B) = P(B)×P(A|B)\text{ for }P(B) > 0$$

$$P(A ∩ B) = P(A)×P(B|A)\text{ for }P(A) > 0$$


## <a name="IndepEve"><u>**Independent Events**</u></a>
Events $A$ and $B$ are independent if and only if

$$P(A ∩ B) = P(A)×P(B)$$

Otherwise, $A$ and $B$ are called dependent events.
