# Biodiversa+ pilot: Monitoring invasive alien species (IAS) with image-based methods

## Rationale

This repository contains the functionality to standardize the data of the [biodiversa+ IAS pilot](https://www.biodiversa.eu/2024/02/02/pilot-on-invasive-alien-species-monitoring-first-year-report/) to a [Darwin Core Archive](https://www.gbif.org/darwin-core) that can be harvested by [GBIF](https://www.gbif.org/).

## Workflow

[source data](data/raw) → Darwin Core [mapping script](src/dwc_mapping.Rmd) → generated [Darwin Core files](data/processed)

## Repo structure

The repository structure is based on [Cookiecutter Data Science](http://drivendata.github.io/cookiecutter-data-science/) and the [Checklist recipe](https://github.com/trias-project/checklist-recipe). Files and directories indicated with `GENERATED` should not be edited manually.

```
├── README.md              : Description of this repository
├── LICENSE                : Repository license
├── ias-pilot.Rproj        : RStudio project file
├── .gitignore             : Files and directories to be ignored by git
│
├── src
│   ├── dwc_mapping.Rmd    : Darwin Core mapping script
│   ├── _site.yml          : Settings to build website in docs/
│   └── index.Rmd          : Template for website homepage
│
├── docs                   : Repository website GENERATED
│
└── data
    ├── raw                : Source data, input for mapping script
    └── processed          : Darwin Core output of mapping script GENERATED
```

## Contributors

[List of contributors](https://github.com/inbo/ias-pilot/contributors)

## License

[MIT License](LICENSE) for the code and documentation in this repository. The included data is released under another license.
