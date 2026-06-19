# Cyber Bot - Cybersecurity Awareness Assistant

## Overview

Cyber Bot is a Windows Presentation Foundation (WPF) chatbot application developed in C#. Its purpose is to educate users about cybersecurity concepts through an interactive conversation interface.

The chatbot provides information on common cybersecurity topics, answers follow-up questions, remembers basic user information during the session, and responds with educational explanations, examples, and safety tips.

---

## Features

### User Interaction

* Greets users with a welcome message and voice greeting.
* Requests and remembers the user's name.
* Displays messages in a modern chat-style interface.
* Supports sending messages using:

  * Send button
  * Enter key

### Cybersecurity Topics

The chatbot can explain:

* Password Security
* Phishing
* Malware
* Online Scams
* Privacy Protection
* Safe Browsing
* Ransomware
* Two-Factor Authentication (2FA)
* Public Wi-Fi Security
* Firewalls

### Follow-Up Questions

Users can ask:

* **Why?**
* **How?**
* **Give me an example**
* **Tell me more**

The chatbot provides topic-specific responses based on the previous conversation context.

### Sentiment Awareness

The chatbot detects certain user emotions and adjusts responses accordingly:

* Worried
* Scared
* Confused
* Curious

### Memory Features

The chatbot remembers:

* User's name
* First cybersecurity topic discussed

Users can ask:

* "What do you remember about me?"
* "My name"

### Audio Greeting

A welcome audio file (`Greeting.wav`) is played when the application starts.

---

## Technologies Used

* C#
* .NET Framework / WPF
* XAML
* ObservableCollection
* Dictionaries for knowledge storage
* SoundPlayer API

---

## Project Structure

```text
Cyberbot/
│
├── MainWindow.xaml
├── MainWindow.xaml.cs
├── Greeting.wav
├── MessageItem.cs
└── README.md
```

### Main Components

#### MainWindow

Handles:

* User input
* Chat flow
* Topic detection
* Response generation
* Sentiment analysis
* Memory management

#### MessageItem

Represents a chat message with:

* Sender name
* Message text
* Timestamp
* Alignment
* Styling information

---

## How the Chatbot Works

### Step 1: User Identification

When the application starts:

```text
Cyber Bot: Welcome to your Cybersecurity Awareness Assistant Chatbot.
Cyber Bot: Enter your name:
```

The chatbot extracts and stores the user's name.

### Step 2: Topic Detection

The chatbot searches user input for cybersecurity keywords.

Example:

```text
What is phishing?
```

Detected Topic:

```text
phishing
```

### Step 3: Generate Response

A random response is selected from the topic's response collection.

### Step 4: Follow-Up Support

Example:

```text
User: What is phishing?
Bot: [Explanation]

User: Why?
Bot: [Why phishing is dangerous]

User: How?
Bot: [How to avoid phishing]

User: Give me an example
Bot: [Real-world phishing example]
```

---

## Supported Commands

| User Input                     | Action                            |
| ------------------------------ | --------------------------------- |
| What is phishing?              | Topic explanation                 |
| Why?                           | Gives importance of current topic |
| How?                           | Gives protection tips             |
| Give me an example             | Provides real-world example       |
| Tell me more                   | Provides additional information   |
| What do you remember about me? | Displays stored information       |
| My name                        | Shows remembered name             |
| Bye                            | Ends conversation                 |

---

## Installation

### Requirements

* Visual Studio 2022 (or later)
* .NET Framework compatible with the project
* Windows OS

### Steps

1. Clone or download the project.
2. Open the solution in Visual Studio.
3. Ensure `Greeting.wav` is placed in the output directory.
4. Build the solution.
5. Run the application.

---

## Example Conversation

```text
Cyber Bot: Enter your name:

User: My name is Asanda

Cyber Bot: Nice to meet you, Asanda.

User: What is malware?

Cyber Bot: Malware is harmful software designed to damage your device, steal information, spy on your activity, or give attackers control of your system.

User: Why?

Cyber Bot: Malware is dangerous because it can work silently in the background...

User: How?

Cyber Bot: To avoid malware, download only from trusted websites...
```

---

## Educational Purpose

This project was created to promote cybersecurity awareness by teaching users about common online threats and safe digital practices through an interactive chatbot experience.

---

## Future Improvements

Possible enhancements include:

* Database-backed memory
* More cybersecurity topics
* Speech-to-text support
* Text-to-speech responses
* AI/NLP integration
* User progress tracking
* Dark mode interface
* Multi-language support

---

## Author

**Asanda Ndlovu**

Cybersecurity Awareness Assistant Project
