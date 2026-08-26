# 🌱 AgriSmart

### AI-Powered Smart Agriculture Decision Support System

AgriSmart is an AI-powered agriculture decision support system designed to help farmers make informed decisions by combining **crop disease detection, soil assessment, weather information, and personalized farming recommendations** in a single platform.

---

## 🎯 Project Overview

Farmers often need to make decisions related to crop health, soil condition, irrigation, fertilizers, pesticides, and weather. These tasks can become difficult when information is scattered across different sources.

**AgriSmart** aims to provide these capabilities through one integrated platform.

The system combines AI-based analysis with environmental and farm information to provide practical recommendations for crop management.

---

## 🚀 Key Features

### 🍃 Crop Disease Detection

* Upload a crop leaf image
* Analyze the image using an AI/CNN-based approach
* Identify potential crop diseases
* Display the predicted disease and relevant information

### 🧪 Soil Assessment

* Upload a soil laboratory report
* Extract important soil information using OCR
* Support soil image-based assessment
* Collect additional field information through a questionnaire
* Analyze soil health indicators

### 🌦️ Weather Forecasting

* Integrate weather forecast data
* Display relevant environmental conditions
* Provide weather-related farming information
* Support weather-aware recommendations

### 🌱 Fertilizer Recommendation

Generate fertilizer recommendations using available soil and crop information.

### 💧 Irrigation Recommendation

Provide irrigation guidance based on crop and environmental conditions.

### 🐛 Pesticide Recommendation

Provide crop-health-related pesticide recommendations based on detected problems and available crop information.

### 📊 Crop Health Dashboard

The dashboard brings important information together, including:

* Disease status
* Soil condition
* Weather information
* Recommendations
* Previous reports
* Crop health information

### 📋 Reports & History

Users can view previous assessments and recommendation history.

---

## 🏗️ System Workflow

```text
                    👨‍🌾 Farmer
                       │
                       ▼
                Registration/Login
                       │
                       ▼
                  Select Crop
                       │
          ┌────────────┴────────────┐
          │                         │
          ▼                         ▼
   Upload Leaf Image          Soil Assessment
          │                    ┌──────┴──────┐
          ▼                    │             │
   Disease Detection      Soil Report    Soil Image
          │                    │             │
          ▼                    ▼             ▼
 Disease Prediction         OCR       AI Soil Assessment
          │                    │             │
          └────────────┬───────┴─────────────┘
                       │
                       ▼
                Weather Forecast
                       │
                       ▼
              Recommendation Engine
                       │
          ┌────────────┼────────────┐
          ▼            ▼            ▼
      Fertilizer   Irrigation   Pesticide
     Recommendation Recommendation Recommendation
          │            │            │
          └────────────┴────────────┘
                       │
                       ▼
                Crop Health Dashboard
                       │
                       ▼
              Recommendation History
```

---

## 🛠️ Technologies Used

### Frontend

* React
* JavaScript
* HTML5
* CSS3
* Vite
* Tailwind CSS

### AI / Machine Learning

* Python
* Machine Learning
* Convolutional Neural Networks (CNN)
* Computer Vision
* Image Processing

### APIs & Services

* REST APIs
* Weather API
* OCR-based data extraction

### Development Tools

* Git
* GitHub
* VS Code

---

## 📁 Project Structure

```text
agri-smart/
│
├── src/
│   ├── components/
│   │   ├── AppLayout.jsx
│   │   ├── Brand.jsx
│   │   ├── NotificationMenu.jsx
│   │   ├── Page.jsx
│   │   └── StatCard.jsx
│   │
│   ├── pages/
│   │   ├── Dashboard.jsx
│   │   ├── Disease.jsx
│   │   ├── Landing.jsx
│   │   ├── Login.jsx
│   │   ├── Profile.jsx
│   │   ├── Reports.jsx
│   │   ├── Schemes.jsx
│   │   ├── Settings.jsx
│   │   ├── Signup.jsx
│   │   ├── Soil.jsx
│   │   ├── Tasks.jsx
│   │   └── Weather.jsx
│   │
│   ├── lib/
│   │   ├── api.js
│   │   └── storage.js
│   │
│   ├── App.jsx
│   ├── index.css
│   └── main.jsx
│
├── .env.example
├── .gitignore
├── index.html
├── package.json
├── package-lock.json
├── vite.config.js
└── README.md
```

---

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/shahida-ansari/agri-smart.git
```

### 2. Navigate to the project

```bash
cd agri-smart
```

### 3. Install dependencies

```bash
npm install
```

### 4. Configure environment variables

Create a `.env` file based on `.env.example`.

```text
VITE_API_URL=your_api_url
VITE_WEATHER_API_KEY=your_api_key
```

> ⚠️ Never commit real API keys or passwords to GitHub.

### 5. Start the development server

```bash
npm run dev
```

The application will then be available through the local development URL provided by Vite.

---

## 📸 Screenshots

Screenshots of the application will be added here.

### Landing Page

*Add screenshot here*

### Dashboard

*Add screenshot here*

### Disease Detection

*Add screenshot here*

### Soil Assessment

*Add screenshot here*

### Weather

*Add screenshot here*

---

## 🎯 Project Objectives

1. Develop an AI-based crop disease detection system using leaf images.
2. Develop a soil health assessment module using soil information, images, questionnaires, and optional OCR-based soil report extraction.
3. Integrate weather forecasting to evaluate environmental conditions affecting crop health.
4. Develop personalized fertilizer, irrigation, and pesticide recommendations.
5. Provide a crop health dashboard for monitoring disease, soil, weather, and recommendation history.

---

## 🔮 Future Scope

* Support additional crops and diseases
* Improve AI model accuracy using larger datasets
* Add multilingual support
* Add mobile application support
* Integrate IoT-based soil and environmental sensors
* Improve personalized recommendation models
* Add real-time farm monitoring
* Integrate additional agricultural datasets

---

## 👥 Project

**Project:** AgriSmart
**Domain:** Artificial Intelligence · Machine Learning · Smart Agriculture
**Development:** Academic / Final-Year Project

---

## 📄 License

This project is developed for academic and educational purposes.
