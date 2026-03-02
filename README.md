# Scripts and data associated with the Microbiology Galaxy Lab (MGL) and microGalaxy 2026 paper

[![DOI](https://zenodo.org/badge/754032685.svg)](https://doi.org/10.5281/zenodo.15088382)

This repository includes all data and scripts needed to produce figures and statisctical information presented in the paper.

# Running the MGL locally

```bash
docker run --rm -i -t --privileged -p 8080:80 -v ~/export.microbiology/:/export quay.io/galaxy/docker-galaxy-microbiology-lab
```

Visit the [MGL Docker development repository](https://github.com/usegalaxy-eu/docker-galaxy-microbiology-lab) for more details.

# Requirements

- Install [conda](https://conda.io/miniconda.html)

    ```
    $ make install-conda
    ```

- Create the conda environment

    ```
    $ make create-env
    ```

# Usage

## Retrieve citations

- Launch [Jupyter](https://jupyter.org/) to access the notebooks to generate graphs

    ```
    $ make run-jupyter
    ```

- Go to [http://localhost:8888](http://localhost:8888) (a page should open automatically in your browser)

## Update data

- Launch the dedicated script

    ```
    $ bash bin/get_data.sh
    ```
  
## Rebuild figures

```{r}
bash bin/build_figures.sh
```

# MGL paper's supplementary information (figures, tables, and methods)

This section provides easy access to the MGL paper's figures, extended data, and supplementary materials.

## Figures (in [`docs/figures`](docs/figures) folder)

- [`Graphical abstract`](docs/figures/graphical_abstract.png)
- [`Figure 1`](docs/figures/figure_1.png): Microbiology Galaxy Lab (MGL) interface (A) in comparison with default Galaxy interfaces on the UseGalaxy server (B, C).
- [`Figure 2`](docs/figures/figure_2.png): Citation trends in Galaxy publications and survey results from the microbiology research community (March–September 2023).
- [`Figure 3`](docs/figures/figure_3.png): Growth and usability of microbiology-related tool suites, training materials/tutorials, and workflows within the Galaxy ecosystem that are included in the Microbiology Galaxy Lab (MGL).
- [`Figure 4`](docs/figures/figure_4.png): Overview of microbiological data analysis tasks with corresponding tool suites and potential analyses available on the MGL.
- [`Figure 5`](docs/figures/figure_5.png):  Applications of MGL tools and workflows in health, disease, and ecosystem research.

## Supplementary information (in [`docs/supplementary`](docs/supplementary) folder)

- [`Supplementary Figure 1`](docs/supplementary/supplementary_figure_1.png): Microbial Research Topics in Galaxy Publications.
- [`Supplementary Figure 2`](docs/supplementary/supplementary_figure_2.png): Availability of microbiology-related tool suites within the Galaxy ecosystem.
- [`Supplementary Figure 3`](docs/supplementary/supplementary_figure_3.png): Usage of microbiology-related tool suites across workflows.
- [`Supplementary Figure 4`](docs/supplementary/supplementary_figure_4.png): Usage of microbiology-related tool suites across training materials.
- [`Supplementary Figure 5`](docs/supplementary/supplementary_figure_5.png): Flowchart illustrating the process to select and annotate the microbiology-related publications citing the Galaxy Project's major publication.
- [`Supplementary Table 1`](https://docs.google.com/spreadsheets/d/e/2PACX-1vRLzfV-VrXUya3OTBkHvBKYdj00h_56TTBs2AYZlCs9phKWpMTRVd5r8Rgt3cHZ9x4SeDz_GzRPSfxm/pubhtml): Features and capabilities of 45 existing user-friendly microbiological data analysis platforms (non-exhaustive list).
- [`Supplementary Table 2`](docs/supplementary/supplementary_table_2.tsv): Anonymous results from the microbiology research community survey conducted between March and September 2023.
- [`Supplementary Table 3`](docs/supplementary/supplementary_table_3.tsv): Publications citing the Galaxy Project from Google Scholar.
- [`Supplementary Table 4`](docs/supplementary/supplementary_table_4.tsv): Publications citing the Galaxy Project from Google Scholar classified as microbiology-related citations. 
- [`Supplementary Table 5`](docs/supplementary/supplementary_table_5.tsv): Overview of the 319 microbiology-related tool suites available in the Microbiology Galaxy Lab (MGL).
- [`Supplementary Table 6`](docs/supplementary/supplementary_table_6.tsv): Tool suites corresponding to numbers on Figure 4.
- [`Supplementary Table 7`](docs/supplementary/supplementary_table_7.tsv): Comprehensive list of the 117 microbiology-related workflows available in the Microbiology Galaxy Lab (MGL).
- [`Supplementary Table 8`](docs/supplementary/supplementary_table_8.tsv): Summary of use case submissions collected from survey participants and other highlighted use cases.
- [`Supplementary Table 9`](docs/supplementary/supplementary_table_9.tsv): Comprehensive list of tutorials from the Galaxy Training Network (GTN) dedicated to microbiological data analysis.
- [`Supplementary Table 10`](docs/supplementary/supplementary_table_10.tsv): Overview of microbiology-related training events conducted between 2019 and 2025.
- [`Supplementary Table 11`](docs/supplementary/supplementary_table_11.tsv): Manual binary document-level validation of microbiology-related citation classification.
- [`Supplementary Table 12`](docs/supplementary/supplementary_table_12.tsv): Manual multi-label keyword-level validation of automated microbiology citation classification.
- [`Supplementary Method 1`](docs/supplementary/supplementary_method_1.pdf): List of survey questions shared with the microbiology research community via a Google Form between March and September 2023.
- [`Supplementary Method 2`](docs/supplementary/supplementary_method_2.pdf): microGalaxy Community Roadmap (2026–2030), outlining the strategic priorities, goals, and planned developments for the Microbiology Galaxy Lab (MGL).
- [`Supplementary Method 3`](docs/supplementary/supplementary_method_3.pdf): Template to collect use cases from survey participants who expressed interest in contributing to the planned manuscript.
- [`Supplementary Method 4`](docs/supplementary/supplementary_method_4.pdf): Manual validation framework for automated citation classification.