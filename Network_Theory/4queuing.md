# Queuing and Modelling Delay in the Networks

## Markov Property

[马尔可夫链](https://blog.csdn.net/bitcarmanlee/article/details/82819860)

[马尔可夫状态转移矩阵](https://www.zhihu.com/question/41423304)

## Queuing Models

**M/M/1**: Poisson arrivals, exponential service times.

**M/G/1**: Poisson arrivals, general service times.

**M/D/1**: Poisson arrivals, deterministic service times.

## Poisson process (M/M/1 queues)

$\mu$: the service rate

$\lambda$: the arrival rate

$\rho = \frac{\lambda}{\mu}$

**Little's theorem**: $N = \lambda T$

**The transmitter**: $D_{TP}=$ packet transimission time

- Average number of packets at transmitter $=\lambda D_{TP} = \rho = link\ utilisation$.

**The transimission line**: $D_P =$ propagation delay

- Average number of packets in flight $=\lambda D_P$

**The buffer**: $D_q=$ average queuing delay

- Average number of packets in buffer $N_q = \lambda D_q$

**Transmitter + buffer**

- Average number of packets $=\rho + N_q$

From the equilibrium equations:

$$
\sum_{i=0}^{\infty}P(n) = 1\\
\sum_{i=0}^{\infty}\rho^iP(0) = \frac{P(0)}{1-\rho}=1\\
P(0) = 1 - \rho \\
P(n) = \rho^n(1-\rho)
$$

N: **Average number** of customers in the system
$$
N = \sum_{n=0}^{\infty}nP(n) = \frac{\rho}{1-\rho}\\
N=\frac{\rho}{1-\rho}=\frac{\lambda / \mu}{1-\lambda/\mu}=\frac{\lambda}{\mu-\lambda}
$$

T: **Average amount of time** that a customer spends in the system

$$
T = \frac{N}{\lambda} = \frac{1}{\mu - \lambda}
$$

W: **Average time** spent in queue (queuing delay + the service time)

$$
W = \frac{1}{\mu-\lambda} - \frac{1}{\mu}
$$

$N_Q$: **Average number of customers** in the queue (not in service)

$$
N_Q =\lambda W = \frac{\lambda}{\mu-\lambda} - \frac{\lambda}{\mu} = N - \rho
$$

## M/M/m Queue

### Balance Equations

When $n \leq m (\rho = \lambda/\m\mu)$:

$$
\lambda P(n-1) = n\mu P(n) \\
P(n) = \frac{(m\rho)^n}{n!}P(0)
$$

When $n > m (\rho = \lambda/\m\mu)$:

$$
\lambda P(n-1) = m\mu P(n) \\
P(n) = \frac{(m^m\rho^n)^n}{m!}P(0)
$$

## M/G/1 Queue

### Pollaczek-Khinchin (P-K) Formula

Average waiting time in an M/G/1 queue:

$$
W = \lambda \frac{E[X^2]}{2(1-\frac{\lambda}{\mu})}
$$

- where $\mu = E[X]$
- From Little's formula: $N_Q=\lambda W$
- Then:

$$
T = W + E[X] \\
N = \lambda T = N_Q + \rho
$$

#### Speical cases of M/M/1

- Exponential service with rate $\mu$
- $E[X] = 1/\mu, E[X^2] = \frac{2}{\mu^2}$

$$
W = \frac{\lambda}{\mu^2(1-\frac{\lambda}{\mu})} = \frac{1}{\mu-\lambda}-\frac{1}{\mu}
$$

#### Speical cases of M/D/1

- Deterministic service with rate $\mu$
- $E[X] = 1/\mu, E[X^2] = \frac{1}{\mu^2}$

$$
W = \frac{\lambda}{2\mu^2(1-\frac{\lambda}{\mu})} = \frac{1}{2(\mu-\lambda)}-\frac{1}{\mu}
$$

## Priority Queuing: Highest priority queue

## M/M/k/m