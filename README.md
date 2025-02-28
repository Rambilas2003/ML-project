# ML-project

 Installation

Install Dependencies

pip install -r requirements.txt

🔹 Training the Models

(Only required for first-time setup)

This will train and save models in the models/ directory.

🔹 Predict a Song (CLI Mode)

Example Input:

Enter a song lyric snippet: "I've got sunshine on a cloudy day"

Output:

TensorFlow Identified Song ID: 42
PyTorch Identified Song ID: 42

🔹 Run the API Server

python app.py

The Flask API will start on http://127.0.0.1:5000

🔹 API Usage (Postman / Curl)

Send a POST request with a JSON payload containing the text snippet.

curl -X POST http://127.0.0.1:5000/predict \
     -H "Content-Type: application/json" \
     -d '{"text": "I've got sunshine on a cloudy day"}'

Example Response:
{
  "TensorFlow": "My Girl - The Temptations",
  "PyTorch": "My Girl - The Temptations"
}
