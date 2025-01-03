# URL to Video Generator

This project generates a URL to a video based on the contents of a provided URL. It uses OpenAI's GPT-4 model to generate images, text summaries, transcripts, and audio, summarizing the URL's content in less than 150 words. The project includes a frontend built with React and Vite, and a backend powered by Express.

## Features

- **Text Summary**: A concise summary of the URL content (less than 150 words).
- **Image Generation**: Generate images based on the URL content.
- **Transcript**: A textual representation of the audio content.
- **Audio Generation**: Generate audio based on the URL content.

## Technologies Used

- **Frontend**: React, Vite
- **Backend**: Express
- **AI Model**: OpenAI GPT-4o

## Project Structure

/frontend ├── package.json 
          └── (React + Vite setup)

/backend  ├── package.json 
          ├── index.js (Express backend setup) 
          └── script.gpt (GPT script configuration file)


## Requirements

- GPT-4 API keys (OpenAI)
- **gptscript** installed on your machine (Windows/Mac)

### Frontend
1. React app powered by Vite.
2. Runs on `localhost` by default.

### Backend
1. Express server for handling API requests.
2. Uses `script.gpt` configuration for the GPT-4o setup.

## Installation

### 1. Install Dependencies

#### For Frontend

1. Navigate to the `frontend` directory.
2. Run the following command to install dependencies:
   
    ```bash
    cd frontend
    npm install
    ```

#### For Backend

1. Navigate to the `backend` directory.
2. Run the following command to install dependencies:
   
    ```bash
    cd backend
    npm install
    ```

### 2. Install `gptscript`

The backend requires the `gptscript` to interface with the GPT-4 model. Follow the installation steps from the official `gptscript` documentation for your operating system.

#### Installation Documentation

- **Windows/Mac Installation**: Follow the steps outlined on the official [gptscript installation guide](https://gptscripts/docs).

#### Verify Installation

Ensure `gptscript` is properly installed by running the following command:

```bash
gptscript --version
```

### 3. Configure API Keys

You need to provide your GPT-4o API key for video generation.

1. Add your GPT-4o API key to your path:

    ```bash
    set OPENAI_API_KEY="your-api-key-here"
    ```

### 4. Running the Application

#### Start the Backend

1. Navigate to the `backend` directory.
2. Run the following command to start the Express server:
   
    ```bash
    npm start
    ```

#### Start the Frontend

1. Navigate to the `frontend` directory.
2. Run the following command to start the React development server:
   
    ```bash
    npm run dev
    ```

The application should now be running on `http://localhost:3000` (or another port specified by Vite for the frontend) and the backend on `http://localhost:8080` (or another port for Express).

## Usage

1. Enter a URL into the provided input field on the frontend.
2. The app will generate a video link containing:
   - A summary of the URL's content.
   - An image, transcript, and audio of the content.

## Contributing

If you'd like to contribute to this project, feel free to fork the repository, submit pull requests, or open issues for discussion.
