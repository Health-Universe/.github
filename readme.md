# 15 Second Quick-Start

This quick-start will guide you through packaging your python app with Streamlit and deploying it to Health Universe, the open-source health research cloud for ML/AI.

## Prerequisites

- An idea for a health application you'd like to create
- Light familiarity with Streamlit
- A GitHub account and a Health Universe account

## Step 1: Create a GitHub repository

1. Create a new (public) repository on GitHub to host your project.
- Repo is public
- Repo has a readme.md
- Use the "python" .gitignore template (to ignore .env)

2. Clone the repository to your local machine:
`git clone https://github.com/<your_account>/<your_repo_name>.git`

3. Change to your project directory:`cd <your_repo>`

4. Create a virtual environment using:
`python -m venv .env`

5. Activate your virtual environment with: 
`source .env/bin/activate`

6. Upgrade pip to make sure things go smoothly:
`python -m pip install --upgrade pip`

7. Install the streamlit library with:
`pip install streamlit`

# Step 2: Create your python app
In your local repository, create the following files:
- main.py: This file should contain your Python model.
- requirements.txt: This file will list your project dependencies.

Next, learn a little bit about how Streamlit works.
- Overview of the main concepts for creating UI with Streamlit.
- Here's a nifty cheat sheet for all the interface elements you can create.

### main.py
```
import streamlit as st

st.title("Welcome to Health Universe!")
st.write("This is a sample application.")

alarm_clock = st.slider('hour', 0, 23, 17) # min: 0h, max: 23h, default: 17h
st.header(alarm_clock) # print in large text
```

###requirements.txt
```streamlit
# Include any other libraries required by your app.
```

Test out your app by running it locally:
`streamlit run main.py`

## Step 3: Deploy to Health Universe
1. Push your local repo to GitHub.
2. Log in or create a Health Universe account if you haven't already.
3. Go to https://healthuniverse.com and navigate to "Apps."
4. Click "Add App" to create a new app.
5. Fill out the following fields:
- App Name: Name of your app
- Description: A brief description of your app
- Github Account: Your GitHub username
- Github Repo: The exact name of your GitHub repository
- Main File: The name of your python file (usually main.py)
6. Click "Add App" to deploy your app. This process may take a few minutes.

Once you've completed these steps, your app will be published on Health Universe!
### 🥳🥳🥳
