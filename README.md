# Multi-Targeted Virtual Screening (VS) Pipeline

This repository contains scripts and workflows for performing **multi-targeted virtual screening (VS) for targets involved in taupathies** using structure-based docking and machine learning-based scoring. The pipeline is designed to identify compounds with strong or selective binding affinities across multiple protein targets, enabling polypharmacology and selectivity analysis in drug discovery.

## Features

- **Rescoring of compounds based on gnina:**  
  Batch docking of compound libraries against multiple protein targets using [Gnina](https://github.com/gnina/gnina) or similar docking tools.

- **Pose Extraction and Scoring:**  
  Extraction of the best-scoring 3D poses per compound for each target, using CNN-based affinity predictions.

- **Multi-Target Analysis:**  
  - Aggregation of docking results across targets.
  - Calculation of mean, best, and selectivity-based scores for each compound.
  - Ranking and filtering compounds for polypharmacology or target selectivity.

- **Data Processing:**  
  Uses [RDKit](https://www.rdkit.org/) and [pandas](https://pandas.pydata.org/) for handling chemical data and tabular results.

### Prerequisites

- Python 3.x
- RDKit
- pandas
- Instadock ( for docking )
- Gnina ( for docking )

### Example Usage

1. **Dock compounds against each target** and generate SDF files.
2. **Run the provided scripts** to extract the best poses and aggregate results.
3. **Analyze and rank compounds** using the generated summary tables.

## File Structure

- `docking/` — Scripts and configs for running docking jobs.
- `processing/` — Scripts for extracting, ranking, and aggregating docking results.
- `data/` — Example input and output files.

## Citation

If you use this pipeline, please cite the appropriate docking software (e.g., Gnina), RDKit, and any relevant publications.

## License

This project is licensed under the MIT License.

---

*For questions or contributions, please open an issue or submit a pull request.*
