# Data Analyst Assignment

Thank you for taking the time to complete the Opply Data Analyst Assignment. You find the instructions for the task below.

## Motivation

We aim to increase our request to order conversion. In order to do that, we want to develop deeper insights into how we can encourage suppliers to offer quotes that are more likely to convert to orders, considering various factors such as buyer request target and unit prices or whether a Supplier offers free samples (that the buyer can request when they review the quote)
The flow is as follows:

1. A Buyer submits a request for a specific product (<https://www.loom.com/share/15893d46ed9e47308b9e6642980db316>)
2. One or more Suppliers submit quotes for this request (<https://www.loom.com/share/93c8b94efca54b789bfa89885f10ebdf>)
3. If the Buyer is happy they can order the quote

## Assignment

You will analyze past request and quote data (incl whether quotes were ordered) and derive insights about what increases the likelihood of a quote converting to an order and how we can use this data for when Suppliers quote.
The data including an explanation about the most relevant fields is listed below:

- Request Data: <https://docs.google.com/spreadsheets/d/1moA36oyLG7mKP_6_H_47VJV-OKcZwV05eoR7p1cLLLg/edit#gid=0>
  - Request UUID: Unique ID of the request
  - Current Unit Price: Unit price the Buyer claims to be paying for the ingredient right now
  - Target Unit Price: The price the Buyer hopes to get
  - Supply Priority: Whether the Buyer cares most about Price or Quality or none of the two in particular
- Quote Data: <https://docs.google.com/spreadsheets/d/1gT4gniN3hhLE1Bh6hRHIbVIouE3N7aDaMP8Wr8W2SG4/edit#gid=0>
  - Request UUID: ID of the request the quote belongs to (a request can have multiple quotes)
  - Quote Unit Price: Unit price quoted by the Supplier
  - Status: Whether the quote has been `Ordered`, the Buyer has `Declined` it, the quote is still `Available` or it has `Expired` in the meantime
  - Decline Reason: Reason provided by the Buyer when a quote was declined
  - Samples Available: Whether the Supplier provides free samples - the buyer can then request those when reviewing the quote
  - Documents Provided: Whether the Supplier has attached specification sheets to the quote
We recommend downloading the google sheets as a csv file and import them after.

## Key Objectives

- Data Cleaning: Clean the data set as you consider it appropriate
- Data Analysis: Examine the data to determine factors which increase chances that a quote is accepted by buyers. Your analysis could include:
  - Identifying trends or patterns in accepted and declined quotes. Note that declining quotes is optional.
  - Assessing the impact of factors such as Supplier quoted unit prices vs request current and target unit prices on the likelihood of acceptance.
  - Investigating the role of samples in increasing the likelihood of orders.
  - ...
- Insight Generation: Provide insights on how we can influence Suppliers during quote creation to increase the probability of acceptance. As a use case think about tooltips that we display along the quote creation process. For example we may display: "Why not add a specification sheet? Quotes with specification sheets attached have a 20% higher chance of being ordered"
  
Please consider that some requests have unrealistic target and unit prices (0.01), so they should be handled accordingly.

## Deliverables

A single Github repository shared with `martinOpply` and `clemsage` that includes:

- Your code
- A brief report detailing your findings and insights, data visualisations are optional
- Recommendations for guiding Suppliers during quote creation to increase chances of quotes being ordered

We expect that the assignment takes around 2-3 hours. Do as much as you can within this timeframe and provide a description of what else you'd like to do but were unable to due to limited time.
