# Basic Math Concepts

Basic Math Fundations for a Quant

- [Basic Math Concepts](#basic-math-concepts)
  - [Calculus](#calculus)
  - [Algebra](#algebra)
    - [Linear Algebra](#linear-algebra)
  - [Stochastic Calculus](#stochastic-calculus)
    - [Measure-based Probability](#measure-based-probability)
    - [Stochastic Process](#stochastic-process)
    - [Stochastic Integration](#stochastic-integration)

## Calculus

1. $$(lnx^{lnx})'$$
   1. use the log trick and chain rule
2. Integrate
   1. ln\(x\)
   2. sec\(x\) 
      1. method1 : multiplies $$\frac{secx+tanx}{secx+tanx}$$
      2. method2: sec\(x\) = 1/cosx = cosx/cos^2 x = cosx / \(1- sin^2x \)
   3. E\(X\|X&gt;0\) for normal random variable
   4. - total area under curve for normal p.d.f- - 
      1. Calculate $$\int_{-\infty}^{\infty} e^{-x^2/2} \int_{-\infty}^{\infty} e^{-y^2/2}$$ and use polar \(rcos, rsin\) axis \(Fubini's Rule\)
3. Calculate volume/distance/mass/probability using integration
   1. snow begins 12pm, snow plow can clear constant volume per minute, 1pm moved 2miles, 2pm, 3 miles, when did the snow fall?
4. Proof
   1. Mean-Value Theorem
   2. Newton's Method
5. Concepts
   1. Remann vs Lebesgue
6. Tricks
   1. x^x^... = 2, x = ? if = 4, x = ?

## Algebra

-  100th digit of \(1+sqrt\(2\)\)^3000
  -  use Binomial Theorem

### [Linear Algebra](https://xinheliu.github.io/MachineLearning/math/linear-algebra.html)

## Stochastic Calculus

### [Measure-based Probability](https://xinheliu.github.io/MachineLearning/math/math.html#probability)

### Stochastic Process

Brownian motion(Wiener process)

- zero mean
- normal i.i.d. increments with variance dt
- continuous
- Markov

Martingale

- Stopping Times
  - [Doob’s optional sampling theorem](https://en.wikipedia.org/wiki/Optional_stopping_theorem?wprov=sfti1)
-  reflection principle
-  Important Martingales
   -  B\(t\)-t, exponential martingale

### Stochastic Integration

Variation

- First Variation
- Quadratic Variation

Different Integrations

- Reimann Integration
- Lebsgue Integral
- Ito Integral

[Ito's Lemma](https://en.wikipedia.org/wiki/It%C3%B4's_lemma?wprov=sfti1)