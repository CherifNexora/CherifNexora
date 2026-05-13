# ⚖️ Assistant Juridique Algérien – RAG Anti‑Hallucinations

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/votre-utilisateur/assistant-juridique-algerien/blob/main/assistant_juridique.ipynb)
[![Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/downloads/)

Un assistant juridique 100 % local et open source spécialisé dans le droit algérien.  
Il répond **uniquement** à partir du contenu d’un document PDF (constitution, code, loi…) en combinant une recherche vectorielle multilingue (RAG) avec un grand modèle de langue (LLM) local, **sans inventer de réponses**.

🔹 **Arabe & Français** pris en charge nativement  
🔹 **Aucune hallucination** – blocage strict des informations hors document  
🔹 **Streaming** des réponses pour une expérience instantanée  
🔹 Fonctionne sur **Google Colab gratuit** (GPU T4) ou en local

---

## ✨ Fonctionnalités

- **Chargement de PDF** : importez n’importe quel document juridique (constitution, code civil, etc.).
- **Recherche contextuelle** : recherche sémantique multilingue (arabe ↔ français) grâce aux embeddings **BGE‑M3**, les plus performants à ce jour.
- **Filtre de pertinence** : seuls les passages avec un score de similarité suffisant sont fournis au LLM.
- **Prompt anti‑fabrication** : le modèle reçoit l’ordre strict de ne pas utiliser ses propres connaissances.
- **Génération streaming** : les mots s’affichent au fur et à mesure, donnant une impression de grande réactivité.
- **Interface Gradio** : discussion en ligne avec historique, copie possible, thème moderne.
- **100 % local** : aucun appel API externe, pas de limite de tokens ni de quota.

---

## 🧠 Architecture

