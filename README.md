# AI Chatbot - Android Chatbot App

## Overview

AI is an Android application that leverages OpenAI's API to provide intelligent and dynamic conversational experiences. This chatbot app comes equipped with a range of features, including text-to-speech, speech-to-text, clipboard integration, answer sharing, and a clear chat option.

## Key Features

- OpenAI Integration: Utilizes OpenAI's API for accurate and engaging responses.
- Text-to-Speech: Enables hands-free interaction with the chatbot.
- Speech-to-Text: Allows users to communicate with the chatbot using their voice.
- Clipboard Integration: Seamlessly copy and paste text for efficient conversations.
- Answer Sharing: Easily share insightful responses with friends or other apps.
- Clear Chat Option: Maintain privacy and declutter the conversation space.

  ## Front-End Design

- Logo: The app's logo was created using Canva, a versatile graphic design tool.
- About Page:The design of the About page was crafted using Canva to provide a visually appealing and informative experience.


## Getting Started

### Prerequisites

- Android Studio
- OpenAI API Key (You can generate your API key by following [this tutorial](https://youtu.be/nafDyRsVnXU?si=l9-1iF96xh24JJ_U).)


### Installation

1. Clone the repository: `git clone https://github.com/aTh1ef/AI-Chatbot-AndroidStudio.git`
2. Open the project in Android Studio.
3. Add your OpenAI API key in the appropriate configuration file.

### Usage

- Build and run the app on your Android device or emulator.
- Engage in intelligent conversations using the various features.

### Important Note

In the `MainActivity.java` file, locate the `callAPI` method responsible for making API calls to OpenAI. Ensure that you replace the placeholder API key in the `Authorization` header with your own OpenAI API key.
You can generate your API key by following [this tutorial](https://youtu.be/nafDyRsVnXU?si=l9-1iF96xh24JJ_U).

```java
void callAPI(String question) {
    // ... (existing code)

    Request request = new Request.Builder()
            .url("https://api.openai.com/v1/completions")
            .header("Authorization", "Bearer YOUR_OPENAI_API_KEY_HERE")
            .post(body)
            .build();
    // ... (remaining code)
}

Replace "YOUR_OPENAI_API_KEY_HERE" with your actual OpenAI API key.
