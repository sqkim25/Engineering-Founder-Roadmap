Now, use the following framework to create a full spectrum of problems both in variety and diffculty that would fully prepare a student for a highly challenging test on the content:

Let me give you a _framework_ for thinking about how Korean-style books generate that dense, vertically-layered spectrum of problems.

---

## 0. First principle: difficulty = structure, not just ugly numbers

Before talking about generation, it helps to unpack what makes a problem “easy” or “hard”:

- **Surface difficulty**
    
    - Ugly numbers, fractions, big exponents, long statements
        
- **Structural difficulty**
    
    - How _hidden_ the main idea is
        
    - How many _steps_ and _switches of viewpoint_ are needed
        
    - How many _concepts_ are entangled
        
    - How likely students’ **default habits** will fail / mislead
        

Korean books are really good at controlling structural difficulty in _small steps_. That’s what we want to imitate.

So: when generating problems, think less “change 2 into 3” and more “what mental move do I want to force? how can I hide it / emphasize it / combine it?”

---

## 1. Classic starting point: variables & constraints (and how to push beyond)

You already mentioned:

> identify variables/constraints and choose which are known/unknown.

Example: distance-rate-time problems

- Variables: (d, r, t)
    
- Constraints: (d = rt), maybe multiple trips, relationships like “they meet”, “one arrives earlier”, etc.
    

From here, you can vary:

1. **Number of constraints vs variables**
    
    - Exactly determined (one solution)
        
    - Underdetermined (many solutions → ask “find all”, “describe set of solutions”)
        
    - Overdetermined (check consistency, “does such a number exist?”)
        
2. **Visibility of constraints**
    
    - Given explicitly as equations
        
    - Hidden inside words, diagrams, or patterns
        
    - Split across sentences so the student must integrate
        
3. **Nature of unknown**
    
    - Numerical answer
        
    - Expression in terms of parameters
        
    - Condition (e.g., “for which values of (k) does this system have solutions?”)
        

This is a good base, but we can attack it from more angles.

---

## 2. Lens A: “Type → Variation → Fusion → Creative”

This is basically the Korean 쎈 → 일품 → 블랙라벨 philosophy in abstract form.

Pick a **single core idea** (a “type”):

> Example core idea: “Use the discriminant to reason about number of real roots.”

Then build levels:

### Level 1 – Pure type (Mechanical)

- Direct application of the idea, nothing hidden.
    
- Data is nice; wording is plain.
    

> “Find the number of real roots of (x^2 - 5x + 6 = 0).”

### Level 2 – Variation (Same core, slightly hidden)

- Same idea, but:
    
    - more symbols (parameters),
        
    - or extra steps before applying the idea,
        
    - or small twist (inequality, absolute value, etc.).
        

> “For which values of (k) does (x^2 - (k+1)x + k = 0) have two distinct real roots?”

### Level 3 – Fusion (Multiple ideas combined)

- Combine **2–3 types**: e.g. discriminant + factoring + inequality.
    
- Students must **recognize** which tools are relevant.
    

> “Find all integers (k) such that the equation  
> [  
> x^2 - (k+1)x + k = 0  
> ]  
> has two distinct positive integer roots.”

Now you need:  
discriminant, sum/product of roots, integer conditions.

### Level 4 – Creative / Non-routine

- Put the core idea inside an unfamiliar context.
    
- Ask for explanation, proof, or classification.
    

> “Let (f(x) = x^2 - (k+1)x + k).  
> Show that there are infinitely many integers (k) such that the graph of (y=f(x)) passes through **two distinct points** with integer coordinates on the line (y=1).”

Now there’s:  
“connect graph ↔ equation, solve, reason about integer solutions ⇒ constrain (k).”

**Takeaway:**  
One powerful way to generate problems is:

1. Fix _one_ central technique.
    
2. Build a **ladder**: direct → parametric → integrated → creative.
    
3. Repeat this for each “type” in the chapter.
    

---

## 3. Lens B: “Solution path graph”

Think of each problem’s solution as a **graph of moves**:

- Nodes = mental actions (e.g., “expand”, “factor”, “use parity”, “consider case (x\ge0)”, etc.)
    
- Edges = logical flow (“after I notice A, I can do B”).
    

You can vary difficulty by modifying this graph:

1. **Length** – more steps = usually harder
    
    - Easy: 2–3 node chain
        
    - Medium: 4–6 steps
        
    - Hard: multiple branches, backtracking
        
2. **Branching** – multiple possible paths vs single obvious one
    
    - Easy: there is one natural, direct move.
        
    - Hard: several “tempting but wrong” moves, only one works.
        
3. **Hidden node** – place a “non-obvious” move in the middle
    
    - E.g., suddenly substituting (y = x-1), or noticing symmetry, or rewriting as a known identity.
        

So to _generate_ problems:

- Start with a **target solution path** you want students to practice.
    
- Then **encode** that path into a problem statement.
    

Example:

You want a path like:

> “Notice symmetry → set (a+b = s), (ab = p) → rewrite expression in (s,p) → solve quadratic in s or p.”

Then you design a problem whose algebraic structure _naturally rewards_ that sequence.  
Changing the sequence (more steps, more hidden moves, more branches) = changing difficulty.

---

## 4. Lens C: “Change the representation”

Same mathematics, different _wrapper_ → big variety.

Represent the same underlying constraint in many forms:

- **Algebraic**: equations/inequalities
    
- **Numeric**: tables, patterns of numbers, sequences
    
- **Geometric**: area/length, diagrams, coordinate plane
    
- **Verbal**: word problems, stories
    
- **Logical**: “Which statements are always true?” multiple-choice
    

