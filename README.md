# Hyperbolic Labs Chatbot
This repository contains a simple automated chatbot built using the [Hyperbolic Labs API](https://app.hyperbolic.xyz). The chatbot asks 100 unique, pre-defined questions and retrieves answers from the API, simulating a conversational AI experience. It’s a fun demonstration of how to integrate Hyperbolic Labs' AI models into a Python application.

## About Hyperbolic
[Hyperbolic Labs](https://hyperbolic.xyz) provides an accessible and affordable platform for AI development, offering open-access AI models and scalable computing resources via their API.
* This project uses their language model (`meta-llama/Meta-Llama-3.1-8B-Instruct`) to generate responses to a variety of questions, showcasing the power of their tools for developers.
* Check out their [official documentation](https://docs.hyperbolic.xyz) for more details.

## VPS 1 NEEDED You can purchase it here: https://contabo.com/en/vps/
![image](https://github.com/user-attachments/assets/99553649-06da-41b2-b7da-c8d510475ae8)


## Features
- Contains a list of 100 unique questions on diverse topics.
- Randomly selects and asks questions without repetition.
- Integrates with the Hyperbolic Labs API to fetch answers.
- Adds random delays (1-2 minutes) between questions to simulate natural pacing.
- Built with Python and the `requests` library.

## Prerequisites
- Python 3.6+
- A [Hyperbolic API key](https://app.hyperbolic.xyz/settings) (replace the placeholder in the code with your own key)

## Setup
1. **Install Packages**
   ```bash
   sudo apt update && sudo apt upgrade -y
   sudo apt install git screen python3 python3-pip python3-venv -y
   ```
2. **Clone the Repository**
   ```bash
   git clone https://github.com/0xmoei/chatbot-app.git
   cd chatbot-app
   ```
3. **Install Dependencies**
   ```bash
   python3 -m venv venv
   source venv/bin/activate
   pip install requests
   ```
4. **Configure the API Key**

Replace the `YOUR_API_KEY_HERE` in `chatbot.py` with your own [Hyperbolic API Key]:
- Get Hyperbolic API Key
- Sign Up or Log In at https://app.hyperbolic.xyz/settings
- Go to Settings → API Keys
- Create/copy your API key

```bash
nano chatbot.py
   ```
![image](https://github.com/user-attachments/assets/90475511-b1ed-426e-a060-953aab5c256d)

## Create Session
  ```bash
   screen -S Hyper
   ```

5. **Run the Chatbot**

Execute the script to start the chatbot:
   ```bash
   python3 chatbot.py
   ``` 


## Detach Session: PRESS CTRL A+D



## Usage
Once running, the chatbot will:
* Print each of the 100 questions one by one.
* Fetch and display answers from the Hyperbolic Labs API.
* Pause for a random interval (60-120 seconds) between questions.
* Stop after completing all 100 questions.

Example output:
```
Question 1: What’s the best way to learn programming?
Answer: The best way to learn programming is a mix of structured learning and hands-on practice...
Waiting 87.3 seconds before next question...
```

Hyperbolic Dashboard output: https://app.hyperbolic.xyz/
![image](https://github.com/user-attachments/assets/be2fce45-ba0f-498e-9b94-ee63aa680633)


## Notes
* The API key in the code is a placeholder. You’ll need to sign up at [Hyperbolic Labs](https://app.hyperbolic.xyz/) to get your own.
* Be mindful of API usage limits and costs depending on your Hyperbolic Labs plan.
* Feel free to modify the `questions` list in `chatbot.py` to suit your interests!




