# 👵🏽🎙️ Rural Senior AI Care: Local Voice Companion

## 🎯 The Mission
Combating extreme digital and social isolation among rural senior citizens in India. 

Current AI companions fail in rural demographics because they lack linguistic authenticity (local dialects) and cultural resonance (local traditions, dietary habits, agricultural calendars). This open-source project provides the architecture to build an **offline, voice-first AI companion** tailored to under-resourced Indian dialects like Tulu, Beary, and Konkani.

## ⚠️ The Problem We Are Solving
1. **Linguistic Exclusion:** Existing AI models struggle with regional Indian dialects and phonetic quirks.
2. **Digital Literacy Barrier:** Rural seniors often cannot use text-based apps; voice is the only viable interface.
3. **Connectivity Issues:** Cloud-dependent AI fails in remote areas with unstable internet.
4. **Cultural Hallucinations:** Generic AI gives westernized advice that doesn't fit rural Indian lifestyles.

## 🛠️ Architecture & Stack
This repository houses the code, datasets, and training pipelines to deploy localized AI to low-end Android devices.

*   **Foundation Model:** Fine-tuning base models using **Supervised Fine-Tuning (SFT)** via LoRA adapters.
*   **Dataset:** Processing audio and transcription data from **Project Vaani** (IISc & ARTPARK).
*   **On-Device Engine:** Android **AICore / Gemini Nano** for fully offline, low-latency processing without cellular data.
*   **Audio Pipeline (TTS/STT):** Integrating Indic-TTS (AI4Bharat) and Google Gemini Audio Tuning to capture the phonetic warmth and accent of rural speech.

## 🗺️ Project Roadmap
- [ ] **Phase 1:** Data Formatting — Filter and process Project Vaani audio/text JSONL pairs for Dakshina Kannada/Udupi dialects.
- [ ] **Phase 2:** Cloud Fine-Tuning — Train cultural adapters via Google Vertex AI / AI Studio.
- [ ] **Phase 3:** Audio Engine — Map phonetic SSML / IPA tags to local pronunciations.
- [ ] **Phase 4:** Android Deployment — Build the offline voice-loop architecture using Android AICore.

## 🤝 Contributing
We are looking for open-source contributors with experience in:
- NLP and Dataset formatting (JSONL pipelines)
- Android native development (AICore / ML Kit)
- Local dialect speakers (Tulu, Beary, Kannada, Konkani) to verify cultural context.

## 📄 License
This project is licensed under the MIT License - see the LICENSE file for details.
