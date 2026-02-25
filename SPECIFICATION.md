# NAO Assertion Monitor 2.1a-beta Specification

## Score Formula

Score = (S_add - S_damp'') / N

### Additive Term (S_add)
- strong × 2.0
- normal × 1.5
- exclude × 2.0
- hidden × 1.0

### Damping Term (S_damp)
S_damp = (disprove + damp) × 2.0  
Cap at 4.0

### Conclusion Protection
If final sentence contains strong or exclude term:
S_damp'' = S_damp × 0.5

### Sentence Count (N)
- Split by 。！？?
- Bullet lines count as 1 sentence
- Minimum N = 1

---

## Thresholds

Strict High ≥ 1.8  
Broad High ≥ 1.2  

---

## Notes

- Rule-based prototype
- Japanese language oriented
- Not intended for automated blocking
