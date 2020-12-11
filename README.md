# Currency Implied Volatility

Overview

	An implied volatility is the volatility implied by the market price of an option based on the Black-Scholes option pricing model. A volatility surface is derived from quoted volatilities that provides a way to interpolate an implied volatility at any strike and maturity.
	Unlike in other markets that quote volatility versus strike directly, the FX smile is given implicitly as a set of restrictions implied by market instruments and as such a calibration procedure to construct a volatility- delta or volatility-strike smile is used.

Summary
	Implied Volatility Introduction
	Volatility Surface in FX Market
	Risk Reversal and Butterfly
	FX Volatility Surface Data
•	FX Volatility

Implied Volatility Introduction
	An implied volatility is the volatility implied by the market price of an option based on the Black-Scholes option pricing model. 
	An FX volatility surface is a three-dimensional plot of the implied volatility as a function of term and Delta and smile. 
	The term structures of implied volatilities provide indications of the market’s near- and long-term uncertainty about future short- and long-term swap rates.
	Vol skew or smile pattern is directly related to the conditional non-nomality of the underlying return risk-neutral distribution. 
	In particular, a smile reflects fat tails in the return distribution whereas a skew indicates return distribution asymmetry.
	A crucial property of the implied volatility surface is the absence of arbitrage.

Volatility Surface in FX Market
	Unlike in other markets that quote volatility versus strike directly, the FX smile is given implicitly as a set of restrictions implied by market instruments and as such a calibration procedure to construct a volatility- delta or volatility-strike smile is used
	The volatility surface in FX market is constructed based on the sticky delta rule. The underlying assumption is that options are valued depending on their delta, so that when the FX spot rate moves and the delta of an option changes accordingly, a different implied volatility has to be used into the pricing formula.
	Therefore, FX volatility smile is represented by three entities: at-the-money (ATM) volatility, risk reversal, and butterfly. The standard market quotes are ATM level, 10 delta risk reversal, 10 delta butterfly, 25 delta risk reversal, and 25 delta butterfly.
	The ATM volatilities quoted by brokers can have various interpretations depending on currency pairs. Here we introduced the most popular one used by the FX brokers. The ATM volatility is the value from the smile curve where the strike is such that the delta of the call equals, in absolute value, that of the put (this strike is called ATM “straddle” or ATM “delta neutral”).

Risk Reversal
	A risk reversal (RR) is a combination of a long call option and a short put option with the same maturity. This is a zero-cost product as one can finance a call option by selling a put option. Risk reversal volatility is the difference between the volatility of the call option and the put option at the same moneyness level, i.e.,
	
25 𝑅𝑅=25 𝐷𝑒𝑙𝑡𝑎 𝐶𝑎𝑙 𝑉𝑜𝑙 −25 𝐷𝑒𝑙𝑡𝑎 𝑃𝑢𝑡 𝑉𝑜𝑙

Butterfly
	A butterfly (BF) is a combination of a long call option, a long put option, a short ATM call option, and a short ATM put option. Butterfly volatility is the average of the difference between the volatility of the call option and put option minus the ATM volatility, i.e.,
	
25 𝐵𝐹= 25 𝐷𝑒𝑙𝑡𝑎 𝐶𝑎𝑙 𝑉𝑜𝑙+25 𝐷𝑒𝑙𝑡𝑎 𝑃𝑢𝑡 𝑉𝑜𝑙﷮2﷯−𝐴𝑇𝑀

FX Volatility Data
	FX volatility is quoted 10 and 25 delta call and put, such as

•	FX Volatility

	The original volatility cannot be used for valuation directly. The processed ready-to-use FX implied volatility surface looks like



You can find more details at
https://finpricing.com/lib/FxVolIntroduction.html

