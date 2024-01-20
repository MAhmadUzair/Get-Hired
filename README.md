# **Get Hired - Resume Evaluation App**

## **Introduction**
Welcome to the "Get Hired" app - a tool designed to enhance your job application success! This Streamlit application leverages the Google Generative AI model (specifically, the Gemini Pro Vision) to provide insights and feedback on your resume in relation to a given job description.

## **Setup**

### **Prerequisites**
- Python 3.x
- [Streamlit](https://www.streamlit.io/)
- [dotenv](https://pypi.org/project/python-dotenv/)
- [base64](https://docs.python.org/3/library/base64.html)
- [Pillow (PIL)](https://pillow.readthedocs.io/)
- [pdf2image](https://pypi.org/project/pdf2image/)
- [Google Generative AI](https://github.com/googleapis/python-generators)

### **Installation**
Make sure to install the required Python packages by running:
```bash
pip install -r requirements.txt
Usage
Run the App:

bash
Copy code
streamlit run your_file_name.py
Input Job Details:

Provide the job description in the text area labeled "Job Description."
Upload your resume in PDF format using the file uploader.
Choose Action:

Five buttons are provided to perform different actions based on the uploaded resume:
"Tell Me About the Resume"
"How Can I Improve my Skills"
"Percentage Match"
"What I Lack?"
"Should I Apply for This Job"
View Responses:

The app will generate responses based on the chosen action and display them under the respective subheader.
Functionality Overview
get_gemini_response(input, pdf_content, prompt)
This function interacts with the Google Generative AI model (Gemini Pro Vision) to generate responses based on the given input, PDF content, and prompt.

input_pdf_setup(uploaded_file)
This function converts the uploaded PDF resume into an image and prepares it for further processing.

Streamlit App
The Streamlit app consists of input fields for job description and resume upload.
Action buttons trigger specific evaluations using the Gemini Pro Vision model.
Responses are displayed under the respective subheaders based on the selected action.
Notes
Ensure you have a valid Google API key stored in a .env file for authentication.
The app utilizes Streamlit for the user interface and Google Generative AI for content generation.
Feel free to explore and customize the app for your specific needs! If you encounter any issues, refer to the documentation of the used libraries or contact the developer for assistance.
