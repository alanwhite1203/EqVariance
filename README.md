# Variance Swap and Swaption Pricing

A variance swap is an instrument which allows investors to trade future realized (historical) volatility against current implied volatility. The Variance Swap pays the difference between observed variance and a strike variance, possibly subject to a cap and a floor. The observed variance is computed from the stock price returns over a series of specified sampling dates.

The market value of a variance swap is based on the variance determined from a combination of realized (historical) volatility and unrealized volatility. The unrealized volatility forecast is obtained by integrating the replicated portfolio of vanilla European options with infinite number of strikes. 

A Variance Swap contract has a payoff which is dependent on realized variance. In order to calculate the fair value of future delivery variance, the variance swap can be replicated by a forward contract and a portfolio of appropriately weighted European call and put options with a continuous range of strikes. This continuous spectrum of options is not observable and
hence a (finite) discrete approximate replication must be performed in practice. 

It should be aware that the replication portfolio is derived under assumptions of existence of a perfect replication portfolio comprised of an infinite number of vanilla call/put options. In reality, the replication portfolio will only have finite number of call & put options within a certain strike range.

Usually, the model assumes continuous underlying evolution, while in reality the underlying (stock prices or index) can jump. The replication portfolio then may no longer capture the realized volatility and this may lead to the replication error. As such, it may distort the accuracy of the hedging/risk measurement.

A variance swaption is an OTC option that grants its owner the right but not the bligation to enter an underlying variance swap.

1.	Payoff of Variance Swap
Payoff (equity amount) =  
Where VA ~ variance amount/(K*2)

RV ~ realized volatility =  ; It is the annualized 
          standard deviation of the stock’s returns 
N ~ number of business days
  ~ spot price
K ~ annualized volatility strike

Fair strike: when skew is linear
	 


2.	Valuation
The value of a variance swap is given by

 


References:

https://finpricing.com/lib/EqVariance.html

https://fliphtml5.com/download/download-pdf-file.php?str=x0DZh9GTud3bENXamMjM5kzN3MTPkl0av9mY


