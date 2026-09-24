# Chapter 1: Introduction to Logic
*Formal Logic — FSM, First-Year Bachelor's in Big Data and Data Analysis*

## 1. What is Logic?

The word "Logic" comes from the Greek *logos* (reason, discourse), meaning **"science of reason."** It studies **discourse** and **reasoning**.

## 2. Reasoning

In every discipline (math, computer science, exact sciences...) we need to reason about concrete or abstract objects — numbers, geometric shapes, programs, data structures, systems, networks — that have well-defined properties.

**Reasoning** is:
- a mental activity
- expressed through discourse
- carried out in natural language (words, sentences, texts)

**To reason** means to produce a **conclusion** from:
- pre-existing information (**premises**)
- mechanisms for transforming information (**inference rules**)

### Example
> "If it is raining, the road is wet; but the road is not wet — therefore it isn't raining."

| | Statement | Role |
|---|---|---|
| H1 | If it rains, the road is wet | Premise |
| H2 | The road is not wet | Premise |
| C | It isn't raining | Conclusion |

### More examples of reasoning
1. *If it's raining, the road is wet, and it is raining → the road is wet.*
2. *If it's raining, the road is wet, but the road is not wet → it isn't raining.*
3. *To go out in the rain, I take my umbrella; I'm outside without an umbrella → it isn't raining.*

## 3. Validity of an Argument

A reasoning is either:
- **correct / valid**, or
- **incorrect / invalid**

> ✅ **Valid:** "If it's raining, the road is wet, and it is raining → the road is wet."
> ❌ **Invalid:** "If it is raining, the road is wet, and it is not raining → the road is not wet." *(Just because it's not raining doesn't rule out other reasons the road could be wet — e.g. someone hosed it down.)*

## 4. Why Study Logic?

