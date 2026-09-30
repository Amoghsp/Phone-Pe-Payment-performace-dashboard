# Phone-Pe-Payment-performace-dashboard
📊 Power BI dashboard analysing 300K PhonePe transactions (₹3.3B+ processed). Loans, Insurance, Money Transfer & recharge and bills. Tracks revenue by service, monthly trends, success rate (96%) and failure root causes.
**The report answers three business questions:**
Which service drives the most transaction value?
How does payment volume change month to month?
Why do payments fail, and how often?

**Problem Statement**

Failed payments mean lost revenue and unhappy users. A business team needs one place to see how much money each service processes, how it changes over the year, and why payments fail, so they can act on it.

**Project Highlights**

5-page interactive report with a date-range slicer and page navigation on every page.
Same layout on every service page, so services are easy to compare.
Covers 4 services and 16 sub-categories (for example Gold loan, Term Life, UPI ID, Electricity Bill).
Goes beyond charts: each finding comes with a recommended action.

**Dashboard Pages**

**Home:** overall KPIs, amount by service, monthly trend and failed payment reasons.

**Insurance:** payment status, failure reasons, users per month, and Bike, Car, Term Life and Health split.

**Loans:** payment status, failure reasons, monthly trend, and Gold, Auto, Mutual Funds and Credit Score split.

**Money Transfer:** payment status, failure reasons, and amount by UPI ID, Self Account, QR Code and Mobile Number.

**Recharge & Bills:** payment status, failure reasons, and Electricity, DTH, Mobile and Cable TV split.

**Key Numbers**
Successful amount: 3,333M
Total transactions: 300K (288K successful, 12K failed, about 96% success).
Loans 2,532.51M, Insurance 512.92M, Money Transfer 378.19M, Recharge & Bills 50.69M.

**Key Insights**
Loans make up about 73% of the total value processed.
Monthly amounts stay between 279M (February) and 304M (July), with July as the peak.
Failure rate is about 4% in every service, so the causes are platform-wide.
Around 60% of failures are user-side (wrong PIN, insufficient funds, wrong info). Server error is the biggest single cause.

**Business Recommendations**
Add automatic retries and better monitoring to cut server-error failures.
Show PIN-retry hints and low-balance warnings to reduce user-side failures.
Prioritise reliability of loan payment flows, since they carry most of the value.

**Skills Demonstrated**
Dashboard design and data storytelling.
KPI selection and trend analysis.
Failure root-cause analysis.
Power BI: cards, bar, pie, donut and line charts, slicers, page navigation.
Data quality checking (for example, spotting a "Successful" category inside the failure-reason chart on the Money Transfer page)

**Future Improvements**
Year-over-year comparison and forecasting.
Average ticket size KPI.
Slicers for city, device or bank.
