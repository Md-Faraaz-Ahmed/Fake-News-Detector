#  Fake News Detector  

A desktop application built with **Tkinter**, **OCR (Tesseract)**, **Speech Recognition (Vosk)**, and **Google Generative AI** to help identify whether a piece of news is real or fake.  
It supports:  
-  Text extraction from images using OCR  
-  Speech-to-text transcription with Vosk  
-  AI-powered fake news detection with Google Gemini  
-  User-friendly Tkinter interface with login authentication  

##  Features
- **OCR Integration** – Extracts text from uploaded images.  
- **AI Fake News Detection** – Uses Google Generative AI to analyze news content.  
- **Speech Recognition** – Converts spoken words into text for verification.  
- **Modern UI** – Simple Tkinter-based GUI with custom buttons and login screen.  

## Installation  

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/fake-news-detector.git
cd fake-news-detector
````

### 2. Install Dependencies

```bash
pip install pillow pytesseract google-generativeai vosk pyaudio
```

### 3. Install Tesseract OCR

* **Windows**: [Download here](https://github.com/UB-Mannheim/tesseract/wiki) and set the path in the code:

  ```python
  pytesseract.pytesseract.tesseract_cmd = r'C:\\Program Files\\Tesseract-OCR\\tesseract.exe'
  ```
* **Linux / Mac**:

  ```bash
  sudo apt-get install tesseract-ocr   # Linux
  brew install tesseract               # Mac
  ```

### 4. Download Vosk Model

* Download an English model from [Vosk Models](https://alphacephei.com/vosk/models).
* Update `model_path` in the code:

  ```python
  model_path = r'C:\\vosk-model\\vosk-model-en-us-0.22'
  ```

### 5. Run the App

```bash
python app.py
```

##  Technologies Used

* **Python** – Core programming language
* **Tkinter** – GUI framework
* **Pillow + Tesseract OCR** – Image text extraction
* **Vosk** – Offline speech recognition
* **Google Generative AI (Gemini)** – Fake news analysis
