# Probability Questions

## Concepts

- example of dependent variables with zero covariance
  - Z - N(0,1), U +1 with 0.5 prob, -1 with 0.5 prob, X = UZ and Z are dependent

## Card, Coin and Dice

- Coin Toss Game: A \(n+1\) coins, B n coins, probability that A has more heads than B?
  - symmetry
- 1000 coins one unfair, 10 times head toss, prob to get unfair coin
- generate fair prob by unfair coin
- Card Game: A and B pick up a card and compare, what's the probability A wins \(in tie, B wins\)
- probability of in texas-hold'em
  - four of a kind: 0.241%
  - full house: 1.463%
  - two pairs: 4.754%
- [prob 4 people each get an A](https://math.stackexchange.com/questions/2521017/probability-of-deck-of-cards-such-that-each-person-receives-one-ace)
- [number of cards to be turned over before seeing one A](https://math.stackexchange.com/questions/961247/what-is-the-probability-that-the-first-ace-in-a-deck-is-the-30th-card)
- throw srictly increasing dice sequence
- roll dice, 1,2,3 game stops, pay points, expected pay off?

## Counting

- 11 screwy priates to lock a case, only above 5 can open
- probability \(a+10b\)^3 last digit is 1?
  - binomial theorem
- letters in wrong evenlope\(Bernoulli's Letter Problem\)

## Events and Game

- Drunk Passenger: 100 passengers, first 1 drunk. others will randomly pick one is seat is taken, prob your seat is taken
- N points in a circle: put n points in a circle, the probability they all end up in a same semi-circle
  - inclusion/exclusion/mutual exclusive
- probability of triangle: stick to form a triangle
  - **\(\*\) what is the distribution of longest piece?**
    - geometric - rule of Lazy Statistician
- Chess tournament: what's the probability the strongest and second strongest meet in final?
- n people in the room, what's the probability 2 has same birthday? how many people in the room to make the prob of two same birthday &gt; 1/2
- All girl world, conditional boy prob
- Dart game: 3rd dart farther than the first
  - the event nth is the best
- [Monty Hall problem](https://brilliant.org/wiki/monty-hall-problem/)
- candies in a jar: red, blue, green 10,20,30 the probability last is green
- Russian Roulette
  - the prob of first and second win
  - if spin the barrel, first and second win
  - first did not die, should you spin the barrel
  - put in two consecutive positions, first did not die
- meeting prob: arrive in 1h, meet in 5min interval

## Expectation, Variance, Covariance, Order Statistics

Skills

- Use indicator variables
- Begin with simple case

Examples

- sum of n random variables c.d.f **\(\*\)**
  - eg. N i.i.d uniform\(0,1\) random variables sum that &lt;= 1
    - use conditional probability $$P(S_{n+1} \leq 1 = \int_0^1 f(X_{n+1}) P(S_n < 1- X_{n+1}) dX_{n+1}$$ and mathematical induction
- coupon collections of N types\(\*\)
  - expected boxes to be opend
    - process of geometric distributions
  - open n box, expected number of coupon types\(\*\)
    - indicator variable I to indicate type I is there
      - $$E(X) = E(\sum I_i)$$
- joint probability of two random variables
  - eg. two bonds default, range of probability and correlation\(\*\)
    - for correlation use, indicator variable
      - $$P(A \cap B) = E(I_A) + E(I_B) - E(I_A I_B) = E(I_A) + E(I_B) - (E(I_AI_B) - cov(I_AI_B))$$
- [correlation x,y and x,z are 0.8, maximum and minimum correlation between x, z](http://jakewestfall.org/blog/index.php/2013/09/17/geometric-argument-for-constraints-on-corrxz-given-corrxy-and-corryz/)
  - [cosine and correlation](https://www.johndcook.com/blog/2010/06/17/covariance-and-law-of-cosines/)

### Order Statistics

- x, y \(or x_1, ..., xn\)_ follow certain distributions, the p.d.f of max\(xi\), min\(xi\) and their expectation
  - eg. i.i.d case - use c.d.f
- correlation of max and min of x1, x2 follow distribution**\(\*\)**
  - calculate E\(YZ\), E\(Y\), E\(Z\), E\(Y^2\), E\(Z^2\) separately
  - need to find F\(yz\) using graph
- 500 random ants expected fall down time
- expected number of tosses of an unfair coin to get two heads in a row
- roll a dice 3 times, can stop at any point, pay the number on dice, what's the strategy

## Distributions

- calculate the mean and variance of
  - geometric distribution
  - binomial distribution
- explain the intuitions behind
  - normal distribution
  - gamma distribution
  - beta distribution
  - chi-square distribution

## Bayes

- coin-making machine make coins with head prob p, p from uniform\(0,1\), whats the conditional distribution of the probability of head if you toss 1000 times and see 750 heads

## Central Limit Theorem

- stock prices either increase by 0.2% or decrease by 0.1% with equal probability, what is the probability after 100 days it goes up twice
  - use Y as log return

## Moment Generating Functions

- X is Poisson\(lambda\)\(number of events in a interval\) y is binomial\(X,p\) \(given x, p is the probability it will be a certain type\), distribution of y \(also Poisson\)

## Process

- Birthday  line: choose optimal position in line
- Amoeba Die out
  - recurrance
- Gambler's Ruin Problem\*: has n money, lose them all time/probability
- AB fair coin toss, toss HT in sequence wins \(first 1 to be T\)
- Basket ball game, 100 throws, prob proportional to success rate
- Observe car in 20 min interval p, prob for observing car in 5min
- Poisson Process expected waiting time
- connect 100 noodles, the prob to form a circle

---

## Stochastic Process

### Markov Chain

- Chameleon Colors: 12, 15 and 17 Chameleons
- Dice game: A first dice 7-7 wins, B first dice sum of 12 wins. Probability?
- Coin Game: expected tosses to see HHH or THH?
- Color Balls\*: each time take out ball, paint first same as second, expected time to see all balls same color

### Martingale and Random Walk

- drunk man walk on the 100 meter bridge \(at 17 meter position\), expected num of steps to walk down
- Dice game: 1,2,3 payoff, 4,5,6 continue, expected payoff
- ticket line: 5,10 bills, no change to start with, what is the probability no extra money is needed
- coin sequence\*: toss a fail coin, expected number of tosses to get n heads in a row?
