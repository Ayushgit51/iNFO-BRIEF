# Text Summarizer App

A FastAPI-based web application that generates concise summaries from long text using a fine-tuned T5 Transformer model.

---

## Features

* Summarizes long text into short, meaningful output  
* Built using FastAPI for high performance  
* Uses Hugging Face Transformers (T5 model)  
* Simple frontend using HTML  
* Clean and modular backend  

---

## Tech Stack

* FastAPI  
* Python  
* PyTorch  
* Hugging Face Transformers  
* HTML  

---

## Project Structure

```
TeXtSuMmArIzErApP/
│── app.py
│── index.html
│── requirements.txt
│── README.md
│── .gitignore
```

---

## Model Information

The trained model is not included in this repository due to GitHub file size limitations.

Download the model from the link below:

https://drive.google.com/drive/folders/1tktIeTsECQFPpubPpae0PxGBHM0qmKZp?usp=sharing

---

## Setup Instructions

### 1. Clone the repository

```
git clone https://github.com/Ayushgit51/iNFO-BRIEF.git
cd iNFO-BRIEF
```

---

### 2. Download the model

* Open the Google Drive link  
* Download the folder named `save_summary_model`  
* Place it inside the root project directory  

Final structure should look like:

```
TeXtSuMmArIzErApP/
│── app.py
│── index.html
│── save_summary_model/
│     ├── config.json
│     ├── tokenizer_config.json
│     ├── tokenizer.json
│     ├── generation_config.json
│     ├── model.safetensors
```

---

### 3. Install dependencies

```
pip install -r requirements.txt
```

---

### 4. Run the application

```
uvicorn app:app --reload
```

---

### 5. Open in browser

```
http://127.0.0.1:8000
```

---

## API Usage

### Endpoint

```
POST /summarize/
```

### Request Body

```
{
  "dialogue": "Your long text here..."
}
```

### Response

```
{
  "summary": "Generated summary text"
}
```

---

## Notes

* Ensure the model folder name is exactly `save_summary_model`  
* Do not modify internal model files  
* Application will not run if the model is missing  

---

## .gitignore (Important)

Make sure this is included:

```
save_summary_model/
```

---

## Future Improvements

* Add authentication system  
* Improve UI/UX  
* Deploy on cloud (Render / Railway)  
* Add support for multiple languages  

---

## Author

Ayush Kumar
