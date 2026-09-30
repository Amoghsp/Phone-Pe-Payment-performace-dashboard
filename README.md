# Phone-Pe-Payment-performace-dashboard
📊 Power BI dashboard analysing 300K PhonePe transactions (₹3.3B+ processed). Loans, Insurance, Money Transfer & recharge and bills. Tracks revenue by service, monthly trends, success rate (96%) and failure root causes.
The report answers three business questions:
Which service drives the most transaction value?
How does payment volume change month to month?
Why do payments fail, and how often?

Dashboard structure
The report has 5 pages. A side navigation bar links them, and a date-range slicer filters each page.
Page	What it shows
Home	Headline KPIs, amount by service, monthly trend, failed-payment reasons
Insurance	Total amount, payment status, failure reasons, users per month, Bike/Car/Term Life/Health split
Loans	Loan amount, payment status, failure reasons, monthly trend, Gold/Auto/Mutual Funds/Credit Score split
Money Transfer	Amount, unique users, payment status, transfers by type (UPI ID, Self Account, QR Code, Mobile No.)
Recharge & Bills	Amount, payment status, failure reasons, Electricity/DTH/Mobile/Cable TV split

Key numbers
Metric	Value
Successful amount	3,333M
Total transactions	300K
Successful / failed transactions	288K / 12K (about 96% success)
Total amount by service	Loans 2,532.51M, Insurance 512.92M, Money Transfer 378.19M, Recharge & Bills 50.69M
Insights
Loans carry about 73% of processed value (2,532.51M of about 3,474M), followed by Insurance at about 15%.
Volume is steady through the year. Monthly totals stay between 279M (February) and 304M (July).
July is the peak for total amount, loan amount, insurance users and recharge value. Money Transfer peaks in May.
Failure rate is about 4% in every service (3.84% to 4.25%).
Most failures are user-side. Wrong PIN, insufficient funds and wrong info together account for roughly 60% of failed payments. Server errors are the largest single cause (4.1K).
Recommendations: reduce server-error failures through retries and monitoring, and reduce user-side failures with PIN-retry guidance and low-balance warnings.
---
Tools and techniques
Power BI Desktop for data modelling and report design
Visuals: KPI cards, bar, pie/donut, line and area charts
Interactivity: date-range slicer, page navigation buttons, custom icons
Metrics: sum of amount, count of transactions, count of users, payment-status split, failure-reason breakdown
Data notes
The dataset appears to be simulated. Transactions are split almost evenly across sub-categories (about 12.5K each), and the amounts are very close to each other.
On the Money Transfer page, the "Failed Payment Reason" chart includes a "Successful" category. This looks like a data-quality issue in the reason column that should be cleaned in Power Query.
Currency is not shown on the dashboard.
