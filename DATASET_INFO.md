# Bank Marketing Dataset

## Overview

Portuguese bank marketing campaign data for predicting term deposit subscriptions.

## Dataset Size

- **Train**: 2,999 customers × 21 features
- **Test**: 1,120 customers × 20 features (no target)

## Target Variable

- `y`: Did the client subscribe? (yes/no)
- **Highly imbalanced**: 89% no, 11% yes

## Features

### Customer Info

- `age`: Customer age
- `job`: Job type (admin, technician, services, etc.)
- `marital`: Marital status
- `education`: Education level

### Financial

- `default`: Has credit in default?
- `housing`: Has housing loan?
- `loan`: Has personal loan?

### Campaign

- `contact`: Contact method (cellular/telephone)
- `month`: Last contact month
- `day_of_week`: Last contact day
- `duration`: Call duration in seconds
- `campaign`: Number of contacts this campaign
- `pdays`: Days since last contact (999 = never contacted)
- `previous`: Number of contacts before this campaign
- `poutcome`: Previous campaign outcome

### Economic Indicators

- `emp.var.rate`: Employment variation rate
- `cons.price.idx`: Consumer price index
- `cons.conf.idx`: Consumer confidence index
- `euribor3m`: Euribor 3 month rate
- `nr.employed`: Number of employees

## Key Findings

- **Previous success** = 65% subscription rate (strongest predictor)
- **Cellular** works 2.5x better than telephone
- **Best months**: March (52%), December (50%), September (38%)
- **Age 65+**: 47% subscription rate
- **Duration**: Strong predictor but can't use (data leakage)

## Data Quality

- No missing values
- Some features have "unknown" values (~20% in default)
- Delimiter: semicolon (`;`)
