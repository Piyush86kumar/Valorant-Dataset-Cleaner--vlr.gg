# Valorant Dataset Cleaner

## Objective

This project is designed to clean and process Valorant esports data scraped from vlr.gg. It provides tools to extract data from zip files, clean the data, and format it for further analysis.

## Dataset

The raw data for this project is expected to be in the form of zip files located in the `Zip_files` directory. Each zip file should contain a set of CSV files with Valorant match data. The cleaned data will be output to the `Output` directory.

## Project Structure

```
.
├── Valorant_dataset_cleaner Advanced.ipynb
├── Valorant_dataset_cleaner.ipynb
├── README.md
├── requirements.txt
├── .git/
├── Dataset_upload/
├── Kaggle Guide/
│   ├── Multiple event/
│   └── Single event/
├── Output/
├── vlr_cleaner/
└── Zip_files/
```

## Local Setup

To run this project locally, you will need to set up a Python virtual environment and install the necessary dependencies.

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/Piyush86kumar/Valorant-Dataset-Cleaner--vlr.gg.git
    ```

2.  **Create a virtual environment:**
    ```bash
    python -m venv venv
    # or you can use conda to create venv in the specified directory
    conda create -p venv python=3.12
    ```

3.  **Activate the virtual environment:**
    -   On Windows:
        ```bash
        .\venv\Scripts\activate
        ```
    -   On macOS and Linux:
        ```bash
        source venv/bin/activate
        ```

4.  **Install dependencies:**
    Once the virtual environment is activated, install the required libraries from the `requirements.txt` file:
    ```bash
    pip install -r requirements.txt
    ```

## How to Run

After setting up the local environment, you can run the project using the provided Jupyter notebooks.

1.  **Place the dataset zip files** in the `Zip_files` directory.

2.  **Open and run the Jupyter notebook:**
    -   For processing multiple datasets with an interactive interface, use `Valorant_dataset_cleaner Advanced.ipynb`.
    -   For a simpler, single-dataset cleaning process, use `Valorant_dataset_cleaner.ipynb`.

3.  **Follow the notebook instructions:**
    -   If using the "Advanced" notebook, you will be presented with interactive widgets to select the zip files you wish to process.
    -   The notebook will then extract the data, clean it, and save the processed CSV files to the `Output` directory, organized in folders corresponding to the original zip files.

## Kaggle Guide

The `Kaggle Guide` directory contains resources to help you upload the cleaned dataset to Kaggle.

-   **`Kaggle Guide/`**: This directory contains templates for `dataset-metadata.json` and `columns_description.csv` which are required for Kaggle dataset uploads. It has subdirectories for "Single event" and "Multiple event" uploads.
-   **`Dataset_upload/`**: Place the cleaned CSV files that you want to upload to Kaggle in this directory.

Please refer to the `Command.txt` files within the `Kaggle Guide` subdirectories for the Kaggle API commands to upload your dataset.

## Scripts and Files

-   **`Valorant_dataset_cleaner Advanced.ipynb`**: A more advanced Jupyter notebook for cleaning multiple Valorant datasets from zip files, with an interactive UI for selecting the files to process.
-   **`requirements.txt`**: A file listing the Python dependencies for this project.
-   **`Zip_files/`**: Directory where the raw dataset zip files should be placed.
-   **`Output/`**: Directory where the cleaned and processed data will be saved.
-   **`Kaggle Guide/`**: Contains templates and instructions for uploading the dataset to Kaggle.
-   **`Dataset_upload/`**: Staging area for files to be uploaded to Kaggle.
-   **`vlr_cleaner/`**: Contains the executable for the data cleaning process.
