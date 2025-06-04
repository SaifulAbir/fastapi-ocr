# 🧾 FastAPI OCR API

A simple Optical Character Recognition (OCR) API built with FastAPI and Python. This project allows users to upload image files and receive extracted text in response using `pytesseract`, a wrapper for Google's Tesseract OCR engine.

---

## 🚀 Features

- Upload image files (PNG, JPG, etc.)
- Perform OCR on uploaded files
- Return extracted text in JSON response
- Lightweight, fast, and easy to deploy

---

## 🛠️ Technologies Used

- **FastAPI** – for API creation
- **pytesseract** – for OCR processing
- **Tesseract-OCR** – backend OCR engine (installed separately)
- **Uvicorn** – for running the FastAPI server

---

## 📦 Installation

### 1. Clone the repository

```bash
git clone https://github.com/SaifulAbir/fastapi-ocr.git
cd fastapi-ocr
```

### 2. Create and activate a virtual environment

```bash
python -m venv venv
source venv/bin/activate     # On Windows: venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Install Tesseract-OCR

- **Ubuntu**:
  ```bash
  sudo apt update && sudo apt install tesseract-ocr
  ```

- **macOS**:
  ```bash
  brew install tesseract
  ```

- **Windows**:  
  Download from [Tesseract GitHub](https://github.com/UB-Mannheim/tesseract/wiki)

---

## ▶️ Running the App

```bash
uvicorn main:app --reload
```

Then open your browser to:

> 📍 http://127.0.0.1:8000/docs

Use the Swagger UI to upload an image and test the OCR.

---

## 📝 API Usage

### `POST /ocr`

Upload an image file and get back the extracted text.

#### Request (multipart/form-data):

- `image`: an image file (JPG, PNG, etc.)

#### Example Response:

```json
{
  "Extracted text from the image."
}
```

---

## 💡 What I Learned

- How to build and run APIs using FastAPI
- How to integrate third-party libraries like `pytesseract`
- How OCR works and how to expose it via an API
- The role of FastAPI in the frontend-backend communication layer

---

## 📄 License

MIT License – free to use and modify.

---

## 👤 Author

**Saiful Islam**  
[GitHub – SaifulAbir](https://github.com/SaifulAbir)  
[LinkedIn – saifulislamcse](https://www.linkedin.com/in/saifulislamcse)
