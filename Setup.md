# Local environment setup

## Prerequisites

1. Install python
2. Install pip
3. Install uv package manager

## Activate environment

1. Go to project root folder and run uv sync. It will set up a virtual envrironment.
2. Activate the virtual environment by running `source venv/bin/activate`
3. Run the app file \
   `uv run app.py`

## Set up .env file for environment variables

1. For the project to run end to end we will need some api keys to be configured in .env file.
2. Create a .env file in the root directory of the project.

3. [Set up open api key](https://platform.openai.com/api-keys). Add the key to the .env file as \
   **OPENAI_API_KEY=\<your-key\>**

4. [Set up pushover account for push notifications](https://pushover.net/)
   a. Once you set up your account you will get a pushover user key. Add it to the .env file as \
      **PUSHOVER_KEY=\<your-key\>**
   
   b. You will also need to create an application. Add the application token to the .env file as \
      **PUSHOVER_TOKEN=\<your-token\>**

5. Rerun `uv run app.py`
