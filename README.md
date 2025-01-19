# UI to HTML Code using Gemini

This Streamlit app allows you to upload an image of a UI design, and the app will generate the corresponding HTML code based on the image description. The app uses the Google Gemini model to generate the UI description and HTML code.

## Features
- **Upload Image:** Upload an image (JPG, JPEG, PNG) of the UI design.
- **Generate UI Description:** The app analyzes the image and generates a detailed description of the UI elements, including names, bounding boxes, and colors.
- **Refine Description:** The description is refined by comparing it with the uploaded image for accuracy.
- **Generate HTML Code:** Based on the refined description, the app generates an HTML file with inline CSS that matches the original UI.
- **Download HTML:** The generated HTML file can be downloaded for use.

## Requirements
- `streamlit`
- `pathlib`
- `PIL`
- `google-generativeai`
- `os`

## How it works
1. **Google API Key:** The app uses a Google API key for generating responses. The key must be set in the environment variables.
2. **Model Configuration:** The app uses the "gemini-1.5-pro-latest" model from Google Generative AI for generating UI descriptions and HTML code.
3. **Image Upload and Display:** The user uploads an image of a UI design, which is displayed in the app.
4. **UI Description Generation:** The app sends the image to the Gemini model for generating a description of the UI elements.
5. **HTML Code Generation:** The app creates HTML code based on the UI description and styles it using the specified CSS framework.
6. **Refining HTML:** The generated HTML is refined for accuracy and responsiveness.
7. **Download Link:** The final HTML code can be downloaded as an `index.html` file.

## Setup
1. Set the `GOOGLE_API_KEY` environment variable.
2. Run the Streamlit app:
