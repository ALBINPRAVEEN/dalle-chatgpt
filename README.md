# ✨ Streamlit based ChatGPT/DALLE-2
A simple streamlit based webapp using OpenAI APIs empowered with text generation and image generation functionalities


## Installation:
* Simply run the command ***pip install -r requirements.txt*** to install the dependencies.

## Usage:
1. Clone this repository and install the dependencies as mentioned above.
2. Navigate to the [OpenAI API section](https://beta.openai.com/account/api-keys) to login and generate your API Key. Ensure you save this API Key as **"OpenAI_API_Key"*** in the form of a system environment variable which shall be used by the webapp. ***( I am only using the Free Trial version which provides 18$ of credits. )***
2. Simply run the command: 
```
streamlit run app.py
```
3. Navigate to http://localhost:8501 in your web-browser.


### Running the Dockerized App
1. Ensure you have Docker Installed and Setup in your OS (Windows/Mac/Linux). For detailed Instructions, please refer [this.](https://docs.docker.com/engine/install/)
2. Navigate to the folder where you have cloned this repository ( where the ***Dockerfile*** is present ).
3. Build the Docker Image (don't forget the dot!! :smile: ): 
```
docker build -f Dockerfile -t app:latest .
```
4. Run the docker:
```
docker run -p 8501:8501 app:latest
```

This will launch the dockerized app. Navigate to ***http://localhost:8501/*** in your browser to have a look at your application. You can check the status of your all available running dockers by:
```
docker ps
```
