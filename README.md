This is a RESTful API built with FastAPI that classifies news articles as real or fake using a Logistic Regression model. The model was trained on a dataset containing 76,353 examples of real and fake news articles.

Overview
This project originated as an MSc project for building an application to detect fake news. Initially designed with FastAPI, it has since been deprecated in favor of integrating the functionality into the Streamlit framework.

Installation
Clone the repository:

bash
Copy code
git clone https://github.com/Nathb2001/FakeNews-RestApi.git
cd your-repo
Download the dataset from Google Drive and place it in the project folder.

Install the required dependencies:

bash
Copy code
pip install -r requirements.txt
Usage
Start the FastAPI server:

bash
Copy code
uvicorn main:app --reload
Open your web browser and go to http://localhost:8000/docs to access the Swagger UI. Here, you can test the API endpoints interactively.

API Endpoints
POST /classify/: Endpoint to classify news articles. Send a JSON payload with the news content.

Example request body:

json
Copy code
{
  "news_text": "Here is the news article content..."
}
Example response:

json
Copy code
{
  "prediction": "real"
}
Contributing
Contributions are welcome! If you'd like to contribute to this project, please fork the repository and create a pull request.

License
This project is licensed under the MIT License - see the LICENSE file for details.


