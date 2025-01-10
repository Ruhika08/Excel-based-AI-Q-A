# AI-Powered XLSX Q&A

## 📋 Project Overview
This project is a **Streamlit-based application** that allows users to upload an Excel (`.xlsx`) file and ask questions about the data using **Google's Generative AI API (Gemini)**. The app extracts text from the uploaded file and uses the **Google Generative AI** to generate meaningful responses based on the user's questions.

---

## 🧰 Technologies Used
- **Python**
- **Streamlit**
- **Pandas**
- **Google Generative AI API (Gemini)**
- **dotenv**

---

## 📂 Project Structure
```
├── app.py             # Main application code
├── requirements.txt   # Python dependencies
├── .env               # Environment variables (API keys)
├── README.md          # Project documentation (this file)
├── .gitignore         # Files and directories to be ignored by Git
├── Dockerfile         # Docker configuration for deployment
```

---

## ⚙️ Installation & Setup
### 1️⃣ **Clone the Repository**
```bash
git clone <repository-url>
cd <repository-folder>
```

### 2️⃣ **Create a Virtual Environment**
```bash
python -m venv venv
```

### 3️⃣ **Activate the Virtual Environment**
- On **Windows**:
  ```bash
  venv\Scripts\activate
  ```
- On **Mac/Linux**:
  ```bash
  source venv/bin/activate
  ```

### 4️⃣ **Install Dependencies**
```bash
pip install -r requirements.txt
```

### 5️⃣ **Set Up the `.env` File**
Create a `.env` file in the root directory and add your **Gemini API key**:
```
GEMINI_API_KEY=your_google_api_key_here
```

---

## 🚀 Running the Application
```bash
streamlit run app.py
```
This will open the Streamlit app in your default web browser.

---

## 🛠 How It Works
1. **Upload an Excel File:**
   - Users can upload `.xlsx` files containing tabular data.
2. **Ask a Question:**
   - Enter a question related to the uploaded data.
3. **Get an Answer:**
   - The app uses the Google Generative AI API to provide an answer based on the data.

---

## 🧪 Example Usage
1. **Upload File:**
   - Example: `sales_data.xlsx`
2. **Ask a Question:**
   - "What was the total revenue in Q1?"
3. **Generated Answer:**
   - "The total revenue in Q1 was $500,000."

---

## 🛠 Troubleshooting
### Common Errors and Fixes:
- **Error: GEMINI_API_KEY not found**
  - Ensure the `.env` file is correctly set up with your API key.
- **Error: 404 Requested entity was not found**
  - Ensure you're using the correct model (e.g., `models/chat-bison-001`).
- **Error: 'GenerateContentResponse' object has no attribute 'result'**
  - Update your code to use `response.responses[0].text`.

---

## 📜 License
This project is licensed under the MIT License.

---

## Developed by Ruhika Joshi

---
