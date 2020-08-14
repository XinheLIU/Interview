# Derivatives Pricing and Hedging

## Options

Option Pricing

* Put-call Parity \(c - p = S - PV\(K\)\)
* Black-Scholes P.D.E
  * for American options, &lt;= 0
* Black-Scholes formula, Black's formula
  * difference Black's vs. Black Scholes

Option Trading Strategies

* protective put, covered call
* collar \(protective put + covered call\)
* risk reversal \(short p, long c\)
* bull/bear spread with call/put
* calendar spread
* straddle, strangle, butterfly
* condor
* iron-butterfly

Greeks change with

* Time to maturity
* underlying price

## Asset Pricing

* Difference in modeling log return and percentage return, why they are the same, when different
* Explain
  * volatility jump modeling
  * local volatility models
  * stochastic volatility models
  * smile
  * term structure
### Option price

* S, K, T-t, sigma, r, d
  * time to maturity impact of European call depends on the dividends
* Put call parity
  * synthetic forward
* American option
  * never early exercise a call
    * time value of option
      * use put-call parity
      * use replication
      * use Jensen' inequality
* [Black-Scholes formula](https://en.wikipedia.org/wiki/Black–Scholes_model)
  * assumptions
  * [Black's \(76\) formula](https://en.wikipedia.org/wiki/Black_model)
* Black-Scholes P.D.E
* Greeks
  * definition, intuition, formula
  * greeks vs spot, maturity, and strike
    * when European options have positive theta
      * deep in the money put, near maturity
  * Gamma sculpting
* Volatility surface
  * call is a convex option regarding to vol 
    * stochastic vol will increase call value
  * [local volatility models](https://en.wikipedia.org/wiki/Local_volatility)
    * Dupire-Derman-Khani
    * what is risk-neutral distribution of stock price at time T
* exotic options
  * binary option
    * price
    * delta hedge 
    * replicate \(bull spread\)
  * exchange option \(currency options\)
    * change of numerie
* option trading strategies
  * bull spread, straddle, strangle

### Fixed-Income

* Duration and Convexity
* interest rate swap
  * floater, inverse floater
* Interest rate models
  * forward rate model
    * Heath-Jarrow-Merton model
  * short-rate models
    * equilibrium models
      * Vasicek, Cox-Ingersoll-Ross model
    * no-arbitrage short-rate models
      * Hoo-Lee model
      * Hull-White model
* Bond portfolio

### Others

* Futures and forward
  * future price vs forward price
    * futures is a martingale \(stochastic interest rate and funding/reinvesting risk\)
* Risk management
  * value at risk
    * [coherent risk measures](https://en.wikipedia.org/wiki/Coherent_risk_measure)