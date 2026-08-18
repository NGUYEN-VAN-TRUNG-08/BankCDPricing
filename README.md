## 1. Research Question

Can bank CDs trading at YTMs above the issuing bank's comparable rate generate short-term relative-value opportunities?

## 2. Market Mechanism

Users can now sell CDs before maturity to other users instead of selling to the bank and forfeiting interest payments.

CDs are listed on the TransferD mini app within the MBB app. Listings include the asking price, maturity length, and payment at maturity. If another user agrees to the asking price, they pay the amount and receive the CD. A listing can expire before anyone buys it.

## 3. Pricing Model

Because CDs only pay the total principal and interest at maturity, they can be priced similarly to zero-coupon bonds.

Payment = Principal × (1 + Annualized Rate)^(Duration in days / 365)

From the listing, we know the asking price and the final payment. We can calculate the YTM for this CD.

Asking Price = Payment / ((1 + YTM)^(Days to Maturity / 365))

The value of YTM satisfies the equation above.

The bank is selling new CDs at interest rate i for the same duration. If i is smaller than YTM, we can expect YTM to converge to i, which would increase the price. We price the CD using the equation:

Resell Price = Payment / ((1 + i + Liquidity Spread)^(Days to Maturity / 365))

*Liquidity Spread affects liquidity; the higher the spread, the easier it is to sell the CD.*

Annualized Return = (Resell Price / Asking Price)^(365 / (Days to Maturity - Holding Period)) - 1

## 4. Trading Rule

Entry Spread = YTM - i

Select CDs with the highest entry spread, where the spread is greater than or equal to 1%.

Choose the Liquidity Spread so that the annualized return equals the desired ROI, then calculate the Resell Price. For the trades made, the annualized return was greater than or equal to 20%. We initially set the spread high and lowered it if we felt the price was too high.

## 5. Data

Data are collected from actual listings and realized trades (currency in VND).

## 6. Results

- Number of trades:
- Average holding period:
- Maximum holding period:
- Average ROI per trade:
- Maximum ROI per trade:
- Total annualized return:

## 7. Risks and Limitations

- The sample size is small and requires more time to collect data.
- Liquidity risk: there is no guarantee of a buyer, so we may have to hold CDs longer. Although we can simply hold the CD to maturity and suffer no nominal loss, we still suffer an opportunity cost.
- Potential low capacity: the market for a specific bank's CDs can be very small. Even if this strategy proves profitable, we cannot scale up.
- Changes in trading rules and regulations: in the future, the bank may choose to charge fees, and trading profits may be taxed.

## 8. Future Work

- Continue to collect data and expand the sample size.
- Perform spread/return regressions, liquidity analysis, and sensitivity tests.
