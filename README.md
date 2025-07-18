# FUTURE_PE_01
Task 1 - AI-Powered YouTube Script and Thumbnail Generator 
Welcome to my first task as a Prompt Engineering Intern at **Future Interns**!  
This project demonstrates how I use prompt chains and AI tools to generate engaging **YouTube videos**, including:

- 📌 Topic research
- 🧠 Prompt engineering
- 📝 Full video scripting
- 🖼️ Thumbnail design (AI-generated)
- 🎬 Final AI-edited video

---

## 🔧 Tools Used
- **ChatGPT (Prompt generation & scripting)**
- **Pictory / InVideo (Video generation)**
- **DALL·E / MidJourney (Thumbnail image)**
- **Canva (Mockups & visuals)**
- **Notion (Planning)**

---

## 🚀 Prompt Chain Strategy

> 📁 Detailed prompt chain documented in [`PromptChain.md`](./PromptChain.md)

1. **Find a trending topic**
2. **Generate SEO-optimized titles**
3. **Create full video script (800–1500 words)**
4. **Suggest engaging thumbnails**
5. **Generate thumbnail image with DALL·E**
6. **Build video using AI editors**

---

## 📺 Video Topic Chosen
**"The Rise of AI in African Education: Is it Revolution or Risk?"**

---

## ✅ Deliverables

- [x] PromptChain.md (documented prompt chain)
- [x] Full video script
- [x] Thumbnail concept + AI image
- [x] Final AI video (link below 👇)

📹 **Watch the final video here** → [link to video once uploaded]

---

## 🧠 What I Learned
- How to structure complex prompt chains for creative output
- How to guide AI tools toward specific branding goals
- Combining multiple AI tools for a full pipeline project

---

## 🌐 Connect
🔗 [My LinkedIn](https://www.linkedin.com/in/khalidag/)  
🎓 [Future Interns](https://www.futureinterns.com/)
from pathlib import Path

# Créer le contenu du fichier PromptChain.md
prompt_chain_content = """
# 🎯 Prompt Chain – Task 1: AI-Powered YouTube Script & Thumbnail Generator

## Sujet choisi : « 5 outils d’IA qui peuvent remplacer un emploi à temps plein (en 2025) »

### 1️⃣ Génération d’idées de sujets
**Prompt :**  
"Give me 5 trending YouTube video ideas in the AI & Freelance career niche that are likely to go viral in 2025."

**Résultat :**
- Top 5 AI Tools That Can Replace Your 9–5 Job
- Freelancers, Beware: AI That Does Your Job Better
- How I Run a Business With Just AI Tools
- No Team, No Problem: AI That Works For You
- Can AI Really Replace Human Creativity?

🎯 Choix final : **“5 AI Tools That Can Replace a Full-Time Job in 2025”**

---

### 2️⃣ Génération du titre
**Prompt :**  
"Based on the topic, generate 3 SEO-optimized YouTube titles."

**Résultat :**
- "5 outils d’IA qui peuvent remplacer un emploi à temps plein (en 2025)"
- "Ces outils d’IA font le travail de 5 employés"
- "Travailler sans travailler : l’IA prend le relais"

---

### 3️⃣ Script YouTube (voir Script.md)

---

### 4️⃣ Idée de miniature
**Texte de vignette :** "Replaced by AI?"

**Prompt IA pour DALL·E :**  
"A humanoid robot sitting at a modern office desk, with papers flying in the air, a coffee mug, a laptop open to ChatGPT, cinematic lighting, 16:9 aspect ratio — digital art style."

---

### 5️⃣ Outils utilisés :
- ChatGPT (scripting)
- MidJourney / DALL·E (miniature)
- InVideo / Pictory (montage vidéo)
- Canva (mockup)
- Notion (documentation)
"""

# Créer le contenu du script vidéo
script_video_content = """
# 🎥 Script YouTube — « 5 outils d’IA qui peuvent remplacer un emploi à temps plein (en 2025) »

## INTRO
Et si je vous disais que certaines personnes gèrent déjà une entreprise... sans aucune équipe ?
Grâce à l’intelligence artificielle, des outils ultra-puissants peuvent aujourd’hui faire le travail d’un employé à temps plein.
Dans cette vidéo, je vous présente 5 outils d’IA qui peuvent remplacer un emploi à plein temps en 2025 — et comment vous pouvez les utiliser.

## 1. Copy.ai – Le rédacteur automatique
🎯 Remplace : Copywriter
Génère des articles, emails, posts LinkedIn. Idéal pour freelances & agences.
💡 Ex : 30 publications réseaux en 10 minutes.

## 2. Pictory – Le vidéaste automatisé
🎯 Remplace : Monteur vidéo
Transforme un texte en vidéo complète avec voix et visuels.
💡 Ex : newsletter → vidéo hebdo auto.

## 3. ElevenLabs – Le doubleur vocal IA
🎯 Remplace : Voix off
Crée des voix naturelles, clones vocaux. Multilingue.
💡 Ex : séries TikTok doublées automatiquement.

## 4. MidJourney – Le graphiste génératif
🎯 Remplace : Designer graphique
Crée des visuels pro via simple prompt.
💡 Ex : 10 visuels IG pour une boutique en ligne.

## 5. ChatGPT – L’assistant universel
🎯 Remplace : Assistant / analyste
Organise, résume, écrit, code. Polyvalent et scalable.
💡 Ex : gérer toute ta journée de travail sans changer d’outil.

## OUTRO
Ces outils ne sont pas des gadgets. Ils redéfinissent le travail.
👉 Est-ce que l’IA va te remplacer... ou vas-tu apprendre à la piloter ?
Abonne-toi, commente l’outil que tu utiliserais en premier, et reste connecté pour d’autres vidéos sur l’IA et le futur du travail.
"""

# Enregistrer les fichiers dans un répertoire temporaire
base_path = Path("/mnt/data/Task1_FutureInterns")
base_path.mkdir(parents=True, exist_ok=True)

# Sauvegarde des fichiers .md
prompt_file = base_path / "PromptChain.md"
script_file = base_path / "Script.md"

prompt_file.write_text(prompt_chain_content.strip(), encoding="utf-8")
script_file.write_text(script_video_content.strip(), encoding="utf-8")

# Afficher les chemins des fichiers générés
prompt_file, script_file
