# LexiPioneers — Pronunciation Analyzer (GenAI)

**LexiPioneers** is an interactive pronunciation training tool powered by AI.  
It challenges users with words of varying difficulty, records their pronunciation, and analyzes it using speech recognition, phonetic dictionaries, and similarity metrics.

## 🚀 Features
- **AI-based Word Generation** — Uses GPT-2 to generate words for pronunciation practice at *easy*, *medium*, and *hard* difficulty levels.
- **Speech Recording** — Captures the user's pronunciation via microphone.
- **Phonetic Dictionary Lookup** — Matches words against a phonetic dataset to retrieve IPA (International Phonetic Alphabet) transcriptions.
- **Pronunciation Scoring** — Compares user pronunciation with correct pronunciation using Levenshtein similarity.
- **Feedback System** — Indicates whether the pronunciation is accurate, slightly off, or significantly different.

## 📂 Project Structure
dyslexia_empowerment/
--LexiPioneers(PronunciationAnalyzerGenAI).ipynb # Main notebook
--phoneticDictionary.xls # Original phonetic dataset
-- phoneticdict_with_labels.xls # Labeled phonetic dataset
-- .gitignore



## 🛠 Installation
1. **Clone this repository**
2. 
git clone https://github.com/<your-username>/dyslexia_empowerment.git
cd dyslexia_empowerment

Install dependencies
pip install pandas SpeechRecognition transformers python-Levenshtein

Download required datasets
Ensure phoneticDictionary.xls and phoneticdict_with_labels.xls are in the root directory.

🎯 Usage
Open the Jupyter Notebook
Run LexiPioneers(PronunciationAnalyzerGenAI).ipynb cell by cell.

Select the difficulty level (easy, medium, hard).

Speak the prompted word into your microphone.

View your similarity score and feedback.

📊 Pronunciation Scoring
Similarity ≥ tolerance → ✅ Accurate

poor_match_threshold ≤ Similarity < tolerance → ⚠ Slightly off but acceptable

Similarity < poor_match_threshold → ❌ Significantly different

📌 Requirements
Python 3.8+

Microphone access

Internet connection (for speech recognition & AI model downloads)

💡 Future Improvements
Add GUI for easier interaction

Integrate real-time waveform visualization

Support for multiple languages
