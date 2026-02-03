# WeightProject

This repository contains code and reference material for imputing missing emission data for Norwegian passenger cars. The work supports analysis of vehicle scrappage patterns and fleet-level emissions using data from the Norwegian motor vehicle registry.

Notebooks
 ## matching_with_OFV.ipynb

Imputes missing CO₂ emissions using data from OFV.
Used to complete vehicle-level CO₂ values where registry data is incomplete.

 ## matching_with_copert.ipynb

Imputes missing NOₓ emissions using COPERT emission factors.
The notebook matches vehicle characteristics to COPERT factors to estimate emissions.

Reference Documents
 ## 1.A.3.b.i-iv Road transport 2025.pdf

Official COPERT documentation describing methodologies and emission factors used for road transport.

 ## 1_A_3_b_i_iv_Road_Transport_Appendix_4_Emission_Factors_Oct_2025.xlsx

Appendix containing detailed COPERT emission factors used in the NOₓ imputation process.

Notes and Limitations

COPERT emission factors are used primarily for NOₓ imputation.

The same framework can be extended to PM emissions, but this requires an additional classification of driving mode (urban, rural, motorway), which is not currently implemented.

 ## fuel_consumption_estimation.ipynb
This script imputes missing fuel consumption values for Norwegian passenger
cars using technical and regulatory information from the REGTEK vehicle
registry. The imputed fuel consumption values are intended for downstream
use in emissions modeling (e.g. CO₂).
