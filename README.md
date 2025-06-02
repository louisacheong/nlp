# NLP & GenAI Portfolio by Louisa Cheong

Welcome! This portfolio showcases my hands-on projects in Natural Language Processing (NLP), Generative AI (GenAI), and applied machine learning. Each project is built with practical tools like spaCy, Hugging Face, and Google Cloud, focusing on real-world tasks such as entity recognition and domain-specific question answering.

---

## Projects
1. [Custom Dutch NER using spaCy](./dutch-ner/README.md)
2. [Domain-specific Q&A using LoRA](./genai-qa-lora/README.md)

### 1. Custom Dutch NER using spaCy
Created a Named Entity Recognition (NER) model tailored to Dutch insurance documents. Trained using spaCy with annotated entities such as:
- `ZORGVERZEKERAAR` – the insurance provider
- `POLISNUMMER` – the policy number
- `BEDRIJFSNAAM` – company name

The model was evaluated on precision/recall and deployed using a simple web interface. It supports Dutch-specific tokenization and was trained on realistic data collected from anonymized use cases.

### 2. Domain-specific Q&A using LoRA and Hugging Face
Developed a question-answering system fine-tuned for domain-specific tasks using Hugging Face transformer models. The process involved:

- Fine-tuning pre-trained LLaMA/GPT models using Low-Rank Adaptation (LoRA) via the `PEFT` library.
- Creating a custom Q&A dataset for semantic tuning in a specialized domain.
- Applying prompt engineering to improve output coherence and relevance.
- Evaluating model performance using BLEU and F1 metrics and iterating based on user feedback.
- Deploying the model through a Gradio UI to support non-technical users in querying the system interactively.

This project showcases the use of lightweight fine-tuning for scalable enterprise GenAI solutions.

---

## Technologies & Tools
- Python, spaCy, Hugging Face Transformers
- PEFT & LoRA fine-tuning
- Jupyter, Google Colab, Gradio
- Git, GitHub, Markdown

---

## About Me
I'm a data scientist based in Antwerp, Belgium, passionate about scalable AI and accessible NLP solutions. I specialize in applied ML for real-world domains such as healthcare, insurance, and education.

Connect with me on [LinkedIn](https://www.linkedin.com/in/phui-san-louisa-cheong-6a62772/)

