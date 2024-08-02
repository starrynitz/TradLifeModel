+++
title = "Projecton Flow"
+++

The model projects a best estimate cashflow projections including policy liabilities and capital requirement. The projections have been segregated and grouped under various functions which allows the policy liabilities and capital requirement projections to reuse some of these functions.

The flow of the projection is structured as follows:
1. Iterate through selected runs based on run settings
2. Iterate through selected products based on general settings
3. For each product:
   - Read all model points into DataFrame
   - Load product feature set
   - Load assumption sets for base projection and reserving and capital requirement inner projections
4. For each model point:
   - Load the model point
   - Project policy information tables
   - Project assumptions tables based on base projection assumption set
   - Project Per Policy Table with product feature set
   - Project Per Policy Table with assumption tables
   - Project survivalship
   - Project in force cash flow before reserve and capital requirement
   - Project present value of in force cash flow before reserve and capital requirement
   - Project reserve per policy based on reserving assumption set
   - Project capital requirement per policy based on capital requirement assumption set
   - Project in force cash flow and present value for and after increase in reserve and capital requirement