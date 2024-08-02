+++
title = "Runs"
+++

### To run the projections:

1. Clone or download this repository to your local machine.
2. Navigate to the directory where the program is located.
3. Open a command prompt.
4. After the formula variables have been validated successfully, run the script `TradLifeModel.jl` using the following command:
   
   ```

   julia src/TradLifeModel.jl

   ```

### To validate User Defined Formula (UDF):
   Run the validation script `ValidateUDF.jl` using the following command to validate that User Defined Table contains all the variables used in User Defined Formula for each product and their product features.
   
   ```

   julia src/ValidateUDF.jl
   
   ```
   
   This step can be skipped if there's no User Defined Tables that are being used or if they have been validated previously and no changes have been made since then.