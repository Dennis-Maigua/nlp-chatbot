[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

This project is licensed under the MIT license.

# AI Medical Assistant

![chatbot_blog-1](https://github.com/Dennis-Maigua/ai-medical-assistant/assets/32156551/37f7de8b-e13c-42fd-a711-09d6122677cb)

This project implements a Conversational AI Chatbot using RASA Open Source Framework, Flask, and Python.

# Design

### 1. Natural Language Understanding (NLU)
- **Intent Classification**: Identifies the intent or purpose behind user messages (e.g., booking an appointment, asking a question).
- **Entity Recognition**: Extracts specific pieces of information (entities) from user messages (e.g., dates, names, symptoms).

### 2. Dialogue Management
- **State Management**: Tracks the context of the conversation to maintain coherence and relevance in responses over multiple turns.
- **Policy-Based Decision Making**: Determines the next action or response based on the current dialogue state, past interactions, and predefined rules or machine learning models.

### 3. Responses and Actions
- Response Generation: Crafts appropriate replies or actions based on identified intents, entities, and current dialogue context.
- Action Execution: Performs backend operations (e.g., database queries, API calls) to fulfill user requests or provide information.
  
### 4. Training Pipeline:
- **Data Annotation**: Involves labeling datasets with intents and entities to train the NLU model effectively.
- **Model Training**: Uses machine learning algorithms (often neural networks) to train NLU and dialogue management models on annotated datasets.
- **Evaluation and Iteration**: Tests and refines the chatbot's performance based on real or simulated interactions to improve accuracy and user satisfaction.

### 5. Integration and Deployment:
- **Platform Integration**: Allows deployment on various platforms (e.g., web, mobile apps, messaging platforms) to interact with users where they are.
- **Continuous Learning**: Supports ongoing updates and improvements based on user feedback and evolving needs.

# Setup

### 1. Clone the repository

Download and open the project in your local machine:

  ```bash
    $ cd Desktop
    $ git clone https://github.com/Dennis-Maigua/ai-medical-assistant.git
    $ cd ai-medical-assistant-main/ai-medical-assistant-main
  ```

### 2. Create a virtual environment

Build a venv and activate it inside the project:

   ```bash
     $ python -m venv venv
     $ ./venv/Scripts/activate
   ```
   
### 3. Install packages and dependencies

Install `rasa` and python `requirements`:
  
   ```bash
     $ pip install rasa
     $ pip install -r requirements.txt
   ```

# Testing and Performance

### 1. Train the model

Map all the datasets, intents, responses, and actions for the chatbot:
  
   ```bash
     $ rasa train
   ```

### 2. Interact with the Chatbot

- Open Terminal 1 and run:

```bash
    # rasa run actions
```

- Open Terminal 2 and run:

```bash
    # rasa shell
```

# Contributing:

We welcome contributions from developers, legal experts, and blockchain enthusiasts. Feel free to fork the repository, make improvements, and submit pull requests.
