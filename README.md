1. RESEARCH QUESTION
Can bank CDs trading at YTMs above the issuing bank's comparable rate generate short-term relative-value opportunities?
2. MARKET MECHANISM
Users can now sell CDs before maturity to other users instead of selling to the bank and forfeiting interest payment.
CDs are listed on TransferD miniapp in the MBB app. Listings include: asking price, maturity-length, and payment at maturity. If another user agree to the asking price, he pays the amount and receive the CD. A listing can expire before anyone buys it.
3. PRICING MODEL
Because CDs only pay the total principal and interest at maturity, it can be priced similarly to zero-coupon bonds.
Payment = Principal * (1 + Annualized Rate) ^ (Duration in day / 365)
From the listing we know the asking price and final payment. We can calculate YTM for this CD.
Asking Price = Payment / ( (1 + YTM) ^ (Days to Maturity / 365) )
The value of YTM satisfies the equation above.
The bank is selling new CDs at interest rate "i" for the same duration. If "i" is smaller then YTM, we can expect YTM to converge to "i", thus increasing the price. We price the CD using the equation:
Resell Price = Payment / ( (1 + i + Liquidity Spread) ^ (Days to Maturity / 365) )
*Liquidity Spread affects liquidity, the higher the spread the easier we can sell it.
Annualized return = (Resell Price / Asking Price) ^ (365 / (Days to Maturity - Holding period)) - 1
4. TRADING RULE
Entry Spread = YTM - i
Select CDs with highest entry spread and spread larger or equal to 1%.
Choose Liquidity Spread so that Annualized Return equals the desired ROI, then calculate Resell Price. For the trades made, Annualized Return was larger or equal to 20%. We first set spread high and lowered it if we felt the price was too high.
5. DATA
Data is collected from actual listings and realized trades (currency in VND)
6. RESULTS
Number of trades:
Average Holding period:
Maximum Holding period:
Average ROI per trade:
Maximum ROI per trade:
Total Annualized Return:
7. RISKS AND LIMITATIONS
Sample size is small, requires more time to collect data.
Liquidity risk: there is no guarantee of buyer so we may have to hold CDs for longer. Although we can simply hold the CD to maturity and suffer no nominal losses, we still suffer opportunity cost.
Potential low capacity: the market for a specific bank's CDs can be very small. Even if this strategy proves profitable, we cannot scale up.
Changes in Trading rules and Regulations: in the future, the bank may choose to charge fees and trading profit can be taxed.
8. FUTURE WORKS
Continue to collect data, expand sample size.
Perform spread/return regressions, liquidity analysis, sensitivity tests.
