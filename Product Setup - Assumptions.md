+++
title = "Product Setup - Assumptions"
+++

For each of the assumptions, enter the following inputs:
- Mult (Multiple)
- Table
- Table Type
- Table Column (applicable to Discount Rate only)
- PAD (applicable to Valuation and Capital Requirement Loops only)

## Mortality
The following `Table Type` are available:
- Attained Age
    - Applied to all model points regardless of sex or smoker status of each model point
- Attained Age Sex Distinct
    - Applied in accordance to the sex field of each model point
- Attained Age Sex Smoker Distinct
    - Applied in accordance to the sex and smoker fields of each model point
- Select and Ultimate
    - Applied to all model points regardless of sex or smoker status of each model point
- Select and Ultimate - Sex Distinct
    - Applied in accordance to the sex field of each model point
- Select and Ultimate - Sex Smoker Distinct
    - Applied in accordance to the sex and smoker fields of each model point
- Select and Ultimate - Sex Distinct - SOA Table ID
    - Applied in accordance to the sex field of each model point
    - This is read from MortalityTables.jl package from JuliaActuary.org
- Select and Ultimate - Sex Smoker Distinct - SOA Table ID
    - Applied in accordance to the sex and smoker fields of each model point
    - This is read from MortalityTables.jl package from JuliaActuary.org

## Lapse
The following `Table Type` are available:
- Rate by Policy Year and Policy Term
- Rate by Policy Year and Policy Term and Premium Term
    - This is a multi-index table

## Expense
The following `Table Type` are available:
- Per Policy and Perc of Premium by Policy Year

## Discount Rate
The following `Table Type` are available:
- Projection Year
- Calendar Year
- Mix of Projection Year and Calendar Year

## Investment Return
The following `Table Type` are available:
- Projection Year
- Calendar Year
- Mix of Projection Year and Calendar Year

## Premium Tax
The following `Table Type` are available:
- Scalar
- Projection Year

## Tax
The following `Table Type` are available:
- Scalar
- Projection Year

