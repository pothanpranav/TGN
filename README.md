# 🧠 Addressing Class Imbalance in Temporal Graph Networks for E-Commerce Interaction Prediction

**Author:** Pranav Pothan  
**Affiliation:** Chennai Mathematical Institute  
**Contact:** pothanpranav@gmail.com  

---

## 🚀 Overview

E-commerce platforms generate massive streams of user interactions—most of which are low-value events like product views, while high-value actions (like purchases) are rare.

This project tackles a key challenge:

⚠️ How do we accurately predict rare but important interactions in temporal graphs?

We propose a hybrid framework that combines:
- Temporal Graph Networks (TGN)
- JODIE-based dynamic embeddings
- Temporal SMOTE (for imbalance handling)
- Adaptive Focal Loss (for better training focus)

---

## 🏗️ Key Contributions

- 🔁 Temporal Modeling using TGN + JODIE projection  
- ⚖️ Class Imbalance Handling:
  - Temporal SMOTE (data-level)
  - Adaptive Focal Loss (algorithm-level)
- 📊 Explainability using Cohen’s d effect size  
- 📈 Significant improvement in minority-class prediction  

---

## 📊 Results

### Edge Classification

| Model | Accuracy | Macro F1 |
|------|--------|---------|
| Baseline TGN | 85.2% | 32.4% |
| TGN + JODIE | 91.8% | 48.7% |
| Full Hybrid | 95.0% | 63.32% |

✔️ +30.9% improvement in Macro F1

---

### Link Prediction

- Baseline AUC: 0.55
- Full Hybrid AUC: 0.71

---

### Minority Class Performance

| Class | Baseline F1 | Hybrid F1 |
|------|------------|----------|
| Add-to-Cart | 3.9% | 52.0% |
| Purchase | 1.5% | 41.5% |

👉 Huge improvement on commercially critical events

---

## 🧩 Architecture

The framework integrates three components:

1. TGN Backbone  
2. JODIE Projection  
3. Imbalance Handling (Temporal SMOTE + Adaptive Focal Loss)

---

## 🗂️ Dataset

- Amazon E-commerce interaction dataset  
- ~60,000 interactions  

Classes:
- View (79.4%)
- Add-to-cart (15.3%)
- Purchase (5.3%)

---

## ⚙️ Training Details

- Optimizer: Adam  
- Learning Rate: 1e-4  
- Epochs: 20  
- Embedding Dimension: 100  

---

## 📈 Evaluation Metrics

- Accuracy  
- Macro F1  
- AUC  
- Cohen’s d  

---

## 🔍 Explainability

Cohen’s d = 0.80 → strong separation between true and false interactions.

---

## 💡 Why This Matters

- Predict purchases (high-value events)
- Improve recommendations
- Increase conversions

---

## ⚠️ Limitations

- Single dataset  
- Scalability not tested  
- Link prediction can improve  

---

## 🔮 Future Work

- Hard negative sampling  
- Better scalability  
- Richer embeddings  
- Instance-level explainability  

---

## ⭐ If you find this useful

Give a ⭐ on GitHub!
