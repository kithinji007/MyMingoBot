# Mingobot

Mingobot is a chatbot developed using Rasa NLU (Natural Language Understanding) and deployed on the Telegram messaging platform. It is designed to provide information and answer questions regarding Moringa School's data science program. It serves as a helpful resource for prospective students, current learners, and anyone interested in understanding the program's details. Mingobot employs natural language processing techniques to provide accurate and informative responses, making it a valuable tool for those exploring the world of data science education.

![newMingo](https://github.com/kithinji007/MingoBot/assets/122665283/585ff0ab-b6ed-4f65-81ec-812dac76f75e)

**Key Features:**
- Answers common questions about Moringa School's data science program.
- User-friendly and accessible via Telegram chat interface.

**Inspiration:**
Mingobot was created to enhance the accessibility of information about Moringa School's data science program and to make the application process more transparent and user-friendly.

## Table of Contents:

1. [Project Name and Description](#Mingobot)
2. [Installation](#Installation)
3. [Files used in the Project](#Files-used-in-the-project)
4. [Usage](#Usage)
5. [Features](#Features)
6. [Mingobot Flowchart](#Mingobot-Flowchart)
7. [Model Evaluation](#Model-Evaluation)
8. [Conclusion](#Conclusion)

# Installation

To get Mingobot up and running, follow these installation steps. You can deploy Mingobot on your own system or server.

### Prerequisites

Before you begin, ensure you have the following prerequisites installed on your system:

- [Python](https://www.python.org/downloads/) (Version 3.6 or higher)
- [Pip](https://pip.pypa.io/en/stable/installation/) (Python package manager)
  
 ### To install rasa and set up your environment 

- [To set up your environment](https://rasa.com/docs/rasa/installation/environment-set-up/)
- [To Install Rasa Open Source](https://rasa.com/docs/rasa/installation/installing-rasa-open-source)

# Files used in the project

## 1. domain.yml:

### Purpose:

Define how the chatbot behaves. Specify which intents it can understand, the responses it should give, and any information it needs to extract from user messages.

### Use-Case:

Customize responses, manage the chatbot's knowledge, and define how it handles different types of interactions.

## 2. nlu.yml(NLU Training Data):

### Purpose:
Train the chatbot's language understanding. Provide examples of user messages and what they mean (intents and entities) to help the chatbot understand and respond accurately.

### Use-Case:

Teach the chatbot to recognize different intents and extract important information from user input.

## 3. config.yml: 

### Purpose:

Configure the chatbot's behavior, including the language understanding pipeline and machine learning models. Set training parameters and customize how the chatbot understands language.

### Use-Case:

Customize the chatbot's language understanding, improve its performance, and adapt it to specific use cases.

## 4. endpoints.yml: 

Connect the chatbot to external services for performing actions, tracking user interactions, and integrating with other systems.

### Purpose:

Configure external services and connections. Specify how the chatbot interacts with external systems, such as action servers or user trackers.

### Use-Case:
Connect the chatbot to external services for performing actions, tracking user interactions, and integrating with other systems.

# Usage

Mingobot is designed to make it easy for users to access information about Moringa School's data science program through Telegram. You can interact with Mingobot by following these simple steps:

1. **Start a Chat with Mingobot**:

   - Open your Telegram app.
   - Search for your Mingobot by its username or display name. @myMingo_bot
   - Start a chat with Mingobot by clicking on it.

2. **Ask Questions**:

   - Once you're in a chat with Mingobot, you can start asking questions about the data science program at Moringa School. For example, you can inquire about the application process, curriculum, or any specific details you're interested in.

   - Mingobot uses natural language processing to understand your questions and provide relevant responses.

3. **Example Interactions**:

   Here are some examples of questions you can ask Mingobot:

   - "Where is Moringa located?"
   - "What are the learning modes are available?"
   - "How do I apply to Moringa School's data science program?"
   - "What career opportunities are avilable after completion of the program?"

4. **Receive Responses**:

   - Mingobot will respond to your questions with informative and helpful answers. It may also provide links or references for additional information.

5. **Continue the Conversation**:

   - Feel free to continue the conversation and ask follow-up questions. Mingobot is designed to provide a conversational experience.

Mingobot is here to assist you in getting the information you need about Moringa School's data science program. Don't hesitate to reach out and start a chat with Mingobot today!

# Features

Mingobot is equipped with several features that make it a valuable resource for users interested in Moringa School's data science program. Here are some of its key features:

1. **Question Answering**: Mingobot can answer a wide range of questions related to the data science program at Moringa School. Users can inquire about admission requirements, curriculum details, program benefits, and much more.

2. **Natural Language Processing (NLP)**: Mingobot utilizes advanced NLP techniques to understand and interpret user questions. This enables it to provide accurate and context-aware responses, making the conversation more natural and engaging.

3. **Telegram Integration**: Mingobot is integrated with the Telegram messaging platform, allowing users to access information conveniently through their Telegram accounts.

4. **User-Friendly Interface**: The chatbot provides a user-friendly chat interface, making it easy for users to initiate conversations and receive answers to their questions.

5. **Conversational Experience**: Mingobot is designed to provide a conversational experience, allowing users to ask follow-up questions and engage in informative dialogues.

6. **Informative Responses**: The chatbot provides detailed and informative responses, often including links or references to additional resources for further exploration.

7. **Availability**: Mingobot is available 24/7, ensuring that users can access information whenever it's convenient for them.

8. **Continuous Improvement**: We are committed to improving Mingobot's knowledge base and capabilities to ensure that users receive the most up-to-date and accurate information.

Mingobot's features are designed to make the process of gathering information about Moringa School's data science program as straightforward and informative as possible. Whether you're a prospective student or just curious about the program, Mingobot is here to assist you.

# Mingobot Flowchart

<img width="1280" alt="chart1" src="https://github.com/kithinji007/MingoBot/assets/122665283/9c31525c-0ba0-40e6-acbe-c6eaf9ed3521">

## How does Mingobot Work ?
<img width="1280" alt="chart2" src="https://github.com/kithinji007/MingoBot/assets/122665283/94de6fa6-c9b0-4b0a-a526-eef48bbdcb52">

**1.Students Interact with Mingo on Telegram:** Students initiate conversations with the chatbot by sending messages on the Telegram platform. They can ask questions or make inquiries about the data science program.

**2.NGROK Connects Telegram to Local Server:** NGROK acts as a secure tunnel that establishes a connection between Telegram's platform and our local server. This enables seamless communication between the Telegram interface and the chatbot.

**3. Local Server Connects to RASA:** The local server serves as an intermediary between NGROK and the RASA framework. It receives incoming messages from Telegram, then forwards them to RASA for processing.

**4. RASA (Breaks Down the Interaction Identifying the Intent and Chooses the Appropriate Response:)** RASA, equipped with Natural Language Understanding (NLU) capabilities, analyzes the incoming message to understand the user's intent. 
It identifies the purpose behind the query and determines the most suitable course of action or response.

**5. Back to MingoBot** After processing the user's message, RASA formulates a tailored response based on the identified intent. This response is then sent back to the user through the Telegram platform, providing them with the information or assistance they requested.

This flow ensures a smooth and effective interaction between students and the MingoBot, allowing them to obtain the information they need about the data science program in a user-friendly manner.

# Model Evaluation

To give you a visual representation of Mingobot in action, here are some video demos and screenshot of how the chatbot works:

### Screenshot 1: Asking a Question

![IMG-6442](https://github.com/kithinji007/MingoBot/assets/122665283/7169a932-78a6-4715-8bb4-988a58b49e81)

*Description: A user asking a question about Moringa School's data science program and Mingobot providing a detailed response to a user's question.*

### Demo: A Brief Interaction

https://github.com/kithinji007/MingoBot/assets/122665283/bd09e2d7-06f1-407b-b56d-0da01e653379

https://github.com/kithinji007/MingoBot/assets/122665283/6863801b-ee6d-412a-ab5d-7544050c349d

The above screenshot and videos show user interactions with mingobot.

# Conclusion 
Moringa School is an institution which is very big on matters of feedback. MingoBot is a solution that enhances this two-way communication channel, in a split of a second. Being readily available, to provide consistent assistance to current students, potential students, parents and other interested parties is very vital. 
Having MingoBot be easily accessible on Telegram messaging platform, enhances its usability, while continuously monitoring and improving it, to ensure that it remains relevant and effective. 
The ultimate goal is to create a chatbot that acts as a reliable, efficient, and engaging communication support tool, that will enrich the educational experience and facilitate smooth school operations.

