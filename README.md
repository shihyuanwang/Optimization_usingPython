# Optimization using Python with Pyomo package or Google’s OR-Tools

**(1) Markdown Pricing Linear Optimization with Pyomo package**

Solve a linear pricing optimization model for 200 products in a given week to determine a pricing plan, and get:
- The optimized pricing plan (weeks at each price)
- Revenue projection
- The current price according to the optimized pricing plan

https://github.com/shihyuanwang/Optimization_usingPython/blob/main/1_Markdown%20Pricing%20Linear%20Optimization.ipynb

\
**(2) Minimum Cost Network Optimization with Google’s OR-Tools** (https://developers.google.com/optimization/flow/assignment_min_cost_flow)
 
Solve the assignment problem using a minimum cost network flow solver.

https://github.com/shihyuanwang/Optimization_usingPython/blob/main/2_Minimum%20Cost%20Network%20Optimization.ipynb

\
**(3) Mixed Integer Linear Optimization - DC Location and Transportation Model with Pyomo package**

Consider data from a manufacturer who distributes nationwide. They are now deciding where to locate their distribution centers (DCs). There are 23 potential DC locations and 76 cities they need to serve. Each potential DC location has a fixed annual operating cost if they locate a distribution center there. The data also includes the per unit distribution cost from each potential DC location to each region, the capacity of each potential DC location, and the required shipping demand in each region. We need to determine how many and which DC locations to use – and how DCs satisfy the retail city demand needs - in order to minimize the total fixed operating expenses plus distribution costs. Formulate and solve the model as a mixed integer linear program and use Pyomo package to solve it.

https://github.com/shihyuanwang/Optimization_usingPython/blob/main/3_DC%20Location%20and%20Transportation_Mixed%20Integer%20Optimization.ipynb

\
**(4a) Vehicle Routing Problem with Google’s OR-Tools** (https://developers.google.com/optimization/routing/vrp)

Solve the vehicle routing problem for the dataset on branch locations in Canada for a medium sized business. The travel time matrix is provided in the file "P5_VRPtraveltimes.xlsx." Please assume:
- 6 vehicles
- The vehicles start and end their route at location "T5B 0S1"

https://github.com/shihyuanwang/Optimization_usingPython/blob/main/4a_Vehicle%20Routing%20Problem%20.ipynb

\
**(4b) Job Shop Problem with Google’s OR-Tools** (https://developers.google.com/optimization/scheduling/job_shop)

Solve the job shop problem for the data provided in "P5_JobShopData.xlsx."

https://github.com/shihyuanwang/Optimization_usingPython/blob/main/4b_Job%20Shop%20Problem.ipynb

\
**(5) Personalized Assortment Optimization at Birchbox**

The subscription box retail business model has been one of the fastest growing parts of e-commerce in the past decade. This problem is inspired by the beauty subscription box
company Birchbox (see https://www.birchbox.com/). Subscribers pay a fixed fee to receive a monthly package of 5 samples of beauty products. They then have the option to purchase the items they like most. At the heart of Birchbox’s business model is their personalized assortment algorithm – how do we decide which five samples to send to each customer every month?

The file "Birchboxdata2020.xlsx" contains 2 sheets. The “item info” sheet contains information about the samples Birchbox has in stock:
- Item – an index number for the SKU
- Category – an integer denoting the type of sample (lotion, cleanser,…etc)
- Inventory – the number of sample units available to ship this month
- Sample cost – the cost to send the sample
- Margin if purchase – the profit if a customer decides to purchase the sample product.
- PurchaseProb_X – the output of the proprietary prediction model that predicts the probability of purchase for a customer in segment X.

The “cust info” sheet contains information about the customer subscriber base:
- Cust – an index number for the customer
- Seg – the segment number to be used to determine the purchase probability
- Item X – a binary indicator for each item, where a 1 indicates that the customer has already received that sample in the past.

\
**Part 1.** The Base Integer Program Formulation

Solve the problem in Python as an integer program according to the following guidelines:
- Assume the objective is to maximize the total expected margin minus the cost of the samples for the next round of boxes.
- 5 items need to be sent to each customer.
- You can’t run out of inventory.
- You can’t send a customer a sample they’ve already received.

\
**Part 2.** Next Month’s Revenue with Zero Replenishment

- Imagine that Birchbox failed to source any new samples next month – so they must make new assortments but also cannot send customers what they just sent them this month. 
Solve next month’s problem in this scenario. How much profit should they expect?

https://github.com/shihyuanwang/Optimization_usingPython/blob/main/5_Personalized%20Assortment%20Optimization.ipynb

