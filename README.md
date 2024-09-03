Multilanguage Invoice Extractor
Multilanguage Invoice Extractor is a Streamlit application designed to analyze and understand invoices in multiple languages. By leveraging Google's Gemini API, this app can process uploaded invoice images and answer questions based on the extracted content from these images.

Features
Image Upload: Allows users to upload invoice images in various formats such as JPG, JPEG, and PNG.
Invoice Analysis: Uses Google's Gemini model to analyze the uploaded invoice images and provide detailed responses based on the content.
Multilanguage Support: Capable of understanding invoices written in different languages, making it versatile for global use.
How It Works
User Input: The user provides an image of an invoice by uploading it through the Streamlit interface.
Processing: The uploaded image is processed and sent to the Gemini model, along with a prompt that guides the model to analyze the invoice.
Response Generation: The Gemini model generates a response based on the content of the invoice, which is then displayed to the user.
Installation
To run this project locally, follow these steps:

Clone the repository:

bash
Copy code
git clone https://github.com/ivats2911/multilanguage-invoice-extractor.git
Navigate to the project directory:

bash
Copy code
cd multilanguage-invoice-extractor
Install dependencies: Make sure you have Python installed, then run:

bash
Copy code
pip install -r requirements.txt
Set up the environment variables: Create a .env file in the root directory of the project and add your Google API key:

plaintext
Copy code
GOOGLE_API_KEY=your_google_api_key_here
Usage
To start the application, run:

bash
Copy code
streamlit run app.py
This will launch the Streamlit app in your default web browser.

Input Prompt: Enter any specific prompt or question you have regarding the invoice.
Upload Image: Upload an image of the invoice.
Submit: Click the "Tell me about the Invoice" button to process the image and receive an analysis.
Code Overview
Libraries Used:

streamlit: For creating the web interface.
PIL: For image handling.
dotenv: To manage environment variables.
google.generativeai: For accessing the Google Gemini API.
Core Functions:

get_gemini_response(input, image, prompt): Sends the input image and prompt to the Gemini model and returns the generated response.
input_image_setup(uploaded_file): Prepares the uploaded image file for processing by converting it into a format suitable for the Gemini API.
Customization
Feel free to customize the application according to your needs. You can modify the prompt provided to the Gemini model to refine the type of analysis or information you wish to extract from the invoices.

Contributing
Contributions are welcome! Please fork the repository and submit a pull request for any enhancements or bug fixes.
