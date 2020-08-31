# Benchmark Probabilistic Programs
| Program id| Loop Invariant | Type of Invariant| 
| ----------| -----------    | ----------       |
| pp0       | (z >= 0) * z + (z >= 0 and flip == 0) * ((1 - p)/p)| Linear |
| pp1       |  rounds + [b > 0] * ((1 - p)/ p)      | Linear |
|pp2 (first loop)| x + [flip==0] * (p/(1-p))     |Linear |
|pp3(outer loop) | x + [flip==0]*(p/(1-p))       |Linear|
|pp4   | [x − 1 >= 0 and x − y + 1 <= 0] * (z + x * y − x^2) |Non-linear |
|pp5   | [x >= 0 and z − 1 <= 0 and z >= 0 and y >= 0] * (x + 3 * z * y) |Linear |
|pp6 | [z >= 0 and z − 1 <= 0 and x >= 0 and y >= 0] * 10 * (5 * p * z − 2 * p * z * z + x + p * n * x) |Non- Linear |
|pp7 | [y >= 0 and n − 1 >= 0] * (x + p * n * y) | Non-linear |
|pp8 |  [y >= 0 and n − 1 >= 0] * (x + (0.5) * p * n * n + 0.5 * p * n − 3 * p * n * y) | Non-linear |
|pp9 | [n − 1 >= 0] * (x + (1/4) * n * n + (1/4) * n) | Non-linear |
|pp10| -(1/4) * n + x * y + (1/2) * x * n + (1/2) * y * n + (1/4) * n^2 | Non-linear|
|pp11 | [x == 0 and y − 1 == 0] − [x − 1 == 0 and y==0] | Linear |
|pp12 | [x = 0] * 0.7 + [x = 1] | Linear |
|pp13 | [h >= 0 and t >= 0 and count >= 0] * (1) | Linear|
|pp14 | [x >= 0] * (c + 2x) |Linear |
|pp15 | y - x | Linear
|pp16| 1 + \sum_{l=0}^{w} ([x>l] * (3 + 2 * \sum_{k=0}^{w} ((#col+l)/N)^k) - (2 * [cp[i] == 0] * [x>0] * \sum_{k=0} ^{w} (#col/N)^k)| Non-linear
|pp17 |[x >= 0 and x − 1 <= 0 and (b − 1 == 0 or x == 0 or x − 1 == 0)] * (x) | Linear|
| pp18 |[x ≥ 0 and x − n ≤ 0 and n − M ≤ 0] * (x/M - p*n/M + p) | Linear |
|pp19 | [t == A and c == 0] + [t == A and C == 1] * (p1 / (p1 + p2 - p1 * p2))+  [t == B and c == 1] * ((1 - p2) / (p1 + p2 - p1 * p2))|Linear |
|pp20 | [n <= 10] + [n > 10] * (n * (7/8) * m)| Linear| 
|pp21 | [x - 1 >= 0] + [x-1 < 0] * z | Linear |
|pp22 | [x - 1 >= 0] * x + 1 | Linear |
|pp23 |[c != 1] * [x even] + [c = 1] * ((2/3) + ( 4 * [x odd]) / 15 + [x even] / 15) | Linear |

