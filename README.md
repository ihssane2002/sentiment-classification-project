# sentiment-classification-project
# Sentiment Classification App with BERT
Bienvenue sur ce dépôt GitHub dédié à la **classification de sentiments** à l’aide d’un modèle RoBERTa entraîné sur les **avis produits Amazon**. Le modèle obtenu est ensuite utilisé dans une **application Streamlit** hébergée sur [Hugging Face Spaces](https://huggingface.co/spaces/ihssane20/emotiview-app/tree/main).


##  Description du projet

Ce projet combine deux parties principales :

1. **Un modèle BERT personnalisé** que j'ai entraîné pour la classification de sentiments.  
   👉 Entraîné dans le notebook [`sentiment_classification_model.ipynb`].
  a pour but de :

- **Prétraiter et préparer un jeu de données réel** (Amazon Review Dataset) pour une tâche de classification de sentiments.
- **Entraîner un modèle RoBERTa (base)** sur ce jeu de données.
- **Déployer une interface Streamlit** intuitive pour tester le modèle en ligne.


## 2.  📊 Résultats de l'entraînement

Le modèle **RoBERTa-base** a été fine-tuné pendant environ 2 époques. Voici les performances obtenues :

```text
- eval_loss: 0.2088
- eval_accuracy: 96.02%
- eval_f1: 95.93%
- eval_runtime: 14.13s
- eval_samples_per_second: 69.39
- epoch: ~2.08

3. **Une interface interactive avec Streamlit**, permettant à l'utilisateur :
   - D’écrire un texte ou une phrase
   - De recevoir la prédiction du modèle (positive, négative, neutre)
   - De visualiser les résultats facilement

## 🧩 Contenu du dépôt sur hugging face

Le dépôt contient :

| Fichier                  | Description                                  |
|--------------------------|----------------------------------------------|
| `app.py`                | Interface Streamlit principale               |
| `database.py`           | Gestion de la base de données (si utilisée) |
| `requirements.txt`      | Dépendances du projet                        |
| `model.safetensors`     | Poids du modèle entraîné                     |
| `pytorch_model.bin`     | Backup du modèle (PyTorch)                   |
| `config.json`, `vocab.json`, etc. | Fichiers du tokenizer BERT       |





