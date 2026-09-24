# Chapter 1: Generalities

## 1.1 Basic Definitions

**Definition (Mapping):** A mapping from $E$ to $F$ is any relation $f$ such that every element of $E$ has a **unique** image in $F$.

**Domain of definition:** The domain of $f$ is the set
$$D_f = \{x \in D \mid f(x) \text{ exists}\}$$

> 💡 In plain terms: not every $x$ you plug in has to "work" (think $\sqrt{x}$, or $1/x$) — $D_f$ is just the set of inputs where it actually does.

---

## 1.2 Injective Functions

**Definition:** A mapping $f: E \to F$ is **injective** if
$$\forall x, y \in E,\quad f(x) = f(y) \Rightarrow x = y$$

**Proposition (contrapositive form):** $f$ is injective if and only if
$$\forall x, y \in E,\quad x \neq y \Rightarrow f(x) \neq f(y)$$

> 💡 Injective = "no two different inputs share an output." Think of it as a function that never repeats itself.

---

## 1.3 Surjective Functions

**Definition:** A mapping $f: E \to F$ is **surjective** if
$$\forall y \in F,\ \exists x \in E \text{ such that } y = f(x)$$

> 💡 Surjective = "every element of $F$ gets hit" — nothing in the destination set is left out.

---

## 1.4 Bijective Functions

**Definition:** A mapping $f: E \to F$ is **bijective** if it is both injective **and** surjective.

**Proposition:** $f$ is bijective if and only if
$$\forall y \in F,\ \exists! x \in E \text{ such that } y = f(x)$$

> ⚠️ **Correction:** the "$\exists!$" here means "there exists a *unique*" $x$ — not just "there exists" (that would just be surjectivity again). Bijective functions guarantee **exactly one** preimage for every $y$, which is what combines the two properties.

---

## 1.5 Monotonicity

Let $f$ be a function defined on a domain $D \subset \mathbb{R}$:

| Property | Condition (for $x, y \in D$, $x < y$) |
|---|---|
| Increasing | $f(x) \le f(y)$ |
| Strictly increasing | $f(x) < f(y)$ |
| Decreasing | $f(x) \ge f(y)$ |
| Strictly decreasing | $f(x) > f(y)$ |

> ⚠️ **Correction:** the original notes compared $x$ and $y$ directly instead of $f(x)$ and $f(y)$ — easy typo to make, but it changes the meaning completely (comparing $x<y$ to itself is trivially true and says nothing about $f$).

---

## 1.6 Symmetry

Let $f$ be a function on a domain $D \subset \mathbb{R}$:

1. **Even function:** $f$ is even on $D$ if
   $$x \in D \Rightarrow -x \in D \quad \text{and} \quad f(-x) = f(x)$$
2. **Odd function:** $f$ is odd on $D$ if
   $$x \in D \Rightarrow -x \in D \quad \text{and} \quad f(-x) = -f(x)$$

> 💡 Geometrically: even functions are symmetric about the y-axis (like $x^2$), odd functions are symmetric about the origin (like $x^3$).

---

*Notes cleaned up and organized by Claude. Original lesson in progress — more sections to come.*
