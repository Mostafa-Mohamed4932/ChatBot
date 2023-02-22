Chat Bot
This is a Python project that implements a chatbot that reacts to the information provided by the user. Once the user sends a message to the bot, it cleans the message and compares it with the data available in a file named Chatbot (1).txt that is uploaded to Google Drive. If it finds a match, the bot responds with the corresponding message from the file. If it cannot find a match, the bot informs the user that it cannot understand the message.

Prerequisites
Before running this chatbot, make sure that you have a Google account to access Google Colab. Also, ensure that you have the following Python libraries installed:

re (Regular expressions library)
difflib (Library for comparing sequences)
Usage
Open Google Colab and create a new notebook.

Mount your Google Drive in the notebook by running the following code:

python
Copy code
from google.colab import drive
drive.mount('/content/drive')
Upload the Chatbot (1).txt file to your Google Drive.

Open a new cell in the notebook and copy-paste the following code to install the required libraries:

diff
Copy code
!pip install difflib
In a new cell, copy-paste the code from the chatbot.py file in this repository.

Run the cell to start the chatbot.

The chatbot will prompt you to enter your message. Type your message and press enter.

The bot will clean the message and compare it with the data available in Chatbot (1).txt on your Google Drive. If it finds a match, it will respond with the corresponding message from the file. If it cannot find a match, the bot will inform you that it cannot understand the message.

If the bot finds multiple lines that match the user's prompt, it will grade them according to how close they are to the sentence, and then use the one with the highest score.

Example
Here is an example conversation with the chatbot:

vbnet
Copy code
User: Hello!
Bot: Hi there!

User: What is your name?
Bot: My name is Chatbot.

User: Can you help me with my homework?
Bot: I'm sorry, I cannot understand your message.
Conclusion
This is a simple chatbot that can be used to automate basic conversations. You can modify the data available in Chatbot (1).txt to customize the bot's responses. If you have any questions or suggestions, please feel free to contact me.
 
