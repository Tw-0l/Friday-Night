# Friday Night

![Friday Night](https://img.shields.io/badge/Friday-Night-purple?style=for-the-badge)
![Entertainment](https://img.shields.io/badge/Entertainment-Recommender-blue?style=for-the-badge)
![Streamlit](https://img.shields.io/badge/Streamlit-App-red?style=for-the-badge)

## 🌙 Project Overview
Friday Night is an intelligent entertainment recommendation system designed specifically for weekend relaxation. This Streamlit application helps users discover personalized movie, music, restaurant, and activity suggestions for the perfect Friday night experience, based on their preferences, mood, and social context.

## ✨ Live Demo
Explore the live demo: [Friday Night App](https://friday-night.streamlit.app/)

![Friday Night Demo](https://raw.githubusercontent.com/Tw-0l/Friday-Night/main/images/app_screenshot.png)

## 🎯 Key Features

### 🎬 Personalized Entertainment Recommendations
- **Movies & Shows**: Curated suggestions from popular streaming platforms
- **Music & Playlists**: Mood-based music recommendations
- **Dining Options**: Restaurant recommendations based on cuisine preferences
- **Activities**: Local events and activities matching your interests

### 🧠 Intelligent Recommendation Engine
- Preference learning from user interactions
- Contextual awareness (weather, time, location)
- Social recommendation features for groups
- Mood-based suggestion calibration

### 📱 User Experience
- Clean, intuitive Streamlit interface
- Interactive elements for preference selection
- Visual representation of recommendations
- Mobile-friendly design

## 🛠️ Technologies Used

### Core Technologies
- **Streamlit**: Web application framework
- **Python**: Backend programming
- **Pandas**: Data manipulation and analysis
- **Scikit-learn**: Machine learning algorithms

### Data Sources
- Movie and TV show databases
- Music streaming APIs
- Restaurant and dining information
- Local event listings

## 📊 App Structure
```
Friday-Night/
├── app.py                      # Main Streamlit application
├── pages/
│   ├── home.py                 # Home page interface
│   ├── movies.py               # Movie recommendations
│   ├── music.py                # Music recommendations
│   ├── dining.py               # Restaurant suggestions
│   └── activities.py           # Activity recommendations
├── utils/
│   ├── recommendation.py       # Recommendation algorithms
│   ├── data_processing.py      # Data cleaning and preparation
│   ├── visualization.py        # Data visualization functions
│   └── user_preferences.py     # User preference management
├── data/
│   ├── movies.csv              # Movie dataset
│   ├── music.csv               # Music dataset
│   ├── restaurants.csv         # Restaurant information
│   └── events.csv              # Local activities data
├── assets/
│   ├── images/                 # App images and icons
│   └── styles/                 # CSS customization
├── requirements.txt            # Project dependencies
└── README.md                   # Project documentation
```

## 🚀 Getting Started

### Prerequisites
- Python 3.8+
- Pip package manager

### Local Installation
```bash
# Clone the repository
git clone https://github.com/Tw-0l/Friday-Night.git
cd Friday-Night

# Create and activate virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run the Streamlit app
streamlit run app.py
```

## 💻 Usage Guide

### 1. Start Your Friday Night Journey
Open the app and navigate through the clean interface to start discovering personalized recommendations for your perfect Friday night.

![Home Screen](https://raw.githubusercontent.com/Tw-0l/Friday-Night/main/images/home_screen.png)

### 2. Set Your Preferences
Select your mood, interests, and preferences to receive tailored recommendations:

```python
# Example preference selection in the app
mood = st.selectbox(
    'How are you feeling tonight?',
    ['Relaxed', 'Energetic', 'Romantic', 'Social', 'Adventurous', 'Thoughtful']
)

group_size = st.slider('How many people are joining?', 1, 10, 2)

interests = st.multiselect(
    'Select your interests:',
    ['Movies', 'Music', 'Food', 'Outdoor Activities', 'Indoor Activities', 'Arts & Culture']
)
```

### 3. Explore Recommendations
Browse through personalized suggestions across different categories:

![Recommendations Screen](https://raw.githubusercontent.com/Tw-0l/Friday-Night/main/images/recommendations_screen.png)

## 🌟 Features in Detail

### Mood-Based Recommendations
The app provides different recommendations based on your mood:
- **Relaxed**: Calm movies, mellow music, comfortable dining
- **Energetic**: Action films, upbeat music, lively venues
- **Romantic**: Love stories, smooth jazz, intimate restaurants
- **Social**: Comedies, popular hits, group-friendly locations
- **Adventurous**: Thrillers, world music, exotic cuisine
- **Thoughtful**: Documentaries, classical music, quiet cafés

### Interactive Visualization
Explore trends and patterns in entertainment preferences through interactive charts:

```python
# Example visualization in the app
import plotly.express as px

fig = px.bar(
    genre_data, 
    x='Genre', 
    y='Popularity', 
    color='Mood',
    title='Popular Genres by Mood'
)
st.plotly_chart(fig)
```

## 📈 Roadmap
- **Feature Enhancement**: Adding more recommendation categories
- **User Profiles**: Saving preferences for returning users
- **Social Integration**: Sharing recommendations with friends
- **Location Awareness**: Geo-specific suggestions
- **API Integration**: Connecting with entertainment platforms

  
## 👥 Team
We're a passionate team of developers committed to enhancing your weekend experience:

- **Abdullah Altuwayjiri** - [@Tw-0l](https://github.com/Tw-0l)
- **Ahmed Alhassan**
- **Faisal Alossaimi**
- **Mohammed Alaklabi**

## 🤝 Contributing
Contributions are welcome! Please feel free to submit a Pull Request or open an Issue to suggest improvements or report bugs.

### Development Workflow
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request



## 📞 Contact
- GitHub: [@Tw-0l](https://github.com/Tw-0l)
- Demo: [Friday Night App](https://friday-night.streamlit.app/)

---

*Friday Night - Turning decision fatigue into discovery joy, one weekend at a time.*
