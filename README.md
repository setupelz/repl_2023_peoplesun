# Electricity supply quality and use among rural and peri-urban households and small firms in Nigeria

[![paper](https://img.shields.io/badge/paper-10.1038%2Fs41597--023--02185--0-1f6feb)](https://doi.org/10.1038/s41597-023-02185-0) [![Zenodo](https://zenodo.org/badge/611306776.svg)](https://zenodo.org/badge/latestdoi/611306776) [![licence](https://img.shields.io/badge/licence-MIT-8a8f98)](LICENSE)

- Paper: https://doi.org/10.1038/s41597-023-02185-0
- Archive of record: https://zenodo.org/badge/latestdoi/611306776 (every release is archived on Zenodo)
- Summary page: https://setupelz.com/work/nigeria-survey.html

Replication archive for:

> Pelz, S., Chinichian, N., Neyrand, C. and Blechinger, P. (2023). Electricity
> supply quality and use among rural and peri-urban households and small firms
> in Nigeria. *Scientific Data* 10, 273.
> https://doi.org/10.1038/s41597-023-02185-0

The paper describes the PeopleSuN survey of households and small enterprises
in rural and peri-urban Nigeria (2021). This archive holds the descriptive
analysis behind the paper's figures and tables, run on the anonymised survey
data.

## What is here

| Path | Content |
| --- | --- |
| `R/paper1.R` | The whole analysis, top to bottom: reads the survey files, builds the descriptive tables and figures of the paper. Packages are loaded with `pacman` at the top. |
| `Data/Survey/` | Anonymised household (`peoplesun_hh_*`) and enterprise (`peoplesun_ent_*`) survey files with their appliance and stove modules, the enumeration-area key (`eaidgeokey_eas_anon.csv`), and the ODK codebooks and choice lists (`*_odk_codebook.xlsx`, `*_odk_choices.xlsx`) that name every variable and answer code. |
| `Analysis.Rproj` | RStudio project; paths in the script resolve with `here()` from this root. |

## Running

Open `Analysis.Rproj` and source `R/paper1.R`. The script installs nothing
itself; `pacman::p_load` fetches the listed packages on first run.

## Data

The survey data are the anonymised public release of the PeopleSuN survey as
documented in the paper (sampling, questionnaire, anonymisation). Reuse under
the paper's terms (CC BY 4.0), citing the paper.

## Licence

MIT for the code in this archive (`LICENSE`).