**Reasoning needs formalizing** because natural language isn't suited to it:
- **Ambiguity** — "I went to the bank" (riverbank or financial bank?); "This bag is light" (not heavy, or not dark?)
- **Hard-to-verify truth** — "it will rain tomorrow," "logic is difficult"
- **Paradoxes** — "I am lying" (if true, it's false, and vice versa); "I am certain that nothing is certain"

Logicians want **formal systems** that let reasoning be *mechanized* — turned into a calculus, like arithmetic. Key questions: What is reasoning? Can we guarantee it's consistent? Can it be automated?

## 5. The Logical Approach

1. Study reasoning processes and identify what makes them valid, ignoring irrelevant details.
2. Model natural-language statements using **symbols/formulas** suited to mathematical calculation.
3. Assign a **truth value** to the result.

```
Reasoning to validate  →  Modeled reasoning  →  Valid?
   {Sentences}              {Formulas}
   Natural language         Logical language
   Words, texts             Symbols
        (Representation/modeling)     (Calculus logic)
```

**Logic** = a symbolic language for representing knowledge, built on two concepts:
- **Syntax**: what expressions are possible
- **Semantics**: what an expression *means* (its truth value)

## 6. Types of Logic

- **Classical (mathematical) logic**
  - Propositional logic
  - First-order predicate logic
- **Non-classical logics** (needed to model the real world more precisely)
  - Belief logic, Temporal logic, Non-monotonic logic, Fuzzy logic

Classical/mathematical logic developed through Boole, De Morgan, and Frege (late 19th century), then boomed with Hilbert, Russell, Whitehead, and Gödel (early 20th century), leading to set theory. This course focuses on **propositional logic** and **first-order predicate logic**, using both semantic methods (truth tables, semantic trees) and syntactic methods (proof trees, normal forms).

## 7. Modeling Examples

**Propositional logic** — let P = "it is raining," R = "the road is wet":

| Reasoning | Premises | Conclusion |
|---|---|---|
| If it rains → road wet; it's raining → road is wet | (P ⇒ R), P | R |
| If it rains → road wet; road not wet → it's not raining | (P ⇒ R), ¬R | ¬P |

**Predicate logic** — "All men are mortal; Socrates is a man; therefore he is mortal." Let H(x) = "x is a man," M(x) = "x is mortal":

$$\forall x\,(H(x) \Rightarrow M(x)), \quad H(\text{Socrates}) \ \vdash\ M(\text{Socrates})$$

## 8. Inference Rules

An **inference rule** is a formal mechanism for deriving a new conclusion from known statements.

### Modus Ponens
$$P,\ (P \Rightarrow Q) \ \vdash\ Q$$
*"P implies Q, and P is true; therefore Q is true."*

> Example: "If all students attend class, they'll take their exams; all students attend class → all students will take their exams." Valid by Modus Ponens.

### Modus Tollens
$$\neg Q,\ (P \Rightarrow Q) \ \vdash\ \neg P$$
*"If P implies Q, and Q is false, then P is false."*

> Example: "To go out in the rain I take an umbrella; I'm outside without one → it isn't raining." Valid by Modus Tollens.

### More valid/invalid examples
- ✅ "If it's snowing then it's cold; it is not cold → it isn't snowing." (Modus Tollens)
- ❌ "If f is differentiable at a point, it's continuous there; |x| is continuous at 0 → |x| is differentiable at 0." *(Invalid — this confuses the direction of the implication; continuity doesn't imply differentiability.)*
- ❌ "A cultured man has read Tintin; Mr Salah is well-read → Mr Salah has read Tintin." *(Invalid — being well-read doesn't guarantee reading that specific book.)*

## 9. Tools of Logic

- **Propositions**: statements that are true or false, never both.
- **Logical connectives**:

| Connective | Symbol | Example |
|---|---|---|
| Negation | ¬ | ¬(it_is_raining) |
| Conjunction (and) | ∧ | (it_is_raining) ∧ (no_umbrella) |
| Disjunction (or) | ∨ | (it_is_raining) ∨ (no_umbrella) |
| Implication | ⇒ | (it_is_raining) ⇒ (road_is_wet) |
| Equivalence | ⇔ | (it_is_raining) ⇔ (road_is_wet) |
| Existential quantifier | ∃ | ∃x, man(x) |
| Universal quantifier | ∀ | ∀x, (man(x) ⇒ mortal(x)) |

These combine into complex propositions, e.g.: ¬(road_is_wet) ⇒ ¬(it_is_raining)

## 10. Components of a Logical System

Every logic has three components:
1. **Syntax (Language)**: what counts as a well-formed formula, and how it's written.
2. **Semantics (Model theory)**: the meaning/truth value of each formula; rules for validity and logical consequence.
3. **Deductive system (Proof theory)**: how new results are proved — a formal method for deriving conclusions from premises.

### Two approaches
- **Syntactic approach**: concerned with *formal proof* — deriving new facts from axioms/hypotheses via inference rules.
  > Example: "If it rains, there are clouds; it is raining → there are clouds." (Modus Ponens)
- **Semantic approach**: concerned with truth/falsity of statements, logical consequence, and consistency.
  > Example: Can "Paul does not eat chocolate" and "Paul eats bread or chocolate" both be true at once? *(Yes — Paul eats bread.)*

## 11. Applications of Logic

- **Mathematics**: proving theorems
- **Everyday life**: analyzing arguments (political, legal discourse)
- **Computer Science**:
  - Software specification (requirements)
  - Programming (correctness proofs, logic programming/PROLOG, constraint programming)
  - Networks (proving absence of deadlocks, etc.)
  - AI (robotics/plan generation, fault diagnosis, human-computer dialogue, automatic summarization)
  - Deductive databases (generalizing relational databases)
  - Expert systems

## Course Outline

- **Chapter 1**: Introduction to Logic *(this lesson)*
- **Part I — Propositional Logic**
  - Ch. 2: Syntax
  - Ch. 3: Semantics
  - Ch. 4: Proof Systems
- **Part II — First-Order Predicate Logic**
  - Ch. 5: Syntax
  - Ch. 6: Semantics
  - Ch. 7: Proof Systems

## References
1. Cormen, Leiserson, Rivest — *Introduction to Algorithms*, Dunod, 1994
2. Velu — *Mathematical Methods for Computer Science*, Dunod, 1999
3. Arnold, Guessarian — *Mathematics for Computer Science*, Masson, 2000
4. Bocage, Friedel, Naquet — *L'option informatique en classes prépas. MPSI-MP*, Ellipses, 1997
5. Jaoua — *Logique symbolique et représentation des connaissances*, 1988
6. Kayser — *Knowledge Representation*, Hermes, 1997
7. Lassaigne, de Rougemont — *Logic and the Foundations of Computer Science*, Hermes, 1993
8. Zahnd — *Elementary Logic: A Basic Course for Computer Scientists*, 1998

---
*Notes cleaned up and organized by Claude, from lecture slides prepared by Ms. Elkamel Hager (FSM 2026-2027).*
