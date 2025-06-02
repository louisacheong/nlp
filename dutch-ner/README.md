# 🧠 Custom Dutch Named Entity Recognition (NER) with spaCy

**Author**: Phui San Louisa Cheong  
**Portfolio Project – 2025**

---
[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/louisacheong/nlp/blob/main/Dutch_NER_Portfolio_Cheong.ipynb)

[![LinkedIn](https://img.shields.io/badge/-PhuiSanCheong-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/phui-san-louisa-cheong-6a62772/)](https://www.linkedin.com/in/phui-san-louisa-cheong-6a62772/)
## 🎯 Project Objective

This project demonstrates the training of a **custom Named Entity Recognition (NER)** model in Dutch using the [spaCy](https://spacy.io/) NLP library. The aim is to identify domain-specific entities not recognized by default models — especially within the **insurance and business sectors**.

---

## 🏷️ Custom Entities

The model was trained to recognize the following entity types:

- **`ZORGVERZEKERAAR`** – Dutch health insurers (e.g., Zilveren Kruis, VGZ)
- **`POLISNUMMER`** – Insurance policy numbers (e.g., CD123456X)
- **`BEDRIJFSNAAM`** – Dutch company names (e.g., d'Arschot en Gezelschap)

---

## 🛠️ Technologies Used

- Python 3.11
- spaCy 3.7
- Pre-trained model: `nl_core_news_lg`
- Jupyter Notebook / Colab
- `displacy` for NER visualization

---

## 🧪 Methodology

1. Generated synthetic but realistic training data
2. Verified character span alignment using `char_span()` to avoid misalignment issues
3. Fine-tuned the NER component with a limited dataset
4. Evaluated the model using test examples
5. Visualized entities using spaCy's built-in `displacy` module
6. Saved and reloaded the custom model for deployment

---

## 💾 Example Prediction

```python
text = "Mijn polisnummer is CD123456X en ik ben verzekerd bij Zilveren Kruis."
doc = nlp(text)
for ent in doc.ents:
    print(ent.text, ent.label_)
```

**Expected Output:**
```
CD123456X POLISNUMMER
Zilveren Kruis ZORGVERZEKERAAR
```

---

## 📈 Results

The custom NER model successfully identifies domain-specific Dutch entities with high precision in synthetic examples. It can be extended for production use cases with more annotated data.

---

## 📌 Next Steps

- Expand with real-world annotated data
- Add other entities like `KLANTNUMMER`, `IBAN`, `STRAATNAAM`
- Integrate into a **Streamlit** or **FastAPI** frontend for live use

---

## 📁 Repository Structure

```
nlp/
│
├── Dutch_NER_Portfolio_Cheong.ipynb     # Full notebook (Colab-ready)
├── dutch_ner_training_data.json         # Custom training data
├── custom_dutch_ner_model/              # Saved spaCy model (optional)
├── README.md
```

---

## 🔗 Author

Phui San Louisa Cheong  
🔗 [LinkedIn Profile](https://www.linkedin.com/in/phui-san-louisa-cheong-6a62772/)  
📧 Contact: available upon request

