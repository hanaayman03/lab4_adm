# lab4_adm
# Weather and Calculation Assistant

## Setup Instructions

### Prerequisites
Make sure you have the following installed:
- Python 3.8+
- `pip` package manager
- `virtualenv` (optional, but recommended)

### 1. Clone the Repository
```sh
git clone <repository_url>
cd <repository_directory>
```

### 2. Create and Activate Virtual Environment (Optional but Recommended)
```sh
python -m venv venv
# On Windows
venv\Scripts\activate
# On macOS/Linux
source venv/bin/activate
```

### 3. Install Dependencies
```sh
pip install -r requirements.txt
```

### 4. Set Up Environment Variables
Create a `.env` file in the project directory and add the following:
```ini
API_KEY=<your_openai_api_key>
WEATHER_API_KEY=<your_weatherapi_key>
BASE_URL=<openai_base_url>
LLM_MODEL=<your_model_name>
```

### 5. Run the Application
```sh
python main.py
```

## Features
- Fetch current weather data for any location
- Retrieve weather forecasts for up to 3 days
- Perform mathematical calculations using an evaluation tool
- Simulated web search for predefined queries
- Supports Chain of Thought (CoT) and ReAct reasoning for better responses

## Usage
After running the application, you can interact with the assistant by typing queries related to weather, calculations, or web searches.

Example queries:
```
What is the weather like in Cairo today?
What is 25 * 4 + 10?
Tell me about climate change.
```

Type `exit` to end the conversation.

## Notes
- The application relies on OpenAI and WeatherAPI services, so ensure you have valid API keys.
- The `eval()` function is used for calculations. This is safe for basic use but should be sandboxed in production environments.

## License
This project is licensed under the MIT License.

