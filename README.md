# Bitcoin-OTC-Network-Analysis
Network analysis of the Bitcoin OTC trust dataset to uncover trust dynamics for financial transaction reliability.
--
# Network Analysis: Bitcoin OTC Trust Weighted Signed Network

An end-to-end network analysis project exploring trust dynamics in the Bitcoin OTC trust weighted signed network dataset to support reliable financial transactions.

---

## 🧠 Project Overview

This project analyzes the [Bitcoin OTC trust weighted signed network dataset](https://snap.stanford.edu/data/soc-sign-bitcoinotc.html), which includes 5,881 users and 35,592 trust ratings (from -10 to +10). The analysis supports **Reconxi**, a tool for ensuring trust and accuracy in financial transactions, by uncovering patterns for fraud detection and transaction reliability.

---

## 📌 Research Questions

1. Do users who joined the network earlier (first 10%) receive higher trust scores than latecomers, and does this advantage persist over time?
2. Which users exhibit the highest fluctuations in trust over time?
3. Are there users bridging distrustful communities, and do they accelerate distrust propagation?
4. How does the volume of trust ratings change over time?
5. Do the top 20 most trusted users form a tightly interconnected core, and does this concentration of trust create systemic vulnerabilities in the network?
6. How does the overall trust distribution (positive vs. negative) impact the credibility of the network?

---

## 🛠️ Methodology

- **Tools**: Pandas, NetworkX, Matplotlib, Seaborn, python-louvain.
- **Data Prep**: Loaded `soc-sign-bitcoinotc.csv`, converted timestamps, built a directed graph.
- **Analysis**: Computed trust scores, variability, community detection, and more.

See [Bitcoin_OTC_Analysis.ipynb](./Bitcoin_OTC_Analysis.ipynb) for full code.

---

## 📊 Key Findings

- Early adopters have higher trust scores (1.81 vs. 0.82).
- Top user variability: 14.14, indicating potential fraud risks.
- Bridge users connect distrust clusters, amplifying negativity.
- Trust ratings peaked in 2011/2013, then declined.
- Top 20 trusted users form a dense core (45 edges), posing vulnerabilities.
- 89.9% positive ratings support network credibility.
  
See [Technical Report](Technical_Report_Network_Analysis.pdf) for full report.
---

## 📂 Repository Structure
 - Figures/                   # Visualization images
 - Bitcoin_OTC_Analysis.ipynb        # Jupyter Notebook with code and analysis
 - README.md                         # Project overview
 - Technical_Report_Network_Analysis.pdf  # Detailed technical report


*Note*: The dataset (`soc-sign-bitcoinotc.csv`) is not included but can be downloaded from the [Stanford Large Network Dataset Collection](https://snap.stanford.edu/data/soc-sign-bitcoinotc.html).

---

## 🚀 Getting Started

To explore the analysis:
1. Clone the repository: `git clone https://github.com/OLUWAJOMILOJU/Bitcoin-OTC-Network-Analysis.git`
2. Install dependencies: `pip install pandas networkx matplotlib seaborn python-louvain jupyter`
3. Run the notebook: `Bitcoin_OTC_Analysis.ipynb`
---
## 👤 Author

**Oluwajomiloju Emmanuel Oladeji**  
📍 Lagos, Nigeria  
🔗 [LinkedIn](https://www.linkedin.com/in/oluwajomiloju-oladeji-5baba6260) • 📧 [Email](mailto:oluwajomilojuoladeji@gmail.com)

---

## Feedback & Collaboration

Interested in extending this project or collaborating? Open issues, submit pull requests, or reach out via [email](mailto:oluwajomilojuoladeji@gmail.com). Feedback is welcome!

---
##  References

- [Bitcoin OTC Dataset](https://snap.stanford.edu/data/soc-sign-bitcoinotc.html)
