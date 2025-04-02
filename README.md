# Market Basket Analysis

Market Basket Analysis is a data mining technique used to uncover associations between products purchased together by customers. This analysis helps retailers understand customer purchasing behavior, optimize product placements, and design effective marketing strategies.

## Table of Contents

- [Overview](#overview)
- [Project Structure](#project-structure)
- [Setup Instructions](#setup-instructions)
- [Usage](#usage)
- [Extracted Insights](#extracted-insights)
- [Dependencies](#dependencies)
- [License](#license)

## Overview

This project implements Market Basket Analysis using the Apriori algorithm to identify frequent itemsets and generate association rules from transaction data. The analysis aims to reveal patterns in customer purchases, such as which products are frequently bought together.

**Key Concepts:**

- **Support**: The proportion of transactions that contain a particular item or itemset.
- **Confidence**: The likelihood that an item B is purchased when item A is purchased.
- **Lift**: The ratio of the observed support to that expected if A and B were independent.

These metrics help evaluate the strength and significance of the association rules derived from the data.

## Project Structure

The repository contains the following files:

- `market-basket-analysis-using-apriori.ipynb`: A Jupyter Notebook that performs data loading, preprocessing, application of the Apriori algorithm, and visualization of the results.
- `Market Basket.csv`: A CSV file containing transaction data, where each row represents a transaction and columns represent items purchased.

## Setup Instructions

To set up and run the project locally, follow these steps:

1. **Clone the Repository**: Use the following command to clone the repository to your local machine:

   ```bash
   git clone https://github.com/dattatejaofficial/Market-Basket-Analysis.git
   ```

2. **Navigate to the Project Directory**: Move into the project directory:

   ```bash
   cd Market-Basket-Analysis
   ```

3. **Create a Virtual Environment** (optional but recommended): Set up a virtual environment to manage project dependencies:

   ```bash
   python3 -m venv env
   ```

   Activate the virtual environment:

   - On Windows:
     ```bash
     .\env\Scripts\activate
     ```
   - On macOS/Linux:
     ```bash
     source env/bin/activate
     ```

4. **Install Dependencies**: Install the required Python packages using pip. The necessary packages are listed in the `requirements.txt` file. If `requirements.txt` is not present, you can manually install the following packages:

   ```bash
   pip install pandas apyori
   ```

## Usage

To run the analysis:

1. **Ensure the Virtual Environment is Activated**: Make sure your virtual environment is active (refer to the setup instructions above).

2. **Run the Notebook**: Open `market-basket-analysis-using-apriori.ipynb` in the Jupyter interface and execute the cells sequentially to perform the analysis and visualize the results.

## Extracted Insights

By applying the Apriori algorithm to the transaction data, the following insights were obtained:

- **Frequent Itemsets**: Identified combinations of items that frequently occur together in transactions. For example, customers who purchase item A often purchase item B as well.

- **Association Rules**: Generated rules that indicate the likelihood of purchasing item B given that item A is purchased. For instance, if a customer buys item A, there is a 70% chance they will also buy item B.

- **Lift Values**: Calculated lift values to assess the strength of the association rules, helping to identify the most significant product relationships.

These insights can be utilized to enhance product placement strategies, cross-selling opportunities, and targeted marketing campaigns.

## Dependencies

The project requires the following Python packages:

- `pandas`
- `apyori`

These dependencies are essential for data manipulation and applying the Apriori algorithm.
