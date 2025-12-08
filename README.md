# Multi-Targeted Virtual Screening (VS) Pipeline

This repository contains ML scripts and workflows for performing **multi-targeted virtual screening (VS) for targets involved in taupathies** which involves ensembl model building and machine learning-based scoring. The pipeline is designed to identify compounds with strong or selective binding affinities across multiple protein targets involved in taupathies, enabling polypharmacology and selectivity analysis in drug discovery.

- **Data Processing:**  
  Uses [RDKit](https://www.rdkit.org/) and [pandas](https://pandas.pydata.org/) for handling chemical data and tabular results.

### Prerequisites

- Python 3.x
- RDKit
- pandas
- Instadock ( for docking )
- gnina ( for docking and rescoring )


## Citation

If you use this pipeline, please cite the appropriate docking software (e.g., Gnina), RDKit, and any relevant publications.

## License

This project is licensed under the MIT License.

---

*For questions or contributions, please open an issue or submit a pull request.*
