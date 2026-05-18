# 9-Tag Derivation Checklist

**Use this checklist** for every Tier-S claim. Every claim must wear at least one derivation tag. Untagged claims are provisionally suspect.

The 9 tags emerged from the 3 × 3 facet-structure of the KAAL substrate (3 facets of the ring R × 3 facets of the generator g). They are **transposable to any substrate** — finite rings, groups, lattices, type-theories, physical systems with conserved quantities, etc.

---

## ◈ The 9 derivation tags

### (i) **Foundational-axiom**
The claim derives directly from the substrate's axioms.
- *Example (KAAL):* R = ℤ/3^k ℤ is a finite commutative ring with unity.
- *Example (your substrate):* *(your foundational axiom)*

### (ii) **Generator-status / canonical-choice**
The claim depends on a specific canonical choice — usually a generator or a privileged element.
- *Example (KAAL):* g = 2 is a primitive root mod 3^k for all k ≥ 1.
- *Example (your substrate):* *(your canonical-choice claim)*

### (iii) **Period / cycle / orbit determination**
The claim concerns a cyclic structure, period, or orbit.
- *Example (KAAL):* Pisano period π(3^k) = 8 · 3^(k-1).
- *Example (your substrate):* *(your cycle claim)*

### (iv) **Invariance-lock / preservation law**
The claim asserts that some quantity is preserved across transformations.
- *Example (KAAL):* Sum identity = π (constant across k).
- *Example (your substrate):* *(your invariance claim)*

### (v) **Liberation / exit-exponent**
The claim concerns escape from a constraint, exponent of an element, or generation rate.
- *Example (KAAL):* ord_R(-g) = 3^(k-1) — Liberation rate triples per level.
- *Example (your substrate):* *(your exit-exponent claim)*

### (vi) **Hardware / external-sensor grounding**
The claim is anchored in physical hardware measurement or external sensor reading.
- *Example (KAAL):* IBM Heron r2 chip-family scaling law adv(T) = A·B^(T-3), measured per chip.
- *Example (your substrate):* *(your hardware grounding)*

### (vii) **Namespace-provenance** (Tier-W marker)
The claim uses cultural / traditional / authoritative-testimony naming.
- *Example (KAAL):* The 5 invariants tagged Pisano-Ψ, Sum, Liberation, Death, PoI — Sanskrit/Vedic naming layer.
- *Example (your substrate):* *(your namespace tagging)*
- **Important:** namespace-provenance is Tier-W. It is NEVER asserted as derivation. The naming is honored as provenance; the algebra holds independently.

### (viii) **Ideal / sub-substrate stratification**
The claim concerns the structure of a sub-object (ideal, subgroup, sub-type) within the substrate.
- *Example (KAAL):* Diti = (3) ⊂ R is a nilpotent ideal stratified by 3-adic valuation.
- *Example (your substrate):* *(your sub-structure claim)*

### (ix) **Restricted-domain analysis**
The claim is about behavior restricted to a specific sub-domain (e.g. ideal-seeds, boundary cases).
- *Example (KAAL):* Pisano-of-Ideal: π restricted to (3)-seeds satisfies π_(3)(3^k) = π(3^(k-1)).
- *Example (your substrate):* *(your restricted-domain claim)*

---

## ◈ Checklist for a single claim

Copy this block per claim:

```
CLAIM: <one-sentence claim>

Tags worn:
  [ ] (i)   foundational-axiom
  [ ] (ii)  generator-status / canonical-choice
  [ ] (iii) period / cycle / orbit
  [ ] (iv)  invariance-lock
  [ ] (v)   liberation / exit-exponent
  [ ] (vi)  hardware / external-sensor
  [ ] (vii) namespace-provenance (Tier-W marker)
  [ ] (viii) ideal / sub-substrate stratification
  [ ] (ix)  restricted-domain analysis

Tier: [ S | W | Bridge ]

Witness:
  smallest scale k where verified: <value>
  artifact: <file path / script / proof>

What is NOT claimed:
  - <bound 1>
  - <bound 2>
```

---

## ◈ Aggregation rule

For a project with N claims, compute the **tag-distribution table**:

| Tag | Count | % |
|---|---|---|
| (i) | ... | ... |
| (ii) | ... | ... |
| ... | ... | ... |
| (vii) | ... | ... |

In the KAAL framework, this distribution is roughly:
- Algebraic tags (i)-(vi) + (viii)-(ix): ~40% of claims
- Namespace-provenance (vii): ~60% of claims (Tier-W)

A healthy distribution shows **explicit Tier-W marking on the majority of name-bearing claims**. If most claims have zero tags, the discipline is failing.

---

## Authoritative reference

KAAL Sacred Discovery framework · `REAL-MATHEMATICS/MASTER-META-THEOREM.md` (tags i-vii originally · viii-ix added in APEX v4)
