MCQs Generator with LangChain

Overview

This project is an MCQ (Multiple Choice Questions) Generator application built with LangChain and Streamlit. It allows users to upload a PDF or text file, specify the number of MCQs, subject, and complexity level, and generate MCQs using OpenAI's API. The application can be run locally or deployed on AWS.

Features

Upload PDF or text files
Generate MCQs based on the uploaded content
Specify the number of MCQs, subject, and complexity level
Display generated MCQs in a tabular format
Installation

->Prerequisites
Python 3.12 or later
Git
Streamlit
OpenAI API key
AWS account (for cloud deployment)
Local Setup

->Clone the Repository
git clone https://github.com/Priyamshah05/MCQsGenerator.git
cd MCQsGenerator

->Create and Activate a Virtual Environment
python -m venv myenv
source myenv/bin/activate  # On Windows, use `myenv\Scripts\activate`

->Install Dependencies
pip install -r requirements.txt

->Set Up Environment Variables
Create a .env file in the project root and add your OpenAI API key:
makefile
OPENAI_API_KEY=your_openai_api_key

->Run the Application
streamlit run StreamlitAPP.py

->Access the Application
Open your browser and go to http://localhost:8501.


AWS Cloud Deployment

Set Up an AWS EC2 Instance
Launch an EC2 instance with Ubuntu 24.04 LTS.
Connect to your instance via SSH.


->Install Required Packages
sudo apt update
sudo apt install git curl unzip -y

->Clone the Repository
git clone https://github.com/Priyamshah05/MCQsGenerator.git
cd MCQsGenerator

->Create and Activate a Virtual Environment
python3 -m venv myenv
source myenv/bin/activate

->Install Dependencies
pip install -r requirements.txt

->Set Up Environment Variables
Create a .env file in the project root and add your OpenAI API key:
makefile
OPENAI_API_KEY=your_openai_api_key

->Run the Application
streamlit run StreamlitAPP.py --server.port 8501 --server.enableCORS false

->Access the Application
Open your browser and go to http://<your-ec2-public-ip>:8501.

Usage

Upload a PDF or text file.
Specify the number of MCQs, subject, and complexity level.
Click on "Create MCQs" to generate the questions.
View the generated MCQs in the table.

Contributions are welcome! Please open an issue or submit a pull request for any changes or improvements.

License

This project is licensed under the MIT License. See the LICENSE file for details.

Acknowledgments

Streamlit
LangChain
OpenAI