# DatasetX-submission#34-BuildSys26

This anonymized repository contains DatasetX's data and associated code for experiments and figures.

### Dataset content and description
In the `DatasetX_dataset` directory you'll find all data contained in the dataset - we provide two formats: CSV (to make it more easy to surf through) and JSON (that contains that full data tagging). More details about the data tagging structure and further details about how to use it under `DatasetX_dataset/README.md`

### Reproducibility
We provide information below about how to reproduce the results from the paper, for figures, tables, particular numbers inlined in text, and experiments.

#### 1. Reproducing figures
The code and data used for the MobiSys submission can be found under `code_mobisys` and `data_mobisys_visualizations`.

For the data itself, check `DatasetX_dataset` - we also derived CSVs that can be easily surfed at `DatasetX_dataset/Site J`, `DatasetX_dataset/Site M`, `DatasetX_dataset/Site S1`, `DatasetX_dataset/Site S2`, `DatasetX_dataset/Site T`, `DatasetX_dataset/Site V`.

#### 2. Reproducing figures and tables (go to `code_mobisys` for complete instructions)

1. Figure 1a (`code_mobisys/figure_1a_1b.py`) – (a) Diverse measurement patterns among sensors placed inside building; (b) Differences in measurement patterns among sensors placed inside (colored in shades of blue) vs. outside (purple and turquoise lines)
2. Figure 2 (`code_mobisys/figure2.py`) – Data accumulation over time per site
3. Figure 3a (`code_mobisys/figure_3a_3b.py`) - (a) Measurements per sensor type (with MB info); (b) Data acumulation per sensor type
4. Table 3 (`code_mobisys/table3.py`) – Sensor composition
5. Figure 4 (`code_mobisys/figure4.py`) – Site availability
6. Figure 6a (`code_mobisys/figure6a.py`) – Firmware induced CO2 anomalies at Site V
7. Figure 6b (`code_mobisys/figure6b.py`) – Humidity dynamics at Site V without firmware errors
8. Table 5 (`code_mobisys/table5.py`) – Baseline anomaly detection performance
9. Table 6 (`code_mobisys/table6.py`) – Estimated HVAC energy savings at Site T

#### 3. Reproducing particular numbers inlined
1. Claim of no. `ppm` measurements in paper (page no. 7, second paragraph); We ran `grep -ro "ppm" DatasetX | wc -l`;
2. Claim of no. `65535` anomalies in paper (page no. 7, second paragraph); We ran `grep -ro "65535" DatasetX | wc -l`; <br>
For the complete list of all commands we ran for extracting the particular numbers showcased in tables or inlined, please refer to `code_mobisys/COUNTING.md`
