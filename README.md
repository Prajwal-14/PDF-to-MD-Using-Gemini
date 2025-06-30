## PDF to Markdown Converter using Gemini API

This project is a Python-based PDF to Markdown converter that utilizes the Gemini API to extract and convert content from PDF documents into clean, structured Markdown format.

## Features

Select and convert multiple PDF files

Uses Google's Gemini 1.5 API for accurate text extraction and formatting

Automatically saves Markdown files to a dedicated folder

Command-line interface with user-friendly prompts

## Technologies Used

Python 3.11

Gemini API (Google Generative AI)

PyMuPDF (fitz) for reading PDF

InquirerPy for command-line interaction

## Installation & Setup

1. Clone the repository

git clone (https://github.com/Prajwal-14/PDF-to-MD-Using-Gemini)

2. Create a virtual environment

python -m venv .venv
.venv\Scripts\activate  # for Windows

3. Install dependencies

pip install -r requirements.txt

4. Set up Gemini API key

Create a .env file in the root folder and add your Gemini API key:

GOOGLE_API_KEY=your_gemini_api_key_here

## How to Run

python main.py

Follow the on-screen prompts to choose the PDF file(s) you want to convert. Output Markdown files will be saved in the folder: PDF-to-MD-Using-Gemini_converted-md

## Key Learnings

Practical usage of Gemini API for document parsing

File I/O handling in Python

CLI interactivity with InquirerPy

Markdown formatting logic

## Author

Prajwal TalwareGitHub: github.com/PrajwalTalware

## License

This project is for educational/internship purposes and currently not licensed for production use.

## Live Demo

Not applicable for this CLI-based project.

## The stepwise process of how the application will work is:

1. New directory is created.
2. User will select files using inquirer.
3. The application will take those files and send them to gemini one by one.
4. The response is to be stored in a file with .md extension with same name as the .pdf file.
5. The .md files will be stored in the created directory.

## Things to keep in mind:

- _NO AI CODE SHALL BE USED._ Any plagarised or code given by LLMs can be detected. Anyone found using these tactics will be barred from receiving the completion certificate.
- _NO CODE SHARING_. Every intern must have their own unique code and project style. Same rules as above for violation of this rule.
- Any number of files can be created depending on the neccesity and use.
- Do not clutter the main.py file, try and create multiple files for different logic sections (Eg: converter.py handle the conversion using gemini, filesystem_update.py creates and updated directories and files in filesystem).
