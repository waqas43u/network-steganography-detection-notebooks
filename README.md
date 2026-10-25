# Network steganography detection notebooks

Exploratory Python notebooks for assembling network-traffic features, preparing normal/covert labels, fitting a transformer-based detector, and testing leave-one-technique-out (LOTO) generalization.

## Contents

| Notebook | Purpose |
| --- | --- |
| `Dataset_Network_StegAnalysis.ipynb` | Explores and samples multiple traffic resources. |
| `3 Levels features Normal+ Covert(Preprocessing).ipynb` | Protocol-wise labelling, feature assembly and initial preprocessing. |
| `Final_Preprocessing.ipynb` | Final dataset preparation, split and encoder creation. |
| `Final_Transformer_model.ipynb` | Transformer model training and evaluation. |
| `LOTO_Testing.ipynb` | Leave-one-technique-out testing. |
| `Preprocessing_new_Protocol-wise.ipynb` | Alternative preprocessing draft; not confirmed as the final path. |

These descriptions are conceptual, **not a verified end-to-end execution order**. Several notebooks contain exploratory branches, duplicated operations and machine-specific file paths. `notebook_inventory.csv` records the source and prepared SHA-256 hashes. `input_paths_from_code.csv` lists literal CSV paths found in the code to help locate required inputs.

## Data and execution

**No datasets, trained weights, result tables or saved notebook outputs are included.** The notebooks refer to local/Google Drive CSVs that were not present in the supplied folder. Many paths begin with `/content/` or `/content/drive/MyDrive/`; one uses a Windows desktop path. You must obtain the datasets from their respective owners, verify their terms, and update each notebook's paths before attempting to run it. The dataset inventory and exact preparation history are incomplete, so a fresh run cannot currently be claimed to reproduce a published result.

For a local environment, install the approximate imports with `python -m pip install -r requirements.txt` and open the notebooks in Jupyter. The original versions of these packages were not supplied. Google Colab-specific cells, including `drive.mount`, need a Colab session or manual adaptation. The original notebooks were not refit or tested as an end-to-end pipeline when this repository bundle was prepared.

## Public-sharing notes

Saved outputs and execution counts were removed from these public copies because outputs may embed data previews and local run details. The source notebooks remain untouched in the source folder. No licence is granted by this bundle: obtain the code and data owners' permission before making the repository public or adding an open-source licence. Do not describe this as a fully reproducible benchmark until the input datasets, preprocessing decisions, package versions and model outputs have been independently verified.
