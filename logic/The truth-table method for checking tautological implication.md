
---

Nice, you’ve basically pasted the _entire_ bit we care about 🙂 So let me connect **your example** directly to **Enderton’s Section 1.2** and show exactly what the method is and how it applies.

---

## 1. What Enderton calls this

In your pasted text, the relevant bits are:

- The **definition of tautological implication**:
    
    > “$\Sigma$ tautologically implies $\tau$ (written $\Sigma \models \tau$) iff every truth assignment … that satisfies every member of $\Sigma$ also satisfies $\tau$.”
    
- The subsection titled **“Truth Tables”**, which begins:
    
    > “There is a systematic procedure … for checking, given wffs $\sigma_1,\dots,\sigma_k$ and $\tau$, whether or not ${\sigma_1,\dots,\sigma_k} \models \tau$.”
    

So the method you’re asking about is exactly:

> **The truth-table method for checking tautological implication**  
> (or “truth-table method” for short).

---

## 2. How the method works in Enderton’s terms

Given formulas $\sigma_1,\dots,\sigma_k$ (premises) and $\tau$ (conclusion):

1. Let $\mathcal{S}$ be the set of all sentence symbols occurring in $\sigma_1,\dots,\sigma_k,\tau$.
    
2. Consider **all truth assignments** $v : \mathcal{S} \to {T,F}$.
    
3. For each such $v$, compute the extended $\bar v$ on all formulas (using the 0–5 clauses for $\neg,\wedge,\vee,\to,\leftrightarrow$).
    
4. **Keep only those rows** (truth assignments) where every premise $\sigma_i$ is satisfied (i.e. $\bar v(\sigma_i)=T$ for all $i$).
    
5. Check whether in every such row we also have $\bar v(\tau)=T$.
    
    - If yes, then ${\sigma_1,\dots,\sigma_k} \models \tau$.
        
    - If not, any row where all premises are true and $\tau$ is false is a **counterexample**.
        

That’s exactly what he does in the example with  
$(\neg(A\wedge B)) \models ((\neg A)\vee(\neg B))$.

---

## 3. Applying it to _your_ example

You gave:

**Premises:**

1. $$  
    \sigma_1 =  
    \bigl[(p \rightarrow q) \land (\lnot q \lor p)\bigr] \rightarrow  
    \bigl[(p \land \lnot q) \lor (\lnot p \land q)\bigr]  
    $$
    
2. $\sigma_2 = p$
    

**Conclusion:**  
$\tau = \lnot q$

We want to check, in Enderton’s sense, whether  
$$  
{\sigma_1, \sigma_2} \models \lnot q.  
$$

---

### Step 1: List sentence symbols

Only two: $p, q$.  
So there are $2^2 = 4$ truth assignments.

---

### Step 2: Build the truth table

Let’s compute the values of $\sigma_1$, $\sigma_2$, and $\lnot q$ for each assignment of $(p,q)$.

I’ll write T/F for truth/falsity.

|$p$|$q$|$(p\to q)$|$(\lnot q \lor p)$|antecedent $(p\to q)\land(\lnot q\lor p)$|consequent $(p\land\lnot q)\lor(\lnot p\land q)$|$\sigma_1$|$\sigma_2=p$|$\lnot q$|
|---|---|---|---|---|---|---|---|---|
|T|T|T|T|T|F|**F**|T|F|
|T|F|F|T|F|T|**T**|T|T|
|F|T|T|F|F|T|**T**|F|F|
|F|F|T|T|T|F|**F**|F|T|

Explanation of key columns:

- $(p\to q)$ is false only when $p=T, q=F$; otherwise T.
    
- $(\lnot q \lor p)$ is T if either $q$ is false or $p$ is true (or both).
    
- Antecedent of $\sigma_1$ is their conjunction.
    
- Consequent of $\sigma_1$ is “exclusive or”: $p$ and not $q$, or not $p$ and $q$.
    
- $\sigma_1$ itself is the conditional “antecedent → consequent”.
    

A simplified table:

|$p$|$q$|$\sigma_1$|$\sigma_2=p$|$\lnot q$|
|---|---|---|---|---|
|T|T|F|T|F|
|T|F|T|T|T|
|F|T|T|F|F|
|F|F|F|F|T|

---

### Step 3: Restrict to rows where all premises are true

Premises: $\sigma_1$ and $p$.

We need:

- $\sigma_1 = T$
    
- $p = T$
    

Checking rows:

- (T, T): $\sigma_1 = F$ → reject.
    
- **(T, F): $\sigma_1 = T$, $p=T$** → keep.
    
- (F, T): $p=F$ → reject.
    
- (F, F): both false → reject.
    

So there is **exactly one truth assignment** satisfying _both_ premises:  
$$  
p = T,\quad q = F.  
$$

---

### Step 4: Check the conclusion on those rows

On that one row:

- $q = F$, so $\lnot q = T$.
    

Thus every truth assignment that satisfies both premises also satisfies $\lnot q$.

Hence:  
$$  
{\sigma_1, p} \models \lnot q.  
$$

---

So in words:

> Under the truth-table method of Section 1.2 (“Truth Assignments” / “Truth Tables”), the premises force $q$ to be false; hence the argument with conclusion $\lnot q$ is **tautologically valid**.

---

So: the name in Enderton is **tautological implication** tested via the **truth-table method** (subsection _Truth Tables_ in Section 1.2). What you’re doing with your example is exactly “check whether ${\sigma_1, p} \models \lnot q$ via a truth table,” in his sense.

---

If you want, I can convert more text or even write a regex script to batch-convert `\(` `\[` delimiters to `$` math for Obsidian.