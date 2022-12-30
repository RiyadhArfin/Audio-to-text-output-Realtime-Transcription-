<p align="center">
  <img width="60px" src="https://user-images.githubusercontent.com/6180201/124313197-cc93f200-db70-11eb-864a-fc65765fc038.png" alt="giant microphone"/><br/>
  <h2 align="center">Audio-to-text-output-Realtime</h2>
</p>

A Audio-to-text-output-Realtime transcription project using React and a socketio python server. The goal of this project is to enable developers to create web demos and speech2text prototypes with just a few lines of code. Examples can be medical dictation apps, a note-taking CRM for entrepreneurs, etc.

*Currently only supports real-time transcription using Google Cloud Speech*

# Installation
* Python 3 [instructions](https://realpython.com/installing-python/)
* `yarn` [instructions](https://classic.yarnpkg.com/en/docs/install/#mac-stable)

## Google Speech API
The code assumes an environment variable `GOOGLE_SERVICE_JSON_FILE` that points to a valid GCP service account file.

The Json key is given

But

If you need to get a service account:
  - Within your Google Cloud console, create or select a project
  - Enable the Cloud Speech API for that project
  - Create a service account
  - Download a private key as JSON

More info in Google Cloud's docs [here](https://cloud.google.com/speech-to-text/docs/quickstart-client-libraries#before-you-begin) and [here](https://codelabs.developers.google.com/codelabs/cloud-speech-text-python3#0).<br/>

Then, set the environment variable `GOOGLE_SERVICE_JSON_FILE` to the path of the JSON file containing your service account key, e.g. `"C:\Users\ARFIN\Documents\audio-to-text-output-ea3e0df5005b.json"`.
# Setup
1. Clone or fork this repository
2. Create a virtual environment in the root directory: `python -m venv $ENV_NAME`
3. Activate the virtual environment: ` source $ENV_NAME/bin/activate` (for MacOS, Unix, or Linux users) or ` .\ENV_NAME\Scripts\activate` (for Windows users)
4. Install requirements: `pip install -r backend/requirements.txt`
5. Set your environment variable `GOOGLE_SERVICE_JSON_FILE` to point to your file path
6. Run `yarn install` in the root directory
7. Run `yarn start` to start the frontend and `start-backend` to run the backend
