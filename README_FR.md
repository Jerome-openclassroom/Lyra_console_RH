# 🤖 Lyra_Console_RH — Assistant RH IA (RAG + OpenAI)

**Lyra_Console_RH** est un assistant de recrutement basé sur l’intelligence artificielle, léger et réactif.  
Il simule le comportement d’un recruteur intelligent grâce à l’API Assistants d’OpenAI, à une mémoire de conversation persistante, à un système RAG (génération augmentée par récupération), et à une interface Gradio.

---

## 🚀 Fonctionnalités principales

- 🧠 **Assistant OpenAI avec RAG** : Connecté à un magasin vectoriel construit à partir de README liés à l’IA, l’écologie, la météorologie et l’agronomie.
- 🧾 **Mémoire persistante** : Utilise un `thread_id` fixe pour conserver l’historique des échanges.
- 🪄 **Génération naturelle de mails** : Produit des emails RH personnalisés et immédiatement exploitables.
- 🎛️ **Console interactive** : Interface simple via Gradio simulant un bureau RH virtuel.
- 🔐 **Sécurité API** : Utilise un fichier `.env` local pour gérer la clé API (`ENV/env.txt`).

---

## 📦 Mode d’emploi

### 1. Cloner le dépôt

```bash
git clone https://github.com/Jerome-openclassroom/Lyra_Console_RH.git
cd Lyra_Console_RH
```

### 2. Ajouter votre clé API

Créez un fichier nommé `env.txt` dans le dossier `ENV/` avec ce contenu :

```
OPENAI_API_KEY=sk-XXXXXXXXXXXXXXXXXXXXXXXX
```

### 3. Lancer la console

```bash
python lyra_console_rh.py
```

L’interface Gradio s’ouvrira localement.

---

## 📬 Exemple d’usage

**Prompt utilisateur :**
```
Peux-tu me rédiger un mail de réponse à l'attention de Jérôme FRASSON sollicitant un échange suite à sa candidature spontanée ?
```

**Réponse générée par l’IA :**
> *"Nous serions ravis d'organiser un échange afin de discuter de vos idées et voir comment nous pourrions collaborer..."*

👉 Le mail est prêt à être copié-collé, contextualisé, et adapté au profil du candidat.

---

## 📚 Corpus vectoriel

Les documents intégrés dans le RAG incluent :

- Plus de 10 fichiers README issus des [dépôts GitHub de Jérôme](https://github.com/Jerome-openclassroom)
- Sujets abordés : Workflows IA, diagnostics écologiques, fine-tuning, jeux de données environnementaux

---

## 🧪 Technologies utilisées

- [OpenAI Assistant API](https://platform.openai.com/)
- Python 3.10+
- Gradio
- Fichier `.env` local
- Récupération de documents via vector store OpenAI

---

## 📂 Organisation du dépôt

```
📁 Lyra_Console_RH/
├── 📄 README.md                   # README principal en anglais
├── 📄 README_Lyra_Console_RH_FR.md  # Version française du README
├── 📄 requirements.txt            # Dépendances Python minimales (OpenAI, Gradio, etc.)
│
├── 📁 code/                       # Code source (Notebook IA)
│   └── Lyra_RH_console.ipynb      # Console RH interactive utilisant OpenAI Assistant + Gradio
│
├── 📁 screenshots/                # Captures d’écran illustratives
│   ├── prompting_console.png      # Fenêtre de prompt avec interface utilisateur
│   ├── questions_list.png         # Exemple de réponse listant les questions posées
│   └── Reply_mail.png             # Exemple de mail RH généré automatiquement


```

## 🧠 Auteur

**Jérôme Frasson**  
GitHub : [@Jerome-openclassroom](https://github.com/Jerome-openclassroom)  
Email : jerome.frasson.vsi@gmail.com  
Thèmes : IA × Environnement × Workflows agentiques

---

## 📝 Licence

Projet open source destiné à un usage personnel, éducatif et de recherche.  
La réutilisation est encouragée sous réserve de mention de l’auteur.
