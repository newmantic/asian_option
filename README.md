# asian_option


An Asian Option is a type of exotic option where the payoff depends on the average price of the underlying asset over a certain period, rather than just the price at expiration. This feature makes Asian options less sensitive to extreme price movements and can provide a more stable hedging or investment tool.

There are two primary types of Asian options:
1) Average Price Option
2) Average Strike Option

Underlying Asset (S): The asset on which the option is based (e.g., a stock, index).
Strike Price (K): The price at which the option can be exercised, relevant for the Average Price Option.
Average Price (A): The arithmetic or geometric average of the underlying asset's price over a specified period.
Maturity (T): The time until the option expires.

Call Option: Gives the holder the right to buy the underlying asset.
Put Option: Gives the holder the right to sell the underlying asset.


1) Average Price Option
The payoff is based on the difference between the average price of the underlying asset over a specific period and the strike price.

Call Option Payoff:
Payoff = max(A - K, 0)
Where:
A is the average price of the underlying asset.
K is the strike price.

Put Option Payoff:
Payoff = max(K - A, 0)
This type of option reduces the impact of volatility because the average price is generally less extreme than any single point price.


2) Average Strike Option
The strike price is set to the average price of the underlying asset over the life of the option. The payoff is then determined by the difference between the final price of the asset and this average strike price.

Call Option Payoff:
Payoff = max(S_T - A, 0)
Where:
S_T is the price of the underlying asset at maturity.
A is the average price of the underlying asset.

Put Option Payoff:
Payoff = max(A - S_T, 0)
This option type is useful for investors who want protection against a sharp increase or decrease in the asset's price just before maturity.


The average price A can be calculated in different ways, but it is commonly the arithmetic mean of the underlying asset's prices at different observation points.

Arithmetic Average:
A = (1/n) * sum_{i=1}^{n} S_i
Where:
n is the number of observation points.
S_i is the price of the underlying asset at observation point i.
