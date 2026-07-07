# Mdm2InPred

A QSAR (Quantitative Structure-Activity Relationship) model that predicts the bioactivity of query compounds against MDM2.

## Description

Mdm2InPred is a machine learning-based QSAR model designed to predict the bioactivity of chemical compounds targeting MDM2 (Mouse Double Minute 2 homolog), a protein commonly studied in cancer research for its role in inhibiting the p53 tumor suppressor. Given a query compound, the model predicts its likely bioactivity, helping researchers prioritize candidates for further experimental validation without needing to run costly wet-lab assays upfront.

## Features

- Predicts bioactivity of a query compound against MDM2
- Built on QSAR modeling principles
- Useful for early-stage drug discovery and virtual screening
- Fast, computational alternative to initial experimental screening

## Installation

```bash
git clone https://github.com/username/Mdm2InPred.git
cd Mdm2InPred
pip install -r requirements.txt
```

## Usage

```bash
python predict.py --input compound.smi
```

Example:
```bash
python predict.py --smiles "CC(=O)Oc1ccccc1C(=O)O"
```

*(Update the commands above to match your actual script names and input formats.)*

## Input Format

Describe what input the model expects, for example:
- SMILES string of the query compound
- A `.csv` file with a column of SMILES strings
- Molecular descriptors (if precomputed)

## Output

Describe what the model returns, for example:
- Predicted bioactivity class (active/inactive)
- Predicted activity value (e.g., pIC50)
- Confidence score

## Model Details

- **Model type:** QSAR (e.g., Random Forest / SVM / XGBoost — specify which)
- **Target:** MDM2
- **Descriptors used:** (e.g., molecular fingerprints, physicochemical descriptors)
- **Training data:** (source of bioactivity data, e.g., ChEMBL)

## Requirements

List key dependencies, for example:
```
rdkit
scikit-learn
pandas
numpy
```

## Contributing

Contributions are welcome. Feel free to open an issue or submit a pull request.

## License

Distributed under the BSD 3-Clause. See `LICENSE` for details.
