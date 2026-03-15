# RainGaugeNet-Sub6G-CSI-dataset

An open dataset of CSI-based rainfall attenuation at 2.8 GHz. It includes both LOS and NLOS measurements, labeled weather conditions, and supports the RainGaugeNet model, which achieves over 90% classification accuracy using only 20 seconds of CSI data.

## Future Releases

We will release our measured data and code in several stages.

## Data Description

We conducted three experiments, corresponding to `data1`, `data2`, and `data3`.  
Each experiment contains multiple data sets. We use `data1/i_data.mat` to represent the `i`-th data collected from `data1`. The corresponding data for each experiment is shown below.

---

| Dataset      | Mode   | No Rain Group IDs | Moderate Rain Group IDs | Heavy Rain Group IDs |
|--------------|--------|-------------------|-------------------------|----------------------|
| **data1**    | **LoS-O** | Group 10           | Group 3, 4, 8, 9           | Group 5, 6, 7        |
|              | **LoS-I** | -                 | -                       | -                    |
|              | **Ref-O** | -                 | -                       | -                    |
| **data2**    | **LoS-O** | Group 12           | Group 3                   | Group 2              |
|              | **LoS-I** | Group 9            | Group 11                  | Group 10             |
|              | **Ref-O** | Group 4            | Group 6                   | Group 5              |
| **data3**    | **LoS-O** | Group 7            | Group 9                   | Group 8              |
|              | **LoS-I** | Group 1            | Group 3                   | Group 2              |
|              | **Ref-O** | Group 4            | Group 6                   | Group 5              |

---

## Mode Explanations

- **LoS-O**: Through rain to receiver outside rain  
  **Explanation**: The signal passes through the rain region and then propagates in a rain-free area, with the receiver located outside the rain.  
  **Details**: While the receiver is not directly affected by the rain, the signal still experiences attenuation due to the rain region.

- **LoS-I**: Through rain to receiver in rain  
  **Explanation**: The signal passes through the rain region and reaches a receiver located within the rain.  
  **Details**: The signal is directly affected by the rain in the reception area, resulting in significant signal attenuation.

- **Ref-O**: Reflection through rain to receiver outside rain  
  **Explanation**: The signal passes through the rain region, then reflects and propagates in a rain-free area, reaching the receiver located outside the rain.  
  **Details**: Even though the receiver is outside the rain, the reflected signal still suffers from attenuation caused by the rain region.

Dataset

Due to the large size of the dataset, the full dataset is not hosted on GitHub.

The publicly available data can be accessed :
  https://1drv.ms/f/c/6b440dd6275abb84/IgD39yeeb6bFQahyFdhRbhxVASlQ8F4oNZxvsTzwQBTJpeQ?e=tSVhab
