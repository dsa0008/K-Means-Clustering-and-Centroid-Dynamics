# Adult Dataset Fetching Example

## Description

This project demonstrates how to fetch and load the Adult dataset (also known as the "Census Income" dataset) using the `fetch_openml` function from the `scikit-learn` library. The dataset is commonly used for binary classification tasks and contains demographic information to predict whether a person earns more than $50K annually.

### Key Features
- Fetches the Adult dataset directly from OpenML.
- Separates the dataset into features (`X`) and target (`y`).
- Prints a detailed description of the dataset.

## Installation

### Prerequisites
- Python 3.x
- `scikit-learn` library

### Setup

1. Install the necessary Python packages:
    ```bash
    pip install scikit-learn
    ```

2. Clone the repository (if applicable):
    ```bash
    git clone https://github.com/username/repository.git
    ```
3. Navigate to the project directory:
    ```bash
    cd repository
    ```

## Usage

To run the code and fetch the dataset:

1. Open a Python environment or script and paste the following code:
    ```python
    from sklearn.datasets import fetch_openml

    # Fetch the Adult dataset
    adult = fetch_openml(name='adult', version=2)

    # Data and target
    X = adult.data
    y = adult.target

    # Print some information
    print(adult.DESCR)  # Dataset description
    ```

2. Run the script. The dataset will be fetched, and a description will be printed.

### Example Output

The output will include the dataset's description, detailing the features, target variable, and other relevant information.


