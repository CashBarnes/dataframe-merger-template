# DataFrame Merger Template

## Overview
This project is designed to merge data from multiple Excel files into a single DataFrame and save the results. It processes each file in the input directory, matches data targets with their data sources within the same file, merges derived and non-derived fields based on specified columns, and appends all output CSV files into one final CSV file with a single set of headers.

## Features
- Load data from Excel files.
- Match data targets with their data sources within the same file.
- Filter derived and non-derived fields based on a new indicator.
- Merge DataFrames on specified columns.
- Save merged DataFrames to CSV and Excel files.
- Append all output CSV files into one final CSV file with a single set of headers.

## Requirements
- Python 3.x
- pandas
- openpyxl

## Installation
1. Clone the repository:
    ```sh
    git clone https://github.com/CashBarnes/DataFrame-Merger-Template.git
    ```
2. Navigate to the project directory:
    ```sh
    cd DataFrame-Merger-Template
    ```
3. Install the required packages:
    ```sh
    pip install -r requirements.txt
    ```

## Usage
1. Place your Excel files in the `data` directory.
2. Update the column names and IDs in `main.py`:
    - `data_source_col`: Column name in the source DataFrame.
    - `data_target_col`: Column name in the target DataFrame.
    - `data_source_id`: ID column in the source DataFrame.
    - `data_target_id`: ID column in the target DataFrame.
    - `desired_columns`: List of columns in the desired order.
3. Run the `main.py` script:
    ```sh
    python main.py
    ```
4. The merged output files will be saved in the `output` directory.

## Project Structure
- `data/`: Directory containing input Excel files.
- `output/`: Directory where output files will be saved.
- `main.py`: Main script to process and merge data.
- `requirements.txt`: List of required Python packages.
- `README.md`: Project documentation.

## License
This project is licensed under the MIT License.