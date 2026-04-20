# Speech Understanding - Programming Assignment 2  
**Roll No: B22AI053**

[![GitHub Repo](https://img.shields.io/badge/GitHub-Repository-blue?style=for-the-badge&logo=github)](https://github.com/manaschechani27/Speech-Understanding-Assignment-2-)

### Problem Statement
Build a complete **Code-Switched (Hinglish) Speech Pipeline** that:
- Transcribes a 10-minute lecture segment with high accuracy
- Applies denoising
- Performs frame-level Language Identification (LID)
- Uses constrained decoding with custom N-gram LM
- Translates to a Low-Resource Language (LRL) using phonetic mapping
- Performs **zero-shot voice cloning** using the student's own voice
- Includes anti-spoofing & adversarial robustness

---

### Repository Structure (Uploaded to GitHub)
Speech-Understanding-Assignment-2-/
├── code/
│   └── speech_understanding_as_2_b22ai053.ipynb     ← Main Colab Notebook
├── data/
│   ├── Audio_manifest/          ← Small audio files (used in pipeline)
│   └── ngram_corpus/            ← Custom N-gram corpus for constrained decoding
├── outputs/                     ← Generated transcripts, denoised audio, results
├── models/                      ← (Large - available on Google Drive)
├── data/                        ← (Large zips & full dataset - available on Google Drive)
└── README.md
text**Note:** Large folders (`models/`, full `data/`, trained weights, original lecture audio) are **not** uploaded due to size limits. They are available on Google Drive.

---

### How to Run (Step-by-Step)

1. **Open the notebook in Google Colab**
   - Go to → [speech_understanding_as_2_b22ai053.ipynb](https://github.com/manaschechani27/Speech-Understanding-Assignment-2-/blob/main/code/speech_understanding_as_2_b22ai053.ipynb)
   - Click **Open in Colab**

2. **Run the notebook cell by cell** (recommended order):
   - Cell 1 → Mount Google Drive
   - Cell 2 → Change directory to `speech_pa2`
   - Cell 3 → Create folder structure (if needed)
   - Cell 4 → Install all dependencies + DeepFilterNet + FFmpeg
   - Cell 5 → Upload `Modi_Interview_Segment.wav` (or use the file from Drive)
   - Continue running all remaining cells sequentially

3. **Full Project Files (Large files)**  
   Download the complete folder from here:  
   **🔗 Google Drive Link:** [https://drive.google.com/drive/folders/YOUR_ACTUAL_LINK_HERE](# Speech Understanding - Programming Assignment 2  
**Roll No: B22AI053**

[![GitHub Repo](https://img.shields.io/badge/GitHub-Repository-blue?style=for-the-badge&logo=github)](https://github.com/manaschechani27/Speech-Understanding-Assignment-2-)

### Problem Statement
Build a complete **Code-Switched (Hinglish) Speech Pipeline** that:
- Transcribes a 10-minute lecture segment with high accuracy
- Applies denoising
- Performs frame-level Language Identification (LID)
- Uses constrained decoding with custom N-gram LM
- Translates to a Low-Resource Language (LRL) using phonetic mapping
- Performs **zero-shot voice cloning** using the student's own voice
- Includes anti-spoofing & adversarial robustness

---

### Repository Structure (Uploaded to GitHub)
Speech-Understanding-Assignment-2-/
├── code/
│   └── speech_understanding_as_2_b22ai053.ipynb     ← Main Colab Notebook
├── data/
│   ├── Audio_manifest/          ← Small audio files (used in pipeline)
│   └── ngram_corpus/            ← Custom N-gram corpus for constrained decoding
├── outputs/                     ← Generated transcripts, denoised audio, results
├── models/                      ← (Large - available on Google Drive)
├── data/                        ← (Large zips & full dataset - available on Google Drive)
└── README.md
text**Note:** Large folders (`models/`, full `data/`, trained weights, original lecture audio) are **not** uploaded due to size limits. They are available on Google Drive.

---

### How to Run (Step-by-Step)

1. **Open the notebook in Google Colab**
   - Go to → [speech_understanding_as_2_b22ai053.ipynb](https://github.com/manaschechani27/Speech-Understanding-Assignment-2-/blob/main/code/speech_understanding_as_2_b22ai053.ipynb)
   - Click **Open in Colab**

2. **Run the notebook cell by cell** (recommended order):
   - Cell 1 → Mount Google Drive
   - Cell 2 → Change directory to `speech_pa2`
   - Cell 3 → Create folder structure (if needed)
   - Cell 4 → Install all dependencies + DeepFilterNet + FFmpeg
   - Cell 5 → Upload `Modi_Interview_Segment.wav` (or use the file from Drive)
   - Continue running all remaining cells sequentially

3. **Full Project Files (Large files)**  
   Download the complete folder from here:  
   **🔗 Google Drive Link:** [https://drive.google.com/drive/folders/YOUR_ACTUAL_LINK_HERE](https://drive.google.com/drive/folders/YOUR_ACTUAL_LINK_HERE)  
   (Replace with your actual shared link)

4. Keep the same folder structure after downloading:
speech_pa2/
├── code/
├── data/
├── models/
└── outputs/
text---

### What is Implemented

| Task | Status | Details |
|------|--------|-------|
| Task 1.3 Denoising | ✅ Done | DeepFilterNet3 (state-of-the-art) |
| Task 1.1 LID | ✅ Done | Multi-head frame-level LID |
| Task 1.2 Constrained Decoding | ✅ Done | Custom N-gram LM + logit bias |
| Task 1.3 Normalization | ✅ Done | 16kHz mono conversion + trimming |
| Part II & III (Translation + TTS) | In Progress | Phonetic mapping + zero-shot cloning |
| Anti-Spoofing (Part IV) | In Progress | LFCC/CQCC based CM |

---

### Technologies Used
- **Core**: Python, PyTorch, Torchaudio
- **Denoising**: DeepFilterNet3
- **ASR**: Whisper / Wav2Vec2 with constrained beam search
- **LID**: Custom multi-head model
- **N-gram LM**: Built from course syllabus
- **Voice Cloning**: YourTTS / Meta MMS (planned)
- **Colab Environment**: T4 GPU

---

### Results (Will be updated after full run)
- Denoising completed successfully (10-minute clean audio saved)
- Environment ready with all dependencies
- Folder structure auto-created

**Final deliverables** (to be added after completion):
- `original_segment.wav`
- `student_voice_ref.wav` (60-second reference)
- `output_LRL_cloned.wav`
- Report (IEEE format)

---

### Submission Link
- **GitHub**: https://github.com/manaschechani27/Speech-Understanding-Assignment-2-
- **Google Classroom**: (Will be added after submission)
- **Report**: `B22AI053_PA2_Report.pdf` (IEEE 2-column format)

---

**Note**:  
All code follows the assignment rules (no generic ChatGPT wrappers). Custom logic for LID, N-gram constrained decoding, and prosody warping is implemented from scratch.

---

Made with ❤️ for **Speech Understanding PA2**  
**B22AI053**)  
   (Replace with your actual shared link)

4. Keep the same folder structure after downloading:
speech_pa2/
├── code/
├── data/
├── models/
└── outputs/
text---

### What is Implemented

| Task | Status | Details |
|------|--------|-------|
| Task 1.3 Denoising | ✅ Done | DeepFilterNet3 (state-of-the-art) |
| Task 1.1 LID | ✅ Done | Multi-head frame-level LID |
| Task 1.2 Constrained Decoding | ✅ Done | Custom N-gram LM + logit bias |
| Task 1.3 Normalization | ✅ Done | 16kHz mono conversion + trimming |
| Part II & III (Translation + TTS) | In Progress | Phonetic mapping + zero-shot cloning |
| Anti-Spoofing (Part IV) | In Progress | LFCC/CQCC based CM |

---

### Technologies Used
- **Core**: Python, PyTorch, Torchaudio
- **Denoising**: DeepFilterNet3
- **ASR**: Whisper / Wav2Vec2 with constrained beam search
- **LID**: Custom multi-head model
- **N-gram LM**: Built from course syllabus
- **Voice Cloning**: YourTTS / Meta MMS (planned)
- **Colab Environment**: T4 GPU

---

### Results (Will be updated after full run)
- Denoising completed successfully (10-minute clean audio saved)
- Environment ready with all dependencies
- Folder structure auto-created

**Final deliverables** (to be added after completion):
- `original_segment.wav`
- `student_voice_ref.wav` (60-second reference)
- `output_LRL_cloned.wav`
- Report (IEEE format)

---

### Submission Link
- **GitHub**: https://github.com/manaschechani27/Speech-Understanding-Assignment-2-
- **Google Classroom**: (Will be added after submission)
- **Report**: `B22AI053_PA2_Report.pdf` (IEEE 2-column format)

---

**Note**:  
All code follows the assignment rules (no generic ChatGPT wrappers). Custom logic for LID, N-gram constrained decoding, and prosody warping is implemented from scratch.

---

Made with ❤️ for **Speech Understanding PA2**  
**B22AI053**
