Veridi Logistics — Last Mile Delivery Audit

A. Executive Summary

An audit of 96,470 delivered orders revealed that 7.6% of packages arrive past Veridi's promised date. The problem is not nationwide — it is heavily concentrated in remote Northeast states (AL, MA, SE), where average delays are nearly 50% worse than the national mean. The business impact is severe: on-time orders score 4.3/5 stars on average, while Super Late orders collapse to 1.7/5. Late deliveries are not just a logistics issue; they are the primary driver of negative reviews. Recommended action: renegotiate carrier SLAs for the Northeast region and adjust estimated delivery dates to stop over-promising.

B. Project Links

- Link to Notebook (Colab): https://colab.research.google.com/drive/1ETye6z2gkmVg6ttNHd1c7niQzRowqbHn?usp=sharing
- Link to Dashboard (Looker Studio): https://colab.research.google.com/drive/1ETye6z2gkmVg6ttNHd1c7niQzRowqbHn?usp=sharing
- Link to Presentation: https://docs.google.com/presentation/d/1S-ZD3n0eakY-wyRkGTOtqwzJb7N6CYxo/edit?usp=sharing&ouid=102944517551681890858&rtpof=true&sd=true

C. Technical Explanation

Data Cleaning: Filtered to orders with status = 'delivered' and dropped rows missing actual delivery dates. De-duplicated reviews per order_id by keeping the most recent. Converted date columns to datetime for accurate delay calculations. Classified each delivery as On Time, Late (1-5 days past promise), or Super Late (>5 days).

Candidate's Choice: Added a "Worst Product Categories for Late Delivery" analysis. This matters because if specific product types (like furniture) are consistently delayed, the business can negotiate carrier contracts for those categories specifically — turning a blanket logistics fix into a targeted, cheaper intervention.

