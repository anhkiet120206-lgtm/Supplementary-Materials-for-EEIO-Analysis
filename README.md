# Supplementary-Materials-for-EEIO-Analysis
This folder contains the Python code and data templates to reproduce all results, tables, and figures presented in the paper. The code is released under the MIT License (see LICENSE).
Contents

File Description:

1. eeio_analysis.py (Main script): loads raw IO data, computes baseline matrices, runs all carbon tax scenarios (four recycling mechanisms, four carbon prices) and sensitivity analysis. Outputs results to console and CSV files.

2. F3_OFFICIAL.xlsx (Required input file): The 171‑sector Vietnam Input‑Output table (2019) with emission intensities. The script expects this file in the same folder. If your file has a different name, edit the variable DATA_FILE in the script.

3. requirements.txt: List of Python packages needed (numpy, pandas, openpyxl).

4. LICENSE	MIT License text.

5. README.md

Code Structure
load_io_data() – Reads the Excel file and extracts the 171‑sector matrices (Z, x, y, S, value‑added coefficients, formal labour shares) using the exact column/row labels from the paper’s data source.

compute_baseline() – Calculates A, L, total emissions, and baseline GDP.

run_scenario() – Implements one recycling mechanism given a carbon price and a set of parameters. Returns the DWL‑adjusted GDP change and emission reduction.

main() – Orchestrates the analysis: loads data, runs all scenarios, prints tables, and saves outputs.

All parameters (elasticities, multipliers, formal sector share, deadweight loss) are clearly defined at the top of the script and can be modified by the user.

License
This code is open source under the MIT License. See LICENSE for details. If you use this code in your own research, please cite the original paper.

Contact
For questions or issues, please contact the corresponding author at [anhkiet120206@gmail.com].

Note: The raw input‑output data (F3_OFFICIAL.xlsx) is the property of the General Statistics Office of Vietnam and is not redistributed here. Users must obtain it separately. The provided code assumes the file structure exactly as used in the paper; minor adjustments may be needed if the file format differs. 
