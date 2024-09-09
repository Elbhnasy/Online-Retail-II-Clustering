
# Online-Retail-II-Clustering

This repository contains a project on customer segmentation using clustering techniques applied to the **Online Retail II** dataset. The dataset includes all the transactions occurring for a UK-based non-store online retailer between **01/12/2009** and **09/12/2011**. The goal of this project is to identify distinct customer segments based on their purchasing behavior, which can help in personalized marketing, inventory management, and sales strategies.

## Table of Contents

- [Project Overview](#project-overview)
- [Dataset Information](#dataset-information)
- [Project Objectives](#project-objectives)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Clustering Techniques](#clustering-techniques)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Project Overview

This project applies unsupervised learning techniques to cluster customers based on their transaction history. Clustering helps identify groups of similar customers, allowing us to understand distinct purchasing patterns and behaviors.

## Dataset Information

The **Online Retail II** dataset is publicly available and can be found [here](https://www.kaggle.com/datasets/khaledelbhnasy/online-retail-ii). It consists of the following features:

- **InvoiceNo**: Invoice number. Nominal, a 6-digit integral number uniquely assigned to each transaction.
- **StockCode**: Product (item) code. Nominal, a 5-digit integral number uniquely assigned to each distinct product.
- **Description**: Product name.
- **Quantity**: The quantities of each product per transaction.
- **InvoiceDate**: The date when each transaction occurred.
- **UnitPrice**: Unit price of the product.
- **CustomerID**: Unique ID assigned to each customer.
- **Country**: Country where the customer resides.

## Project Objectives

The main objectives of this project include:
1. Preprocessing the dataset to handle missing values, duplicates, and outliers.
2. Creating relevant customer features (e.g., Recency, Frequency, and Monetary values).
3. Applying clustering algorithms such as K-Means, Hierarchical Clustering, and DBSCAN to identify customer segments.
4. Visualizing the resulting clusters and providing insights into customer behavior.

## Requirements

To run the project, you will need the following libraries:

- Python 3.10+
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/Elbhnasy/Online-Retail-II-Clustering.git
   ```

2. Navigate to the project directory:

   ```bash
   cd Online-Retail-II-Clustering
   ```

3. Install the required libraries:

   ```bash
   pip install -r requirements.txt
   ```

## Usage

To run the project:

1. Download the dataset and place it in the `/data` folder.
2. Run the preprocessing and clustering steps:

   ```bash
   python clustering_analysis.py
   ```

3. View the results and visualizations:

   After running the script, output files and cluster visualizations will be saved in the `/results` folder.

## Clustering Techniques

The following clustering algorithms are explored in this project:

1. **K-Means Clustering**: Partitioning customers into K distinct clusters.
2. **Hierarchical Clustering**: Agglomerative approach for creating a tree-like structure of clusters.
3. **DBSCAN**: Density-based spatial clustering for identifying customer patterns.

## Results

After applying different clustering algorithms, we identified the following customer segments:

1. Cluster 0 (Blue): "Retain"
* Rationale: This cluster represents high-value customers who purchase regularly, though not always very recently. The focus should be on retention efforts to maintain loyalty and spending.
* Action: Implement loyalty programs, personalized offers, and regular engagement to ensure they remain active.

2. Cluster 1 (Orange): "Re-Engage"
* Rationale: This group includes lower-value, infrequent buyers who haven’t purchased recently. The focus should be on re-engagement to return them to active purchasing behavior.
* Action: Use targeted marketing campaigns, special discounts, or reminders to encourage them to return and purchase again.

3. Cluster 2 (Green): "Nurture"
* Rationale: This cluster represents the least active and lowest-value customers, but they have made recent purchases. These customers may be new or need nurturing to increase engagement and spending.
* Action: Focus on building relationships, providing excellent customer service, and offering incentives to encourage more frequent purchases.

4. Cluster 3 (Red): "Reward"
* Rationale: This cluster includes high-value, very frequent buyers, many of whom are still actively purchasing. They are your most loyal customers, and rewarding their loyalty is key to maintaining their engagement.
* Action: Implement a robust loyalty program, provide exclusive offers, and recognize their loyalty to keep them engaged and satisfied.

**Summary of Cluster Names:**

* Cluster 0 (Blue): "Retain"
* Cluster 1 (Orange): "Re-Engage"
* Cluster 2 (Green): "Nurture"
* Cluster 3 (Red): "Reward"
- ![download](https://github.com/user-attachments/assets/0b31f34a-e813-4164-8cfe-ca8f4ee39a85)
- ![download1](https://github.com/user-attachments/assets/83ee049c-c213-4884-adc1-3d55ac99b5b3)



## Contributing

Feel free to contribute to this project. Fork the repository and create a pull request with your changes. All contributions are welcome!

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
