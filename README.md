# NBEATS*: Enhanced N-BEATS for Mid-Term Electricity Demand Forecasting

 We presents an enhanced N-BEATS model, N-BEATS*, for improved
 mid-term electricity load forecasting (MTLF). Building on the strengths of
 the original N-BEATS architecture, which excels in handling complex time
 series data without requiring preprocessing or domain-specific knowledge,
 N-BEATS* introduces two key modifications. A novel loss function
combining pinball loss based on MAPE with normalized MSE, the new loss
 function allows for a more balanced approach by capturing both L1 and L2
 loss terms. A modified block architecture– the internal structure of the
 N-BEATS blocks is adjusted by introducing a destandardization component
 to harmonize the processing of different time series, leading to more efficient
 and less complex forecasting tasks. Evaluated on real-world monthly electric
ity consumption data from 35 European countries, N-BEATS* demonstrates
 superior performance compared to its predecessor and other established fore
casting methods, including statistical, machine learning, and hybrid models.
 N-BEATS* achieves the lowest MAPE and RMSE, while also exhibiting the
 lowest dispersion in forecast errors.

 This repository provides an implementation of the NBEATS* algorithm introduced in [https://arxiv.org/pdf/2412.02722].


| Model | MAPE/MedAPE/IQRAPE | SMAPE/MedSAPE/IQRSAPE | RMSE | MAE | MPE |
|---------------|-------------------|------------------------|------|-----|-----|
| ARIMA | 5.65/3.32/5.24 | 5.19/3.27/5.17 | 463±875 | 409±890 | -2.35±13.62 |
| ETS | 5.05/3.50/4.80 | 4.93/3.53/4.80 | 375±605 | 325±626 | -1.04±7.97 |
| k-NNw+ETS | 4.47/2.71/3.52 | 4.27/2.72/3.53 | 328±535 | 270±560 | -1.25±9.00 |
| FNM+ETS | 4.40/2.64/3.46 | 4.20/2.67/3.41 | 322±522 | 268±545 | -1.26±8.80 |
| N-WE+ETS | 4.37/2.68/3.36 | 4.17/2.68/3.31 | 321±523 | 266±546 | -1.26±8.68 |
| GRNN+ETS | 4.38/2.64/3.51 | 4.19/2.66/3.48 | 325±524 | 268±548 | -1.26±8.61 |
| MLP | 5.27/2.97/3.84 | 4.98/2.99/3.75 | 379±668 | 307±695 | -1.37±13.49 |
| ANFIS | 6.18/3.56/4.87 | 5.81/3.58/4.72 | 489±765 | 384±813 | -2.51±12.63 |
| LSTM | 6.11/3.73/4.50 | 5.73/3.75/4.43 | 432±645 | 341±688 | -3.12±11.79 |
| ETS+RD-LSTM | 4.48/2.74/3.55 | 4.23/2.71/3.54 | 347±624 | 287±646 | -1.11±10.07 |
| TFT | 5.34/3.21/4.14 | 4.96/3.19/4.06 | 388±663 | 324±702 | -3.09±10.72 |
| iTransformer | 5.17/3.09/4.09 | 4.85/3.08/4.02 | 416±735 | 335±769 | -2.32±10.07 |
| TCN | 5.61/4.06/4.22 | 5.39/4.02/4.11 | 467±728 | 382±788 | -2.61±8.57 |
| BiTCN | 4.54/2.88/3.59 | 4.29/2.86/3.54 | 334±578 | 283±597 | -2.35±8.92 |
| RMoK | 4.95/2.96/3.70 | 4.58/2.94/3.62 | 371±626 | 301±655 | -2.81±10.89 |
| N-HiTS | 4.63/2.97/3.72 | 4.42/2.95/3.66 | 355±581 | 298±605 | -2.27±8.40 |
| N-BEATS | 3.78/2.55/**3.30** | 3.74/2.55/**3.27** | 310±506 | 256±528 | **-0.34±6.43** |
| **N-BEATS*** | **3.44**/**2.20**/3.41 | **3.52**/**2.20**/3.38 | **304±544** | **255±561** | 0.57±5.43 |
 

## Citation

If you use this code in any context, please cite the following paper:

```
@misc{kasprzyk2024enhancednbeatsmidtermelectricity,
      title={Enhanced N-BEATS for Mid-Term Electricity Demand Forecasting}, 
      author={Mateusz Kasprzyk and Paweł Pełka and Boris N. Oreshkin and Grzegorz Dudek},
      year={2024},
      eprint={2412.02722},
      archivePrefix={arXiv},
      primaryClass={cs.LG},
      url={https://arxiv.org/abs/2412.02722}, 
}
```
