# Association Rule Mining using Apriori Algorithm

## 📌 Overview
Association Rule Mining is a data mining technique used to discover interesting relationships, patterns, or associations among items in large datasets.  
This project implements the **Apriori Algorithm** to extract frequent itemsets and generate strong association rules based on **support**, **confidence**, and **lift**.

Common real-world applications include:
- Market Basket Analysis
- Recommendation Systems
- Customer Behavior Analysis
- Web Usage Mining

---

## ⚙️ Algorithm Used: Apriori
Apriori works on the principle that:
> *All non-empty subsets of a frequent itemset must also be frequent.*

It follows a **bottom-up** approach:
1. Generate frequent 1-itemsets
2. Iteratively generate k-itemsets
3. Prune itemsets that do not meet minimum support
4. Generate association rules from frequent itemsets

---

## 📊 Key Metrics
- **Support**  
  Frequency of an itemset in the dataset  
  \[
  Support(A) = \frac{\text{Transactions containing A}}{\text{Total transactions}}
  \]

- **Confidence**  
  Likelihood of item B given item A  
  \[
  Confidence(A \rightarrow B) = \frac{Support(A \cup B)}{Support(A)}
  \]

- **Lift**  
  Strength of association between A and B  
  \[
  Lift(A \rightarrow B) = \frac{Confidence(A \rightarrow B)}{Support(B)}
  \]

---

## 🗂️ Dataset
- Input dataset consists of transactional data
- Each row represents a transaction
- Each transaction contains a list of items
