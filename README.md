# Cox-Ross-Rubinstein-Model
The Cox-Ross-Rubinstein (CRR) model, also known as the Binomial Model, is a widely used mathematical approach for valuing options, primarily stock options. It was developed by John Cox, Stephen Ross, and Mark Rubinstein in the late 1970s as an alternative to the Black-Scholes model, which was the dominant option pricing model at the time. The CRR model provides a discrete-time framework for option pricing and is especially useful for understanding and valuing options when the underlying asset's price movement is not continuous but rather occurs in discrete steps.

Here's a simplified explanation of the CRR model:

1. **Time Discretization:** The CRR model divides the time to expiration of the option into discrete intervals. Each interval is typically a small fraction of a year.

2. **Price Movement:** Within each time interval, the underlying asset's price can either move up by a certain factor or move down by another factor. These factors are determined by the volatility of the underlying asset and the length of the time interval. The model assumes that the price change ratios remain constant over each interval.

3. **Binomial Tree:** The CRR model represents the potential price movements of the underlying asset as a binomial tree. At each time step, the asset's price can either move up or down, resulting in two possible future prices at the next time step. This tree structure helps visualize the various possible paths the asset's price can take over time.

4. **Risk-Neutral Valuation:** The model assumes a risk-neutral valuation approach, which means that the expected return on the underlying asset is equal to the risk-free rate. This assumption simplifies the option pricing calculation.

5. **Option Valuation:** Starting from the last time step (expiration date) of the option, the option's value is computed by working backward through the tree. At each node in the tree, the option's value is the discounted expected value of the option's payoff in the next time step, considering both the up and down movement possibilities.

6. **Option Payoff:** The option's payoff at expiration depends on whether it is a call or put option. For a call option, the payoff is the difference between the asset's price and the strike price, if the asset price is higher than the strike price; otherwise, the payoff is zero. For a put option, the payoff is the difference between the strike price and the asset's price, if the asset price is lower than the strike price; otherwise, the payoff is zero.

By iterating backward through the binomial tree, the model calculates the option's value at the present time. The final computed value represents the fair market price of the option given the assumptions and parameters of the model.

While the CRR model has limitations and simplifying assumptions, it provides a useful tool for understanding the basic concepts of option pricing and can be extended to more complex scenarios.
