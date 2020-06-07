Introduction
RASA has 2 main modules —
i)	NLU, which is used for understanding use messages, extracting intents from use messages, etc. 
ii)	ii) Core, which is used for holding conversations and deciding what to do next during a conversation.
In May 2019, RASA X has been introduced. You can find more details here — https://blog.rasa.com/algorithms-alone-wont-solve-conversational-ai-introducing-rasa-x/
RASA X is a tool that helps you build, improve and deploy AI assistants that are powered by RASA framework. RASA X includes a user interface and a REST API.
So let’s get started with RASA X…
Install RASA X on Windows
To install RASA X on your PC, open command prompt and write down following command :
pip install rasa-x --extra-index-url https://pypi.rasa.com/simple

 
Installing RASA X through command prompt using pip
It will install all the required packages and RASA X.
Now create an empty folder for your chatbot and open command prompt into that folder. Then type the following command :
rasa init --no-prompt
Here, --no-prompt argument is just used to avoid the prompts asked during the installation.

 
Creating and training initial model of RASA X
After running the command, the initial model training will start and it will create the following folders into the directory –

 
Directories created after running rasa init command
Now you can train your chatbot and run the RASA X by running the following commands in this directory –
rasa train: To train the chatbot
rasa x: To run RASA X
After running rasa x command, you will see the following on command prompt –

 
You can see the following resources for getting started with RASA X –
1. RASA Docs — http://rasa.com/docs/
2. RASA X — http://rasa.com/docs/rasa-x/
3. RASA User guide — https://rasa.com/docs/rasa/



1.	Telegram Integration:
◦	Download ngrok from https://ngrok.com/download
◦	After extracting the zip file, open the ngrok file and run it.
◦	In ngrok, enter the command ‘ngrok http 5005 ’:
 
•	Then go to telegram and create your own bot using Botfather:
a)	Open the telegram app and search for botfather(it is an inbuilt bot used to create other bots)
b)	Start a conversation with botfather and enter /newbot to create a newbot.
c)	Give a name to your bot
d)	Give a username to your bot, which must end in _bot.This generates an access token.

•	Open ‘credentials.yml’ and enter:
telegram:
access_token: "obtained from telegram"
verify: "your bot username"
webhook_url: "https://<ngrokurl>/webhooks/telegram/webhook"

•	Go to terminal and enter the command ‘rasa run’
•	Open one more terminal and run the command ‘rasa run actions’
•	Now, you can chat with your bot from Telegram.


 


References:
1.	Rasa Official documentation https://rasa.com/docs/rasa/user-guide/installation/

