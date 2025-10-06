🍴 Restaurant Name Generator (LangChain + Streamlit)

This is an AI-powered web app that generates a creative restaurant name and a list of menu items based on a selected cuisine.
It uses LangChain to connect multiple LLM chains and Streamlit for an interactive user interface.

🚀 Features

✅ Choose from multiple cuisines (Indian, Italian, Mexican, etc.)
✅ AI suggests a catchy restaurant name
✅ Automatically generates menu items for that restaurant
✅ Simple and intuitive Streamlit interface
✅ Modular structure with LangChain helper functions

🏗️ Project Structure
project/
├── app.py                 # Streamlit frontend
├── langchain_helper.py    # LangChain logic (chains + prompts)
├── requirements.txt        # Python dependencies
└── README.md              # Project documentation

🧠 How It Works

The user selects a cuisine from the sidebar.

LangChain creates a Sequential Chain:

Chain 1: Generates a restaurant name for the chosen cuisine.

Chain 2: Generates menu items for that restaurant.

The results are displayed in the Streamlit app.

The data automatically flows from one chain to another, showing how SequentialChain connects multiple LLM prompts in a workflow.

⚙️ Installation and Setup
1. Clone this repository
git clone https://github.com/yourusername/restaurant-name-generator.git
cd restaurant-name-generator

2. Create a virtual environment (optional but recommended)
python -m venv venv
source venv/bin/activate      # For Mac/Linux
venv\Scripts\activate         # For Windows

3. Install dependencies
pip install -r requirements.txt

4. Set your OpenAI API Key

Create a file named .env or set the environment variable manually:

export OPENAI_API_KEY="your_api_key_here"


On Windows (PowerShell):

setx OPENAI_API_KEY "your_api_key_here"

▶️ Run the App
streamlit run app.py


Then open the link shown in your terminal (usually http://localhost:8501).

🧩 Example Output

Cuisine: Italian
Generated Restaurant Name: La Dolce Vita Diner
Menu Items:

Margherita Pizza

Penne Arrabbiata

Tiramisu

Bruschetta

🛠️ Tech Stack

Python 3.10+

LangChain (for LLM-based chains)

OpenAI API (for text generation)

Streamlit (for frontend UI)

📦 requirements.txt
streamlit
langchain
openai
python-dotenv

💡 Future Enhancements

Add more cuisines dynamically

Allow user to enter custom cuisine types

Display restaurant logo (AI-generated image)

Add download option for menu

👨‍💻 Author

Prince Keshri
💼 AI & Software Developer
🔗 LinkedIn
 | GitHub
