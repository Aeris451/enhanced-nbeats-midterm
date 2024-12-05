# NBEATS*


## Electricity Price Forecasting Results

| Model         | MedAPE | MAPE | IQrAPE | RMSE  | MPE   |
|---------------|--------|------|--------|-------|-------|
| ARIMA         | 3.32   | 5.65 | 5.24   | 463   | -2.35 |
| ETS           | 3.50   | 5.05 | 4.80   | 374   | -1.04 |
| k-NNw+ETS     | 2.71   | 4.47 | 3.52   | 327   | -1.25 |
| FNM+ETS       | 2.64   | 4.40 | 3.46   | 321   | -1.26 |
| N-WE+ETS      | 2.68   | 4.37 | 3.36   | 320   | -1.26 |
| GRNN+ETS      | 2.64   | 4.38 | 3.51   | 324   | -1.26 |
| MLP           | 2.97   | 5.27 | 3.84   | 378   | -1.37 |
| ANFIS         | 3.56   | 6.18 | 4.87   | 488   | -2.51 |
| LSTM          | 3.73   | 6.11 | 4.50   | 431   | -3.12 |
| ETS+RD-LSTM   | 2.74   | 4.48 | 3.55   | 347   | -1.11 |
| N-BEATS       | 2.55   | 3.78 | 3.30   | 309   | 0.34  |
| **N-BEATS***  | 2.20   | 3.44 | 3.29   | 304   | 0.56  |
 

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
