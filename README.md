# Options-pricing-models-and-their-accuracy-Finsearch
## The Black-Scholes model for options pricing
The Black-Scholes model is a mathematical construct that tries to establish the price of an option based on several market factors. It is primarily used to price **European style**
options, which are the kind of options you can excercise only on a specific date, which is also the **expiration date** of the option contract. The simple equation that descirbes 
this is the following:

C =  N(d<sub>1</sub>)*S<sub>t</sub> - N(d<sub>1</sub>)K*(e<sup>-rt</sup>)

where 

![d1](https://latex.codecogs.com/png.latex?d_1%20%3D%20%5Cfrac%7B%5Cln%5Cleft(%5Cfrac%7BS_t%7D%7BK%7D%5Cright)%20%2B%20%5Cleft(r%20%2B%20%5Cfrac%7B%5Csigma%5E2%7D%7B2%7D%5Cright)t%7D%7B%5Csigma%20%5Csqrt%7Bt%7D%7D)

![d2](https://latex.codecogs.com/png.latex?d_2%20%3D%20%5Cfrac%7B%5Cln%5Cleft(%5Cfrac%7BS_t%7D%7BK%7D%5Cright)%20%2B%20%5Cleft(r%20-%20%5Cfrac%7B%5Csigma%5E2%7D%7B2%7D%5Cright)t%7D%7B%5Csigma%20%5Csqrt%7Bt%7D%7D)

C = Option price

K = Strike price

t = Time to expiration (years)

r = Risk free interest rate (annual rate as a fraction of 100)

&sigma; = Volatility of the underlying asset (annual rate as a fraction of 100)

**&sigma;** is calculated as: 

**&sigma;** = **&sigma;<sub>m</sub> * &radic;N** 

where 

**&sigma;<sub>m</sub>** = standard deviation of the quantity **ln(P<sub>t</sub>/P<sub>t-1</sub>)** with P<sub>t</sub> being the price of the stock on a date t, taken over **N** days

## Datasets used

**Reliance**
Taking **r = 0.07 (7% annual risk free interest rate)** 

**Reliance Dataset 1** : K constant @ 2400, expiry date as 28 dec 2023, for the year 2023

**Reliance Dataset 2** : K constant @ 2500, expiry date as 28 dec 2023, for the year 2023

**Reliance Dataset 3** : K constant @ 2600, expiry date as 28 dec 2023, for the year 2023

## Results
![Dataset 1 result]()
