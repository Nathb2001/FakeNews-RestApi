# Fake News Detection API

This is a RESTful API built with FastAPI that classifies news articles as real or fake using a Logistic Regression model. The model was trained on a dataset containing 76,353 examples of real and fake news articles.

## Overview

This project originated as an MSc project for building an application to detect fake news. Initially designed with FastAPI, it has since been deprecated in favor of integrating the functionality into the Streamlit framework.

## Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/Nathb2001/FakeNews-RestApi.git
   cd your-repo
2. **Download the dataset:**

Download the dataset from Google Drive and place it in the project folder.

Install the required dependencies:

```bash
pip install -r requirements.txt
```
3. **Start the FastAPI server:**


```bash

uvicorn main:app --reload
```
**Access the Swagger UI:**

Open your web browser and go to http://localhost:8000/docs to interactively test the API endpoints.

**API Endpoints**

POST /classify/

Endpoint to classify news articles. Send a JSON payload with the news content.

**Example request body:**



```
{
  "news_text": "Here is the news article content..."
}
```

**Example response:**


```
{
  "prediction": "REAL! We predicted that the probability this News article is Real is 76 percent"
}
```
**Contributing**
Contributions are welcome! If you'd like to contribute to this project, please fork the repository and create a pull request.

**License**
This project is licensed under the MIT License - see the LICENSE file for details.