To generate variety:

1. Fix a core relation, like (a^2 + b^2 = c^2).
    
2. Wrap it as:
    
    - “Find integer solutions …” (number theory)
        
    - “Right triangle with hypotenuse (c)… find area” (geometry)
        
    - “Data in a table – which triple can be sides of right triangle?” (data interpretation)
        
    - “If we increase one leg by 1, what happens to hypotenuse?” (functional thinking)
        

**Difficulty control:**

- Easy: direct algebraic form.
    
- Medium: translation from story/diagram to algebra.
    
- Hard: two-stage translation (diagram → relationship → parameterized algebra) + tricky numbers.
    

---

## 5. Lens D: “Target common mistakes”

Another Korean-book trick: many problems are built to **check** specific misconceptions.

Steps:

1. List typical errors students make:
    
    - e.g., ( (a+b)^2 = a^2 + b^2)
        
    - forgetting sign when distributing
        
    - thinking “prime means odd”
        
    - misusing absolute value inequalities, etc.
        
2. Build problem families that **punish** the misconception:
    
    - The wrong method gives a **plausible but wrong** answer.
        
    - The right method requires the concept you’re teaching.
        

Example:

> “Solve ( |2x - 3| = x + 1 ).”

- If they drop absolute values blindly: (2x-3=x+1 \Rightarrow x=4).
    
- Correct: case split ⇒ (x=4) and (x=\frac{2}{3}), then check which satisfy (x+1\ge0).
    

To generate difficulty levels:

- **Level 1**: “pure trap” – only one step, designed to flush out the misconception.
    
- **Level 2**: trap embedded in a 2–3 step problem.
    
- **Level 3**: mixed problem set where this trap appears without warning.
    

---

## 6. Lens E: “Parameter, extremes, and generalization”

Once you have a seed problem, you can “open it up”:

1. **Add a parameter**
    
    - Turn constants into letters and ask “for what values of (k)…?”
        
    - Raises difficulty because students must consider _families_ of situations.
        
2. **Ask about extremal / boundary cases**
    
    - max/min values (“What is the largest integer (n) such that…?”)
        
    - equality cases in inequalities (“When does equality hold?”)
        
3. **Generalize pattern**
    
    - Easy: work out 2–3 concrete examples.
        
    - Medium: ask for the pattern in words.
        
    - Hard: prove the pattern for general (n).
        

Example ladder from a basic combinatorics count:

- L1: “How many 3-digit numbers use digits 1–5 without repetition?”
    
- L2: “Same question, but must be divisible by 3.”
    
- L3: “Same question, but with a parameter: digits ({1,2,\dots,k})”
    
- L4: “Find a formula in terms of (k). For which (k) is the count maximal?”
    

---

## 7. Lens F: “Integration across topics”

Korean problem books shine in **mixed practice** sections.  
To generate these:

1. Choose 2–3 **topics** you want to integrate (e.g. linear functions + inequalities + geometry).
    
2. Decide a **story** that naturally uses all of them.
    
3. Make sure the solution _cannot_ be done with just one tool.
    

Example:

> A line passes through two fixed points, is tangent to a parabola, and you’re asked for a condition on parameter (k).  
> You need: slope, equation of line, discriminant, maybe area reasoning.

Difficulty tuning:

- Start with integration of **two closely related** topics.
    
- Step up to three topics, or two that feel distant (e.g., modular arithmetic + combinatorics).
    

---

## 8. A concrete mini-template: building a 5-level ladder from one seed

Let’s take a very simple seed:

> Seed idea: “Sum of divisors function / counting divisors.”

Level 0 (Example/Pattern spotting)

- Give table for small (n): list divisors, count them. Ask: “What do you notice about perfect squares?”
    

Level 1 (Direct exercise)

- “Find the number of divisors of (360).”
    

Level 2 (Parameter + form recognition)

- “A number has prime factorization (2^3\cdot 3^2\cdot 5). How many divisors does it have?”
    
- “Given prime factorization (p_1^{a_1} \cdots p_k^{a_k}), express number of divisors in terms of exponents.”
    

Level 3 (Reverse / characterization)

- “List all numbers (\le 100) with an odd number of divisors.”  
    → Forces realization: only perfect squares.
    

Level 4 (Integrated)

- “How many integers (100 \le n \le 400) have exactly 3 divisors?”  
    → Need to use: divisor-count formula + characterization of numbers with exactly 3 divisors = squares of primes.
    

Level 5 (Creative / proof)

- “Prove that a positive integer has an odd number of positive divisors if and only if it is a perfect square.”
    

You can see how each level is just a _systematic distortion or deepening_ of the previous ones.

---

## 9. A practical workflow for you

If you want a repeatable method (like designing your own 쎈/일품 stack):

1. **Choose a micro-objective**
    
    - e.g. “Students can use the discriminant to reason about roots.”
        
2. **Write a seed problem** (the simplest non-trivial one).
    
3. Generate a **family** by iterating these knobs:
    
    - Representation: symbolic / word / graph / table / geometry
        
    - Variables: constants → parameters → more constraints
        
    - Objective: compute → find all → prove/explain → optimize
        
    - Structure: single-step → multi-step → branching/hidden step
        
    - Integration: add 1 more concept, then 2, etc.
        
    - Misconception: design at least 1–2 “trap but fair” items.
        
4. **Label difficulty levels** based on:
    
    - Number of steps
        
    - Degree of abstraction
        
    - Number of concepts required
        
    - How hidden the main idea is
        
5. **Test-run mentally**
    
    - Try to solve each problem as if you were a student at your target level.
        
    - Adjust numbers / wording until each one feels like a small but real increment.
        

---

