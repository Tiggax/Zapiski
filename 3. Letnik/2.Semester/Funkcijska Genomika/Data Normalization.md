- Star is aligner
- Salmon is a mapper

Dplyrer

3 samples in each group -> control


## Fold change

it's calculated as a ratio between avrgae value in gene exspression and 2

it is commanly used as $\log_2(FC)$ where it becomes:
- 100/200 $\to$ 0.5 $\to$ (-1)
- 200/100 $\to$ 2 $\to$ (1)

if we preform 20_000 tests
what is the problem?
if we allow each test to have 1% false positive, then 200 genes could be false positives.
**FDR**(false discorvery rate) $\to$ method to control the number of false positives

