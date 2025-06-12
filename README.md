# 🧠 Pokémon Classification using Machine Learning

This project explores computer vision approaches to Pokémon image classification, including:
- A **binary classifier** distinguishing real-world animals from Pokémon.
- A **multi-label classifier** predicting Pokémon **typings** (e.g., Fire, Water, Ground) based on appearance.

Built using PyTorch, scikit-learn, and image augmentation techniques.  
Collaborators: Joshua Aflleje & Jack Oebker (Arizona State University)

---

## 🗂️ Project Structure

| Folder | Contents |
|--------|----------|
| `binary_classifier/` | MLP model distinguishing Pokémon from real animals |
| `multi_label_classifier/` | CNN model predicting Pokémon types |
| `paper/` | Final write-up explaining methodology, results, and discussion |

---

## 📌 Highlights

### 🔹 Binary Pokémon vs. Animal Classifier
- Used a 3-layer MLP (Multi-Layer Perceptron)
- Images flattened to RGB vectors (224×224)
- Pokémon sprites were randomly positioned on natural backgrounds
- Achieved **78% accuracy** at peak

### 🔹 Multi-label Typing Classifier
- Based on **ResNet18**, modified for Pokémon sprites
- Predicts 1–2 types from 18 possible Pokémon types
- Inputs: Pokémon image + average RGB color
- Achieved **58% accuracy** across 10 epochs

---

## 📊 Sample Output

**Confusion Matrix**  
✔️ TP/FP/FN visualizations help diagnose errors  
**Color-Based K-Means Clustering**  
🎨 Explored correlation between sprite color and Pokémon type

---

## 🔍 Future Work
- Add more sprite variations (Mega, Alolan, etc.)
- Use color embeddings or cosine similarity for type classification
- Try data augmentation with GANs
- Explore ensemble modeling across architectures

---

## 🧾 Files

- 📄 [`Final_Project_Paper.pdf`](paper/Final_Project_Paper.pdf) — Full report with visuals
- 📘 [`FinalProject_Binary_Classifier.html`](binary_classifier/...) — MLP code & results
- 📘 [`FinalProject_Multi_Classifier.html`](multi_label_classifier/...) — CNN code & results

---

## ⚖️ License

Licensed under the [MIT License](LICENSE).

