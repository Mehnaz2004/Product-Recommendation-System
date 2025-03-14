# Product Recommendation System

## Overview
The **Product Recommendation System** is a machine learning-based project that utilizes the **Apriori Algorithm** to generate the best product recommendations. Various Apriori rules, such as **support, confidence, and lift**, are applied to identify strong associations between products and optimize the recommendation process. The system is deployed and available for use at [Streamlit App](https://appuct-recommendation-system-s3qtc2wjdelpvmnnjpnwqc.streamlit.app/).

## Why Apriori?
The **Apriori Algorithm** is effective in identifying frequent product combinations in transactional data. It works by:
- **Mining Frequent Itemsets**: Finds sets of products frequently purchased together.
- **Applying Association Rules**: Generates if-then rules like "If a customer buys A, they are likely to buy B."
- **Using Confidence & Lift**:
  - **Confidence** measures how often a rule is correct.
  - **Lift** indicates the strength of the rule compared to random chance.
  - **Thresholds** for support, confidence, and lift are used to filter out weak rules, ensuring accurate recommendations.

## Features
- **Apriori Algorithm**: Uses association rule mining to find relationships between products.
- **Frequent Itemset Mining**: Identifies patterns in user purchase behavior.
- **Data Visualization**: Insights from data using charts and graphs.
- **Model Training**: Implements Apriori rules for improved recommendations.
- **Jupyter Notebook**: Contains detailed code and visualizations for analysis.
- **Streamlit UI**: Provides a web-based interface for viewing recommendations.
- **Cart-Based System**: Users can add items to their cart and receive recommendations for frequently bought-together products.

## Technologies Used
- **Python**
- **Pandas**
- **NumPy**
- **mlxtend** (for Apriori algorithm implementation)
- **Matplotlib & Seaborn** (for data visualization)
- **Streamlit** (for web deployment)
- **JSON** (to store and load Apriori-generated rules)

## Installation & Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/Mehnaz2004/Product-Recommendation-System.git
   cd Product-Recommendation-System
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the project using Streamlit:
   ```bash
   streamlit run app.py
   ```

## Usage
- Open the **Apriori.ipynb** Jupyter Notebook to analyze the dataset and visualize frequent itemsets.
- The dataset consists of **transactions**, where each row represents a purchase made by a customer.
- The **Apriori Algorithm** is applied to discover patterns and generate association rules.
- These association rules are saved in `apriori_results.json`.
- Run the **Streamlit app** (`app.py`) to interact with the recommendation system:
  - Add items to your cart.
  - View frequently bought-together recommendations.
  - Clear your cart and explore different recommendations.

## Dataset
The dataset used in this project is `Market_Basket_Optimisation.csv`, which contains **transactional data** where:
- Each **row represents a unique transaction** made by a customer.
- Each **column represents a product**, with values indicating whether a product was purchased.
- The **Apriori Algorithm** extracts frequent itemsets and association rules to predict relevant recommendations.
- Example of generated rules from `apriori_results.json`:
  - **French Fries → Chocolate, Green Tea, Burgers** (High confidence & lift)
  - **Spaghetti → Tomatoes, Eggs, Milk** (Commonly purchased together)
  - **Mineral Water → Burgers, Pancakes, Ground Beef** (Frequently co-occurring products)

## Future Enhancements
- Apply **clustering algorithms** for segmented recommendations.
- Implement deep learning-based recommendations.
- Integrate real-time recommendation updates.
- Optimize performance using scalable architectures.

## Contact
For any questions or collaborations, feel free to reach out via [LinkedIn](https://www.linkedin.com/in/mehnaz-ali-7b4764282/) or open an issue in the repository.
