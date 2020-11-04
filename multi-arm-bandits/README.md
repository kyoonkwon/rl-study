# Multi-arm bandits

## Implementations

[[2.3-4 ϵ-greedy]](./e-greedy.ipynb)
 - incremental implementation of simple 10-armed bandits algorithm using ϵ-greedy
 
[[2.5 exponential recency-weighted average]](./exponential-recency-weighted-average.ipynb)
- shows that exponential recency-weighted average(ERWA) method better result on nonstationary problem.

[[2.6-7 optimistic initial value & UCB]](./optimistic-initial-value-and-UCB.ipynb)
- shows effect of using optimistic initial value

[[2.8 gradient bandit algorithm]](./gradient-bandit.ipynb)
- performance difference of gradient bandit algorithm according to reward comparative target existence

[[2.9 summary]](./parameter-study.ipynb)
- parameter study including unstationary problem

## Exercise Problems

### Q2.5 
[exponential recency-weighted average](./exponential-recency-weighted-average.ipynb)

### Q2.6
Because optimal value was selected repeatedly for initial part as its Q value reduced least while exploration.

### Q2.7
![img](https://latex.codecogs.com/gif.latex?Q_%7Bn&plus;1%7D%3D%20%5Cfrac%7B%5Calpha%7D%7B1-%281-%5Calpha%29%5En%7D%281-%5Calpha%29%5E%7Bn-1%7DQ_2%20&plus;%20%5Csum_%7Bi%3D2%7D%5En%281-%5Calpha%29%5E%7Bn-1%7DR_i)
- Q2 = R1 (no bias of Q1)
- shape of ERWA

### Q2.8
- ~10 steps: due to Nt(a) = 0, select every action
- 11 step: greedy selection -> expect high reward
- 12~ steps: high rate of exploration -> expect reward decreases.