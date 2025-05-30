
<a >
<img src="https://github.com/user-attachments/assets/d3b47e75-a198-4058-b141-0b5a84a410ab" alt="Carbon Footprint Tracker" width="1000"/>
</a>

## 🌿 AI-Powered Carbon Footprint Tracker
Category: [Choose relevant category: e.g., AI for Sustainability / Climate Action]

#### 🔍 Relevance :
With global carbon emissions exceeding 40 billion tons annually, individual lifestyle choices significantly impact climate change. However, most individuals lack personalized tools to assess and reduce their carbon footprint. This project addresses the gap by leveraging AI to empower users with actionable insights into their environmental impact.

## 🤖 Our AI-Powered Solution
A visually appealing and interactive Streamlit web app  enhanced by machine learning algorithms, that analyzes users’ habits to estimate carbon footprint based on lifestyle choices — covering areas like diet, travel, energy consumption, waste, and shopping behavior. This tool helps raise awareness and encourages more sustainable habits, with provides tailored recommendations to minimize their carbon impact.


#### ✨ Key Features & Functionality

1.AI-Powered Analysis:-
Uses scikit-learn to identify patterns in energy usage and consumption behaviors.
Predicts personalized CO₂ impact using historical and user-provided data.
Uses a trained MLP Regressor (Neural Network) to predict your monthly CO₂ emissions.

2.Streamlit Interface:-
Clean, multi-tab UI built with Streamlit, featuring custom styling with a dynamic background, icons, and embedded CSS/JavaScript for a polished and enhanced user experience.

3.Visual Insights:-
Dynamic graphs using Matplotlib to display monthly footprint.
Visual summaries of progress and areas for improvement.


4.Offset Integration:-
Tree Offset Estimation and calculates how many trees you'd need to plant to offset your emissions.
Connects users to reforestation initiatives for carbon offsetting via donations.

## 🛠️ Tech Stack

Frontend: Streamlit

Backend & ML:
      scikit-learn for MLPRegressor model
      pickle for model and scaler persistence

Visualization: matplotlib, PIL

Data Processing: pandas, numpy

Custom Styling: CSS + JavaScript + Base64 encoding

Others: Modular architecture via functions.py

## 📦 Folder Structure
.
├── app.py                 # Main Streamlit application

├── functions.py           # Preprocessing, chart rendering, etc.

├── models/
│   ├── model.sav          # Trained MLPRegressor model
│   └── scale.sav          # StandardScaler instance

├── style/
│   ├── style.css          # Custom styles
│   ├── scripts.js         # Interactive JS
│   ├── main.md            # Intro content for homepage tab
│   └── footer.html        # Footer content

├── media/
│   ├── background_min.jpg # Background image (base64-encoded)
│   ├── icon2.png          # Icon for styling
│   ├── icon3.png          # Icon for styling

└── README.md              # Project documentation

## 🧪 How It Works
User Input: You provide details across multiple categories using interactive widgets.

Preprocessing: Inputs are transformed and encoded into a suitable format using input_preprocessing() from functions.py.

Prediction: A pre-trained neural network model estimates your carbon footprint.

Visualization: Your result is shown graphically and translated into the number of trees needed to offset your emissions.

## 🛠️ Setup Instructions
Prerequisites:-
Python 3.7+
Streamlit (pip install streamlit)

Other dependencies:-
pandas, numpy, matplotlib, scikit-learn, Pillow

To Run the App :-
git clone https://github.com/your-username/carbon-footprint-calculator.git

cd carbon-footprint-calculator

streamlit run app.py

## 📌 Notes
Make sure your functions.py contains the input_preprocessing() and chart() functions.

Ensure media files and models are in the correct directories.

The app is optimized for widescreen desktop displays.

#### 📚 Learn More
Want to know how your habits impact the planet? Click the "Did You Know?" popup inside the app for climate facts and insights.



