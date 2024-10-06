# Chat-with-PDF-Document-using-GenAI

A Streamlit app that allows users to upload PDF files and ask questions about the content using Google’s Generative AI. The system extracts text from PDFs, creates embeddings, and performs similarity searches using FAISS to deliver detailed answers based on PDF context.

## Features:
• Upload multiple PDF files.

• Extract and split PDF text into chunks.

• Build FAISS vector storage for efficient similarity search.

• Query the PDF content with AI-powered Q&A functionality.

• Responsive web app with user-friendly interface.

## Project Structure:
📂 Chat-with-PDF-Document-using-GenAI

│

├── 📄 requirements.txt       # Python dependencies

├── 📄 app.py                 # Streamlit application file

├── 📄 config.py              # Core logic for PDF processing & embedding

├── 📄 .env                   # API key configuration

├── 📂 faiss_index/           # Stores FAISS index files (index.faiss, index.pkl)

├── 🖼 logo.jpg               # Logo for app's UI

## Installation & Setup:
### 1. Clone the repository:
  ``` git clone https://github.com/your-repo/Chat-with-PDF-Document-using-GenAI.git  ```
  
  ``` cd Chat-with-PDF-Document-using-GenAI   ```

### 2. Install dependencies:
  ``` pip install -r requirements.txt  ```

### 3. Set up environment variables:

• Create a .env file and add your Google API Key:

  ``` GOOGLE_API_KEY = "Your_Google_API_Key   ```

### 3. Run the app:   

``` streamlit run app.py  ```

## AWS EC2 Deployment:

### 1. Connect to EC2 instance:

• Use SSH to connect to the EC2 instance.  

```ssh -i "key_pdf_app.pem" ec2-user@13.60.243.154  ```

### 2. Transfer project files to EC2:

• Copy all files from your local machine to the EC2 instance:   

```scp -i "key_pdf_app.pem" -r ./Chat-with-PDF-Document-using-GenAI ec2-user@13.60.243.154:~/.  ```

### 3. Install required packages on EC2:   

``` sudo yum update -y   ```   
``` sudo yum install python3 -y   ```   
```pip3 install -r requirements.txt  ```

### 4. Run the app on EC2:  

``` streamlit run app.py   ```

### 5. Access the app:

Open the EC2 public IPv4 DNS in your browser:    ``` http://13.60.243.154:8501/   ```

## Example UI Deployment:
![UI Deployment](https://github.com/Kaushik-Puttaswamy/Chat-with-PDF-Document-using-GenAI/blob/main/UI%20Deployment.png)


##### Contact:
For further assistance, feel free to contact:   ``` https://www.linkedin.com/in/kaushik-puttaswamy-317475148/   ```






