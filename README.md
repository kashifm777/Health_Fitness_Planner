# 🏋️‍♂️ Health & Fitness Plan Generator

This Streamlit application leverages the power of AI, specifically the `agno` library with Google's Gemini models, to generate personalized health and fitness plans. By providing some basic information about yourself, you can receive customized meal plans and workout routines tailored to your goals and preferences.

## ✨ Features

* **Personalized Meal Plans:** Generates dietary plans for breakfast, lunch, dinner, and snacks, considering your dietary preferences (Keto, Vegetarian, Low Carb, Balanced).
* **Customized Workout Routines:** Creates workout plans with warm-ups, main exercises, and cool-downs, adjusted to your fitness level (Beginner, Intermediate, Advanced) and fitness goals (Weight Loss, Muscle Gain, Endurance, Flexibility).
* **Holistic Health Strategy:** Combines the generated diet and fitness plans into a comprehensive health strategy for optimal results.
* **Web Search Integration:** Utilizes DuckDuckGo for the AI agents to fetch additional information if needed to create more informed plans.
* **User-Friendly Interface:** A simple and intuitive Streamlit interface for easy input and plan generation.

## 🚀 How to Use

1.  **Clone the Repository:**
    ```bash
    git clone https://github.com/kashifm777/Health_Fitness_Planner
    cd ai-health-fitness-plan
    ```
2.  **Install Dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
3.  **Set up Google API Key:**
    * Ensure you have a Google Cloud Project with the Generative AI API enabled.
    * Obtain an API key for the Generative AI service.
    * Create a `.env` file in the project root and add your API key:
        ```dotenv
        GOOGLE_API_KEY=YOUR_GOOGLE_API_KEY
        ```
4.  **Run the Streamlit App:**
    ```bash
    streamlit run main.py
    ```
5.  **Enter Your Information:** In the sidebar, provide your age, weight, height, activity level, dietary preference, and fitness goal.
6.  **Enter Your Name:** In the main section, enter your name for a personalized greeting.
7.  **Generate Your Plan:** Click the "Generate Health Plan" button.
8.  **View Your Personalized Plan:** The generated meal plan and workout routine, along with a holistic health strategy, will be displayed in the main area.

## ⚙️ Dependencies

* `streamlit`: For creating the web application interface.
* `agno`: An AI agent framework for building intelligent agents.
* `python-dotenv`: For loading environment variables (like the Google API key).
* `google-generativeai`: The official Google Generative AI library.

You can install all the necessary dependencies using the `requirements.txt` file.

## 💡 How It Works

This application utilizes the `agno` library to create three specialized AI agents:

1.  **Dietary Planner:** This agent focuses on generating personalized meal plans based on your dietary preferences and nutritional needs. It can also search the web for relevant dietary information.
2.  **Fitness Trainer:** This agent creates customized workout routines tailored to your fitness level and goals. It also provides safety tips and progress tracking suggestions.
3.  **Team Lead:** This agent orchestrates the dietary planner and fitness trainer, combining their outputs into a comprehensive health strategy. It ensures that the diet and workout plans are aligned to help you achieve your desired results.

The application uses Google's `gemini-2.0-flash-exp` model for the AI agents, providing fast and efficient responses.

## ➕ Further Enhancements

* Allow users to specify more detailed dietary restrictions and preferences.
* Incorporate more advanced fitness tracking and progress visualization.
* Add options for generating more specific types of workouts (e.g., strength training, cardio).
* Implement user accounts to save and manage personalized health plans.
* Integrate with wearable devices for real-time activity and sleep data.

## 🙏 Contributing

Contributions to this project are welcome! Feel free to submit pull requests with bug fixes, new features, or improvements.
