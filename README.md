# ChatBot Setup Guide ❤️ by Jay Gupta
# ChatBot Setup Guide

## Installation & Configuration

To set up the ChatBot application, follow these steps:

1. **Install Python:**
   - First, make sure you have Python installed on your system. If not, you can download and install it from [Python Official Website](https://www.python.org/downloads/).

2. **Install pip:**
   - Pip is a package manager for Python. If you don't have it installed, you can follow the instructions in this [guide](https://phoenixnap.com/kb/install-pip-mac) to install pip on your Mac.

3. **Check Python and Pip Versions:**
   - Open your terminal or command line tool and check the installed versions of Python and pip using the following commands:
     ```
     python3 --version
     pip --version
     ```

## Installing Flask and Dependencies

4. **Install Flask and Dependencies:**
   - In your terminal, navigate to the project directory where you have the `requirements.txt` file.
   - Run the following command to install the required packages using pip:
     ```
     pip install -r requirements.txt
     ```

## Running the ChatBot Application

5. **Run the ChatBot Application:**
   - After installing the required dependencies, navigate to your project directory in the terminal:
     ```
     cd /path/to/your/directory
     ```
   - Start the ChatBot application by running the following command:
     ```
     python app.py
     ```

## What You Will Create

In this tutorial, you'll build a chatbot that can engage in conversations with users using natural language processing. You'll use Microsoft DialoGPT, a pre-trained language model, and integrate it with Flask to create a web application with a chat interface.

For the frontend, you'll use HTML, CSS, and JavaScript to create an interactive chat interface. jQuery will handle HTTP requests to the backend server.

The tutorial will provide step-by-step instructions for setting up your development environment, installing dependencies, creating necessary files, and training DialoGPT to improve response accuracy.

By the end, you'll have a fully functional chatbot and valuable experience with DialoGPT, Flask, HTML, CSS, and JavaScript.

# ChatBot Model

The Chatbot uses the Microsoft/DialoGPT-medium model. You can find more details about this model at the following link:

[Microsoft/DialoGPT-medium Model](https://huggingface.co/microsoft/DialoGPT-medium)

# User HTML

```html
var userHtml = `
<div class="d-flex justify-content-end mb-4">
   <div class="msg_cotainer_send">
      ${user_input}
      <span class="msg_time_send">${time}</span>
   </div>
   <div class="img_cont_msg">
      <img src="https://i.ibb.co/d5b84Xw/Untitled-design.png" class="rounded-circle user_img_msg">
   </div>
</div>`;

```

# User-Html

```
var userHtml = '<div class="d-flex justify-content-end mb-4"><div class="msg_cotainer_send">' + user_input + '<span class="msg_time_send">'+ time + 
    '</span></div><div class="img_cont_msg"><img src="https://i.ibb.co/d5b84Xw/Untitled-design.png" class="rounded-circle user_img_msg"></div></div>';
```

# Bot-HTML

```
var botHtml = '<div class="d-flex justify-content-start mb-4"><div class="img_cont_msg"><img src="https://i.ibb.co/fSNP7Rz/icons8-chatgpt-512.png" class="rounded-circle user_img_msg"></div><div class="msg_cotainer">' + bot_response + '<span class="msg_time">' + time + '</span></div></div>';
```